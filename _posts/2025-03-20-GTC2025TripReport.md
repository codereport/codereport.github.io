---
layout: post
title: NVIDIA GTC 2025 Trip Report
categories: [GTC,Trip Report]
---

This will be a short "trip report" of the talks I watched over the week of the GTC 2025 (March 18 - 21). All talks are freely available online. You can read previous GTC trip reports here:

* [2024 GTC trip report](https://codereport.github.io/GTC2024TripReport/)
* [2023 GTC trip report](https://codereport.github.io/GTC2023TripReport/)
* [2022 GTC trip report](https://codereport.github.io/GTC2022TripReport/)

### Summary

|     Speaker(s)     |                                                                                                      Talk                                                                                                      |
| :----------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|       Huang        | [🌟⭐GTC 2025 Keynote with NVIDIA CEO Jensen Huang ![image](https://user-images.githubusercontent.com/36027403/159814936-5d2289c8-5ac5-4c04-b4b2-22b6f8f4b9a9.png)](https://www.youtube.com/watch?v=_waPvOwL9Z8) |
|    Bhat et al.     |                            [Accelerated Python: The Community and Ecosystem](https://register.nvidia.com/flow/nvidia/gtcs25/vap/page/vsessioncatalog/session/1727176757800001qp7T)                             |
|      Lelbach       |                                   [⭐ The CUDA C++ Developer’s Toolbox](https://register.nvidia.com/flow/nvidia/gtcs25/vap/page/vsessioncatalog/session/1727452471839001RhBW)                                   |
|     Armstrong      |                                     [What's CUDA All About Anyway? ](https://register.nvidia.com/flow/nvidia/gtcs25/vap/page/vsessioncatalog/session/1727452240578001KWZG)                                     |
|       Jones        |                                    [⭐ CUDA: New Features and Beyond](https://register.nvidia.com/flow/nvidia/gtcs25/vap/page/vsessioncatalog/session/1726614035480001yvEQ)                                     |
|    Goel et al.     |                              [Horizontal Scaling of LLM Training with JAX](https://register.nvidia.com/flow/nvidia/gtcs25/vap/page/vsessioncatalog/session/1728073363553001mzFs)                               |
|  Tillet & Miller   |                        [Blackwell Programming for the Masses With OpenAI Triton](https://register.nvidia.com/flow/nvidia/gtcs25/vap/page/vsessioncatalog/session/1727899732188001d9Fa)                         |
|       Riehl        |                                  [The CUDA Python Developer’s Toolbox](https://register.nvidia.com/flow/nvidia/gtcs25/vap/page/vsessioncatalog/session/1727174376274001QQQl)                                   |
|        Fang        |                              [⭐ 1,001 Ways to Write CUDA Kernels in Python](https://register.nvidia.com/flow/nvidia/gtcs25/vap/page/vsessioncatalog/session/1727175449007001EIKh)                              |
|     Evtushenko     |                                [⭐ How You Should Write a CUDA C++ Kernel](https://register.nvidia.com/flow/nvidia/gtcs25/vap/page/vsessioncatalog/session/1727453154835001sGzr)                                |
|      Maynard       |                               [Build CUDA Software at the Speed of Light](https://register.nvidia.com/flow/nvidia/gtcs25/vap/page/vsessioncatalog/session/1727452901850001PkH4)                                |
| Cecka & Awatramani |                            [Programming Blackwell Tensor Cores with CUTLASS](https://register.nvidia.com/flow/nvidia/gtcs25/vap/page/vsessioncatalog/session/1727748479221001aI91)                             |
|    Sun & Bando     |                       [Enable Tensor Core Programming in Python with CUTLASS 4.0](https://register.nvidia.com/flow/nvidia/gtcs25/vap/page/vsessioncatalog/session/1738891305735001ygGc)                        |

<br>

**Legend** | 🌟 - Keynote | ⭐ - Best talks | ![image](https://user-images.githubusercontent.com/36027403/159814936-5d2289c8-5ac5-4c04-b4b2-22b6f8f4b9a9.png) - Available on YouTube

### Highlights and Thoughts

#### Jensen's Keynote

I tweeted this while recording ADSP Episodes 226-228.

<blockquote class="bluesky-embed" data-bluesky-uri="at://did:plc:iyuh5mhvphwyxordfys7nth4/app.bsky.feed.post/3lksx3onrz22q" data-bluesky-cid="bafyreihpofnlan7jkfx3ataphmcknjclngipvodibklzomtfwg5g3a66zq" data-bluesky-embed-color-mode="system"><p lang="en">Jensen vs Bryce<br><br><a href="https://bsky.app/profile/did:plc:iyuh5mhvphwyxordfys7nth4/post/3lksx3onrz22q?ref_src=embed">[image or embed]</a></p>&mdash; Conor Hoekstra (<a href="https://bsky.app/profile/did:plc:iyuh5mhvphwyxordfys7nth4?ref_src=embed">@codereport.bsky.social</a>) <a href="https://bsky.app/profile/did:plc:iyuh5mhvphwyxordfys7nth4/post/3lksx3onrz22q?ref_src=embed">March 20, 2025 at 10:50 AM</a></blockquote><script async src="https://embed.bsky.app/static/embed.js" charset="utf-8"></script>

Here is the standalone slide from Jensen's deck.

![image](https://github.com/user-attachments/assets/7644e99f-4682-4704-9349-aa55c6f1adc9)

#### [Accelerated Python: The Community and Ecosystem](https://register.nvidia.com/flow/nvidia/gtcs25/vap/page/vsessioncatalog/session/1727176757800001qp7T)
##### Speakers: Anshuman Bhat, Jeremy Tanner, Andy Terrel

This talk covers Python initiatives at NVIDIA. Pretty crazy to think that the first decade of GPU Python initiatives all started outside of NVIDIA.

![Screenshot from 2025-03-19 15-06-45](https://github.com/user-attachments/assets/cad15527-748a-4754-84c1-7db6acbad252)

#### [The CUDA C++ Developer’s Toolbox](https://register.nvidia.com/flow/nvidia/gtcs25/vap/page/vsessioncatalog/session/1727452471839001RhBW)
##### Speaker: Bryce Adelstein Lelbach

Screenshots from Bryce's talk.

![image](https://github.com/user-attachments/assets/5ba83609-c718-4f9f-9a9a-018c0482c23f)
![Screenshot from 2025-03-20 02-07-19](https://github.com/user-attachments/assets/77faf64c-c628-4940-b74a-60f626f94bfe)
![Screenshot from 2025-03-20 02-08-48](https://github.com/user-attachments/assets/d523231a-6b03-4171-abb1-a4457791ea15)
![Screenshot from 2025-03-20 02-12-57](https://github.com/user-attachments/assets/78680651-88a5-42d4-999b-28027e0fe47e)
![Screenshot from 2025-03-20 02-22-46](https://github.com/user-attachments/assets/699f41a5-3e58-4749-88c1-3bba47ca839b)

#### [What's CUDA All About Anyway?](https://register.nvidia.com/flow/nvidia/gtcs25/vap/page/vsessioncatalog/session/1727452240578001KWZG)
##### Speaker: Rob Armstrong

This image is similar to the 2nd screenshot from Bryce's talk above. Rob also notes that Stephen has a slide in his talk covering the same thing. So 3 different slides for the same ecosystem (4 if you include Jensen's slide).

![image](https://github.com/user-attachments/assets/fc05a9a5-4336-4c2e-be0a-4120f81f5d25)

#### [CUDA: New Features and Beyond](https://register.nvidia.com/flow/nvidia/gtcs25/vap/page/vsessioncatalog/session/1726614035480001yvEQ)
##### Speaker: Stephen Jones

This seems to be the slide that Rob (Armstrong) referred to.

![image](https://github.com/user-attachments/assets/04c3d60b-2121-4373-b4a0-7bcf45c1f4b6)

And a Python version of this graphic:

![image](https://github.com/user-attachments/assets/23fc4e90-5700-4c0d-9cf5-9c7584e5dbba)

And a slightly different graphic for kernel authoring:

![image](https://github.com/user-attachments/assets/dbb39424-7f71-4227-af9f-2a3bc24b38d8)

#### [Blackwell Programming for the Masses With OpenAI Triton](https://register.nvidia.com/flow/nvidia/gtcs25/vap/page/vsessioncatalog/session/1727899732188001d9Fa)
##### Speakers: Phil Tillet & dePaul Miller

An interesting graphic showing where OpenAI Triton sits between PyTorch and CUDA C++ for authoring kernels.

![image](https://github.com/user-attachments/assets/23a03a78-2111-4020-ba32-9b1c6369f8f6)

#### How You Should Write a CUDA C++ Kernel
##### Speakers: Georgii Evtushenko

This is a fantastic talk. Walks you through how to handroll your own `transform` kernel using `nvbench` while comparing it to speed of light `thrust::transform`. A must watch.
