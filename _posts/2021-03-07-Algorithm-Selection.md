---
layout: post
title: Algorithm Selection
categories: [Algorithms, STL, C++]
author: Conor Hoekstra
---

Yesterday, a contributor to one of my open source projects ([Robert](https://twitter.com/sebanisu)) [pointed out](https://github.com/codereport/An-Algorithm-Library/issues/5) to me that `std::find_if(f, l, pred) != l` is just `std::any_of(f, l, pred)`. I totally missed this while refactoring even though it is implicitly covered in my [STL Algorithm Cheatsheet](https://github.com/codereport/Algorithms/blob/master/CheatSheet/The%20STL%20Algorithm%20Cheat%20Sheet%20v0.0.pdf):

![image](https://user-images.githubusercontent.com/36027403/110241938-9d9ea400-7f21-11eb-9be1-45ebf264f539.png)

So thank you Robert for pointing it out! And because of this I decided to write up a short blog about the following:

> Always choose the most specialized algorithm.

Below is a diagram that captures the specializations / relationships between `std::find_if`, `std::any_of` and all of the `std::mismatch` algorithms.

![image](https://user-images.githubusercontent.com/36027403/110241992-dc345e80-7f21-11eb-9a63-3dd5993a924b.png)

I assert that you should always choose the most specialized algorithm, aka the algorithm that is furthest from `mismatch` *that works for your problem*. Here are a couple of C++ snippets that show how you can implement these in terms of each other. The implementations also double as examples of code that should just be replaced by the more specialized / better named algorithm.

```cpp
auto adjacent_find(auto f, auto l, auto pred) {
    return std::mismatch(f, std::prev(l), std::next(f), pred).first;
}

auto is_sorted_until(auto f, auto l, auto comp = std::less_equal{}) {
    return std::adjacent_find(f, l, std::not_fn(comp));
}

auto is_sorted(auto f, auto l, auto comp = std::less_equal{}) {
    return std::is_sorted_until(f, l, comp) == l;
}

auto equal(auto f, auto l, auto f2) {
    return std::mismatch(f, l, f2, std::not_equal_to{}).first == l;
}

auto find_if(auto f, auto l, auto pred) {
    return std::mismatch(f, l, f, [&](auto a, auto b) {
        return pred(a);
    }).first;
}

auto any_of(auto f, auto l, auto pred) {
    return std::find_if(f, l, pred) != l;
}

auto find(auto f, auto l, auto val) {
    return std::find_if(f, l, [&](auto e) { return e == val; });
}
```
[Godbolt link](https://www.godbolt.org/z/Ts5ca1)

_____

### Update

[Stephan T. Lavavej](https://twitter.com/StephanTLavavej) (aka STL, one of the [MSVC Standard Library](https://github.com/microsoft/STL/graphs/contributors?from=2019-09-01&to=2021-03-08&type=a) implementers) pointed out that `is_partitioned_until` and `is_partitioned` could be added to the diagram.

<center><blockquote class="twitter-tweet"><p lang="en" dir="ltr">is_partitioned_until and is_partitioned could be added to the diagram, as they can be thought of as weaker versions of is_sorted.</p>&mdash; Stephan T. Lavavej (@StephanTLavavej) <a href="https://twitter.com/StephanTLavavej/status/1368701581839925251?ref_src=twsrc%5Etfw">March 7, 2021</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script></center>

So I updated my diagram. Note that `is_partitioned_until` isn't actually in the C++ Standard Library which is why it is in grey. The code snippets have been provided as well.

![image](https://user-images.githubusercontent.com/36027403/110389223-37557680-8032-11eb-867c-39d8d67b7b1b.png)

```cpp
auto is_partitioned_until(auto f, auto l, auto pred) {
    return std::next(std::adjacent_find(f, l, [&](auto a, auto b) { 
        return not pred(a) and pred(b);
    }));
}

auto is_partitioned(auto f, auto l, auto pred) {
    return is_partitioned_until(f, l, pred) != l;
}
```
[Updated Godbolt](https://www.godbolt.org/z/YrfbTf)

Finally, I have received a couple comments on Reddit and Twitter asking "Why?" or stating that I did not provide any reasoning. That was an oversight on my part. 

> The motivation for choosing the most specialized algorithm is that it leads to simpler and more readable code. 

The more specialized algorithms contain more *meaning* and therefore communicates more information to futures readers of the code. For example, `is_sorted` is much more meaningful than `adjacent_find` with the `greater` function object or the `less_equal` function object + `not_fn`. Furthermore, code using more specialized algorithms is simpler. An example of this is that using many of the specialized algorithms avoids having to write `!= container.end()`.

That's all. Happy coding!

Feel free to leave a comment on the [reddit thread](https://old.reddit.com/r/cpp/comments/lzrqv4/algorithm_selection/) or [tweet](https://twitter.com/code_report/status/1368569503379042304).


