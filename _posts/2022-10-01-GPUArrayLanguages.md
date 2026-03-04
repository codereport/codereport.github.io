---
layout: post
title: GPU Array Languages, Compiler & Libraries
categories: [Programming Languages, Array Languages, GPU]
---

![image](https://user-images.githubusercontent.com/36027403/193055974-8d8008a2-a1e6-4bd4-8ecc-7624fa611f25.png)

On the most recent episode of [ArrayCast](https://www.arraycast.com/), we interviewed [Troels Henriksen](https://sigkill.dk/) about [the Futhark Programming Language](https://futhark-lang.org/). From the website, "Futhark is a statically typed, data-parallel, and purely functional array language in the ML family, and comes with a heavily optimising ahead-of-time compiler that presently generates either GPU code via CUDA and OpenCL, or multi-threaded CPU code."

<div id="buzzsprout-player-18617090"></div><script src="https://www.buzzsprout.com/2592851/episodes/18617090-troels-henriksen-and-futhark.js?container_id=buzzsprout-player-18617090&player=small" type="text/javascript" charset="utf-8"></script>

While talking to Troels about accelerating array languages, I asked what other languages and projects operate in the same space. This short blog post is basically highlighting the response we got from Troels.

* 🇩🇰 **[Futhark](https://futhark-lang.org/)**, a Haskell-inspired language out of DIKU at the University of Copenhagen
* 🏴󠁧󠁢󠁳󠁣󠁴󠁿 **[Single Assignment C](https://www.sac-home.org/index)** (SaC), a C-inspired language out of Heriot-Watt University
* 🇺🇸 **[Dex](https://github.com/google-research/dex-lang)**, a research array language out of Google
* 🇺🇸 **[Co-dfns](https://github.com/Co-dfns/Co-dfns)**, an APL compiler out of Indiana University / Aaron Hsu
* 🇦🇺 **[Accelerate](https://www.acceleratehs.org/)**, a Haskell library out of University of New South Wales and NVIDIA
* 🇺🇸 **[Copperhead](https://github.com/bryancatanzaro/copperhead)**, a Python-inspired research language/compiler out of NVIDIA

On top of this, several other initiatives were mentioned, including:

* 🇩🇰 **[Typed Array Intermediate Language (TAIL)](http://hiperfit.dk/pdf/array14_final.pdf)**, out of the University of Copenhagen
* 🇩🇰 **[apltail](https://github.com/melsman/apltail)**, an APL compiler targeting TAIL, out of the University of Copenhagen
* 🇺🇸 **[Remora](https://www.ccs.neu.edu/home/jrslepak/typed-j.pdf)**, a typed array language out of Northeastern University
* 🇨🇦 **[APEX](https://gitlab.com/bernecky/apex)**, a Dyalog APL compiler targeting SaC out of Snake Island Research

The following people have been or are actively involved in working on the above projects:

|       |   Project    |                                  Individual*                                  |                    Twitter                     |                    GitHub                     |                               ArrayCast?                                |
| :---: | :----------: | :---------------------------------------------------------------------------: | :--------------------------------------------: | :-------------------------------------------: | :---------------------------------------------------------------------: |
|   ✅   |   Futhark    |                    [Troels Henriksen](https://sigkill.dk/)                    |   [Twitter](https://twitter.com/sigkill_dk)    | [GitHub](https://github.com/Athas/sigkill.dk) |   [Episode 37](https://www.arraycast.com/episodes/episode37-futhark)    |
|   ✅   |   Co-dfns    |                     [Aaron Hsu](https://www.sacrideo.us/)                     |                       -                        |     [GitHub](https://github.com/arcfide)      |  [Episode 19](https://www.arraycast.com/episodes/episode19-aaron-hsu)   |
|   ✅   |     APEX     |                 [Bob Bernecky](https://www.snakeisland.com/)                  |                       -                        |     [GitHub](https://github.com/bernecky)     | [Episode 55](https://www.arraycast.com/episodes/episode55-bob-bernecky) |
|   ✅   |     SaC      | [Sven-Bodo Scholz](https://www.macs.hw.ac.uk/~sbs/homepage/main/Welcome.html) |                       -                        |     [GitHub](https://github.com/sbscholz)     |    [Episode 107](https://www.arraycast.com/episodes/episode107-sac)     |
|       |     SaC      |               [Artem Shinkarov](https://ashinkarov.github.io/)                |                       -                        |    [GitHub](https://github.com/ashinkarov)    |                                    -                                    |
|       |    Remora    |                 [Justin Slepak](https://jrslepak.github.io/)                  |                       -                        |     [GitHub](https://github.com/jrslepak)     |                                    -                                    |
|       | TAIL/apltail |                     [Martin Elsman](https://elsman.com/)                      |                       -                        |     [GitHub](https://github.com/melsman)      |                                    -                                    |
|       |  Copperhead  |                     [Bryan Catanzaro](https://ctnzr.io/)                      |      [Twitter](https://twitter.com/ctnzr)      |  [GitHub](https://github.com/bryancatanzaro)  |                                    -                                    |
|       |  Accelerate  |                [Manuel Chakravarty](https://justtesting.org/)                 |  [Twitter](https://twitter.com/TacticalGrace)  |   [GitHub](https://github.com/mchakravarty)   |                                    -                                    |
|       |  Accelerate  |                [Trevor McDonell](https://tmcdonell.github.io/)                |                       -                        |    [GitHub](https://github.com/tmcdonell)     |                                    -                                    |
|   ✅   | Dex/PyTorch  |                   [Adam Paszke](http://apaszke.github.io/)                    |     [Twitter](https://twitter.com/apaszke)     |     [GitHub](https://github.com/apaszke)      | [Episode 58](https://www.arraycast.com/episodes/episode58-adam-paszke)  |
|       |     Dex      |          [Dougal Maclaurin](https://dougalmaclaurin.com/index.html)           | [Twitter](https://twitter.com/dougalmaclaurin) |     [GitHub](https://github.com/dougalm)      |                                    -                                    |

\* Links to personal website

My plan is to try and have as many of the above folks on ArrayCast in the future. I will update this blog post with links whenever one of them appears.

Some honorable mention projects (some that didn't get mentioned) but are relevant to the space are:

* [**JAX**](https://github.com/google/jax), Autograd and XLA, brought together for high-performance ML research
* [**XLA**](https://www.tensorflow.org/xla), a domain-specific compiler for linear algebra that targets CPUs, GPUs and TPUs
* [**PyTorch**](https://github.com/pytorch/pytorch), tensors and dynamic neural networks in Python with strong GPU acceleration
* [**TensorFlow**](https://github.com/tensorflow/tensorflow), an open source platform for machine learning
* [**Nx**](https://github.com/elixir-nx/nx), multidimensional arrays (tensors) and numerical definitions for Elixir
* [**MLIR**](https://mlir.llvm.org/), a hybrid IR for building compiler infrastructure
* [**NESL**](http://www.cs.cmu.edu/~scandal/nesl.html), a parallel, functional, array programming language designed at CMU
* [**Nessie**](http://nessie.cs.uchicago.edu/), a NESL compiler the generates CUDA code for NVIDIA GPUs

Other links of interest that I came across while compiling all the links for this blog are:

* [A comparison of Futhark and Dex](https://futhark-lang.org/blog/2020-12-28-futhark-and-dex.html)
* [Array language compilation in context](https://mlochbaum.github.io/BQN/implementation/compile/intro.html) specifically the section on [Typed Array Languages](https://mlochbaum.github.io/BQN/implementation/compile/intro.html#typed-array-languages)
* [Futhark on ArrayCast](https://futhark-lang.org/blog/2022-10-03-futhark-on-arraycast.html)

The last link was written a few days after the ArrayCast episode aired. Finally, you can find comparisons of different array languages at my [Array Language Comparison GitHub repository](https://github.com/codereport/array-language-comparisons), which is where the graphic at the top of the article is from.

Feel free to leave a comment on the [reddit thread](https://old.reddit.com/r/programming/comments/xsxetm/gpu_array_languages_compiler_libraries/?).
