---
layout: post
title: NVIDIA GTC 2022 Trip Report
categories: [GTC,Trip Report]
---

This will be a ~~short~~ "trip report" on the talks I watched over the week of the virtual GTC 2022 (March 21 - 24). All talks a freely available online.

### Summary

|Speaker(s)|Talk|
|:-:|:-:|
|Larkin|[⭐ No More Porting: Coding for GPUs with ISO C++, Fortran, and Python](https://reg.rainfocus.com/flow/nvidia/gtcspring2022/aplive/page/ap/session/1637347431411001IRfd)|
|Jones|[⭐ How CUDA Programming Works](https://reg.rainfocus.com/flow/nvidia/gtcspring2022/aplive/page/ap/session/16372907317160016bDB)|
|AH & MM|[⛔ Deep Dive into GPU-accelerated Big Data and DS Technologies](https://reg.rainfocus.com/flow/nvidia/gtcspring2022/aplive/page/ap/session/1639159624485001KeMt)|
|Huang|[🌟⭐ GTC 2022 Keynote with NVIDIA CEO Jensen Huang ![image](https://user-images.githubusercontent.com/36027403/159814936-5d2289c8-5ac5-4c04-b4b2-22b6f8f4b9a9.png)](https://www.youtube.com/watch?v=39ubNuxnrK8)|
|Costa|[⭐ A Deep Dive into the Latest HPC Software](https://reg.rainfocus.com/flow/nvidia/gtcspring2022/aplive/page/ap/session/1637338932019001yA05)|
|GP & MA|[Inside the NVIDIA Hopper Architecture](https://www.nvidia.com/gtc/session-catalog/?search=Hopper&tab.scheduledorondemand=1583520458947001NJiE&search=Hopper#/session/1644354440262001BZNv)|
|Jones|[⭐ CUDA: New Features and Beyond](https://reg.rainfocus.com/flow/nvidia/gtcspring2022/aplive/page/ap/session/1637286764806001dtJj)|
|Lelbach|[⭐ C++ Standard Parallelism ![image](https://user-images.githubusercontent.com/36027403/159814936-5d2289c8-5ac5-4c04-b4b2-22b6f8f4b9a9.png)](https://youtu.be/1wFtONGVRI8)|
|GT & VM|[⛔ Optimizing CUDA Applications for NVIDIA Hopper Architecture](https://reg.rainfocus.com/flow/nvidia/gtcspring2022/aplive/page/ap/session/16373134932300012k2M)|
|MC & NG|[Accelerating PyTorch with Native CUDA Graphs Support](https://events.rainfocus.com/widget/nvidia/gtcspring2022/sessioncatalog/session/1638833046344001X1tZ)|
|Enemark|[⭐ Scaling Web and Visualization Apps with GPUs](https://reg.rainfocus.com/flow/nvidia/gtcspring2022/aplive/page/ap/session/1639779978640001b7km)|
|MA, AD, NB|[Large-scale Machine Learning with Snowflake and RAPIDS](https://reg.rainfocus.com/flow/nvidia/gtcspring2022/aplive/page/ap/session/16385568434230010NKr)|
|Hammond|[⭐ Shifting through the Gears of GPU Programming](https://reg.rainfocus.com/flow/nvidia/gtcspring2022/aplive/page/ap/session/1638453336105001vPx8)|
|CWE|[⭐ Standard and CUDA C++ User Forum](https://reg.rainfocus.com/flow/nvidia/gtcspring2022/aplive/page/ap/session/1638815023541001evyQ)
|CWE|[👋 Thrust, CUB, and libcu++ User Forum](https://www.nvidia.com/gtc/session-catalog/?search=CWE41948)
|CWE|[NVCC CUDA Compiler Toolchain](https://reg.rainfocus.com/flow/nvidia/gtcspring2022/aplive/page/ap/session/1638579379537001IMpK)|
|Panel|[⭐ Future of Standard and CUDA C++](https://reg.rainfocus.com/flow/nvidia/gtcspring2022/aplive/page/ap/session/1638830085320001YWIE)|

<br>

||Meaning|
|:-:|:-:|
|🌟|Keynote|
|⭐|Best talks / CWEs|
|👋|I participated in|
|⛔|Bad audio / don't watch|
|![image](https://user-images.githubusercontent.com/36027403/159814936-5d2289c8-5ac5-4c04-b4b2-22b6f8f4b9a9.png)|Available on YouTube|
|CWE|**C**onnect **W**ith the **E**xperts (Panel Q&A)|

### [⭐ No More Porting: Coding for GPUs with ISO C++, Fortran, and Python](https://reg.rainfocus.com/flow/nvidia/gtcspring2022/aplive/page/ap/session/1637347431411001IRfd)

#### Speaker: Jeff Larkin

This was an awesome talk, one of my favorites of the conference. It shows multiple examples of refactoring code from C++ with OpemMP/OpenACC to Standard C++. The refactoring code is always cleaner, smaller and faster. The talks also gives a couple algorithm tips when refactoring, such as preferring `std::transform_reduce` to `std::trasform` + `std::reduce`.

![image](https://user-images.githubusercontent.com/36027403/159341504-f1072e7c-80e1-4e0e-af53-b238ee920930.png)
![image](https://user-images.githubusercontent.com/36027403/159341792-b997229c-8473-44df-ad08-bef982303fbf.png)
![image](https://user-images.githubusercontent.com/36027403/159342041-f62cdc05-e97a-4819-b650-d19f0001395a.png)
![image](https://user-images.githubusercontent.com/36027403/159342316-3149aa0d-5571-4273-abe9-20197e51edb0.png)

### [⭐ How CUDA Programming Works](https://reg.rainfocus.com/flow/nvidia/gtcspring2022/aplive/page/ap/session/16372907317160016bDB)

#### Speaker: Stephen Jones

This was a summary of not just **how** CUDA programming but **why** it works the way it does. If you have ever been curious of what a grid, warp, (thread) block or thread is and how that relates to CUDA programming and writing CUDA kernels, this is the talk for you.

![image](https://user-images.githubusercontent.com/36027403/159525764-aca5bee8-dcc4-41fe-9382-eaf1dd51c09b.png)
![image](https://user-images.githubusercontent.com/36027403/159525889-05882be5-48ae-426b-b5e8-27b88307f3bc.png)

### [⭐ Standard and CUDA C++ User Forum](https://reg.rainfocus.com/flow/nvidia/gtcspring2022/aplive/page/ap/session/1638815023541001evyQ)

If you are interested in either Standard C++ or CUDA C++, this CWE is worth a watch. Some of the "experts" come and go as they split off into separate 1-on-1 rooms, but many of the panelists remain in the main room to answer audience questions.

#### Panelists:

![image](https://user-images.githubusercontent.com/36027403/160424321-e330fb13-7c92-42f7-ba5e-451baa4ab5eb.png)


### [🌟⭐ GTC 2022 Keynote with NVIDIA CEO Jensen Huang ![image](https://user-images.githubusercontent.com/36027403/159814936-5d2289c8-5ac5-4c04-b4b2-22b6f8f4b9a9.png)](https://www.youtube.com/watch?v=39ubNuxnrK8)

#### Speaker: Jensen Huang, CEO of NVIDIA

The keynote was awesome (as always). It started out with a "virtual fly through" of NVIDIA HQ in Santa Clara. It looks surreal but that is actually what HQ looks like (minus the robots trapped in the basement). JHH designed it to feel like a futuristic spaceship. I always feel inspired after watching Jensen keynotes. Key announcements:

* [NVIDIA Announces Hopper Architecture, the Next Generation of Accelerated Computing](https://nvidianews.nvidia.com/news/nvidia-announces-hopper-architecture-the-next-generation-of-accelerated-computing?ncid=so-yout-835293&sfdcid=undefined#cid=gtcs22_so-yout_en-us)
* [NVIDIA Announces DGX H100 Systems – World’s Most Advanced Enterprise AI Infrastructure](https://nvidianews.nvidia.com/news/nvidia-announces-dgx-h100-systems-worlds-most-advanced-enterprise-ai-infrastructure?ncid=so-yout-469678&sfdcid=undefined#cid=gtcs22_so-yout_en-us)
* [NVIDIA Introduces Grace CPU Superchip](https://nvidianews.nvidia.com/news/nvidia-introduces-grace-cpu-superchip?ncid=so-yout-373335&sfdcid=undefined#cid=gtcs22_so-yout_en-us)
* [NVIDIA Introduces 60+ Updates to CUDA-X Libraries, Opening New Science and Industries to Accelerated Computing](https://nvidianews.nvidia.com/news/nvidia-introduces-60+-updates-to-cuda-x-libraries-opening-new-science-and-industries-to-accelerated-computing?ncid=so-yout-811963&sfdcid=undefined#cid=gtcs22_so-yout_en-us)
* [NVIDIA Announces Digital Twin Platform for Scientific Computing](https://nvidianews.nvidia.com/news/nvidia-announces-digital-twin-platform-for-scientific-computing)

### [⭐ A Deep Dive into the Latest HPC Software](https://reg.rainfocus.com/flow/nvidia/gtcspring2022/aplive/page/ap/session/1637338932019001yA05)

#### Speaker: [Tim Costa](https://twitter.com/timothybcosta)

This was another great talk. This talk has some overlap with the [No More Porting](https://reg.rainfocus.com/flow/nvidia/gtcspring2022/aplive/page/ap/session/1637347431411001IRfd) talk but most of it is different. The highlight (for me at least) was the example of Maxwell's equation using [Senders and Receivers](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2022/p2300r4.html) (a C++ proposal that looks like it will go into C++ early in the C++26 cycle). I am really looking forward to the new paradigm that senders & receivers will unlock for C++. 

![image](https://user-images.githubusercontent.com/36027403/159545703-88537eb2-550a-47ec-8fca-df5040dec32b.png)
![image](https://user-images.githubusercontent.com/36027403/159545413-1b06ed0a-8b9c-43ca-b271-a5009015119b.png)

### [⭐ CUDA: New Features and Beyond](https://reg.rainfocus.com/flow/nvidia/gtcspring2022/aplive/page/ap/session/1637286764806001dtJj)

#### Speaker: Stephen Jones

Another great CUDA talk from Stephen Jones. This talk covers how the architecture changes of Hopper will affect how you program GPUs with CUDA. Specifically, the Hopper architecture introduces the Thread Block Cluster and Cluster Distributed Shared Memory. You can get a high level introduction to it in Stephen's talk and for a deeper dive, you can check out [Optimizing CUDA Applications for NVIDIA Hopper Architecture](https://reg.rainfocus.com/flow/nvidia/gtcspring2022/aplive/page/ap/session/16373134932300012k2M) (note: this is one of the talks that has pretty bad audio, so if you are reading this in the future - it might be worth googling to see if the talk has been given again with better audio quality).

![image](https://user-images.githubusercontent.com/36027403/159725085-e4379c63-6e43-4cd4-b380-f29670b0c00b.png)
![image](https://user-images.githubusercontent.com/36027403/159725235-90eabe64-cc7c-49bf-bfd4-bfddc8d3b643.png)

### [⭐ C++ Standard Parallelism](https://youtu.be/1wFtONGVRI8)

#### Speaker: [Bryce Adelstein Lelbach](https://twitter.com/blelbach)

Bryce always gives great talks and always has some of the nicest slide decks. I have seen different versions of this talk before but there are a few new things in this talk. If you've watched Jeff's [No More Porting](https://reg.rainfocus.com/flow/nvidia/gtcspring2022/aplive/page/ap/session/1637347431411001IRfd) talk or Tim's [A Deep Dive into the Latest HPC Software](https://reg.rainfocus.com/flow/nvidia/gtcspring2022/aplive/page/ap/session/1637338932019001yA05) you will recognize some of the examples. However, most of the content is totally different and there are tons of awesome modern C++ examples. My favorite example is probably using `std::transform_reduce` to get a word count in parallel.

For the sake of transparency, I should state that Bryce and I have a [podcast](https://adspthepodcast.com/) together. 

![image](https://user-images.githubusercontent.com/36027403/160429832-f5c53750-9dc9-48cf-b982-49900533cbc0.png)

### [⭐ Shifting through the Gears of GPU Programming](https://reg.rainfocus.com/flow/nvidia/gtcspring2022/aplive/page/ap/session/1638453336105001vPx8)

#### Speaker: [Jeff Hammond](https://twitter.com/science_dot)

This might be my favorite talk of the conference as it was the only talk that I tweeted about during the conference. Jeff takes you through a whirlwind history of GPU computing and then compares different models / languages for accelerating your code on GPUs and compares to see which is fastest over three different examples. Definitely worth the watch if you have 30 minutes (or 15 minutes on 2x).

![image](https://user-images.githubusercontent.com/36027403/159998921-b1db31c3-c4b3-41d4-a188-53dd29d666ed.png)

<center>
<blockquote class="twitter-tweet"><p lang="en" dir="ltr">One of the highlights of <a href="https://twitter.com/NVIDIAGTC?ref_src=twsrc%5Etfw">@NVIDIAGTC</a> 2022 was <a href="https://twitter.com/science_dot?ref_src=twsrc%5Etfw">@science_dot</a>&#39;s talk comparing CUDA <a href="https://twitter.com/hashtag/Python?src=hash&amp;ref_src=twsrc%5Etfw">#Python</a>, CUDA C++, CUDA <a href="https://twitter.com/hashtag/Fortran?src=hash&amp;ref_src=twsrc%5Etfw">#Fortran</a>, CuPy, Standard C++, OpenMP, OpenACC, and so much more! If you are curious which gets you the most perf, check it out: <a href="https://t.co/pEWaNzEOe4">https://t.co/pEWaNzEOe4</a> <a href="https://twitter.com/hashtag/cpp?src=hash&amp;ref_src=twsrc%5Etfw">#cpp</a> <a href="https://twitter.com/hashtag/cuda?src=hash&amp;ref_src=twsrc%5Etfw">#cuda</a> <a href="https://t.co/TIhvGR8bhE">pic.twitter.com/TIhvGR8bhE</a></p>&mdash; Conor Hoekstra (@code_report) <a href="https://twitter.com/code_report/status/1507099684841693192?ref_src=twsrc%5Etfw">March 24, 2022</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
</center>

### [⭐ Future of Standard and CUDA C++](https://reg.rainfocus.com/flow/nvidia/gtcspring2022/aplive/page/ap/session/1638830085320001YWIE)

Last but not least, this panel was definitely my favorite panel / CWE of GTC 2022. It doesn't list her below but [Daisy Hollman](https://twitter.com/The_Whole_Daisy) of Google and formerly Sandia National Labs was on the panel as well. It was super interesting to hear the thoughts of both NVIDIAns and non-NVIDIAns about the future of standard C++ and parallel compute. There were some pretty interesting exchanges. I would definitely recommend this talk if you are interested.

![image](https://user-images.githubusercontent.com/36027403/160431115-91af6fcc-e020-4c7e-9f47-ade3ea1846f6.png)

## Hope to See You Next Year!

This was my third virtual GTC I have "attended" since joining NVIDIA back in 2019. I've got my fingers crossed that in 2023 we will be able to attend in person and I can meet some of you there!

Feel free to leave a comment on the [reddit thread](https://old.reddit.com/r/nvidia/comments/tqfm1g/nvidia_gtc_2022_trip_report/?).
