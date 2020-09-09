---
layout: post
title:  C++ STL-Like Algorithm Libraries
categories: [C++,STL,Algorithms]
---

I recently watched the extended version of Sean Parent's amazing [C++ Seasoning](https://www.youtube.com/watch?v=qH6sSOr-yk8) talk, which was given at Amazon's A9 and posted on the [A9 YouTube Channel](https://www.youtube.com/user/A9Videos/videos). I highly recommend the extended version, which can be watched in two parts:

* [Programming Conversations Lecture 5 Part 1](https://www.youtube.com/watch?v=IzNtM038JuI)
* [Programming Conversations Lecture 5 Part 2](https://www.youtube.com/watch?v=vxv74Mjt9_0)

<p align="center"><iframe width="640" height="360" src="https://www.youtube.com/watch?v=IzNtM038JuI" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></p>

At [one point in the talk](https://youtu.be/IzNtM038JuI?t=612), Sean points out that the STL is far from complete and that you should write your own algorithm if it isn't there. This is a point that Marshall Clow, maintainer of the `libc++` standard library, dedicated a [whole talk](https://www.youtube.com/watch?v=h4Jl1fk3MkQ) to at CppCon 2016. 

<p align="center"><iframe width="640" height="360" src="https://www.youtube.com/watch?v=h4Jl1fk3MkQ" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></p>

Sean also mentions at another point in the talk that the ASL, [Adobe Standard Library](https://stlab.adobe.com/group__algorithm.html), itself has a number of algorithms added on top of the STL algorithms provided in the standard library. 

This got me wondering, what are all the C++ STL-like open source libraries out in the wild and how many have additional algorithms? The ones that I knew off the top of my head were:

* [ASL (Adobe Standard Library)](https://stlab.adobe.com/)
* [Boost Algorithm Library](https://www.boost.org/doc/libs/1_74_0/libs/algorithm/doc/html/index.html)
* [BSL (Bloomberg Standard Library)](https://github.com/bloomberg/bde/tree/master/groups/bsl/bslalg)

Then I went and did some searching and came across:

* [EASTL (Electronic Arts STL)](https://github.com/electronicarts/EASTL/blob/master/include/EASTL/algorithm.h)

But that was it. Note that BSL has it's own very unique style that is furthest away from the STL. But the rest look and feel very STL-like / Stepanov inspired. My question to the readers is do you know any that aren't listed in the four above? I plan to write a follow up blog post in the near future post-CppCon 2020 that takes a look at some of the algorithms that exist outside of the C++ STL, but before I do that I would love to have a comprehensive list. 

If you know of any libraries, either let me know on Twitter or comment on the corresponding Reddit post. As new libraries are mentioned, I will add them to the list below.

**Added C++ STL-Like Libraries**
* None yet

<center>Hope to virtually see you at CppCon 2020!</center>
