---
layout: default
title: "Horizon Summary: 2026-11-22 (EN)"
date: 2026-11-22
lang: en
---

> From 9 items, 7 important content pieces were selected

---

1. [Lean Formalization of Riemann Hypothesis Sparks Debate](#item-1) ⭐️ 9.0/10
2. [Huge unstable lead azide pile found at former US military facility](#item-2) ⭐️ 7.0/10
3. [Blogger traces 75% download speed loss to monitor's USB hub latency](#item-3) ⭐️ 7.0/10
4. [gopgext Enables PostgreSQL Extensions Written in Go](#item-4) ⭐️ 7.0/10
5. [Muru: AI-Assisted Rust Server for Python ASGI/WSGI Apps](#item-5) ⭐️ 7.0/10
6. [GitHub repo claims to run Inkling-2-Mini in 5.4 GB memory](#item-6) ⭐️ 6.0/10
7. [Zero C#: Compiling C# Without Runtime or GC](#item-7) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Lean Formalization of Riemann Hypothesis Sparks Debate](https://leanprover-community.github.io/blog/posts/riemann-hypothesis/) ⭐️ 9.0/10

A Lean formalization of the Riemann Hypothesis (or its generalization, GRH) was presented on the Lean Prover Community blog, reportedly produced with significant AI assistance (Claude) and human collaboration (Levent). The announcement has generated intense discussion, with 832 points and 683 comments on a major forum. If valid, this would be a groundbreaking result in mathematics and formal verification, demonstrating that major open problems can be formally checked and that AI-human collaboration can tackle extremely complex formalization tasks. It also raises important questions about the reliability of proof checkers and the role of AI in mathematics. The formalization reportedly involved formalizing a huge chunk of modern mathematics, making it a significant result for mathematical foundations as well. Community members note that while a bug in the proof is still possible, the existence of multiple independent checkers (e.g., con-leche and con-ron) with their own consistency proofs makes it vanishingly unlikely that a bug would affect both the consistency proofs and the RH proof itself.

hackernews · g-b-r · Nov 21, 14:36 · [Discussion](https://news.ycombinator.com/item?id=50589618)

**Background**: The Riemann Hypothesis, formulated by Bernhard Riemann in 1859, is one of the most famous unsolved problems in mathematics, asserting that all non-trivial zeros of the Riemann zeta function have real part 1/2. Its generalization, the Generalized Riemann Hypothesis (GRH), extends this to a broader class of L-functions. Lean is an interactive theorem prover and functional programming language used for formal verification, allowing mathematicians to write proofs that are checked by a computer kernel. Formalizing a proof in Lean means expressing it in a precise logical framework that the kernel can verify, which provides high confidence in correctness if the kernel is sound.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Riemann_hypothesis">Riemann hypothesis - Wikipedia</a></li>
<li><a href="https://lean-lang.org/">Lean Programming Language</a></li>
<li><a href="https://arxiv.org/pdf/2501.18639">A Comprehensive Survey of the Lean 4 Theorem Prover ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed both excitement and caution. Some highlighted the vanishingly small chance of a bug slipping through multiple independent checkers, while others recalled past incidents where fake proofs passed certain checkers, emphasizing the importance of the human expert in the loop. There was also praise for Levent's talent in eliciting the proof from Claude, and speculation that this work formalized a large portion of modern mathematics, making it a foundational result beyond GRH.

**Tags**: `#Lean`, `#Riemann Hypothesis`, `#formal verification`, `#mathematics`, `#AI-assisted proof`

---

<a id="item-2"></a>
## [Huge unstable lead azide pile found at former US military facility](https://www.science.org/content/blog-post/detonating-huge-pile-lead-azide-really) ⭐️ 7.0/10

A science blog post details the discovery of a large, unstable pile of lead azide at a former US military facility and the planned operation to destroy it in place. The post highlights the extreme sensitivity of the material and the challenges of safe disposal. The incident raises serious concerns about contractor negligence and oversight in handling military explosives, as the material was left in a dangerously unstable state for years. It also underscores the risks faced by communities near former military sites and the importance of proper hazardous waste management. Lead azide is extremely sensitive to shock, heat, and friction when dry, and can explode violently; the pile was deemed too dangerous to move, so authorities planned to destroy it in place. The blog post and community discussion note that even robotic handling is not feasible due to the risk of detonation.

hackernews · beginning_end · Nov 21, 13:23 · [Discussion](https://news.ycombinator.com/item?id=50588982)

**Background**: Lead azide is a primary explosive commonly used in detonators to initiate secondary explosives. It is unstable when dry and can decompose explosively if shocked, heated, or subjected to friction, making it hazardous to handle and transport. The facility in question was originally built for World War II and later operated by contractors, a common arrangement that has been criticized for poor safety records.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Lead(II)_azide">Lead (II) azide - Wikipedia</a></li>
<li><a href="https://cameochemicals.noaa.gov/chemical/11731">LEAD AZIDE | CAMEO Chemicals | NOAA</a></li>
<li><a href="https://features.propublica.org/military-pollution/military-pollution-contractors-scandal-toxic-cleanups/">How Military Outsourcing Turned Toxic</a></li>

</ul>
</details>

**Discussion**: Commenters expressed outrage at the contractor's negligence and the systemic issues in military outsourcing, with some noting that the only safe option is to destroy such unstable material in place. Others highlighted the broader pattern of hiding problems until they become unavoidable, and questioned the timeline of when the lead azide was discovered versus when cleanup contracts were awarded.

**Tags**: `#chemistry`, `#explosives`, `#military`, `#safety`, `#investigative-reporting`

---

<a id="item-3"></a>
## [Blogger traces 75% download speed loss to monitor's USB hub latency](https://blog.tymscar.com/posts/studiodisplayethernet/) ⭐️ 7.0/10

A blogger documented how routing Ethernet through a monitor's USB hub introduced enough latency to cut download speeds by 75%, and the issue was resolved by switching to a different Ethernet adapter. This case highlights how opaque USB hub behavior can cause severe network performance degradation, affecting anyone using docking stations or monitor hubs for wired connectivity. The extra latency from the monitor's hub prevented the laptop from acknowledging packets quickly enough, causing the Ethernet adapter's buffer to fill and drop packets; a different adapter requiring less frequent acknowledgment fixed the problem.

hackernews · soheilpro · Nov 21, 10:36 · [Discussion](https://news.ycombinator.com/item?id=50587875)

**Background**: USB hubs, especially those integrated into monitors or docking stations, can add latency due to internal chipset processing and shared bandwidth. This latency can interfere with TCP flow control, where timely acknowledgments are crucial for maintaining high throughput. USB Ethernet adapters vary in how they handle buffering and acknowledgment, which can affect performance under latency.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anker.com/blogs/hubs-and-docks/do-usb-hubs-add-latency">Do USB Hubs Add Latency ? How to Lessen It? - Anker US</a></li>
<li><a href="https://superuser.com/questions/1729035/slower-internet-speeds-with-usb-ethernet-adapter-than-card-from-motherboard">networking - Slower Internet speeds with USB ethernet adapter ...</a></li>

</ul>
</details>

**Discussion**: Commenters clarified that the root cause was the USB network switch adding latency, not the monitor per se, and shared analogous bizarre bugs like Ghostty's io_uring affecting game shader compilation. Others felt validated by the post, having experienced similar issues with Thunderbolt docks.

**Tags**: `#networking`, `#usb`, `#debugging`, `#hardware`, `#latency`

---

<a id="item-4"></a>
## [gopgext Enables PostgreSQL Extensions Written in Go](https://jespino.github.io/gopgext/) ⭐️ 7.0/10

A new project called gopgext demonstrates how to write PostgreSQL extensions in Go by leveraging TinyGo and generated C glue code, allowing developers to avoid hand-writing C. The project was shared on Hacker News, where it received 119 points and 20 comments. This approach lowers the barrier for Go developers to extend PostgreSQL, a database widely used in production, and offers an alternative to the established Rust-based pgrx framework. It could encourage more contributions to the PostgreSQL extension ecosystem from the large Go community. gopgext uses TinyGo to compile Go code into a shared library and generates C glue code to interface with PostgreSQL's C API, including support for SPI access and advanced hooks. However, the project is marked as experimental and comes with critical warnings for production use.

hackernews · valyala · Nov 21, 17:08 · [Discussion](https://news.ycombinator.com/item?id=50591260)

**Background**: PostgreSQL extensions are typically written in C and compiled into shared libraries that the server dynamically loads, giving access to internal APIs. Writing extensions in other languages often requires bindings or glue code; for example, pgrx provides a Rust framework for building Postgres extensions safely. gopgext aims to bring similar capabilities to Go, which is not traditionally used for this purpose.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theprotec.com/blog/build-postgresql-extensions-in-go-with-gopgext/">Build PostgreSQL extensions in Go Without Hand-Written C Code</a></li>
<li><a href="https://docs.rs/pgrx/latest/pgrx/">pgrx - Rust - Docs.rs</a></li>
<li><a href="https://github.com/microo8/plgo">GitHub - microo8/plgo: easily create postgresql extensions in...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed enthusiasm for the project, with some sharing related tools like gokm (Linux kernel modules in Go) and plgo (another Go extension tool). One commenter noted they would still choose pgrx for Rust, while another appreciated the Go gopher mascot and compared it to Rust's Ferris the crab.

**Tags**: `#PostgreSQL`, `#Go`, `#extensions`, `#databases`, `#developer-tools`

---

<a id="item-5"></a>
## [Muru: AI-Assisted Rust Server for Python ASGI/WSGI Apps](https://simonwillison.net/2026/Nov/21/muru/) ⭐️ 7.0/10

Graham Dumpleton, creator of mod_wsgi, has launched Muru, a new AI-assisted Rust server designed to run both ASGI and WSGI Python applications in development and production. Over the past three weeks, he has published an extraordinarily detailed public development log, with 18 posts covering topics from worker internals and HTTPS in development to Kubernetes integration and scaling to zero. Muru brings a Rust-based, production-oriented alternative to existing Python application servers, potentially improving performance and deployment ergonomics for both legacy WSGI and modern ASGI apps. Dumpleton's transparent development process and two decades of experience with mod_wsgi lend credibility and could influence how Python web apps are served in the future. The project is still early-stage and not yet a major release, but it already addresses advanced concerns such as import-once-fork-many worker models, canary deployments without a service mesh, and scaling based on worker-reported metrics. Dumpleton emphasizes that while AI assists with much of the work, his judgment from years of mod_wsgi experience remains central to deciding what is good enough.

rss · Simon Willison · Nov 21, 23:56

**Background**: WSGI (Web Server Gateway Interface) is the traditional synchronous standard for Python web servers to communicate with applications, while ASGI (Asynchronous Server Gateway Interface) is its asynchronous successor that supports WebSockets and long-lived connections. mod_wsgi, created by Graham Dumpleton 20 years ago, is a widely used Apache module for hosting WSGI applications. Muru aims to modernize this space by using Rust for the server layer and supporting both WSGI and ASGI together.

<details><summary>References</summary>
<ul>
<li><a href="https://www.geeksforgeeks.org/python/difference-between-asgi-and-wsgi-in-django/">Difference Between ASGI and WSGI in Django - GeeksforGeeks</a></li>
<li><a href="https://dev.to/mcheremnov/wsgi-vs-asgi-complete-guide-466f">WSGI vs ASGI : Complete Guide - DEV Community</a></li>
<li><a href="https://grahamdumpleton.me/posts/2026/08/introducing-wrapture/">Introducing wrapture - Graham Dumpleton</a></li>

</ul>
</details>

**Tags**: `#Python`, `#ASGI`, `#WSGI`, `#Rust`, `#Web Servers`

---

<a id="item-6"></a>
## [GitHub repo claims to run Inkling-2-Mini in 5.4 GB memory](https://github.com/ShinMegamiBoson/lookatmyquant) ⭐️ 6.0/10

A GitHub repository named 'lookatmyquant' claims to run the Inkling-2-Mini model in just 5.4 GB of memory, likely through aggressive quantization techniques. The claim has sparked discussion about the trade-offs between memory footprint and model performance. If validated, such extreme memory reduction could enable running a capable multimodal model on consumer hardware with limited RAM, broadening access to local AI. However, skepticism about the repo's quality and the actual usability of the quantized model tempers the significance. The repository's README is described as messy, and the headline claim of '12X better' does not apply to Inkling-2-Mini according to a commenter. Additionally, users report that the model runs significantly slower than comparable models like Qwen 27B, possibly due to its looped transformer architecture or unoptimized kernels.

hackernews · k__ · Nov 21, 18:02 · [Discussion](https://news.ycombinator.com/item?id=50591853)

**Background**: Inkling-2-Mini is an open-weight vision-language model from Thinking Machines Lab, designed for coding agents, tool use, and knowledge work. Quantization is a model optimization technique that reduces the precision of numerical values such as weights and activations, making models smaller and faster at the cost of some accuracy. Running large models in low memory often involves aggressive quantization, which can degrade performance and speed.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/thinkingmachines/Inkling-2-Mini">thinkingmachines/ Inkling - 2 - Mini · Hugging Face</a></li>
<li><a href="https://thinkingmachines.ai/model-card/inkling-2-mini/">Inkling 2 Mini Model Card - Thinking Machines Lab</a></li>
<li><a href="https://www.geeksforgeeks.org/deep-learning/quantization-in-deep-learning/">What is Quantization - GeeksforGeeks</a></li>

</ul>
</details>

**Discussion**: Commenters express skepticism about the repo's claims, warning that fitting large models into tiny RAM often involves trade-offs and that benchmark scores can be gamed. Some note the model's slow speed compared to Qwen 27B, while others speculate about using multiple instances for boosting or comment on the broader capability gap between frontier and open-source models.

**Tags**: `#quantization`, `#language-models`, `#memory-optimization`, `#model-compression`, `#hackernews`

---

<a id="item-7"></a>
## [Zero C#: Compiling C# Without Runtime or GC](https://onurgumus.github.io/zero-csharp/index.html) ⭐️ 6.0/10

A Show HN project called Zero C# demonstrates compiling C# code into a small native executable without the .NET runtime or garbage collector, based on a fork of the bflat compiler. This experiment sparks debate about whether C# can be used for systems programming without its managed runtime, potentially attracting developers who need low-level control but prefer C# syntax. The project keeps C# syntax, type checking, and generics but removes the runtime and GC, though existing C# code relying on the standard library likely won't run; commenters question its advantage over NativeAOT and existing low-level features like Span<T> and unsafe pointers.

hackernews · reverseblade2 · Nov 21, 15:39 · [Discussion](https://news.ycombinator.com/item?id=50590279)

**Background**: C# traditionally runs on the .NET runtime with automatic garbage collection, which manages memory but adds overhead. NativeAOT is an existing .NET feature that compiles C# to native code ahead-of-time, reducing startup time and binary size but still including a runtime. Zero C# goes further by eliminating the runtime entirely, similar to experimental projects like bflat.

<details><summary>References</summary>
<ul>
<li><a href="https://onurgumus.github.io/zero-csharp/index.html">Zero C# | C# without a runtime , from Linux to a 386</a></li>
<li><a href="https://en.wikipedia.org/wiki/Garbage_collection_(computer_science)">Garbage collection (computer science) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters are skeptical about the project's practical value, noting that C# already offers unsafe pointers, Span<T>, and NativeAOT for performance-critical code. Some argue that the GC is a feature, not a bug, and that removing it introduces unnecessary risk, while others suggest that using languages like C or Rust would be more appropriate for GC-free programming.

**Tags**: `#C#`, `#.NET`, `#NativeAOT`, `#garbage-collection`, `#systems-programming`

---