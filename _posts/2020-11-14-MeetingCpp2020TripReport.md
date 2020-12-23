---
layout: post
title: Meeting C++ 2020 Trip Report
categories: [C++,Meeting C++,Trip Report]
---

This was my second time attending [Meeting C++](https://twitter.com/CppCon). The first time I attended was in 2019, when I gave my first Meeting C++ presentation, [Better Algorithm Intuition](https://youtu.be/TSZzvo4htTQ). 

This year I gave one full length talk, **C++ Concepts vs Rust Traits vs Haskell Typeclasses vs Swift Protocols**, which covered an introduction to C++ concepts and compared them to similar language features in Rust, Swift, Haskell and D. This broad category of language features is sometimes referred to as "constrained parametric polymorphism." 

I will update this blog with links to the YouTube videos when they become available. You can see a short preview in the tweet below.

<center><blockquote class="twitter-tweet"><p lang="en" dir="ltr">Slideware by <a href="https://twitter.com/code_report?ref_src=twsrc%5Etfw">@code_report</a> <a href="https://twitter.com/hashtag/meetingcpp?src=hash&amp;ref_src=twsrc%5Etfw">#meetingcpp</a> <a href="https://t.co/jpMfo6clh8">pic.twitter.com/jpMfo6clh8</a></p>&mdash; Meeting C++ (@meetingcpp) <a href="https://twitter.com/meetingcpp/status/1326912706125983744?ref_src=twsrc%5Etfw">November 12, 2020</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script></center>

## Diversity Spotlight

Since my first [trip report from CppCon 2020](https://codereport.github.io/CppCon2020TripReport/), I have decided to try and highlight diversity in my trip reports. I have decided to focus on the representation of female vs total number of speakers.

|Conference|F/Total|%|
|:-:|:-:|:-:|
|CppCon 2020|6/87|6.9%|
|Meeting C++ 2020|1/14|7.1%|

The 7.1% is very similar to CppCon. If you include AMAs, it goes up to 2/18, which is **11.1%**. It was great to see such diversity in the keynote talks. It was also great to see the D&I (Diversity & Inclusivity) Panel on the first day. Hoping to see more of these at future conferences.

## Thoughts on Remo

I have attended (fully in some cases, briefly popped in for others) 7 online virtual conferences this year:

|Conference|Date|Technology Used|
|:--:|:--:|:--:|:--:|
|[Italian C++ 2020](https://www.italiancpp.org/event/itcppcon20/)|Jun|YouTube + Discord|
|[PLDI 2020](https://conf.researchr.org/home/pldi-2020)|Aug|Gather|
|[CppCon 2020](https://cppcon.org/program2020/)|Sep|Remo|
|[10th RacketCon](https://con.racket-lang.org/2020/)|Oct|Gather|
|[Dyalog 2020](https://www.dyalog.com/uploads/conference/dyalog20/Conference%20Programme%202020.pdf)|Nov|Zoom|
|[Meeting C++ 2020](http://meetingcpp.com/2020/)|Nov|Remo|

From my experience, two things stand out:

* Remo is by far my favorite platform
* Remo tables should be 10+

I am not sure what the limit is for table size on Remo - but the size of 6 that Meeting C++ chose I found to be too small. Typically what happened in the Meeting C++ Remo was there was only 1 or 2 tables with conversations happening. If there is only going to be 1 or 2 tables of active conersation, it is better (in my opinion) to have those tables be a bit larger.

![image](https://user-images.githubusercontent.com/36027403/99158131-9109ed80-269d-11eb-9a62-009867e794d0.png)

## Overall Thoughts

The virtual Meeting C++ was enjoyable but I definitely missed the in person aspect from the previous year's meeting. The highlights were:

* Jonathan O'Connor's talk on Templates
* Dawid Zalewski's talk on Lambdas
* The D&I panel
* All of the keynotes were first time talks :)
* The conversations that I had with folks in between talks

If there is one thing I would improve on it would be have more "new" talks. From what I understand, there were a lower number of submissions this year for both CppCon & Meeting C++, so maybe it isn't possible to avoid the issue of having many repeat talks from CppCon. It is also worth noting (thanks to Jonathan O'Connor for pointing this out) that CFPs for both conferences sometimes overlap, making it difficult to know what talks will be accepted for CppCon. However, it would be nice (especially for a single track conference) if there were more new (aka first time talks). To be clear, I don't consider talks given at meetups (I presented at [C++TO](https://www.meetup.com/CPPTORONTO/) and others at [MUC++](https://www.meetup.com/MUCplusplus/)) as "previous" talks, I view these as practice runs. A repeat talk for me is a talk that has been presented previously at another conference. Of the 11 non-keynote talks, I gave one of them and I had already seen 6 of them, which left only 4 new talks + the keynotes. That combined with only a couple tables of active conversation in Remo left me with the feeling that Meeting C++ was sort of living in the shadow of CppCon. I only say this because after C++Now in 2019, Meeting C++ 2019 was probably my favorite conference.

## Keynotes & Talks

#### Keynotes

|Day|Speaker|Talk|
|:-:|:-:|:-:|
|1|Jonathan Boccara|[Metapolymorphism](https://www.youtube.com/watch?v=mU_n_ohIHQk)|
|2|Teresa Johnson|[ThinLTO: Whole Program Optimization](https://www.youtube.com/watch?v=VAMvr1rXmg8)|
|3|Gabriel Dos Reis|[Programming in the Large with C++20](https://www.youtube.com/watch?v=j4du4LNsLiI)|

#### Talks

|Day|Speaker|Talk|Previous Version|
|:-:|:-:|:-:|:-:|
|1|Timur Doumler|How C++20 changes the <br>way we write code|[CppCon 2020](https://youtu.be/ImLFlLjSveM)|
|1|Nicolai Josuttis|Hidden Features and <br>Traps of C++ Move Semantics|[CppCon 2020](https://www.youtube.com/watch?v=TFMKjL38xAI)<br> [Italian C++ 2020](https://youtu.be/OOLR96-GjsI?t=1633)|
|1|Conor Hoekstra|C++ Concepts vs Rust Traits <br>vs Haskell Typeclasses <br>vs Swift Protocols|C++TO|
|2|Sy Brand|Building an Intuition for Composition|[CppCon 2020](https://www.youtube.com/watch?v=AGRWRwi7rD0)|
|2|Jonathan O'Connor|[Template Shenanigans](https://www.youtube.com/watch?v=83fMx7Grxys)|-|
|2|Jonathan Müller|The Static Initialization Order Fiasco|[MUC++](https://www.youtube.com/watch?v=dlTrziwQU-w)|
|2|Dawid Zalewski|[Lambdas, uses and abuses](https://www.youtube.com/watch?v=Onv9w6FGwIQ)|-|
|2|Phil Nash|OO Considered Harmful|[CppCon 2020](https://youtu.be/pH-q2m5sb04)|
|3|Klaus Iglberger|Calling Functions: A Tutorial|[CppCon 2020](https://www.youtube.com/watch?v=GydNMuyQzWo)<br>[MUC++](https://www.youtube.com/watch?v=B9RT5sVunmk)|
|3|Rainer Grimm|40 Years Of Evolution <br>from Functions to Coroutines|[CppCon 2020](https://youtu.be/jd6P9X8l2bY)|
|3|Marc Mutz|Partially-Formed Objects <br>For Fun And Profit|-|

#### AMAs & Panels

|Day|Speaker|AMA/Panel|
|:-:|:-:|:-:|
|1|Jason Turner & Rob Irving|AMA|
|1|D&I|[Panel](https://www.youtube.com/watch?v=5Typh0bp2SY)|
|2|Hana Dusíková|AMA|
|3|Bjarne Stroustrup|AMA|
|3|Nicolai Josuttis|AMA|

## Top 2 Talks

For my favorite talks, I chose from talks that I hadn't already seen at a previous conference.

#### #1: Template Shenanigans: Testing, debugging and benchmarking template code

**Speaker:** [Jonathan O'Connor](https://twitter.com/ninkibah)<br>
**Link:** [Watch Here](https://www.youtube.com/watch?v=83fMx7Grxys) <br>

Alpacas! Sy Brand may have kittens, but Jonathan O'Connor has alpacas (and pointed out that I do not - at least for now). Alpacas aside, this talk was a distillation of resources for development and debugging tools for metaprogramming in C++. This is a subset of tools/techniques covered (there were many more):

* [Vittorio Romeo](https://twitter.com/supahvee1234)'s [Camomilla](https://github.com/SuperV1234/camomilla) (which Vittorio gave a [lightning talk on at CppCon 2019](https://www.youtube.com/watch?v=3dUZn3eloWE))
* An interactive template metaprogramming shell: [Metashall](http://metashell.org/)
* A gui for Metashell: [MSGUI](https://github.com/RangelReale/msgui)
* [Louis Dionne](https://twitter.com/LouisDionne)'s compile time framework for microprofiling: [metabench](https://github.com/ldionne/metabench)

<center><blockquote class="twitter-tweet"><p lang="en" dir="ltr">This was in response to <a href="https://twitter.com/ninkibah?ref_src=twsrc%5Etfw">@ninkibah</a> saying &quot;Conor Hoekstra ... doesn&#39;t have alpacas!&quot; 🦙🦙🦙 <a href="https://twitter.com/meetingcpp?ref_src=twsrc%5Etfw">@meetingcpp</a> <a href="https://t.co/zJ18hgyG1N">https://t.co/zJ18hgyG1N</a> <a href="https://t.co/ML8Pc7ZYn6">pic.twitter.com/ML8Pc7ZYn6</a></p>&mdash; Conor Hoekstra (@code_report) <a href="https://twitter.com/code_report/status/1327236748032815105?ref_src=twsrc%5Etfw">November 13, 2020</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script></center>

#### #2: Lambdas, uses and abuses

**Speaker:** Dawid Zalewski<br>
**Link:** [Watch Here](https://www.youtube.com/watch?v=Onv9w6FGwIQ) <br>

This was a continuation of Dawid's talk from Meeting C++2019, "Lambdas - the old, the new and the tricky" (which doesn't seem to be online yet). It quickly went from the basics and worked it's way up to implement the Y-Combinator using lambdas. A great talk that everyone should check out (as well as his 2019 talk when it goes online).

## Thank You

Thanks to the volunteers and organizers of the conference. It was great to meet and chat with C++ folks online.

Feel free to leave a comment on the [reddit thread](https://old.reddit.com/r/cpp/comments/juald6/meeting_c_2020_trip_report/).

<center>Hope to see you in person at a C++ conference in 2021 or 2022!</center>
