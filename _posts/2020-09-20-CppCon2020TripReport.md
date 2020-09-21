---
layout: post
title:  CppCon 2020 Trip Report
categories: [C++,CppCon,Trip Report]
---

This was my second time attending [CppCon](https://twitter.com/CppCon). The first time I attended was in 2019, when I gave my first CppCon presentation in two parts, [Algorithm Intuition](https://www.youtube.com/watch?v=pUEnO6SvAMo) - although I personally recommend the [C++Now 2019 version](https://www.youtube.com/watch?v=48gV1SNm3WA) which is 30 minutes shorter. 

This year I gave one lightning talk, **SICP Cover Demystified**  and one full length talk, **Structure and Interpretation of Computer Programs: SICP**, which focuses on the textbook of the same name (which is [available online for free](https://web.mit.edu/alexmv/6.037/sicp.pdf)) - which has been touted as:
> "The best computer science book in the world." 
> <br>\- Brian Harvey in [Why SICP Matters](https://people.eecs.berkeley.edu/~bh/sicp.html)

I will update this blog with links to the YouTube videos when they become available. You can see a preview of some of the code samples in the tweet below.

<center><blockquote class="twitter-tweet"><p lang="en" dir="ltr">For pinning 🙂 <a href="https://t.co/y2Cgujl9jd">https://t.co/y2Cgujl9jd</a></p>&mdash; Conor Hoekstra (@code_report) <a href="https://twitter.com/code_report/status/1307139063376424960?ref_src=twsrc%5Etfw">September 19, 2020</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script></center>

## Diversity Spotlight

As [Bryce Adelstein Lelbach](https://twitter.com/blelbach) has said [in many of his talks](https://youtu.be/zoMZAV6FEbc?t=48)... 

>C++ has a diversity problem.

I finished writing this trip report without this section. Upon reviewing it, I realized that the overwhelming majority of the speakers mentioned in my blog were male. I was curious if this was my bias, and so I went and tallied up the talks with a female speaker - the total came to **6.9% (6/87)**. From now on, I will highlight some aspect of diversity in all of my Trip Reports - in hopes that we can track improvement over time.

I should also mention that I slipped up at the beginning of my talk when I said "I hope you **guys** have enjoyed the conference just as much as I have." I do my best to avoid referring to groups of people as guys but I failed on this occasion (and others). I apologize if I offended anyone - it was unintentional and I will continue to do my best not too.

## Overall Thoughts

It is hard for the virtual CppCon 2020 to compare to my first CppCon in 2019. For me, the best part of CppCon is a "subset" of the hallway track: the lunches and the dinners, where you get to have more personal conversations with those you are dining with. On top of that, CppCon 2019 was where I met so many of my "speaker-heroes" for the first time - I had lunch with [Tony Van Eerd](https://twitter.com/tvaneerd), whose [Words of Wisdom](https://www.youtube.com/watch?v=GgnKycitKyc) and [Postmodern C++](https://www.youtube.com/watch?v=GPP64opjy_Y) are two of my favorite talks. I met [Kate Gregory](https://twitter.com/gregcons) for the first time and thanked her for letting me "steal her words" (see [Episode 30](https://cppcast.com/kate-gregory-stop-teaching-c/) of CppCast) for the title of my first (and second) talk. I went on the CppCon Field trip where I realized that the tall person I was competing with on some video game was [Rob Irving](https://twitter.com/robwirving), co-host and creator of [CppCast](https://cppcast.com/). I could go on and on.

All of that being said, the virtual conference was very enjoyable. Somehow it was just as exhausting as the in-person conference. The highlight for me was the hallway track. When you were able to join a good table/conversation where most people had their video cams on, it was reminiscent of being at an in-person conference. There were, in fact, a number of advantages to having the conference virtual. I try to enumerate some of the pros & cons below.

**Pros of virtual:**
* Ability to watch talks at 1.5x to 2.0x speed
* Increased accessibility: enables certain attendees to participate that might not have been able to travel to in-person conference
* Ability to watch talks that you missed as soon as you would like as private YouTube links are immediately provided to attendees
* Decreased cost for attendees / companies

**Cons of virtual:**
* Time-zone isn't convenient for all global attendees
* No break longer than 30 minutes between talks (due to time-zone considerations)
* Fatigue from sitting in one place for so long (it is nice to walk to different presentation rooms)
* No lunches / dinners with other attendees (where the more personal conversations take place)
* Fewer "random encounters/conversations" take place
* Attendees both working and attending the conference, see poll below

<center><blockquote class="twitter-tweet"><p lang="en" dir="ltr">Are you virtually attending CppCon next week? And if so, are you planning to devote the week to the conference like you were there in real life, or work while attending talks?</p>&mdash; Jason Turner (@lefticus) <a href="https://twitter.com/lefticus/status/1304502821086269440?ref_src=twsrc%5Etfw">September 11, 2020</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script></center>

Overall, given that this was the first virtual CppCon, it was a major success. I look forward to seeing the improvement in virtual platforms like Remo and what they will be able to offer in the future.

## Top 4 Talks

Here are my picks for top four talks (of the ones I have watched - note at this point I have only watched 25/87 talks) for CppCon 2020. Note that my rankings are entirely biased - I am generally most interested in talks that focus on the following:

* Algorithms
* Functional programming
* Programming languages

Please keep that in mind while reading through the list

#### Summary

||Speaker|Talk|
|:-:|:-:|:-:|
|1|David Sankel|Monoids, Monads, and Applicative Functors|
|2|Ben Deane|Constructing Generic Algorithms|
|3|Sy Brand|Building an Intuition for Composition|
|4|Emery Berger|Performance Matters|

#### #1: Monoids, Monads, and Applicative Functors: Repeated Software Patterns

**Speaker:** [David Sankel](https://twitter.com/david_sankel)<br>
**Link:** To be updated in the future <br>
**Previously presented:** [C++Now 2016](https://www.youtube.com/watch?v=DiisKQAkGM4)

This talk is absolutely awesome. I was not expecting it to be "as good" as the other live talks as it was prerecorded - but boy was I in for a surprise. The first several minutes is given in a kind of infomercial (think [Slap Chop](https://www.youtube.com/watch?v=FqWgTM4di4s)) style which is highly entertaining. Then at around the 8 minute mark, he introduces his kids as the audience members and asks them if his explanation of a [Monoid](https://en.wikipedia.org/wiki/Monoid_(category_theory)) makes sense to them. I literally laughed out loud. His kids are adorable and will make sitting through an introductory talk on [Category Theory](https://en.wikipedia.org/wiki/Category_theory) enjoyable for anyone. Note that I highly recommend the updated version of the talk due to 1) the entertainment factor and 2) the fact that the C++Now 2016 has very poor video/audio quality.

<center><blockquote class="twitter-tweet"><p lang="en" dir="ltr">This has to be best talk of <a href="https://twitter.com/CppCon?ref_src=twsrc%5Etfw">@CppCon</a> 2020, the (pre-recorded) &quot;Monoids, Monads, and Applicative Functors: Repeated Software Patterns&quot; by <a href="https://twitter.com/david_sankel?ref_src=twsrc%5Etfw">@david_sankel</a> with his kids (I assume) as the audience members being confused / amazed by <a href="https://twitter.com/hashtag/functionalprogramming?src=hash&amp;ref_src=twsrc%5Etfw">#functionalprogramming</a>! A MUST WATCH ❤️🤣😂 <a href="https://t.co/tZCOvxcZ3z">pic.twitter.com/tZCOvxcZ3z</a></p>&mdash; Conor Hoekstra (@code_report) <a href="https://twitter.com/code_report/status/1306682908741165057?ref_src=twsrc%5Etfw">September 17, 2020</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script></center>

#### #2: Constructing Generic Algorithms: Principles and Practice

**Speaker:** [Ben Deane](https://twitter.com/ben_deane)<br>
**Link:** To be updated in the future <br>
**Previously presented:** [MUC++ Meetup](https://www.youtube.com/watch?v=jCfbyjAyAKU)

This is a talk that I had actually seen twice before: once from a unlisted YouTube link for the [North Denver Metro C++ Meetup](https://www.meetup.com/North-Denver-Metro-C-Meetup/) [YouTube channel](https://www.youtube.com/channel/UCK5v1dZu2AjHfHLIKTG8dPw/featured) and once at the [MUC++ Meetup](https://www.youtube.com/watch?v=jCfbyjAyAKU). If you have seen any of my previous talks, you will know two things: 1) I love algorithms 2) I am a huge fans of Ben Deane's talks (see a full list of his talks [here](https://www.youtube.com/playlist?list=PLVFrD1dmDdvea7aPDCrp9A1EAU3DLw7GE)). One of my favorite talks of all time was his [C++Now 2018 Easy to Use, Hard to Misuse](https://youtu.be/2ouxETt75R4) which ended up winning [Best Presentation](https://cppnow.org/announcements/2018/05/announcing-cpp-now-2019/) of the conference. His talk this year will walk you through how to iterate on designing a generic algorithm in the spirit of Alexander Stepanov and the STL.

#### #3: Building an Intuition for Composition

**Speaker:** [Sy Brand](https://twitter.com/TartanLlama)<br>
**Link:** To be updated in the future <br>
**Previously presented:** N/A

This talk is a fantastic introduction to category theory (although that might not be clear from the title of the talk). Sy starts off slow and eases you into monoids, functors and monads with easy to understand examples. They make it clear that they understand that these concepts can be difficult to grasp. They say at one point:

> I wanted to learn, I wanted to teach myself these things... The point of this talk was to be the kind of talk that I needed when I was trying to teach myself a lot of these concepts from these branches of mathematics and just completely failing.

I highly recommend for anyone interested in dipping their toe into the "category theory" water.

#### #4: Performance Matters

**Speaker:** [Emery Berger](https://twitter.com/emeryberger)<br>
**Link:** To be updated in the future <br>
**Previously presented:** [Strange Loop 2019](https://www.youtube.com/watch?v=r-TLSBdHe1A)

This talk would have been higher on the list but I had already seen it before as it had been presented previously at another conference - which is surprising for a keynote. Emery gave a [talk at CppCon 2019](https://www.youtube.com/watch?v=XRAP3lBivYM) which was very good - and after this I went and tracked down his other talks. This led me to the previously given version of this talk. It currently is the 3rd most viewed video on the [Strange Loop YouTube Channel](https://www.youtube.com/c/StrangeLoopConf/videos) with 154K views (as of Sept. 20, 2020). Although it is #4 on the list - I highly recommend everyone watch it. It will make you re-think your perspective on profiling. When I watched it the first time, it made me think twice about the performance results that [Andrei Alexandrescu](https://twitter.com/incomputable) showed in his CppCon 2019 talk [Speed Is Found In The Minds of People](https://www.youtube.com/watch?v=FJJTYQYB1JQ). I would also like to thank Emery for using monospace fonts for his code samples (something that the majority of the keynote speakers didn't do).

## Other Thoughts

**Keynotes**

There were five keynotes as usual this year.

|Keynote Speaker|Talk|Previously Presented|
|:-:|:-:|:-:|
|Bjarne Stroustrup|The Beauty and Power of "Primitive" C++|-|
|Marc Gregoire|C++20: An (Almost) Complete Overview|-|
|Emery Berger|Performance Matters|[Strange Loop 2019](https://www.youtube.com/watch?v=r-TLSBdHe1A)|
|Lisa Lippincott|Neighborhoods Banding Together|-|
|Herb Sutter|Empirically Measuring & Reducing<br> C++’s Accidental Complexity|[Avast Prague Meetup](https://www.youtube.com/watch?v=qx22oxlQmKc) <br> [ACCU Autumn 2019](https://conference.accu.org/previous/2019_autumn/sessions/#XQuantifyingAccidentalComplexityAnEmpiricalLookatTeachingandUsingC)|

The keynotes were enjoyable as always. Emery Berger's was my personal favorite, and Lisa Lippincott's was my runner up. My one comment on the keynotes is that 3 of the 5 keynote presenters don't use monospace fonts in their slide decks. I find it hard to focus on code that isn't in monospace font; all I can think is "why isn't this in a monospace font." 

**Honorable Mention**

My honorable mention talk list is below. I will update this list as I work my way through the backlog of talks that I haven't yet watched.

* Template Metaprogramming: Type Traits - Jody Hagins
* Just-in-Time Compilation - JF Bastien
* Just-in-Time Compilation: The Next Big Thing? - Ben Deane & Kris Jusiak
* Back to Basics: Algebraic Data Types - Arthur O'Dwyer
* C++20 STL Features: One Year of Development on GitHub - Stephan T. Lavavej
* C++20 Ranges in Practice - Tristan Brindle
* How C++20 Changes the Way We Write Code - Timur Doumler
* OO Considered Harmful - Phil Nash 

**Lightning Talks**

My top five lightning talks were:

* Drinking from the Fire Hose - Brian Ruth
* How We Used To Be - [Ben Deane](https://twitter.com/ben_deane)
* A picture is worth a thousand words - [Honey Sukesan](https://twitter.com/HSukesan)
* How to Cook a Chicken - [Sy Brand](https://twitter.com/TartanLlama)
* Reasoning with function signatures - Gabriel Aubut-Lussier

It is awesome to see first-time attendees (like Honey) stepping up to give a lightning talk! And Gabriel's talk made the top five because his cat was a co-presenter 😂.

**NVIDIA is hiring!**

And finally, as I mentioned in my CppCon talk, NVIDIA is always looking for top talent. Head over to [NVIDIA Careers](https://www.nvidia.com/en-us/about-nvidia/careers/) to see all our openings. If you are interested in joining the RAPIDS C++ team, check out our posting [here](https://nvidia.wd5.myworkdayjobs.com/en-US/NVIDIAExternalCareerSite/job/US-CA-Santa-Clara/Senior-Software-Engineer--Accelerated-Data-Analytics---GPU_JR1932990-1) (if this link goes stale, visit the [NVIDIA Careers](https://www.nvidia.com/en-us/about-nvidia/careers/) site and search **RAPIDS "Software Engineer"**).

## Thank You

A huge thank you to [Jon Kalb](https://twitter.com/_JonKalb), the organizing committee and all of the volunteers who worked extra hard this year. It was awesome to have CppCon happen virtually in the midst of such a challenging year.

Feel free to leave a comment on the [reddit thread](https://old.reddit.com/r/cpp/comments/ix0e1l/cppcon_2020_trip_report/).

<center>Hope to see you in person at a C++ conference in 2021!</center>
