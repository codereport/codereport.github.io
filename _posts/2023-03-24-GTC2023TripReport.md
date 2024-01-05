---
layout: post
title: NVIDIA GTC 2023 Trip Report
categories: [GTC,Trip Report]
---

This will be a short "trip report" on the talks I watched over the week of the virtual GTC 2023 (March 20 - 24). All talks are freely available online. You can read [my GTC trip report from 2022 here](https://codereport.github.io/GTC2022TripReport/).

<br>

### Summary (Watched)

|    Speaker(s)    |                                                                                                       Talk                                                                                                       |
| :--------------: | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|      Huang       |  [🌟⭐GTC 2023 Keynote with NVIDIA CEO Jensen Huang ![image](https://user-images.githubusercontent.com/36027403/159814936-5d2289c8-5ac5-4c04-b4b2-22b6f8f4b9a9.png)](https://www.youtube.com/watch?v=DiGB5uAYKAg)  |
|      Jones       |                              [⭐ How to Write a CUDA Program](https://register.nvidia.com/flow/nvidia/gtcspring2023/attendeeportal/page/sessioncatalog/session/1666205357204001Efly)                              |
|       Buck       |             [Advances in Accelerated Computing for AI & Scientific Computing](https://register.nvidia.com/flow/nvidia/gtcspring2023/attendeeportal/page/sessioncatalog/session/1670537753408001LtOT)             |
|      Jones       |                         [⭐ CUDA: New Features and Beyond (2023)](https://register.nvidia.com/flow/nvidia/gtcspring2023/attendeeportal/page/sessioncatalog/session/1666224659650001N9mU)                          |
| Huang & Suskever | [⭐ Fireside Chat with Ilya Sutskever and Jensen Huang: AI Today and Vision of the Future](https://register.nvidia.com/flow/nvidia/gtcspring2023/attendeeportal/page/sessioncatalog/session/1669748941314001t6Nv) |
|     Lelbach      |                                [C++ Standard Parallelism](https://register.nvidia.com/flow/nvidia/gtcspring2023/attendeeportal/page/sessioncatalog/session/1666644507044001AzeW)                                 |

<br>

|                                                                                                                 |       Meaning        |
| :-------------------------------------------------------------------------------------------------------------: | :------------------: |
|                                                        🌟                                                        |       Keynote        |
|                                                        ⭐                                                        |      Best talks      |
| ![image](https://user-images.githubusercontent.com/36027403/159814936-5d2289c8-5ac5-4c04-b4b2-22b6f8f4b9a9.png) | Available on YouTube |


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

![image](https://user-images.githubusercontent.com/36027403/228353941-d8663b87-af0c-4a1d-9dfd-c670ceafef2d.png)

## Hope to See You Next Year!

This was my fourth virtual GTC I have "attended" since joining NVIDIA back in 2019. I've got my fingers crossed that in 2024 we will be able to attend in person and I can meet some of you there!

