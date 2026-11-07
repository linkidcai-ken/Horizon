---
layout: default
title: "Horizon Summary: 2026-11-07 (EN)"
date: 2026-11-07
lang: en
---

> From 23 items, 21 important content pieces were selected

---

1. [Tesla to wind down Cybertruck production amid poor sales](#item-1) ⭐️ 8.0/10
2. [Google's Muir linear attention enables 10M-token context in 25MB state](#item-2) ⭐️ 8.0/10
3. [Libghostty 1.0 Released with Stable C ABI](#item-3) ⭐️ 7.0/10
4. [Jev orchestrates Opus for LLM judges at 4x lower cost](#item-4) ⭐️ 7.0/10
5. [Practical Firecracker VM Escape Exploit Walkthrough Published](#item-5) ⭐️ 7.0/10
6. [Analysis claims AI is dramatically accelerating AI research](#item-6) ⭐️ 7.0/10
7. [Sodium-ion batteries approach cost parity with LFP, 70 GWh under supply deals](#item-7) ⭐️ 7.0/10
8. [Practical Guide to Bare-Metal UEFI Programming](#item-8) ⭐️ 7.0/10
9. [Boson AI Releases Higgs Realtime Duplex: A 45B Full-Duplex Multimodal Model](#item-9) ⭐️ 7.0/10
10. [FAA to phase out floppy disks from air traffic control by 2028](#item-10) ⭐️ 6.0/10
11. [Devvm.dev offers one VM per project for isolated development](#item-11) ⭐️ 6.0/10
12. [Google launches Gemini Omni 1.2 Flash video model with better character consistency](#item-12) ⭐️ 6.0/10
13. [Nilay Patel Critiques AI Industry's Costs and Hype](#item-13) ⭐️ 6.0/10
14. [Reddit discussion asks if industry still adopts ML ideas from academia](#item-14) ⭐️ 6.0/10
15. [ML Conference Reviewers Accused of LLM-Generated Experiment Requests](#item-15) ⭐️ 6.0/10
16. [ICLR 2027's 1-4 scale: a 2,2,3 average beats most papers](#item-16) ⭐️ 6.0/10
17. [CASP-DREAM TAP Challenge: Predict TCR Activation on Unseen Peptides](#item-17) ⭐️ 6.0/10
18. [ICLR Reviewer Flags Paper as Too Close to Author's Own Workshop Version](#item-18) ⭐️ 5.0/10
19. [MSc Student Asks How to Build Visibility via Open Source Contributions](#item-19) ⭐️ 4.0/10
20. [Reddit Users Share Early ICLR 2027 Review Scores](#item-20) ⭐️ 3.0/10
21. [PhD student seeks TCN forecasting research guidance after hiatus](#item-21) ⭐️ 3.0/10

---

<a id="item-1"></a>
## [Tesla to wind down Cybertruck production amid poor sales](https://www.nbcnews.com/tech/tech-news/tesla-wind-cybertruck-production-years-poor-sales-markets-rcna607817) ⭐️ 8.0/10

Tesla announced it will wind down Cybertruck production in mid-2027, citing poor sales that have fallen to roughly 10% of the originally planned 250,000 units per year. The decision comes as Cybertruck sales dropped 28% in 2026, with only about 20,000 units sold in the US in 2025. The discontinuation of Tesla's flagship electric pickup signals deepening challenges in the US EV market, where sales share has stagnated and federal tax credits have expired. It raises questions about Tesla's product strategy and its ability to compete as Chinese EV makers dominate globally. The Cybertruck was originally touted as an 'apocalypse-proof' vehicle with a 250,000-unit annual production target, but actual sales have been about a tenth of that. Tesla plans to repurpose the production line to increase output of its Cybercab robotaxi instead.

hackernews · PLenz · Nov 6, 12:13 · [Discussion](https://news.ycombinator.com/item?id=50391456)

**Background**: The Cybertruck is Tesla's first electric pickup truck, launched in 2023 after years of delays. It features a stainless steel exoskeleton and was aimed at the lucrative US truck market, but its polarizing design and high price tag limited its appeal. The EV market has also cooled due to rising interest rates, supply chain issues, and increased competition.

<details><summary>References</summary>
<ul>
<li><a href="https://www.usatoday.com/story/cars/shopping/evs/2026/11/06/tesla-cybertruck-production-ending/92639472007/">Why Tesla is ending Cybertruck production for Cybercab</a></li>
<li><a href="https://electrek.co/2026/11/06/tesla-ending-cybertruck-production-sales-10-percent-plan/">Tesla to end Cybertruck production as sales stall at ~10% of ...</a></li>
<li><a href="https://www.businessinsider.com/cybertruck-sales-decline-tesla-elon-musk-cox-automotive-data-2026-1">Tesla Is Really Struggling to Sell the Cybertruck, Data Shows ...</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters offered mixed views: some praised the Cybertruck's massive battery for powering homes during outages, while others criticized its impracticality as a truck, high price, and Tesla's broader business challenges including expired tax credits and competition from Chinese EVs. Many agreed the vehicle was a wrong bet on ever-rising truck prices.

**Tags**: `#Tesla`, `#Cybertruck`, `#EV industry`, `#automotive`, `#business strategy`

---

<a id="item-2"></a>
## [Google's Muir linear attention enables 10M-token context in 25MB state](https://www.reddit.com/r/MachineLearning/comments/1xplbuu/muir_linear_attention_with_sensitivityallocated/) ⭐️ 8.0/10

Google Research introduced Muir, a linear attention architecture that overcomes three bottlenecks in channel-wise gated delta models (like GDN-2) through matched-filter readout, sensitivity-allocated gating, and a numerically stable large-chunk parallel kernel. It streams 10M tokens without perplexity drift in a fixed 25MB state and achieves 90.0% zero-shot passkey accuracy at 1M tokens, where GDN-2 collapses past 4K-8K and a Transformer runs out of memory past 64K. This work directly addresses the prohibitive memory cost of KV caches in long-context Transformers—a 1.3B model needs 2.1TB of KV cache at 10M tokens—by compressing history into a tiny fixed state while improving recall beyond simple passkey tasks. If validated, it could make million-token context practical for deployment on commodity hardware and advance linear attention as a viable alternative to standard Transformers. Muir's matched-filter readout equalizes slow-decaying rows via an inverse fractional power law and per-token query modulation, relaxing write erasure by 17% and extending lookback horizon by 60%; fusing all 5 gates into one rank-512 projection cuts gate parameters 4.5x to widen the FFN by 30.4%. The boundary-pivoted multiplicative decays avoid fp32 underflow and NaN issues (which affected 25% of heads), and a recursive block-Neumann solver routes 98% of chunkwise FLOPs onto matrix units, training 2.7x faster than Splash Attention at 32K.

reddit · r/MachineLearning · /u/CategoryNormal149 · Nov 6, 19:10

**Background**: Linear attention models like Gated DeltaNet compress the entire history into a fixed-size state matrix, avoiding the growing KV cache that standard Transformers require for autoregressive generation. Gated delta models use a delta rule to update this state with key-value error correction and gates to control what is written or forgotten. However, channel-wise gating introduces imbalances—such as slow-decaying rows accumulating excessive energy—that degrade long-range recall. Muir redesigns the readout, gating, and kernel to fix these issues while keeping the state compact.

<details><summary>References</summary>
<ul>
<li><a href="https://divagr.com/attention-lab/delta">Gated DeltaNet Explained — Attention Lab</a></li>
<li><a href="https://huggingface.co/docs/transformers/kv_cache">Cache strategies - Hugging Face</a></li>
<li><a href="https://arxiv.org/abs/2104.03961">[2104.03961] Generalized Approach to Matched Filtering using ... Generalized approach to matched filtering using neural networks Generalized approach to matched filtering using neural networks GeneralizedApproachto MatchedFiltering using Neural Networks Generalized approach to matched filtering using neural networks Generalized approach to matched filtering using neural networks</a></li>

</ul>
</details>

**Tags**: `#linear-attention`, `#efficient-transformers`, `#long-context`, `#gated-delta-networks`, `#google-research`

---

<a id="item-3"></a>
## [Libghostty 1.0 Released with Stable C ABI](https://mitchellh.com/writing/libghostty-1-0) ⭐️ 7.0/10

Libghostty, the core library extracted from the Ghostty terminal emulator, has reached version 1.0, meaning both the library itself and its C ABI are now stable. This milestone provides a stable foundation for developers to build terminal emulators or embed terminal functionality into their applications, potentially accelerating innovation in terminal tooling across platforms. Libghostty is a portable, high-performance C library that is open source under the MIT license, and its 1.0 release ensures long-term API and ABI compatibility for integrators.

hackernews · mfiguiere · Nov 6, 23:30 · [Discussion](https://news.ycombinator.com/item?id=50399933)

**Background**: Ghostty is a fast, feature-rich, cross-platform terminal emulator that uses platform-native UI and GPU acceleration. Libghostty is the underlying library that powers Ghostty, designed to be reusable by other projects. It is written in C and Zig, and Zig is a systems programming language that emphasizes performance and simplicity while maintaining C ABI compatibility.

<details><summary>References</summary>
<ul>
<li><a href="https://mitchellh.com/writing/libghostty-1-0">Libghostty 1.0 – Mitchell Hashimoto</a></li>
<li><a href="https://github.com/ghostty-org/ghostty">GitHub - ghostty-org/ghostty: Ghostty is a fast, feature ...</a></li>
<li><a href="https://ziglang.org/">Home Zig Programming Language</a></li>

</ul>
</details>

**Discussion**: Commenters generally praised the release, with one noting it's refreshing to see a project reach 1.0 in an era of perpetual 0.x software. Some questioned the choice of C over Zig for the interface, and others lamented the lack of a Windows version of Ghostty.

**Tags**: `#terminal`, `#libghostty`, `#release`, `#open-source`, `#zig`

---

<a id="item-4"></a>
## [Jev orchestrates Opus for LLM judges at 4x lower cost](https://hightouch.com/blog/llm-judges-identity-resolution) ⭐️ 7.0/10

A blog post by Hightouch demonstrates that a cheaper orchestrator model, Jev, can query Opus for help on LLM-as-a-judge tasks, achieving accuracy comparable to Opus alone at roughly 4x lower cost. The experiment focuses on identity resolution, a specific task where Jev decides when to escalate to Opus. This approach shows that model orchestration—using a cheaper model to decide when to call a stronger, more expensive model—can significantly reduce costs for evaluation tasks. It suggests a practical path for companies to maintain high accuracy in LLM judges without paying for top-tier models on every query. The result is specific to identity resolution and does not claim general improvements for all LLM-judge tasks or coding agents. The orchestrator, Jev, is a discriminative model that returns typed values with confidence scores, and it decides when to escalate to Opus.

hackernews · theanomaly · Nov 6, 19:48 · [Discussion](https://news.ycombinator.com/item?id=50397429)

**Background**: LLM-as-a-judge is a technique where a large language model evaluates the quality of outputs from another model. Jev, developed by TypeSafe AI, is a discriminative model designed for classification and regression, returning structured decisions with confidence scores rather than generating text. Identity resolution is the process of linking records that refer to the same entity, often used in customer data platforms.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Jev_(AI_model)">Jev (AI model)</a></li>
<li><a href="https://en.wikipedia.org/wiki/LLM-as-a-Judge">LLM-as-a-Judge - Wikipedia</a></li>
<li><a href="https://appperformancelab.com/ai-agents-identity-resolution-in-2026/">AI Agents: Identity Resolution Strategies for 2026</a></li>

</ul>
</details>

**Discussion**: Commenters noted the result is task-specific (identity resolution) and not a general claim, with some debating context curation and reductive-logic pitfalls. Others shared similar experiences, noting that a cheaper model like Jev can effectively decide when to escalate to a stronger model, but the economics are highly task-dependent.

**Tags**: `#llm-judges`, `#cost-optimization`, `#model-orchestration`, `#identity-resolution`, `#ai-agents`

---

<a id="item-5"></a>
## [Practical Firecracker VM Escape Exploit Walkthrough Published](https://pwn.ai/blog/firecracker-escape) ⭐️ 7.0/10

A new blog post titled 'Firecracker VM Escape: PwnEscape Part 2' provides a practical walkthrough for exploiting the previously disclosed PwnEscape vulnerability (CVE-2026-99999) to escape Firecracker microVMs. The writeup demonstrates a guest-to-host escape in a configuration that lacked Firecracker's jailer and seccomp protections. This matters because Firecracker underpins many serverless and multi-tenant platforms (e.g., AWS Lambda), so a practical VM escape highlights the importance of defense-in-depth controls like the jailer and seccomp. It also fuels debate over hypervisor design tradeoffs between minimal VMMs and formally verified microkernels. The tested configuration had no jailer, meaning privileges were not dropped and namespaces/seccomp were not applied; the authors note that a deployment using those controls requires a separate assessment of post-compromise privileges. The vulnerability itself (CVE-2026-99999) is a Linux kernel flaw involving virtio-net checksum offload metadata that enables guest-to-host memory disclosure and potential escape.

hackernews · SerCe · Nov 6, 19:33 · [Discussion](https://news.ycombinator.com/item?id=50397219)

**Background**: Firecracker is a lightweight virtual machine monitor (VMM) designed for serverless computing, using a minimal device model and a per-VM jailer process with seccomp filters to reduce the attack surface. PwnEscape (CVE-2026-99999) is a Linux kernel vulnerability that allows a guest VM to potentially escape to the host by exploiting virtio-net checksum offload handling. Patched kernels have been released by distributions such as AlmaLinux.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/firecracker-microvm/firecracker/blob/main/docs/jailer.md">firecracker/docs/jailer.md at main · firecracker-microvm ...</a></li>
<li><a href="https://almalinux.org/blog/2026-10-16-pwnescape-cve-2026-99999/">PwnEscape (CVE-2026-99999): Patched kernels... | AlmaLinux OS</a></li>
<li><a href="https://news.ycombinator.com/item?id=50397219">Firecracker VM Escape : PwnEscape Part 2 | Hacker News</a></li>

</ul>
</details>

**Discussion**: Commenters highlighted that the tested configuration lacked the jailer and seccomp, so real-world exposure depends on proper hardening; some advocated for the Nova microhypervisor approach with a formally verified microkernel, while others noted a public ClickBench playground running hundreds of database engines could be used to PoC the escape. Several pointed out this is not a new vulnerability but a practical exploitation guide for the previously disclosed PwnEscape flaw.

**Tags**: `#security`, `#virtualization`, `#firecracker`, `#exploitation`, `#hypervisor`

---

<a id="item-6"></a>
## [Analysis claims AI is dramatically accelerating AI research](https://www.planned-obsolescence.org/p/ai-is-dramatically-accelerating-ai) ⭐️ 7.0/10

An analysis piece on planned-obsolescence.org argues that AI is dramatically accelerating AI research right now, and that if this acceleration compounds, naive extrapolation implies superintelligence within a year. The article sparked a highly engaged Hacker News discussion with 192 points and 148 comments. The debate touches on whether recent AI progress reflects genuine intelligence gains or is largely driven by benchmark overfitting and massive capital investment in scaling, which has major implications for how the industry and public should interpret AI capability claims. Commenters raise caveats including that benchmarks are curated and can be expensively trained on, that much uplift may come from horizontal scaling of agent swarms and parallel token spend rather than vertical model intelligence, and that training speed on trillions of tokens may remain a fundamental bottleneck.

hackernews · yurivish · Nov 6, 20:27 · [Discussion](https://news.ycombinator.com/item?id=50397994)

**Background**: AI benchmarks are standardized tests used to measure model capabilities, but models can be optimized specifically for them, a phenomenon known as benchmark overfitting. Neural scaling laws describe how model performance improves predictably as parameters, data, and compute are increased, and recent progress has largely followed this playbook. The debate over whether AI can accelerate its own research is central to discussions of recursive self-improvement and superintelligence.

<details><summary>References</summary>
<ul>
<li><a href="https://www.planned-obsolescence.org/p/ai-is-dramatically-accelerating-ai">AI is dramatically accelerating AI research right now</a></li>
<li><a href="https://en.wikipedia.org/wiki/Neural_scaling_law">Neural scaling law - Wikipedia</a></li>
<li><a href="https://nhimg.org/glossary/benchmark-overfitting/">What Is Benchmark Overfitting ? Definition & Examples</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion is largely skeptical: commenters question whether gains stem from benchmark overfitting, note that AI may accelerate work without changing the world faster, and argue that capital-driven horizontal scaling and parallel token spend explain much of the uplift. Others point to training speed as a fundamental bottleneck and recommend alternative analyses.

**Tags**: `#AI research`, `#AI acceleration`, `#benchmarks`, `#scaling laws`, `#community discussion`

---

<a id="item-7"></a>
## [Sodium-ion batteries approach cost parity with LFP, 70 GWh under supply deals](https://www.pv-magazine.com/2026/11/06/sodium-ion-batteries-approach-cost-parity-with-lfp-with-70-gwh-covered-by-supply-agreements/) ⭐️ 7.0/10

Sodium-ion batteries are nearing cost parity with lithium iron phosphate (LFP) batteries, with 70 GWh of supply already covered by agreements, according to a pv magazine report. This signals that sodium-ion technology is moving from lab research toward commercial-scale deployment in energy storage. If sodium-ion achieves cost parity with LFP, it could reshape the energy storage market by offering a cheaper, safer, and more abundant alternative for grid storage, home batteries, and low-cost electric vehicles. This would reduce reliance on lithium and diversify battery supply chains. Sodium-ion batteries still have lower volumetric energy density than LFP, requiring larger packaging, but they offer advantages in safety and cold-temperature operation. Recent cost estimates place sodium-ion cells at roughly $55–85/kWh in 2026, compared to $95–110/kWh for LFP cells, though pack-level costs may narrow the gap.

hackernews · doener · Nov 6, 23:00 · [Discussion](https://news.ycombinator.com/item?id=50399657)

**Background**: Sodium-ion batteries are rechargeable batteries that use sodium ions as charge carriers instead of lithium, which is more abundant and cheaper. LFP (lithium iron phosphate) is a widely used lithium-ion chemistry known for safety and long cycle life, and it currently dominates grid storage and many EV markets. Sodium-ion technology has been improving in energy density and is now entering mass production, with potential for stationary storage and low-performance EVs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.patsnap.com/resources/blog/articles/sodium-ion-vs-lfp-2026-battery-cost-advantages/">Sodium - Ion vs LFP Battery Costs 2025: 10-20% Cheaper... | PatSnap</a></li>
<li><a href="https://the-adaptist.com/technology/sodium-ion-vs-lithium-home-battery-2026">Sodium - Ion vs Lithium Batteries 2026: Cost , Safety... | The Adaptist</a></li>
<li><a href="https://en.wikipedia.org/wiki/Sodium-ion_battery">Sodium-ion battery - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters expressed enthusiasm for sodium-ion home batteries due to safety and temperature tolerance, with one noting a real-world 12V sodium replacement for lead-acid in an EV. Others were skeptical about commercialization timelines, complaining that announcements are repetitive and asking when the products will actually be available for purchase.

**Tags**: `#batteries`, `#energy-storage`, `#sodium-ion`, `#hardware`, `#cleantech`

---

<a id="item-8"></a>
## [Practical Guide to Bare-Metal UEFI Programming](https://kevinboone.me/efitest_index.html) ⭐️ 7.0/10

Kevin Boone published a multi-part guide on getting started with bare-metal UEFI programming, covering toolchain setup, the absence of a C standard library, and EFI's Windows-like coding conventions. This guide fills a gap for systems programmers interested in UEFI development, providing a practical entry point to a niche but important area of firmware and bootloader programming. The guide highlights that UEFI applications lack a standard C library, requiring developers to use EFI services directly, and notes that the PE32+ binary format and Windows-like conventions stem from Intel's original EFI design.

hackernews · LaSombra · Nov 6, 16:50 · [Discussion](https://news.ycombinator.com/item?id=50394855)

**Background**: UEFI (Unified Extensible Firmware Interface) is the modern firmware interface that replaces BIOS, responsible for initializing hardware and loading the operating system. Bare-metal programming means writing code that runs directly on hardware without an underlying OS, which is essential for bootloaders and firmware. UEFI applications are typically written in C but must adhere to specific calling conventions and use EFI-provided services instead of standard libraries.

<details><summary>References</summary>
<ul>
<li><a href="https://www.baeldung.com/cs/uefi-bare-metal-program-development">How to Make a Bare-Metal Program With UEFI (No OS Required)</a></li>
<li><a href="https://krinkinmu.github.io/2020/10/11/efi-getting-started.html">Getting started with EFI | Welcome to the Mike’s homepage!</a></li>
<li><a href="https://en.wikipedia.org/wiki/UEFI">UEFI - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters shared additional resources like edk2-libc for C standard library support and uefi-rs for Rust development, and suggested using `nm -D --undefined-only` to verify no unresolved symbols remain. Some noted the Windows-like coding style is intentional due to Intel's heritage, while others expressed frustration with UEFI's quirks such as 16-bit character handling.

**Tags**: `#UEFI`, `#bare-metal`, `#systems-programming`, `#bootloader`, `#firmware`

---

<a id="item-9"></a>
## [Boson AI Releases Higgs Realtime Duplex: A 45B Full-Duplex Multimodal Model](https://www.reddit.com/r/MachineLearning/comments/1xpn5pv/higgs_realtime_duplex_a_45b_moe_fullduplex_model/) ⭐️ 7.0/10

Boson AI has released Higgs Realtime Duplex, a 45B-parameter Mixture-of-Experts model that processes audio, video, and text streams simultaneously in 160ms chunks while performing background reasoning, tool calls, and delegation. The model is not open-weight, and access to the Duplex API is via a waitlist, though the previous turn-based Higgs Realtime is available now. This release represents a significant step toward real-time, interactive multimodal AI that can listen, watch, and speak concurrently while handling complex background tasks, potentially enabling more natural and efficient human-computer interaction. It also highlights a design trade-off between mid-sized front models with delegation and larger all-in-one background models, influencing cost and latency in voice AI applications. The model uses a chunked-stream design with 160ms chunks, representing audio at 6.25 tokens/s input and 12.5 tokens/s output, and video at ~12 tokens per camera frame every 6 chunks, totaling ~2.6K tokens per minute for audio and video. It is trained via multi-teacher on-policy distillation from specialist teachers and a self-improvement loop, and benchmarks show it leads on some tasks but lags in turn-taking (Full-Duplex-Bench v1.5: 75.5 vs. 80.1 for OpenAI's best).

reddit · r/MachineLearning · /u/Cali_Cobarde · Nov 6, 20:23

**Background**: Full-duplex models are AI systems that can listen and speak at the same time, unlike traditional turn-based voice assistants that wait for the user to finish before responding. Mixture-of-Experts (MoE) is an architecture that activates only a subset of parameters for each input, improving efficiency. Boson AI's model builds on its previous Higgs Realtime speech-to-speech model and competes with other real-time multimodal systems like Thinking Machines' interaction models and OpenAI's offerings.

<details><summary>References</summary>
<ul>
<li><a href="https://www.boson.ai/blog/higgs-realtime-duplex">Higgs Realtime Duplex: Face to Face, Working in the ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2410.00037">Moshi: a speech -text foundation model for real - time dialogue</a></li>

</ul>
</details>

**Tags**: `#multimodal`, `#full-duplex`, `#MoE`, `#voice-ai`, `#realtime-inference`

---

<a id="item-10"></a>
## [FAA to phase out floppy disks from air traffic control by 2028](https://www.reuters.com/world/us/us-faa-says-it-will-phase-out-floppy-disks-air-traffic-control-by-2028-2026-11-05/) ⭐️ 6.0/10

The US Federal Aviation Administration announced it will replace outdated floppy disks used in air traffic control systems with a new digital platform called E-IDS by 2028. The E-IDS system will unify four legacy systems across 435 air traffic control facilities, handling vital weather and other critical information. This modernization affects the safety and efficiency of US air traffic control, which handles millions of flights annually, and highlights the challenges of upgrading safety-critical legacy systems in government infrastructure. It also serves as a case study for other industries grappling with aging technology. The legacy system, IDS-4, was actually developed in the early 1990s (not the 1980s as sometimes claimed) and runs on MS-DOS using 3.5-inch floppy disks. The E-IDS program has been in development since at least 2020 with a planned rollout starting in 2025, and the FAA's rigorous safety risk management process significantly slows progress.

hackernews · ChrisArchitect · Nov 6, 04:00 · [Discussion](https://news.ycombinator.com/item?id=50388001)

**Background**: Floppy disks are magnetic storage media that were common in the 1980s and 1990s but have been largely obsolete for decades. Safety-critical systems like air traffic control often retain legacy technology because replacing them requires extensive certification and risk management to ensure continued safety. The FAA's modernization efforts involve transitioning from these old systems to modern digital platforms while maintaining strict safety standards.

<details><summary>References</summary>
<ul>
<li><a href="https://arstechnica.com/tech-policy/2026/11/faa-to-finally-ditch-floppy-disks-in-what-it-calls-historic-tech-upgrade/">FAA to finally ditch floppy disks in what it calls "historic ...</a></li>
<li><a href="https://www.nytimes.com/2026/11/06/us/faa-floppy-disks-atc-2028.html">F.A.A. to Phase Out Floppy Disks in Air Traffic Control ...</a></li>
<li><a href="https://tech.yahoo.com/science/articles/faa-still-uses-floppy-disks-183215755.html">The FAA Still Uses Floppy Disks. That Changes by 2028.</a></li>

</ul>
</details>

**Discussion**: Commenters with insider experience emphasized that FAA's safety risk management, while rigorous, significantly slows progress, and noted resistance from long-tenured engineers. Others questioned the technical details, such as whether a floppy emulator could have been used, and criticized political grandstanding around the announcement, while clarifying that the IDS-4 system dates from the early 1990s, not the 1980s.

**Tags**: `#legacy-systems`, `#aviation`, `#government-it`, `#modernization`, `#safety-critical-systems`

---

<a id="item-11"></a>
## [Devvm.dev offers one VM per project for isolated development](https://devvm.dev/) ⭐️ 6.0/10

Devvm.dev launched as a tool that creates a dedicated virtual machine for each software project, aiming to isolate dependencies and toolchains. The project received 112 points and 48 comments on Hacker News, where developers discussed its approach and compared it to alternatives. As development environments grow more complex and AI agents increasingly need access to internal infrastructure, strong isolation between projects becomes critical for security and reproducibility. This tool adds to a growing trend of VM-based dev environments, competing with Canonical Workshop and libvirt-based setups. The discussion revealed that Devvm.dev's documentation does not clearly explain whether images are built per project or copy-on-write from shared toolchains, a key detail for efficiency. Commenters also noted that the tool may lack advanced features like GPU acceleration, memory ballooning, and credential-injecting proxies needed in large enterprises.

hackernews · luispa · Nov 6, 17:30 · [Discussion](https://news.ycombinator.com/item?id=50395450)

**Background**: A VM-per-project approach gives each codebase its own isolated operating system instance, preventing dependency conflicts and limiting the blast radius of untrusted code. This contrasts with container-based tools like Docker, which share the host kernel and offer weaker isolation. Canonical Workshop is a similar recent tool built on LXD system containers, while libvirt is a widely used open-source API for managing virtualization platforms.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/canonical/workshop">GitHub - canonical/workshop: Workshops are secure, fast, and ...</a></li>
<li><a href="https://libvirt.org/">libvirt: The virtualization API</a></li>
<li><a href="https://vm.fyi/en/docs/desktop-virtualization/dev-environment-isolation">Development Environment Isolation - vm.fyi</a></li>

</ul>
</details>

**Discussion**: Commenters were generally skeptical, with some saying the tool is a 'fun toy' that doesn't meet enterprise needs for secure agent access to internal registries, logs, and infrastructure. Others shared their own similar projects built on libvirt/cloud-init or krunkit, and pointed to Canonical Workshop as a competing solution. A common theme was frustration with the difficulty of managing many isolated environments for AI-driven development workflows.

**Tags**: `#virtualization`, `#developer-tools`, `#dev-environments`, `#isolation`, `#hackernews`

---

<a id="item-12"></a>
## [Google launches Gemini Omni 1.2 Flash video model with better character consistency](https://blog.google/innovation-and-ai/technology/developers-tools/introducing-gemini-omni-1-2-flash/) ⭐️ 6.0/10

Google introduced Gemini Omni 1.2 Flash, a new multimodal video generation model that supports generating and editing 15-second videos with improved character consistency compared to its predecessor, Gemini Omni 1.1 Flash. Improved character consistency is a key challenge in AI video generation, and this update could make Google's tools more viable for creative workflows, but the confusing rollout and access restrictions may hinder adoption among developers and paying users. The model is available through Google Flow and the Gemini app for AI Plus, Pro, and Ultra subscribers, with some free access via YouTube Shorts and the YouTube Create app; however, users report vague and contradictory information about availability, and the model still struggles with complex motion and accurate text rendering.

hackernews · thisisauserid · Nov 6, 13:35 · [Discussion](https://news.ycombinator.com/item?id=50392118)

**Background**: Gemini Omni is Google's family of multimodal models designed for video generation, editing, extension, and upscaling. Character consistency refers to the ability to keep a person's appearance stable across frames, which is crucial for storytelling and professional video production. The model is part of Google's broader push into generative AI video, competing with tools like Kling and other text-to-video models.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.cloud.google.com/gemini-enterprise-agent-platform/models/gemini/omni-1-2-flash">Gemini Omni 1 . 2 Flash | Gemini Enterprise Agent Platform</a></li>
<li><a href="https://deepmind.google/models/model-cards/gemini-omni-flash/">Gemini Omni Flash - Model Card — Google DeepMind</a></li>
<li><a href="https://gemini.google/us/overview/video-generation/?hl=en">Gemini Omni – Create & edit videos as easy as having a conversation</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters criticized the confusing rollout, with one noting that asking the Gemini app yields vague and contradictory answers about availability. Others complained about access restrictions and pricing, while some pointed out that the model is available in Google Flow and offers improved character consistency, though its practical benefits remain unclear.

**Tags**: `#AI`, `#video-generation`, `#Google`, `#Gemini`, `#generative-ai`

---

<a id="item-13"></a>
## [Nilay Patel Critiques AI Industry's Costs and Hype](https://simonwillison.net/2026/Nov/6/nilay-patel/) ⭐️ 6.0/10

In a recent Vergecast episode, Nilay Patel argued that AI products do not justify their environmental, economic, and social costs, stating that the industry's spending far outstrips real benefits and that 'agents aren't real' in terms of useful deployment. This critique from a respected tech commentator highlights growing skepticism about the AI industry's economics and social impact, potentially influencing public perception and investor confidence as spending on AI infrastructure continues to soar. Patel specifically criticized AI overviews and deepfake 'slop' as poor justifications for data center noise and costs, and mentioned hacked refrigerators holding blood storage in Europe as an example of misplaced priorities, while also linking AI spending to political corruption.

rss · Simon Willison · Nov 6, 17:13

**Background**: AI Overviews are Google Search's AI-generated summaries at the top of results, and 'AI slop' refers to low-quality content produced by generative AI. AI agents are software systems that autonomously perform tasks, but Patel questions their current usefulness. The Vergecast is a popular tech podcast hosted by Nilay Patel.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_Overviews">AI Overviews - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_slop">AI slop - Wikipedia</a></li>
<li><a href="https://cloud.google.com/discover/what-are-ai-agents">What are AI agents? Definition, examples, and types | Google ...</a></li>

</ul>
</details>

**Tags**: `#AI industry`, `#AI economics`, `#commentary`, `#tech criticism`, `#AI hype`

---

<a id="item-14"></a>
## [Reddit discussion asks if industry still adopts ML ideas from academia](https://www.reddit.com/r/MachineLearning/comments/1xponb2/what_exactly_is_the_relationship_between_ml/) ⭐️ 6.0/10

A Reddit post on r/MachineLearning questions whether the historical dynamic of academia driving industry adoption of ML methods (as with ADAM and TRPO) still holds in 2026, observing that industry appears increasingly self-sufficient and unmoved by academic follow-up work. This matters because it touches on the evolving division of labor between academia and industry in AI, affecting how research funding, talent, and career paths in ML are structured, and raising concerns about the relevance of university research in an increasingly applied field. The poster notes that thousands of academic papers propose new optimization routines and architectures (CNN/RNN) with heavy GPU use, yet serious industry adoption is low to none, suggesting a divergence where industry has become the primary idea generator and works in-house.

reddit · r/MachineLearning · /u/Strong_Boy_757 · Nov 6, 21:25

**Background**: ADAM (Adaptive Moment Estimation) is an optimization algorithm for training deep neural networks, and TRPO (Trust Region Policy Optimization) is a reinforcement learning method; both originated in academia and became widely used in industry. The post reflects on the period 2012-2018 when academic research often paved the way for industrial applications, and contrasts it with the current landscape where large tech companies drive many advances.

<details><summary>References</summary>
<ul>
<li><a href="https://machinelearningmastery.com/adam-optimization-algorithm-for-deep-learning/">Gentle Introduction to the Adam Optimization Algorithm for Deep...</a></li>
<li><a href="https://www.mathworks.com/help/reinforcement-learning/ug/trpo-agents.html">Trust Region Policy Optimization (TRPO) Agent - MathWorks Trust Region Policy Optimization (TRPO) Explained [1502.05477] Trust Region Policy Optimization - arXiv.org rlTRPOAgent - Trust region policy optimization (TRPO ... [2512.23770] SB-TRPO: Towards Safe Reinforcement Learning ... Reinforcement Learning: PPO vs TRPO Comparison</a></li>

</ul>
</details>

**Tags**: `#machine-learning`, `#academia-industry`, `#research-trends`, `#community-discussion`

---

<a id="item-15"></a>
## [ML Conference Reviewers Accused of LLM-Generated Experiment Requests](https://www.reddit.com/r/MachineLearning/comments/1xpsj1p/ml_conferences_what_do_you_think_about_reviewer/) ⭐️ 6.0/10

A Reddit user on r/MachineLearning complained that reviewers at ML conferences are issuing generic requests for additional experiments that appear to be copy-pasted from an LLM, missing the paper's core point and burdening authors under strict page limits. The user plans to raise the issue confidentially with the Area Chair (AC). This highlights a growing concern about the integrity and quality of peer review in ML conferences, where LLM-generated feedback may lead to low-value, generic requests that waste authors' time and undermine the review process. It affects researchers submitting to top conferences and could prompt changes in review guidelines or detection tools. The author notes that the requests are minor, miss the paper's main point, and that reviewers often fail to engage with the results even after authors complete the extra experiments. The strict 10-page limit in ML conferences exacerbates the burden, and the author wishes reviewers would discuss core insights rather than act as 'experiment-running machines.'

reddit · r/MachineLearning · /u/Temporary_Switch_339 · Nov 7, 00:17

**Background**: Peer review at ML conferences like ICML, NeurIPS, and ICLR relies on volunteer reviewers and area chairs (ACs) to evaluate submissions. With the rise of large language models (LLMs), there is increasing evidence that some reviews may be LLM-generated, raising concerns about review quality and integrity. Area chairs oversee the review process and can address conflicts or concerns raised by authors.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sciencedirect.com/science/article/pii/S3050577125000167">Ensuring peer review integrity in the era of large language ...</a></li>
<li><a href="https://qipeng.me/blog/what-does-an-area-chair-do/">What does an area chair actually do, anyway? | Peng Qi</a></li>
<li><a href="https://icml.cc/">2027 Conference</a></li>

</ul>
</details>

**Tags**: `#peer-review`, `#machine-learning`, `#conferences`, `#LLM`, `#academia`

---

<a id="item-16"></a>
## [ICLR 2027's 1-4 scale: a 2,2,3 average beats most papers](https://www.reddit.com/r/MachineLearning/comments/1xps7xu/iclr_2027s_new_14_scale_a_2_2_3_is_better_than_it/) ⭐️ 6.0/10

An analysis of 73,410 public OpenReview reviews for ICLR 2027 found that 57% of all reviews are a 2, only 1.5% are a 4, and the median paper averages exactly 2.0 on the new 1-4 scale. This means a paper with scores 2, 2, 3 (mean 2.33) is already above most papers. This provides authors with a first empirical calibration for ICLR 2027's new 1-4 scale, helping them interpret their scores more accurately and avoid unnecessary panic over seemingly low numbers. It also highlights how score distributions can skew heavily toward the lower end, which may influence reviewer training and conference decision-making. The analysis is based on the first 25,000 of ~40,800 submissions in OpenReview's listing order (read Nov 6), not a random sample, and the public page shows only counts without titles, authors, or review text. The author also built the page, which primarily serves as promotion for their tool.

reddit · r/MachineLearning · /u/latenticlabs · Nov 7, 00:03

**Background**: ICLR (International Conference on Learning Representations) is a top machine learning conference that uses open peer review via OpenReview, where reviews and scores are publicly visible. For 2027, ICLR switched from its previous scoring system to a 4-point scale: 1 clear reject, 2 weak reject, 3 weak accept, 4 clear accept. Because the scale is new, the community lacks intuition for what a given set of scores means, prompting analyses like this one.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Open_peer_review">Open peer review - Wikipedia</a></li>
<li><a href="https://openreview.net/about">About OpenReview</a></li>
<li><a href="https://iclr.cc/Conferences/2026">2026 Conference</a></li>

</ul>
</details>

**Tags**: `#peer-review`, `#ICLR`, `#machine-learning`, `#academic-publishing`, `#statistics`

---

<a id="item-17"></a>
## [CASP-DREAM TAP Challenge: Predict TCR Activation on Unseen Peptides](https://www.reddit.com/r/MachineLearning/comments/1xpn4gp/caspdream_tap_challenge_tcr_peptidemhc_activation/) ⭐️ 6.0/10

The CASP-DREAM TAP Challenge has opened registration, inviting participants to predict whether a T cell activates given a TCR sequence and a peptide-HLA pair. The benchmark contains about 5,800 labeled combinations, and every test peptide is at least four Levenshtein edits away from any peptide with a publicly reported TCR specificity. This challenge addresses a core difficulty in computational immunology: TCRs with similar sequences can recognize different antigens, so models must generalize to truly novel peptides rather than memorizing known specificities. A well-designed held-out benchmark could drive progress in sequence models for immunotherapy and vaccine development. Submissions are scored by AUROC, and participants can use training data options listed on Synapse, including the public VDJdb database and proprietary TCR datasets from Harell Data provided by Adaptive Biotechnologies. The strict four-edit distance constraint on test peptides makes the task substantially harder than standard random splits.

reddit · r/MachineLearning · /u/Harell-Data · Nov 6, 20:22

**Background**: T cell receptors (TCRs) recognize peptide fragments presented by MHC molecules on cell surfaces, and this recognition triggers T cell activation, a key step in immune response. Predicting which TCR binds which peptide-MHC complex from sequence alone is a long-standing challenge because TCR sequence diversity is enormous and similar TCRs can have different specificities. VDJdb is a curated public database of TCR sequences with known antigen specificities, commonly used to train and benchmark such models. AUROC (area under the receiver operating characteristic curve) measures how well a model ranks positive cases above negative ones across all thresholds.

<details><summary>References</summary>
<ul>
<li><a href="https://vdjdb.com/">VDJdb</a></li>
<li><a href="https://en.wikipedia.org/wiki/Receiver_operating_characteristic">Receiver operating characteristic - Wikipedia</a></li>
<li><a href="https://www.nature.com/articles/s41587-026-03128-x?error=cookies_not_supported&code=46e3d7a0-f879-4d7b-909b-a9142ea2a9d7">Deep peptide recognition profiling decodes TCR specificity and...</a></li>

</ul>
</details>

**Tags**: `#computational-biology`, `#machine-learning`, `#benchmark`, `#sequence-models`, `#immunology`

---

<a id="item-18"></a>
## [ICLR Reviewer Flags Paper as Too Close to Author's Own Workshop Version](https://www.reddit.com/r/MachineLearning/comments/1xpf4t6/iclr27_reviewer_says_my_paper_is_too_close_to_the/) ⭐️ 5.0/10

A Reddit user reports that an ICLR reviewer flagged their submission as very closely related to an earlier workshop/arXiv paper by the same authors, and asked for a comparison. The author had changed the method name and title, making the two versions appear distinct at first glance, and now asks how to argue they are the same work without breaking anonymity. This highlights a common tension in ML peer review between double-blind anonymity and the need to disclose prior versions of a paper, especially as arXiv and workshop preprints are increasingly common. How conferences handle self-plagiarism and incremental improvements affects many researchers submitting to top venues like ICLR. The author admits the scores are already bad and has little hope, but says this is a first for them; the core challenge is pointing the reviewer to the earlier paper as their own work without revealing identity. ICLR's double-blind policy generally allows citing anonymous prior work in the third person, but confirming authorship during review is tricky.

reddit · r/MachineLearning · /u/fanconic · Nov 6, 15:09

**Background**: ICLR (International Conference on Learning Representations) is one of the three top machine learning conferences, alongside NeurIPS and ICML, and uses double-blind peer review where authors and reviewers are anonymous to each other. Many researchers first share work as arXiv preprints or workshop papers before submitting extended versions to major conferences, which can raise concerns about self-plagiarism and overlap.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/International_Conference_on_Learning_Representations">International Conference on Learning Representations</a></li>
<li><a href="https://en.wikipedia.org/wiki/Scholarly_peer_review">Scholarly peer review - Wikipedia</a></li>
<li><a href="https://www.enago.com/academy/double-blind-peer-review-anonymity-problems/">Double - Blind Peer Review : Why Anonymity Fails... - Enago Academy</a></li>

</ul>
</details>

**Tags**: `#peer-review`, `#ICLR`, `#academic-publishing`, `#machine-learning`, `#anonymity`

---

<a id="item-19"></a>
## [MSc Student Asks How to Build Visibility via Open Source Contributions](https://www.reddit.com/r/MachineLearning/comments/1xp90lz/how_do_you_build_visibility_through_open_source/) ⭐️ 4.0/10

An MSc computer science student with a 3D computer vision background posted on r/MachineLearning asking how to build visibility and credibility in the AI/ML community by contributing to established open source projects instead of standalone GitHub repositories. The student argues that standalone projects feel like a weaker signal now that AI tools make building things easier than ever. This question reflects a growing concern among early-career AI/ML practitioners that the proliferation of AI-assisted coding tools is devaluing personal projects as a portfolio signal, pushing them toward contributions in established open source communities as a more credible proof of work. The answers could shape how students and job seekers approach career development in a crowded field. The student specifically asks about current challenges for new contributors and how to find projects where meaningful contributions can actually get noticed, seeking experiences from those working in 3D CV, ML, or applied AI. No specific projects, tools, or quantitative data are mentioned in the post.

reddit · r/MachineLearning · /u/Few-Cheetah3336 · Nov 6, 09:55

**Background**: Open source contributions are widely regarded as a democratic way to build credibility in AI, independent of degree, employer, or location. However, the majority of open source contributors are casual contributors who contribute only occasionally, and new contributors often face barriers such as understanding project norms, finding good first issues, and getting maintainers' attention. In 3D computer vision, a field focused on extracting three-dimensional information from images, established projects often have steep learning curves and specialized codebases.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.drjobpro.com/building-credibility-in-ai-publications-talks-and-open-sourc/">Building Credibility in AI: Publications, Talks, and Open So</a></li>
<li><a href="https://opensource.guide/building-community/">Building Welcoming Communities | Open Source Guides</a></li>
<li><a href="https://en.wikipedia.org/wiki/3D_computer_vision">3D computer vision</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#career-advice`, `#machine-learning`, `#computer-vision`, `#community-discussion`

---

<a id="item-20"></a>
## [Reddit Users Share Early ICLR 2027 Review Scores](https://www.reddit.com/r/MachineLearning/comments/1xpedgc/iclr_2027_review_scores_n/) ⭐️ 3.0/10

A Reddit post on r/MachineLearning links to a discussion thread where users share their ICLR 2027 review scores, with one commenter reporting a score of 3/3/2. The post itself contains no substantive analysis, only a title and a link to the comments. ICLR is one of the three most prestigious machine learning conferences, so its review scores directly affect researchers' publication prospects and career trajectories. Early score-sharing threads give authors a rough sense of the score distribution and help them gauge whether to prepare a rebuttal. ICLR uses a discrete rating scale without scores of 2, 4, 7, or 9, so the difference between a 5 and a 6 is often decisive. According to the search results, ICLR 2027 reviews are scheduled for release on November 5, with author discussion running until November 18 and decisions on December 16.

reddit · r/MachineLearning · /u/No-Lab4175 · Nov 6, 14:37

**Background**: ICLR (International Conference on Learning Representations) is held annually in late April or early May and, along with NeurIPS and ICML, is considered one of the three highest-impact conferences in machine learning and AI research. Its peer review is conducted on OpenReview, where reviews and author responses are publicly visible. Review scores are a key signal for authors, but final acceptance also depends on rebuttal, area chair judgment, and the overall score distribution.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/International_Conference_on_Learning_Representations">International Conference on Learning Representations - Wikipedia</a></li>
<li><a href="https://phdflow.ai/guides/iclr-review-scores-explained">ICLR review scores: what 3, 5, 6 and 8 mean - phdflow.ai</a></li>
<li><a href="https://phdflow.ai/deadlines">ML conference deadlines 2026/ 2027 : ICLR , NeurIPS, ACL</a></li>

</ul>
</details>

**Discussion**: The discussion is a casual score-sharing thread where users compare their review results, and one commenter opened with a 3/3/2. The overall sentiment is a mix of anxiety and mutual support typical of conference review waiting periods, with no substantive technical debate.

**Tags**: `#ICLR`, `#peer-review`, `#machine-learning`, `#academia`, `#reddit`

---

<a id="item-21"></a>
## [PhD student seeks TCN forecasting research guidance after hiatus](https://www.reddit.com/r/MachineLearning/comments/1xpb6kb/i_need_some_guidance_after_a_six_month_hiatus_r/) ⭐️ 3.0/10

A fifth-year PhD student who took a six-month mental health hiatus after a second IEEE journal rejection is asking the r/MachineLearning community for pointers on recent Temporal Convolutional Network (TCN) and time-series forecasting research. The student aims to produce a third publication using the MetaboNet continuous glucose monitor (CGM) dataset to unlock the thesis-writing stage. This request highlights the growing pressure on PhD students to publish in high-impact journals and the mental health toll of repeated rejections. It also reflects the practical challenge of identifying novel research directions in mature areas like TCN-based forecasting, where incremental improvements may struggle to meet journal novelty thresholds. The student has chosen TCN as the 'safest option' for forecasting on the MetaboNet dataset, which standardizes CGM and insulin data for type 1 diabetes research. They admit that anxiety and feeling overwhelmed have hindered their own literature search, and they are unsure what would be considered novel enough for publication.

reddit · r/MachineLearning · /u/Neural_Prodigy · Nov 6, 12:06

**Background**: Temporal Convolutional Networks (TCNs) are a class of deep learning models for sequence data that use dilated causal convolutions to capture long-range dependencies, often outperforming recurrent networks like LSTMs in forecasting tasks. MetaboNet is a standardized dataset that consolidates multiple type 1 diabetes management datasets, including continuous glucose monitor (CGM) and insulin data, to enable comparable and generalizable algorithm research. Publishing in IEEE or Elsevier journals typically requires demonstrating clear novelty, such as a new architecture, training method, or application insight.

<details><summary>References</summary>
<ul>
<li><a href="https://metabo-net.org/">MetaboNet</a></li>
<li><a href="https://arxiv.org/abs/2606.18640">[2606.18640] MetaboNet-Bench: A Multi-modal Benchmark for ...</a></li>
<li><a href="https://www.myperfectinternet.com/deep-learning-for-time-series-forecasting-temporal-convolutional-networks-tcn/">Deep Learning for Time - Series Forecasting : Temporal ...</a></li>

</ul>
</details>

**Tags**: `#machine-learning`, `#time-series-forecasting`, `#TCN`, `#PhD-advice`, `#reddit`

---