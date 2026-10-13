---
layout: default
title: "Horizon Summary: 2026-10-13 (EN)"
date: 2026-10-13
lang: en
---

> From 25 items, 24 important content pieces were selected

---

1. [Hackers Trigger Defrost Mode in European Supermarket Fridges](#item-1) ⭐️ 8.0/10
2. [Developer turns WiFi 7 router into 320 Msps SDR receiver](#item-2) ⭐️ 8.0/10
3. [Blood cells from 80-year-old donor reprogrammed into stem cells with molecular age under 20](#item-3) ⭐️ 8.0/10
4. [Codex CLI installs persistent self-updating daemon by default](#item-4) ⭐️ 8.0/10
5. [Python 3.15 Released with PEP 810 Explicit Lazy Imports](#item-5) ⭐️ 8.0/10
6. [learnc tunes constants in unmodified C code to fit data](#item-6) ⭐️ 8.0/10
7. [Z.ai Releases GLM-Legal, a Legal-Domain Agentic LLM](#item-7) ⭐️ 7.0/10
8. [The Mystery of x86 Instruction VFMADDRND231PD](#item-8) ⭐️ 7.0/10
9. [A Modern Web App in C Using CGI Sparks Debate](#item-9) ⭐️ 7.0/10
10. [Plug-in balcony solar panels rise as a shortcut to home renewable energy](#item-10) ⭐️ 7.0/10
11. [Reddit debate: Can next-token prediction plus RL reach AGI?](#item-11) ⭐️ 7.0/10
12. [Looped Diffusion Transformer Reuses Blocks Per Denoising Step](#item-12) ⭐️ 7.0/10
13. [U-Space: Label-Free Single-Pass Uncertainty Estimation for LLMs](#item-13) ⭐️ 7.0/10
14. [RoBERTa AI-text detector compressed to 97 MB for browser use](#item-14) ⭐️ 7.0/10
15. [shad0w: A Tiny Table That Caches Local LLM Classification Answers](#item-15) ⭐️ 7.0/10
16. [Guide Shows How to Make Large Downloads Resumable in Firefox](#item-16) ⭐️ 6.0/10
17. [Agent37 launches low-cost AI agent sandboxes at under 10% of typical provider costs](#item-17) ⭐️ 6.0/10
18. [Citroën Revives the 2CV as a Lightweight Electric Car](#item-18) ⭐️ 6.0/10
19. [ICLR Reviewers Grapple With AI-Generated Submissions](#item-19) ⭐️ 6.0/10
20. [Simon Willison releases web-edit 0.1a0 for phone-based file editing](#item-20) ⭐️ 5.0/10
21. [CL4SM Calls for Papers on Constrained Learning for Science](#item-21) ⭐️ 5.0/10
22. [Developer seeks feedback on LLM pipeline that generates exam questions from school past papers](#item-22) ⭐️ 5.0/10
23. [datasette-ports 0.4 adds PID display and latest Datasette support](#item-23) ⭐️ 4.0/10
24. [Undergrad researcher desk-rejected by TMLR in 2 days without feedback](#item-24) ⭐️ 4.0/10

---

<a id="item-1"></a>
## [Hackers Trigger Defrost Mode in European Supermarket Fridges](https://www.tomshardware.com/tech-industry/cyber-security/unprecedented-cyberattack-cripples-supermarket-fridges-across-europe-as-hackers-activate-automatic-defrosting-delivery-and-store-prices-also-impacted-by-incident) ⭐️ 8.0/10

Hackers exploited outdated internet-connected refrigeration controllers to remotely activate automatic defrosting in supermarket fridges across Europe, disrupting operations at chains such as French retailer Intermarché, where around 150 stores were targeted. The incident also impacted delivery and in-store pricing systems, according to reports dated October 2026. This is a real-world cyber-physical attack on critical retail infrastructure, showing how insecure IoT and OT devices can be weaponized to spoil food, disrupt supply chains, and cause financial damage. It highlights systemic failures in securing connected industrial equipment that underpins everyday services. The suspected vulnerable devices include 15-20 year old Danfoss controllers such as the SM800 (end-of-support 2021) and SC355 (end-of-support 2016), which have known CVEs but are often left unpatched due to cost and operational constraints. Claroty's Team82 previously found multiple vulnerabilities in the Danfoss AK-SM 800A platform's embedded web management interface, allowing attackers to physically manipulate refrigeration systems.

hackernews · Zeekaas · Oct 12, 12:16 · [Discussion](https://news.ycombinator.com/item?id=50055304)

**Background**: Refrigeration controllers are microprocessor-based industrial devices that manage temperature, defrost cycles, and energy efficiency in commercial cooling systems. Many modern controllers are connected to the internet to enable remote diagnostics and efficiency monitoring, but this connectivity expands the attack surface. In operational technology (OT) environments, devices often run for decades without security updates, and patching is complicated by the need for continuous operation and limited budgets.

<details><summary>References</summary>
<ul>
<li><a href="https://www.claroty.com/team82/research/freeze-the-controller-defrost-the-food-uncovering-vulnerabilities-in-danfoss-refrigeration-controllers">Freeze the Controller , Defrost the Food: Uncovering Vulnerabilities in...</a></li>
<li><a href="https://itwire.com/guest-articles/guest-research/chilling-discoveries-claroty-finds-multiple-security-vulnerabilities-in-danfoss-and-copeland-refrigeration-controllers">Chilling discoveries: Claroty finds multiple security vulnerabilities in...</a></li>
<li><a href="https://www.machine.news/vulnerabilities-in-refrigeration-systems-highlight-the-chilling-fragility-of-food-supply-chains/">Vulnerabilities in refrigeration systems highlight the chilling fragility of...</a></li>

</ul>
</details>

**Discussion**: Commenters pointed out that the vulnerable controllers are 15-20 years old and often unpatched because shift-work labor lacks resources for security reviews, and noted that some lab equipment now requires paid subscriptions and internet access to function, explaining why such devices get connected. Others linked the Danfoss vulnerability to a similar incident at US military bases in August 2026 and questioned whether the same group was involved.

**Tags**: `#cybersecurity`, `#IoT`, `#critical-infrastructure`, `#OT-security`, `#supply-chain`

---

<a id="item-2"></a>
## [Developer turns WiFi 7 router into 320 Msps SDR receiver](https://github.com/h0m3us3r/w1700k-sdr) ⭐️ 8.0/10

A developer (h0m3us3r) has released a project that repurposes a WiFi 7 router into a 320 Msps software-defined radio receiver operating at 5 GHz. The project, hosted on GitHub as w1700k-sdr, demonstrates low-cost high-bandwidth SDR using consumer networking hardware. This breakthrough could dramatically lower the cost of high-bandwidth SDR, which normally requires expensive specialized hardware, making advanced wireless experimentation accessible to hobbyists and researchers. It also hints at a future where common WiFi cards in laptops could double as SDRs for a wide range of applications. The project achieves a 320 Msps receive rate at 5 GHz, a capability that commenters note is hard to find at a lower cost. The same developer previously built an SDR from an ESP32 Wi-Fi microcontroller, and the chipset used may also work on the Banana Pi R4, which has built-in PCIe for NVMe.

hackernews · djfergus · Oct 12, 12:41 · [Discussion](https://news.ycombinator.com/item?id=50055593)

**Background**: Software-defined radio (SDR) is a radio communication system where components traditionally implemented in analog hardware (such as mixers, filters, and amplifiers) are instead implemented in software. This allows a single hardware platform to receive and transmit many different radio protocols by simply changing the software. WiFi 7 is the latest generation of wireless networking, offering higher throughput and lower latency, and its routers contain powerful RF chipsets that can be repurposed for SDR tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Software-defined_radio">Software-defined radio - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters are highly enthusiastic, calling the project 'awesome' and noting it as a cheap way to get a 320 Msps receiver at 5 GHz. They highlight related work like the ESP32-based SDR and speculate that the same chipset could work on the Banana Pi R4. Some discuss broader implications, such as why phone manufacturers restrict FM radio access and how cheap components could enable advanced test equipment.

**Tags**: `#SDR`, `#WiFi 7`, `#hardware hacking`, `#wireless`, `#RF`

---

<a id="item-3"></a>
## [Blood cells from 80-year-old donor reprogrammed into stem cells with molecular age under 20](https://doi.org/10.1111/acel.70751) ⭐️ 8.0/10

Researchers successfully reprogrammed blood cells from an 80-year-old donor into induced pluripotent stem cells whose epigenetic molecular age measured under 20 years, according to a study published in Aging Cell. This demonstrates that cellular aging can be substantially reversed at the molecular level through reprogramming. This finding suggests that epigenetic aging is not irreversible and could potentially be reset, opening new avenues for regenerative medicine and therapies targeting age-related diseases. If translated to organismal level, it could reshape how we approach aging and tissue repair. The study used epigenetic clocks to measure biological age, which rely on DNA methylation patterns rather than chronological time. The reprogramming likely employed Yamanaka factors (Oct4, Sox2, Klf4, c-Myc) to convert somatic cells into pluripotent stem cells, though the abstract's dense terminology has drawn some criticism.

hackernews · arunc · Oct 12, 23:34 · [Discussion](https://news.ycombinator.com/item?id=50064536)

**Background**: Cellular reprogramming is the process of reverting specialized adult cells into induced pluripotent stem cells (iPSCs), which can then differentiate into any cell type. This technology, pioneered by Shinya Yamanaka in 2006 (Nobel Prize 2012), typically uses four transcription factors to reset cell identity. Epigenetic clocks are biomarkers that estimate biological age by analyzing age-related DNA modifications, and they have become key tools for assessing the effectiveness of anti-aging interventions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Induced_pluripotent_stem_cell">Induced pluripotent stem cell</a></li>
<li><a href="https://en.wikipedia.org/wiki/Epigenetic_clock">Epigenetic clock - Wikipedia</a></li>
<li><a href="https://www.nature.com/subjects/reprogramming">Reprogramming - Latest research and news | Nature</a></li>

</ul>
</details>

**Discussion**: Commenters expressed a mix of hope and skepticism: some are motivated to stay healthy in case aging is solved, others compared the process to the immortal jellyfish's rejuvenation, and a few raised ethical concerns about dictators potentially exploiting such technology. The discussion also touched on Michael Levin's bioelectricity work and the irony of using cell reprogramming for AI brain organoids before aging remediation.

**Tags**: `#aging`, `#stem cells`, `#cellular reprogramming`, `#regenerative medicine`, `#longevity`

---

<a id="item-4"></a>
## [Codex CLI installs persistent self-updating daemon by default](https://github.com/openai/codex/issues/48195) ⭐️ 8.0/10

OpenAI's Codex CLI now silently installs a persistent, self-updating background daemon by default, starting a process via 'codex app-server --managed-daemon' that runs in its own session with no TTY and keeps running after every Codex window is closed (reparented to PID 1) until explicitly stopped or the machine reboots. A GitHub issue (#48195) asks that 'daemon_auto_start' be made opt-in or at least prompt the user once, reserving the persistent daemon behavior for Remote Control or the desktop app. This is a significant privacy and security concern for a widely used AI coding tool, since a persistent background process that self-updates and pins environment variables (such as proxy settings) can outlive user sessions and silently inherit stale configuration. It affects developers who rely on Codex CLI for local coding tasks and raises broader questions about how much autonomy AI coding agents should have over a user's machine by default. The daemon pins the environment of whichever session first started it, causing later sessions to inherit stale config, and it writes pid files and lock files into ~/.codex at startup. Users report it consuming around 12 GB of disk space by accumulating old versions, and bugs where auto-updating randomly corrupts permissions, such as making .git read-only and blocking goals.

hackernews · whimblepop · Oct 12, 18:29 · [Discussion](https://news.ycombinator.com/item?id=50060694)

**Background**: Codex CLI is OpenAI's coding agent that runs locally in the terminal, letting developers inspect, edit, and run code from the command line. A background daemon is a long-running process that operates without a terminal and can be shared across sessions, which is useful for features like remote control but also means it persists beyond the user's visible workflow. The controversy echoes similar concerns about other AI coding tools such as Claude Code, which also keeps prior binary versions and background processes on disk.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/openai/codex/issues/48195">CLI: make `daemon_auto_start` opt-in — a persistent, self ...</a></li>
<li><a href="https://daily.dev/posts/codex-cli-installs-a-persistent-self-updating-background-daemon-by-default-unpmj86e7">Codex CLI installs a persistent, self-updating background ...</a></li>
<li><a href="https://news.ycombinator.com/item?id=50060694">Codex CLI installs a persistent, self-updating background ...</a></li>

</ul>
</details>

**Discussion**: Community sentiment is largely critical, with users reporting disk bloat of around 12 GB, permission corruption that makes .git read-only, and frequent bugs that erode trust in Codex executing goals reliably. Some users share workarounds such as setting 'daemon_auto_start = false' in ~/.codex/config.toml or symlinking pid and lock files to /dev/null, while others note that Claude Code uses a similar operational model and that simpler bare-bones harnesses like hax are a refreshing alternative.

**Tags**: `#codex-cli`, `#openai`, `#privacy`, `#developer-tools`, `#ai-coding-agents`

---

<a id="item-5"></a>
## [Python 3.15 Released with PEP 810 Explicit Lazy Imports](https://simonwillison.net/2026/Oct/12/python-3-15/) ⭐️ 8.0/10

Python 3.15 has been officially released, with its What's New guide curated by release manager Hugo van Kemenade. The headline feature is PEP 810 explicit lazy imports, which let developers write `lazy import json` or `lazy from pathlib import Path` so the module is only loaded the first time its symbols are actually used. Lazy imports directly address the startup cost that heavy dependencies impose on CLI tools, test suites, and large services, a long-standing pain point for the Python ecosystem. The release also marks the end of support for Python 3.10, meaning library maintainers like Simon Willison can now drop 3.10 and adopt features from Python 3.11 onward. PEP 810 chose an explicit opt-in syntax rather than making all imports lazy, so developers control exactly which imports are deferred. The post also highlights PEP 798 unpacking in comprehensions, which enables syntax like `[*sublist for sublist in lists]` and is an extension of the unpacking generalizations from PEP 448 that landed in Python 3.5.

rss · Simon Willison · Oct 12, 18:15

**Background**: Python is a widely used programming language whose imports are normally executed eagerly when a module is loaded, which can add noticeable startup latency when dependencies are heavy. PEP 810 is the accepted proposal that introduces explicit lazy imports in Python 3.15, following earlier discussions such as PEP 690. Simon Willison is a well-known Python developer whose LLM CLI tool implements plugins, and he had previously recommended manual lazy imports to plugin authors to avoid multi-second startup delays.

<details><summary>References</summary>
<ul>
<li><a href="https://peps.python.org/pep-0810/">PEP 810 – Explicit lazy imports | peps.python.org</a></li>
<li><a href="https://realpython.com/python315-lazy-imports/">Python 3.15 Preview: Lazy Imports – Real Python</a></li>
<li><a href="https://peps.python.org/pep-0690/">PEP 690 – Lazy Imports | peps. python .org</a></li>

</ul>
</details>

**Tags**: `#Python`, `#Programming Languages`, `#Software Engineering`, `#PEP 810`, `#Release`

---

<a id="item-6"></a>
## [learnc tunes constants in unmodified C code to fit data](https://www.reddit.com/r/MachineLearning/comments/1x4dlbm/learnc_fit_the_constants_in_existing_c_code_to/) ⭐️ 8.0/10

learnc is a new MIT-licensed tool that tunes named constants in unmodified C code against a user-written score function and writes the same file back with new values. On held-out data it achieved 9.1% BD-rate improvement at equal SSIM for JPEG (stb_image_write.h's 128 quantization-table entries, tuned on 12 Kodak images and tested on the other 12) and raised Google's WebRTC VAD F1 from 0.810 to 0.859 on LibriParty eval. This offers a general, open-source way to squeeze better performance out of existing C code without rewriting it, which could benefit practitioners in machine learning and systems who rely on hand-tuned constants. The independent validation in libjpeg with scikit-image and the substantial gains on widely used components like JPEG encoding and WebRTC VAD suggest the approach is both practical and broadly applicable. The tool is best suited for tens to hundreds of constants rather than large weight sets, and it reports no JPEG gain below 1 bit per pixel. The JPEG result was checked independently in libjpeg with scikit-image, while mozjpeg's tables only achieve 2.7% under the same setup.

reddit · r/MachineLearning · /u/keep_up_sharma · Oct 12, 20:51

**Background**: JPEG compression relies on quantization tables—sets of constants that determine how aggressively image detail is discarded—and tools like stb_image_write.h ship with fixed, hand-chosen tables. BD-rate is a standard metric for comparing compression efficiency at equal quality, often measured with SSIM, a perceptual similarity score. WebRTC VAD is Google's voice activity detector used in real-time communication, and its accuracy depends on constants in vad_core.c. learnc automates the tedious manual tuning of such constants by searching for values that optimize a user-defined score on data.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/nothings/stb">GitHub - nothings/stb: stb single-file public domain ... Image Loading (stb_image) | nothings/stb | DeepWiki HDK: MaterialXRender/External/StbImage/stb_image_write.h ... c - STB Image Writing JPEG Incorrectly - Stack Overflow A Reliable JPEG Quantization Table Estimator - IPOL</a></li>
<li><a href="https://github.com/wiseman/py-webrtcvad">wiseman/py-webrtcvad: Python interface to the WebRTC Voice ...</a></li>
<li><a href="https://github.com/Netflix/image_compression_comparison">GitHub - Netflix/image_compression_comparison: Image ...</a></li>

</ul>
</details>

**Tags**: `#C`, `#optimization`, `#machine learning`, `#JPEG`, `#WebRTC`

---

<a id="item-7"></a>
## [Z.ai Releases GLM-Legal, a Legal-Domain Agentic LLM](https://z.ai/blog/glm-legal) ⭐️ 7.0/10

Z.ai announced GLM-Legal on October 12, 2026, a legal-domain agentic model built on its GLM-5.3-Flash foundation, reporting a 19.2% all-pass rate on the Harvey LAB benchmark of real-world law firm workflows. The company says the model matches frontier closed-source models on LegalBench and PLawBench despite running on a significantly leaner parameter footprint. Legal work is one of the highest-stakes domains for AI adoption, so a cheaper, openly positioned legal model could pressure incumbents and make legal AI tooling more accessible to smaller firms. The release also intensifies the debate over whether LLMs can be trusted with legal reasoning and client-confidential data at all. GLM-Legal was evaluated across three axes: complex task execution, specialized legal reasoning, and real-world legal workflows, with the 19.2% all-pass rate on Harvey LAB indicating that most real-world legal tasks still fail end-to-end. Like other GLM models, it is likely released under a permissive license such as MIT or Apache 2.0, allowing local or cloud deployment.

hackernews · ilreb · Oct 12, 16:11 · [Discussion](https://news.ycombinator.com/item?id=50058507)

**Background**: GLM is the flagship model series from Z.ai, one of China's so-called 'six AI tigers,' and most GLM weights are released under permissive licenses. LegalBench is a crowd-sourced benchmark of 162 legal reasoning tasks, while Harvey LAB measures performance on realistic law firm workflows. Legal AI adoption raises well-documented concerns around bias, privacy, and regulatory compliance, especially when models handle privileged client information.

<details><summary>References</summary>
<ul>
<li><a href="https://www.unite.ai/z-ai-unveils-glm-legal-an-agentic-model-for-legal-workflows/">Z.ai Unveils GLM-Legal, an Agentic Model for Legal Workflows</a></li>
<li><a href="https://z.ai/blog/glm-legal">GLM-Legal: Advancing Agentic Legal Intelligence - z.ai</a></li>
<li><a href="https://en.wikipedia.org/wiki/GLM_(AI)">GLM (AI) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters were largely skeptical: an attorney noted that a 20% pass rate is unimpressive for litigation work, and others argued law is not built on axioms so LLMs add little value for novel situations. Privacy concerns resurfaced over Z.ai's past workspace snapshotting, while some users shared positive experiences using Claude for contract redlining and argued better legal tools are clearly needed.

**Tags**: `#legal-tech`, `#large-language-models`, `#AI`, `#privacy`, `#benchmarks`

---

<a id="item-8"></a>
## [The Mystery of x86 Instruction VFMADDRND231PD](https://purplesyringa.moe/blog/who-is-vfmaddrnd231pd/) ⭐️ 7.0/10

A blog post investigates the obscure x86 instruction VFMADDRND231PD, which appears in Intel documentation but is not implemented in any known CPU. The author traces its encoding, naming, and likely removal, suggesting it may have been an early FMA variant that never shipped. This investigation sheds light on the messy evolution of the x86 instruction set, showing how undocumented or abandoned instructions can linger in documentation and confuse reverse engineers. It highlights the importance of understanding historical context when working with low-level code. The instruction name includes 'RND' for rounding and '231' indicating operand ordering, but its exact semantics are unclear because it was never implemented. The author notes that similar FMA instructions like VFMADD231PD exist, and the 'RND' variant may have been dropped due to hardware issues or changes in the FMA specification.

hackernews · pngmangi · Oct 12, 21:12 · [Discussion](https://news.ycombinator.com/item?id=50063138)

**Background**: FMA (Fused Multiply-Add) instructions combine multiplication and addition in one operation, improving performance for scientific computing. The x86 instruction set is vast, with many extensions added over decades, and some instructions are documented but never implemented in silicon. Reverse engineers often encounter such ghost instructions when disassembling binaries.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.oracle.com/cd/E37838_01/html/E61064/gnyeh.html">FMA Instructions - x 86 Assembly Language Reference Manual</a></li>
<li><a href="https://www.wikiwand.com/en/articles/FMA_instruction_set">FMA instruction set - Wikiwand</a></li>

</ul>
</details>

**Discussion**: Commenters shared insights: one explained the meaning of 'DDS' in VEX encoding from old binutils docs; another linked to Felix Cloutier's x86 reference and theorized the instruction was removed due to hardware issues; a third lamented how such cryptic names hinder direct understanding; and a fourth initially mistook it for a RISC-V extension.

**Tags**: `#x86`, `#instruction set`, `#hardware`, `#reverse engineering`, `#low-level programming`

---

<a id="item-9"></a>
## [A Modern Web App in C Using CGI Sparks Debate](https://prophitt.me/writing/a-modern-web-app-in-c) ⭐️ 7.0/10

A blog post by prophitt.me demonstrates how to build a modern web application in C using the Common Gateway Interface (CGI), arguing that this classic approach remains viable today. The post drew significant attention on Hacker News with 416 upvotes and 168 comments, where developers debated its merits against contemporary frameworks. This article challenges the assumption that modern web development requires heavyweight frameworks and managed runtimes, showing that C with CGI can still deliver functional, secure web applications. It matters for systems-minded developers and small-scale deployments where simplicity, low resource usage, and minimal dependencies are priorities. The post emphasizes security practices such as pledge, chroot, and privilege dropping to harden CGI processes, and notes that CGI spawns a new process per request, which contrasts with stateful long-running backends. Community members also pointed out that BusyBox has built-in CGI support and that alternatives like FastCGI can reduce per-request overhead.

hackernews · prophittcorey · Oct 12, 16:13 · [Discussion](https://news.ycombinator.com/item?id=50058528)

**Background**: CGI is a standard interface that lets a web server execute an external program to handle HTTP requests and return dynamic content. It was widely used in the 1990s with languages like Perl and C, but fell out of favor due to performance overhead from spawning a process per request. Modern web frameworks typically use long-running application servers, but CGI remains a simple, dependency-free option for small deployments.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Common_Gateway_Interface">Common Gateway Interface - Wikipedia</a></li>
<li><a href="https://www.w3.org/CGI/">CGI - Common Gateway Interface Common Gateway Interface (CGI): A Deep Dive into Dynamic Web ... What is Common Gateway Interface? | How It Works | Skill ... What is the Common Gateway Interface? - Learn Coding Anywhere ... Common Gateway Interface - Online Tutorials Library</a></li>

</ul>
</details>

**Discussion**: Commenters were largely positive about the article's reasoning, with some sharing their own experiences using C and CGI or FastCGI in production. A common concern was the per-request process model, with some developers preferring stateful backends in Rust or C++ for better performance and easier state management. Others highlighted alternatives like BusyBox's built-in CGI and rclone's WebDAV serving.

**Tags**: `#C`, `#Web Development`, `#CGI`, `#Systems Programming`, `#Hacker News`

---

<a id="item-10"></a>
## [Plug-in balcony solar panels rise as a shortcut to home renewable energy](https://www.nationalgeographic.com/environment/article/balcony-plug-in-solar-panels-renewable-energy) ⭐️ 7.0/10

National Geographic reports on the growing adoption of plug-in balcony solar panels, small photovoltaic kits that connect to a home through a standard wall socket instead of requiring professional rooftop installation. The article highlights how this approach sidesteps installation and regulatory bottlenecks, while a Hacker News discussion debates its safety, grid stability, and technical limitations. As solar panels become cheap enough that installation and permitting are the main bottlenecks, plug-in systems could dramatically lower the barrier for renters and apartment dwellers to generate their own electricity. This trend could accelerate distributed solar adoption, but it also raises unresolved questions about grid stability and safety that utilities and regulators will need to address. A typical plug-in kit consists of one or two 300–400W panels paired with a microinverter that feeds power into a standard outlet. Because balcony panels are often mounted vertically, their generation peak is shifted toward the edges of the typical 'duck curve,' and in US-style 120V split-phase systems, plugging into only one leg raises phase-balancing concerns.

hackernews · speckx · Oct 12, 14:19 · [Discussion](https://news.ycombinator.com/item?id=50056822)

**Background**: Balcony solar power, also called plug-in PV or mini solar, is a small photovoltaic system designed for direct use in a home or apartment, popularized in Germany and now spreading to other markets. Unlike rooftop solar, it requires no permanent installation or complex permitting, but it relies on grid-following inverters rather than the synchronous generators that traditionally provide rotational inertia to keep grid frequency stable. As distributed solar grows—representing 48% of global solar PV capacity additions in 2022—these technical trade-offs become more significant.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Balcony_solar_power">Balcony solar power - Wikipedia</a></li>
<li><a href="https://www.nationalgeographic.com/environment/article/balcony-plug-in-solar-panels-renewable-energy">Solar Panels That Plug Into Your Wall Are... | National Geographic</a></li>
<li><a href="https://www.iea.org/commentaries/digital-tools-will-help-keep-distributed-solar-pv-growing-strongly">Digital tools will help keep distributed solar PV growing strongly... - IEA</a></li>

</ul>
</details>

**Discussion**: Commenters broadly agree that plug-in solar is suboptimal but useful for bypassing installation and regulatory hurdles, with one noting that vertical balcony mounting shifts generation to the edges of the duck curve. Key concerns include whether plugging a generator into an outlet is safe, how split-phase 120V systems handle single-leg injection, and what happens to grid frequency stability as synchronous generators are replaced by grid-following inverters. Several users also expressed hope for plug-in battery storage as the next step.

**Tags**: `#solar energy`, `#renewable energy`, `#grid stability`, `#plug-in solar`, `#balcony solar`

---

<a id="item-11"></a>
## [Reddit debate: Can next-token prediction plus RL reach AGI?](https://www.reddit.com/r/MachineLearning/comments/1x4awlk/what_is_the_strongest_mechanistic_argument_that/) ⭐️ 7.0/10

A Reddit post on r/MachineLearning asks for the strongest mechanistic argument that next-token prediction combined with reinforcement learning can produce open-ended general intelligence, explicitly requesting reasoning grounded in causal mechanisms, computational learning theory, information theory, and first principles rather than trend extrapolation. The author clarifies in an edit that this is an engineering question about real-world operational effectiveness, not a philosophical debate about semantic perfection. This question targets the theoretical foundation of the current AI scaling paradigm, which assumes that transformer-based next-token prediction plus RL fine-tuning can eventually yield AGI. The discussion matters because if no strong mechanistic case exists, the industry's massive investment in scaling these methods may rest on extrapolation rather than principled understanding. The post distinguishes mechanistic explanations from appeals to future breakthroughs and asks what is currently understood about existing systems that justifies expecting general intelligence to emerge from continued development. It also emphasizes using reasonable working definitions and focusing on causal explanations over philosophical debates.

reddit · r/MachineLearning · /u/Repulsive_Twist_9221 · Oct 12, 19:09

**Background**: Next-token prediction is the training objective behind large language models such as GPT, where the model learns to predict the next token in a sequence as a multi-class classification task. Reinforcement learning is a paradigm in which an agent learns through trial-and-error interactions with an environment to maximize a reward signal, and it is increasingly used to align and fine-tune language models. Computational learning theory formally studies the design and analysis of machine learning algorithms, including the computational resources required for learning, providing tools to evaluate whether these mechanisms can in principle support general intelligence.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/blog/alonsosilva/nexttokenprediction">Next token prediction with GPT - Hugging Face</a></li>
<li><a href="https://en.wikipedia.org/wiki/Reinforcement_learning">Reinforcement learning</a></li>
<li><a href="https://en.wikipedia.org/wiki/Computational_learning_theory">Computational learning theory</a></li>

</ul>
</details>

**Tags**: `#AGI`, `#next-token prediction`, `#reinforcement learning`, `#computational learning theory`, `#AI safety`

---

<a id="item-12"></a>
## [Looped Diffusion Transformer Reuses Blocks Per Denoising Step](https://www.reddit.com/r/MachineLearning/comments/1x49d61/looped_diffusion_transformer_the_same_blocks_run/) ⭐️ 7.0/10

A new paper, Looped Diffusion Transformer (Looped-DiT, arXiv 2609.40305), proposes running a shared group of transformer blocks multiple times within each denoising step instead of scaling up model size, using deep supervision on every loop plus self-modulating attention to stabilize training. The authors claim a 260M looped model beats a model 6.5x larger on several benchmarks with 4.9x less inference compute, and a community member reproduced the B/16 model on an M5 Pro, showing loop depth can be chosen at sampling time. This approach offers a way to trade compute for quality at inference time without retraining, which could make high-quality text-to-image generation cheaper to run and easier to tune per image. It also connects diffusion transformers to the looped/recurrent-depth ideas already explored in language models, potentially influencing future efficient architecture design. Naive looping reportedly does not reliably help, so the authors add deep supervision on every loop and self-modulating attention; the B/16 code and weights are MIT-licensed and available on Hugging Face under sensenova. In the community reproduction on Apple Silicon, most quality change occurred before loop depth 3, depths 3 and 4 were very close, and generation took about 23-24 seconds at depth 1 versus 43-47 seconds at depth 4.

reddit · r/MachineLearning · /u/Fit-Ant2238 · Oct 12, 18:13

**Background**: Diffusion transformers (DiTs) are the backbone of many modern text-to-image models, generating images by iteratively denoising random noise over many steps. Looped or recurrent-depth architectures reuse the same layers multiple times to increase effective depth without adding parameters, an idea previously popular in language models. Deep supervision means adding training signals at intermediate computation stages, while self-modulating attention lets the attention mechanism adjust its behavior dynamically.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2609.40305">[2609.40305] Looped Diffusion Transformer - arXiv.org</a></li>
<li><a href="https://www.emergentmind.com/papers/2609.40305/">Looped Diffusion Transformer - emergentmind.com</a></li>
<li><a href="https://www.emergentmind.com/topics/looped-diffusion-transformer-looped-dit">Looped Diffusion Transformer (Looped-DiT) - emergentmind.com</a></li>

</ul>
</details>

**Discussion**: The community member who reproduced the model on an M5 Pro highlighted that loop depth is selected at sampling time, similar to iteration count in looped language models, allowing per-image compute-quality trade-offs. They noted that most gains appear before depth 3 and that depths 3 and 4 are nearly identical on the prompts tested.

**Tags**: `#diffusion-models`, `#transformers`, `#efficient-inference`, `#text-to-image`, `#model-architecture`

---

<a id="item-13"></a>
## [U-Space: Label-Free Single-Pass Uncertainty Estimation for LLMs](https://www.reddit.com/r/MachineLearning/comments/1x44f9m/uspace_uncovering_when_and_why_uncertainty_arises/) ⭐️ 7.0/10

Researchers released U-Space (with its U-Lens estimator), a label-free, single-pass method that scores a language model's uncertainty by combining hidden-state projections onto four 'doubt' directions with mean token entropy over reasoning tokens. In a 3-seed, 3-model, 4-benchmark evaluation on Gemma 4, Qwen3.5, and Magistral, it reportedly beat 5-pass, 10-pass, and supervised baselines. Uncertainty signals are increasingly needed to route low-confidence answers to larger models or humans, trigger retrieval, or ask clarifying questions, but existing approaches often require expensive multi-sample generation, a judge model, or labeled data. A single-pass, interpretable estimator that also distinguishes ambiguity, missing information, conflicting evidence, and general uncertainty could make confidence-aware deployment far cheaper for practitioners. The only model-specific ingredient is a Jacobian lens (J-Lens) from Anthropic's global workspace work; once fitted, the four-direction U-Space basis can be built on CPU using only the unembedding rows of a few hundred words, without loading the full model. At inference, a single hidden state from one layer is dotted with four vectors and multiplied by mean token entropy; over 40 pre-fitted lenses are available on Hugging Face, and new ones can be fitted with about 100 unlabeled prompts.

reddit · r/MachineLearning · /u/AdRevolutionary3242 · Oct 12, 15:10

**Background**: Uncertainty estimation aims to assign a confidence score to a model's output, which is important as LLMs are deployed in safety-critical settings. Common baselines include sampling-based methods (generating multiple answers and measuring disagreement) and supervised probes trained on labeled correctness data, both of which add cost or require labels. Token entropy measures how spread out a model's next-token probability distribution is, while the Jacobian lens (J-Lens) is a technique from Anthropic's global workspace paper that maps internal activations to vocabulary directions, revealing what a model is 'disposed' to say.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/anthropics/jacobian-lens">anthropics/ jacobian - lens : Companion code for the global workspace ...</a></li>
<li><a href="https://www.anthropic.com/research/global-workspace">A global workspace in language models \ Anthropic</a></li>
<li><a href="https://www.emergentmind.com/topics/token-entropy">Token Entropy in AI Models - emergentmind.com</a></li>

</ul>
</details>

**Tags**: `#uncertainty estimation`, `#language models`, `#interpretability`, `#reasoning`, `#machine learning`

---

<a id="item-14"></a>
## [RoBERTa AI-text detector compressed to 97 MB for browser use](https://www.reddit.com/r/MachineLearning/comments/1x3vqip/compressed_a_roberta_aitext_detector_from_500_mb/) ⭐️ 7.0/10

A developer compressed a RoBERTa-based AI-text detector from roughly 500 MB in fp32 down to about 97 MB, and a Community Forensics image detector to about 26 MB, so both run fully client-side in the browser via ONNX Runtime Web 1.30. The text model uses WiSE-FT weight interpolation, int4 embedding quantization with fp16 per-row scales, and mixed-precision quantization for the transformer body, while the tokenizer and preprocessing are reimplemented in JavaScript. This shows that large transformer-based detectors can be shrunk enough to run privately in the browser without uploading user content, which matters for privacy-sensitive applications like detecting AI-generated text or images. It also demonstrates a practical compression pipeline (WiSE-FT plus int4 embedding quantization plus ONNX Runtime Web) that other ML engineers can reuse for client-side deployment. The word embedding matrix is stored separately as int4 with fp16 per-row scales (about 19 MB plus 2 MB) and dequantized in JavaScript, while the transformer body is about 75 MB; a text check of roughly 100 tokens takes about 60 ms and an image about 200 ms on the developer's laptop. Limitations include that a high score does not prove authorship, short or casual text, paraphrasing, heavy editing, screenshots, crops and newer generators reduce accuracy, and the first load is a large download, especially on phones.

reddit · r/MachineLearning · /u/Alternative_Detail31 · Oct 12, 07:44

**Background**: RoBERTa is a transformer encoder model from Meta AI that improves on BERT through better pretraining, and it is commonly fine-tuned for classification tasks such as AI-text detection. ONNX Runtime Web is a JavaScript library that runs ONNX models in the browser, using WebGPU when available and threaded WebAssembly otherwise, which enables privacy-preserving client-side inference. WiSE-FT is a weight interpolation technique that ensembles zero-shot and fine-tuned weights to keep a fine-tuned model from drifting too far from its original behavior.

<details><summary>References</summary>
<ul>
<li><a href="https://onnxruntime.ai/docs/tutorials/web/">Web | onnxruntime</a></li>
<li><a href="https://deepwiki.com/mlfoundations/wise-ft">mlfoundations/ wise - ft | DeepWiki</a></li>
<li><a href="https://www.geeksforgeeks.org/machine-learning/overview-of-roberta-model/">Introduction of RoBERTa Model - GeeksforGeeks</a></li>

</ul>
</details>

**Tags**: `#model-compression`, `#onnx`, `#client-side-ml`, `#ai-detection`, `#quantization`

---

<a id="item-15"></a>
## [shad0w: A Tiny Table That Caches Local LLM Classification Answers](https://www.reddit.com/r/MachineLearning/comments/1x3vkej/i_built_a_tiny_table_that_learns_your_local_llms/) ⭐️ 7.0/10

A developer released shad0w, an open-source caching proxy that sits in front of any OpenAI-compatible server (including Ollama) and, after logging roughly 1,000 answers, compiles a small lookup table that serves repeated classification queries on CPU in microseconds. It only returns a cached answer when it agrees with the underlying model at least 95% of the time on held-out data; otherwise the request still goes to the model. Many local LLM workloads are repetitive classification tasks where the same questions are asked hundreds of times, and each answer currently costs seconds of latency; shad0w cuts those repeats to microseconds without retraining or changing the model. This makes it a practical, low-cost optimization for anyone running local inference at scale, though it is an incremental latency win rather than a fundamental modeling breakthrough. shad0w is Apache-2.0 licensed and written in Python, JS, and C, works out of the box with Ollama (e.g. llm="ollama/llama3.1" or shad0w proxy --upstream http://localhost:11434/v1), and includes a demo where it learned to play Snake from an LLM's moves at 10 moves per second. The 95% agreement threshold on held-out answers is the key safety mechanism that limits incorrect cached responses.

reddit · r/MachineLearning · /u/gauravc2796 · Oct 12, 07:33

**Background**: OpenAI-compatible servers such as vLLM and Ollama expose the same HTTP API shape as OpenAI's, so tools can be dropped in front of them without code changes. LLM caching proxies like LiteLLM already cache responses to cut cost and latency, but they typically key on exact prompts; shad0w instead learns a compact classifier table from the model's own logged answers. Classification here means tasks where the model picks a label or category for an input, which tend to be highly repetitive in production.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/v0.8.3/serving/openai_compatible_server.html">OpenAI - Compatible Server — vLLM</a></li>
<li><a href="https://ollama.com/">Ollama · Run AI models locally and in the cloud</a></li>
<li><a href="https://medium.com/@emmaliaocode/llm-proxy-cache-why-and-how-to-use-it-74166453a65d">LLM Proxy Cache : Why and How to Use It | by Emma Liao | Medium</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#caching`, `#inference optimization`, `#local models`, `#open source`

---

<a id="item-16"></a>
## [Guide Shows How to Make Large Downloads Resumable in Firefox](https://lunarwatcher.codeberg.page/til/firefox/resumable-big-downloads.html) ⭐️ 6.0/10

A blog post on lunarwatcher.codeberg.page explains a method for making large downloads resumable in Firefox, addressing a long-standing pain point where interrupted downloads often cannot be continued. The guide focuses on workarounds for one-time download links that break mid-transfer, such as those caused by flaky connections. Reliable resumable downloads matter for anyone downloading large files like game mods, ISOs, or datasets over unstable connections, and Firefox's inconsistent behavior has frustrated users for years. This tip offers a practical fix without requiring external download managers, though alternatives like aria2 and multithreaded extensions remain popular. The workaround involves manipulating Firefox's .part file: moving it to a temp location, restarting the download to generate a new .part file, pausing, then overwriting the new .part with the old one before unpausing. Community members note that Firefox's resumable download behavior has been unstable since at least 2005 and may relate to the network.http.response.timeout setting.

hackernews · speckx · Oct 12, 19:36 · [Discussion](https://news.ycombinator.com/item?id=50061791)

**Background**: When Firefox downloads a file, it stores partial data in a .part file alongside the target file. Resumable downloads rely on HTTP range requests, which let a client fetch only the missing portion of a file from a server that supports them. If the server does not support range requests, or if the download link is a one-time URL, resuming can fail and the transfer must restart from the beginning.

<details><summary>References</summary>
<ul>
<li><a href="https://help.nexusmods.com/article/170-resumable-downloads">Resumable Downloads - Nexus Mods Site Help</a></li>
<li><a href="https://addons.mozilla.org/en-US/firefox/addon/multithreaded-download-manager/">Multithreaded Download Manager – Get this Extension for...</a></li>

</ul>
</details>

**Discussion**: Commenters shared mixed experiences: some described a manual .part file swap workaround for one-time links, while others reported that Firefox resumable downloads are generally unstable and have been problematic since 2005. Several users recommended external tools like aria2 and Getright for more reliable, multi-connection downloads, and one commenter speculated that Firefox may fail to distinguish network EOF from request-level EOF.

**Tags**: `#Firefox`, `#downloads`, `#resumable`, `#browser`, `#tips`

---

<a id="item-17"></a>
## [Agent37 launches low-cost AI agent sandboxes at under 10% of typical provider costs](https://news.ycombinator.com/item?id=50059096) ⭐️ 6.0/10

Agent37, a YC F26 startup founded by former Amazon engineer Vishnu, launched sandboxes for running AI agents at under 10% of the cost of most sandbox providers, with customers spending an average of $0.37 per sandbox per month and free-plan infrastructure costs of just $0.05–$0.10 per user monthly. The company achieves this through burst-aware CPU/RAM management, renting bare-metal hosts from Hetzner and OVH instead of hyperscalers, using gVisor for resource sharing and fast boot times, and optimizing host shapes for RAM density. This launch highlights how AI agent sandboxing is becoming a price-competitive commodity, with startups undercutting hyperscalers by an order of magnitude. It matters for developers running messaging agents and other agent workloads who are sensitive to infrastructure costs, but also raises questions about whether pure cost optimization is a defensible moat against well-funded competitors. Agent37 uses gVisor-based sandboxes that share host memory across instances without reserving a full VM's memory, but these do not support Docker-in-Docker or Android emulators; full VM sandboxes are available at a slightly higher price for those workloads. The company notes RAM, not CPU, is typically the cost bottleneck for agent harness workloads, and its free plan now accounts for over 90% of new signups.

hackernews · vishnukool · Oct 12, 16:46

**Background**: AI agent sandboxes are isolated execution environments where agents can safely run generated code, shell commands, browser actions, and file I/O without touching production systems or user devices. An agent harness is the runtime scaffolding—such as Claude Code, OpenClaw, or Codex—that turns a stateless language model into an agent capable of multi-step tool use and task execution. As more developers deploy agents, demand for cheap, secure, and fast-booting sandboxes has grown, attracting providers like E2B, Daytona, Modal, and Northflank.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Agent_harness">Agent harness</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenClaw">OpenClaw - Wikipedia</a></li>
<li><a href="https://fast.io/resources/best-ai-agent-sandboxes/">Best AI Agent Sandboxes - Secure Execution Guide 2026</a></li>

</ul>
</details>

**Discussion**: Commenters largely praised the product's cost and usability—one user called it 'amazing' for a prototype—but many warned that sandboxes are commoditized and that competing purely on price against well-funded hyperscalers is a race to the bottom. Others raised technical caveats, noting that gVisor is less secure than full VMs and that the price comparison against VM-based providers is not apples-to-apples, while one user compared Agent37 favorably on price to boat.dev but noted less storage.

**Tags**: `#AI agents`, `#sandboxes`, `#cloud infrastructure`, `#startup`, `#YC`

---

<a id="item-18"></a>
## [Citroën Revives the 2CV as a Lightweight Electric Car](https://www.bbc.com/news/articles/c620r33plgppo) ⭐️ 6.0/10

Citroën has unveiled a modern electric reinterpretation of its iconic 2CV, emphasizing a class-leading sub-tonne weight and an affordable target price. The concept includes nostalgic design touches like 'champignon' pedals and a 'Radioën' infotainment system, and a van variant was also shown. This revival highlights how European automakers are leveraging heritage to differentiate themselves amid mounting competition from Chinese manufacturers. The focus on lightweight design could influence how affordable EVs are engineered, prioritizing efficiency over large batteries. The sub-tonne weight enables better range from a smaller battery, reduces tyre wear, and lowers road wear, which helps keep costs down. However, some design elements like the champignon pedals may not survive production due to regulatory requirements, and the seats will likely need headrests.

hackernews · scrlk · Oct 12, 12:09 · [Discussion](https://news.ycombinator.com/item?id=50055220)

**Background**: The original Citroën 2CV was an economy car produced from 1948 to 1990, known for its minimalist design and affordability that helped motorize post-war France. It featured an air-cooled flat-twin engine and was also available as a Fourgonnette van. Lightweighting is a key principle in EV design to improve efficiency and reduce battery size.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Citroën_2CV">Citroën 2CV - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters praised the sub-tonne weight as a standout engineering achievement that enables affordability and efficiency. Some expressed nostalgia for happy-looking car designs and skepticism about whether heritage alone can compete with Chinese EVs on value, while others noted regulatory hurdles for quirky features.

**Tags**: `#automotive`, `#electric vehicles`, `#design`, `#sustainability`, `#product revival`

---

<a id="item-19"></a>
## [ICLR Reviewers Grapple With AI-Generated Submissions](https://www.reddit.com/r/MachineLearning/comments/1x3ve39/hows_iclr_reviewing_going_for_you_any/) ⭐️ 6.0/10

A Reddit discussion on r/MachineLearning has raised concerns about the ICLR reviewing process, with users noting that it may be the first major conference to see automated research submissions and that AI-written text is becoming increasingly difficult to detect. Reviewers are asking how to identify 'slop' papers and how many high-quality versus AI-generated submissions they are seeing in their batches. This discussion highlights a growing challenge for top machine learning conferences: as AI writing tools improve, peer review systems may be overwhelmed by low-quality or AI-generated submissions, potentially undermining the integrity of scientific publishing and increasing the burden on volunteer reviewers. The thread specifically mentions ICLR's OpenReview platform, where submissions are publicly visible, and notes that detecting AI-written text is becoming harder despite advances in AI-text detection methods such as classifiers and statistical analysis. The discussion also touches on the difficulty of distinguishing genuine research from AI-generated 'slop' in early review stages.

reddit · r/MachineLearning · /u/ade17_in · Oct 12, 07:22

**Background**: ICLR (International Conference on Learning Representations) is a premier machine learning conference that uses OpenReview, a platform for open peer review where submissions and reviews are publicly accessible. AI-generated text detection involves using machine learning and natural language processing to identify content produced by AI tools, but these detectors often struggle with false positives and evolving AI models.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/International_Conference_on_Learning_Representations">International Conference on Learning Representations - Wikipedia</a></li>
<li><a href="https://openreview.net/about">About OpenReview</a></li>
<li><a href="https://aimultiple.com/ai-generated-text-detector">Top 20 AI-Generated Text Detectors Comparison</a></li>

</ul>
</details>

**Discussion**: The Reddit thread reflects a mix of concern and curiosity, with users sharing observations about the prevalence of AI-generated submissions and asking for strategies to detect them. Some commenters express frustration with the reviewing burden, while others note that high-quality papers still exist but are harder to find amid the noise.

**Tags**: `#ICLR`, `#peer-review`, `#AI-generated-text`, `#conference`, `#machine-learning`

---

<a id="item-20"></a>
## [Simon Willison releases web-edit 0.1a0 for phone-based file editing](https://simonwillison.net/2026/Oct/12/web-edit/) ⭐️ 5.0/10

Simon Willison released web-edit 0.1a0, an alpha Python web app that provides a browser UI for viewing and editing files in a folder. It is designed to run over Tailscale so an agent can start it and the user can edit files directly from a phone. The tool addresses a practical security concern in agentic coding workflows: editing sensitive files such as credentials without passing their contents through an LLM. It reflects a broader trend of developers building small, self-hosted utilities to safely supervise remote AI coding agents. The editor uses CodeMirror 6 rather than Monaco because Monaco still lacks a good mobile experience, and the app supports browsing, uploading, downloading, deleting, and inline previewing of images under 2 MB. It is an early 0.1a0 alpha release, so features and stability may change.

rss · Simon Willison · Oct 12, 15:54

**Background**: Tailscale is a mesh VPN that creates a private network between your devices, allowing secure access to services without exposing them to the public internet. Codex Remote refers to using OpenAI's Codex coding agent in a remote or cloud workspace, where the agent can read and edit code and run commands. web-edit fits into this setup by giving the human a direct, credential-safe way to edit files on the same machine the agent is working on.

<details><summary>References</summary>
<ul>
<li><a href="https://tailscale.com/learn/understanding-mesh-vpns">Understanding Mesh VPNs - Tailscale</a></li>
<li><a href="https://www.eigent.ai/blog/codex-cloud-remote-workspaces-run-ai-agents-from-anywhere">Codex Cloud Remote Workspaces</a></li>

</ul>
</details>

**Tags**: `#developer-tools`, `#python`, `#tailscale`, `#file-management`, `#llm-agents`

---

<a id="item-21"></a>
## [CL4SM Calls for Papers on Constrained Learning for Science](https://www.reddit.com/r/MachineLearning/comments/1x3vr5g/constrained_learning_for_scientific_modelling/) ⭐️ 5.0/10

A call for contributions has been issued for the CL4SM session at the ELLIS UnConference, a NeurIPS 2026 Paris pre-event, inviting 2-page submissions on machine learning models that respect physical constraints. The submission deadline is October 30, 2026 (23:59 AoE), with the session scheduled for December 8, 2026 at the Palais des Congrès de Paris. This session highlights a growing research direction where purely data-driven models can fit data well yet violate conservation laws, produce negative concentrations, or drift into unphysical regimes. By bringing together constrained learning, physics-informed ML, and structure-preserving architectures, it could help shape standards for trustworthy scientific machine learning in climate, fluids, energy, and engineering. Topics include soft constraint enforcement via penalty and augmented-loss formulations, hard enforcement by construction with structure-preserving architectures, projection and differentiable optimisation layers, constraints from governing equations and symmetries, and probabilistic constraints. Submissions use the PMLR template, are reviewed single-blind, are non-archival, and may include ongoing work, tutorials, demos, software libraries, datasets, or recently published papers from venues such as JMLR, NeurIPS, ICML, ICLR, AISTATS, and IEEE TPAMI.

reddit · r/MachineLearning · /u/cici118 · Oct 12, 07:46

**Background**: Physics-informed machine learning (PIML) embeds physical laws into the learning process, often reducing data requirements and improving generalization, with physics-informed neural networks (PINNs) as a well-known example. Constrained learning directly incorporates constraints during training, while structure-preserving neural networks build architectures that guarantee properties such as energy conservation and entropy inequality. CL4SM sits at the intersection of these areas, targeting scientific and engineering systems where physical consistency is essential.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/marcw_what-is-physics-informed-machine-learning-activity-7351536266015842304-nujt">What Is Physics - Informed Machine Learning ? | Marc Wouters</a></li>
<li><a href="https://en.wikipedia.org/wiki/Constraint_learning">Constraint learning</a></li>
<li><a href="https://arxiv.org/pdf/2004.04653">S tructure - preserving neural networks</a></li>

</ul>
</details>

**Tags**: `#machine-learning`, `#scientific-computing`, `#constrained-learning`, `#physics-informed-ml`, `#call-for-papers`

---

<a id="item-22"></a>
## [Developer seeks feedback on LLM pipeline that generates exam questions from school past papers](https://www.reddit.com/r/MachineLearning/comments/1x3wgif/generating_exam_questions_from_a_schools_own_past/) ⭐️ 5.0/10

A developer building a question bank feature for a high school platform (mixed Cambridge and in-house curriculum) described a working prototype that sends past-paper PDFs and mark schemes to an LLM, splits them into sub-question items tagged to curriculum objectives, has a small model write new questions, and uses a different model to answer them blind as a check. The pipeline currently achieves roughly an 80% pass rate on multiple-choice questions, while structured and practical questions remain weaker, with the small model inventing incorrect chemistry in lab setups. This is a concrete applied case study of using LLMs to generate assessment content grounded in a school's own materials, with curriculum objectives acting as guardrails and multi-model verification as a quality check. It highlights practical obstacles such as PDF extraction of scientific notation and cost at scale that many edtech teams will face when moving from prototype to production. The pipeline checks multiple-choice answer keys in code against the mark scheme rather than trusting the model, and a mid-size model fixed most of the incorrect chemistry generated by the smaller model. The developer is asking specifically about PDF extraction tools such as docling and marker for equations, tables and diagrams, whether pgvector is worth adding from day one, batch API and small-model cost experience at thousands of questions, and evaluation methods beyond human review.

reddit · r/MachineLearning · /u/SnooOpinions9858 · Oct 12, 08:31

**Background**: The project targets a high school platform that combines Cambridge and in-house curricula, and the curriculum's learning objectives already stored in the database are used to keep generated questions in scope. A curriculum admin approves all generated items, and teachers only draw from the approved bank, so the system is designed as a human-in-the-loop content pipeline rather than a fully autonomous generator. The stack is NestJS with Postgres using a schema per tenant on a self-hosted VPS, and exam content stays on the school's server while only curriculum text and question drafts are sent to the model.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/multi-llm-verification-pipeline">Multi-LLM Verification Pipeline - emergentmind.com</a></li>
<li><a href="https://medium.com/@nicole_burns42/what-is-multi-model-verification-and-does-it-actually-help-9aa245a15f6e">What is multi-model verification and does it actually help?</a></li>
<li><a href="https://techbanyan.com/train-ai-models-the-right-way-curriculum-learning-and-guardrails">Train AI Models the Right Way: Curriculum Learning and Guardrails</a></li>

</ul>
</details>

**Tags**: `#llm`, `#education`, `#question-generation`, `#pdf-extraction`, `#applied-ml`

---

<a id="item-23"></a>
## [datasette-ports 0.4 adds PID display and latest Datasette support](https://simonwillison.net/2026/Oct/12/datasette-ports/) ⭐️ 4.0/10

datasette-ports 0.4, a plugin that detects and lists all Datasette instances running on the current machine, now works with the latest version of Datasette and displays the detected process ID (PID) for each instance. Displaying the PID makes it much easier to attach the new Python 3.15 sampling profiler to a running Datasette process, which helps developers diagnose performance issues in their Datasette deployments. The plugin can be installed via 'datasette install datasette-ports' or run directly with 'uvx datasette-ports', and for each instance found it displays the URL, Datasette version, attached databases, and installed plugins.

rss · Simon Willison · Oct 12, 04:57

**Background**: Datasette is a Python tool for exploring and publishing data, often used to serve SQLite databases over HTTP. The datasette-ports plugin scans the local machine for running Datasette instances so users can see what is active. Python 3.15 introduces a new statistical sampling profiler (named Tachyon) that periodically samples the call stack, allowing programs to run at full speed while being profiled, unlike the older profile and cProfile modules.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/datasette/datasette-ports">GitHub - datasette/ datasette - ports : Find all currently running...</a></li>
<li><a href="https://docs.python.org/3.15/library/profiling.sampling.html">profiling . sampling — Statistical profiler — Python ...</a></li>
<li><a href="https://realpython.com/python315-sampling-profiler/">Python 3 . 15 Preview: Sampling Profiler – Real Python</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#python`, `#plugin`, `#release`, `#profiling`

---

<a id="item-24"></a>
## [Undergrad researcher desk-rejected by TMLR in 2 days without feedback](https://www.reddit.com/r/MachineLearning/comments/1x4h5bx/got_desk_rejected_at_tmlr_with_no_idea_why_d/) ⭐️ 4.0/10

An undergraduate researcher posted on r/MachineLearning that their paper on LLM self-explanations was desk rejected by TMLR within two days, with no reviewer comments or explanation, despite five months of work and a properly formatted submission. They are now asking the community whether to resubmit to TMLR, try a different venue, or seek feedback by email. This case highlights a growing tension in ML publishing: as TMLR's submission volume surges, its desk rejection rate has reportedly climbed to around 53%, leaving early-career researchers without feedback and unsure how to improve. It matters because opaque desk rejections can disproportionately hurt undergraduates and others who rely on publications for graduate school applications. The paper was on LLM self-explanations, a niche topic the author says was accepted at a venue in 2024, and the author claims to be the only desk-rejected submission they found on OpenReview. TMLR's desk rejection policy is driven by limited reviewer capacity amid a deluge of submissions, and desk rejections typically occur before peer review, often within one to three weeks.

reddit · r/MachineLearning · /u/Audaticreddit · Oct 12, 23:23

**Background**: TMLR (Transactions on Machine Learning Research) is a journal-style ML venue that uses OpenReview for submissions and reviews, and it has become popular because it offers rolling submissions and does not require a conference deadline. A desk rejection means an editor rejects a manuscript before sending it out for peer review, often due to scope fit, formatting, or capacity limits rather than scientific quality. LLM self-explanations are explanations that a large language model generates about its own reasoning or outputs, a topic within explainable AI (XAI).

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/transactions-on-machine-learning-research-tmlr_asking-authors-about-their-own-papers-activity-7506087797871697920-HbWc">TMLR Desk Rejection Rate Surges to 53% | Transactions... | LinkedIn</a></li>
<li><a href="https://casrai.org/guides/desk-rejection">What Desk Rejection Means and Why It Happens — CASRAI</a></li>
<li><a href="https://news.skrew.ai/llm-self-explanations-predict-model-behavior-faithfulness/">LLM Self - Explanations Can Predict Model Behavior, Study Finds</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion offers moderate advice and shared experiences, with commenters generally sympathizing with the author's frustration while noting that TMLR's high submission volume makes desk rejections increasingly common. Some suggest trying another venue or resubmitting later, and the overall sentiment is that opaque desk rejections are a systemic issue rather than a reflection of the paper's quality.

**Tags**: `#academic publishing`, `#peer review`, `#TMLR`, `#machine learning`, `#career advice`

---