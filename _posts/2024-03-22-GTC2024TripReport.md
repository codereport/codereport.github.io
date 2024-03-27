---
layout: post
title: NVIDIA GTC 2024 Trip Report
categories: [GTC,Trip Report]
---

<center><p><b>🚧 THIS BLOG ENTRY IS UNDER CONSTRUCTION 🚧</b></p></center>

This will be a short "trip report" on the talks I watched over the week of the GTC 2024 (March 18 - 22). All talks are freely available online. You can read previous GTC trip reports here:

* [2023 GTC trip report](https://codereport.github.io/GTC2023TripReport/)
* [2022 GTC trip report](https://codereport.github.io/GTC2022TripReport/)

### Summary

| Speaker(s)  |                                                                                                     Talk                                                                                                      |
| :---------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|  Huang  ✅   | [🌟GTC 2024 Keynote with NVIDIA CEO Jensen Huang ![image](https://user-images.githubusercontent.com/36027403/159814936-5d2289c8-5ac5-4c04-b4b2-22b6f8f4b9a9.png)](https://www.youtube.com/watch?v=Y2F8yisiS6E) |
|    Dally    |                             🔥 [Fei-Fei Li and Bill Dally¹](https://register.nvidia.com/flow/nvidia/gtcs24/attendeeportaldigital/page/sessioncatalog/session/1690423197613001jzhz)                             |
|   Jones ✅   |                            [CUDA: New Features and Beyond](https://register.nvidia.com/flow/nvidia/gtcs24/attendeeportaldigital/page/sessioncatalog/session/1696033648682001S1DC)                             |
|   Lattner   |            [Unlocking Developer Productivity across CPU and GPU with Mojo](https://register.nvidia.com/flow/nvidia/gtcs24/attendeeportaldigital/page/sessioncatalog/session/1695673381291001GYwP)             |
| Catanzaro ✅ |                           [🔥 David Luan & Bryan Catanzaro²](https://register.nvidia.com/flow/nvidia/gtcs24/attendeeportaldigital/page/sessioncatalog/session/1706747368510001RGVh)                            |
|   Hemstad   |                                 [Mastering CUDA C++³](https://register.nvidia.com/flow/nvidia/gtcs24/attendeeportaldigital/page/sessioncatalog/session/1695315322330001eIye)                                  |
|  Bastien ✅  |                                  [What's New in JAX](https://register.nvidia.com/flow/nvidia/gtcs24/attendeeportaldigital/page/sessioncatalog/session/1696886819345001AqHd)                                   |
|   Shoham    |                            [🔥 Yoav Shoham & Vartika Singh⁴](https://register.nvidia.com/flow/nvidia/gtcs24/attendeeportaldigital/page/sessioncatalog/session/1709084371927001buHn)                            |

* 1 - The High-Speed Revolution in AI and Managing the Impact on Humanity
* 2 - The Future of AI and the Path to AGI
* 3 - Mastering CUDA C++: Modern Best Practices with the CUDA C++ Core Libraries
* 4 - Going Beyond LLMs, the Future of AI That Understands

✅ - I have watched

<!-- |      Jones       |                              [⭐ How to Write a CUDA Program](https://register.nvidia.com/flow/nvidia/gtcspring2023/attendeeportal/page/sessioncatalog/session/1666205357204001Efly)                              |
|       Buck       |             [Advances in Accelerated Computing for AI & Scientific Computing](https://register.nvidia.com/flow/nvidia/gtcspring2023/attendeeportal/page/sessioncatalog/session/1670537753408001LtOT)             |
|      Jones       |                         [⭐ CUDA: New Features and Beyond (2023)](https://register.nvidia.com/flow/nvidia/gtcspring2023/attendeeportal/page/sessioncatalog/session/1666224659650001N9mU)                          |
| Huang & Suskever | [⭐ Fireside Chat with Ilya Sutskever and Jensen Huang: AI Today and Vision of the Future](https://register.nvidia.com/flow/nvidia/gtcspring2023/attendeeportal/page/sessioncatalog/session/1669748941314001t6Nv) |
|     Lelbach      |                                [C++ Standard Parallelism](https://register.nvidia.com/flow/nvidia/gtcspring2023/attendeeportal/page/sessioncatalog/session/1666644507044001AzeW)                                 | -->

<br>

|                                                                                                                 |       Meaning        |
| :-------------------------------------------------------------------------------------------------------------: | :------------------: |
|                                                        🌟                                                        |       Keynote        |
|                                                        🔥                                                        |    Fireside Chat     |
| ![image](https://user-images.githubusercontent.com/36027403/159814936-5d2289c8-5ac5-4c04-b4b2-22b6f8f4b9a9.png) | Available on YouTube |

### Screenshot from "What's New in JAX?"

![image](https://github.com/codereport/jello/assets/36027403/41dbfd97-0148-49e1-882f-691f58ab43fa)

<!-- 

### [GTC Keynote](https://www.youtube.com/watch?v=DiGB5uAYKAg)

#### Speaker: Jensen Huang, CEO of NVIDIA

![image](https://user-images.githubusercontent.com/36027403/226699501-fc6d9377-3aa8-4ec4-a738-83f9582258c3.png)

### [How to Write a CUDA Program](https://register.nvidia.com/flow/nvidia/gtcspring2023/attendeeportal/page/sessioncatalog/session/1666205357204001Efly)

#### Speaker: Stephen Jones

This was a great talk, especially if you are new to CUDA. It walks you through a building a simple CUDA program in steps:

1. [Downloading CUDA and the CUDA toolkit](https://developer.nvidia.com/cuda-downloads)
2. Writing a "hello world" GPU kernel
3. Determining the number of blocks and threads for your kernel (image below)
   * When in doubt, use a block size of 256
   * Corollary: avoid block sizes smaller than 128 if you can
4. Using [NVIDIA Nsight Systems](https://developer.nvidia.com/nsight-systems) for profiling and analysis

![image](https://user-images.githubusercontent.com/36027403/226651965-66fc82fd-d13b-413f-a214-26177aa98d71.png)

### [⭐ CUDA: New Features and Beyond (2023)](https://register.nvidia.com/flow/nvidia/gtcspring2023/attendeeportal/page/sessioncatalog/session/1666224659650001N9mU)

#### Speaker: Stephen Jones

This is a summary of the latest and greatest things in CUDA and the CUDA ecosystem. Highlights include: 

* Overview of [cuNumeric](https://developer.nvidia.com/cunumeric) and Legate
* Overview of CUTLASS 3.0 and CuTe
* Overview of NVIDIA GPU Computing Tools

and much more!

![image](https://user-images.githubusercontent.com/36027403/226760336-25228af5-4374-4eb3-a9c4-17af5f842019.png)

### [C++ Standard Parallelism](https://register.nvidia.com/flow/nvidia/gtcspring2023/attendeeportal/page/sessioncatalog/session/1666644507044001AzeW)

#### Speaker: [Bryce Adelstein Lelbach](https://twitter.com/blelbach)

This talk is largely the same as Bryce's [GTC 2022 with the same name](https://youtu.be/1wFtONGVRI8). However, it has been updated, as shown by the slide below. ⬇️

![image](https://user-images.githubusercontent.com/36027403/228353941-d8663b87-af0c-4a1d-9dfd-c670ceafef2d.png) -->

