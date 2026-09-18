---
layout: default
title: "Horizon Summary: 2026-09-18 (EN)"
date: 2026-09-18
lang: en
---

> From 28 items, 20 important content pieces were selected

---

1. [Android 17 Adds New APIs Without Releasing Them to AOSP](#item-1) ⭐️ 8.0/10
2. [Photon-Emission-Guided Laser Fault Injection Bypasses RP2350 Secure Debug](#item-2) ⭐️ 8.0/10
3. [Cactus Needle 3: 8-29MB Automation Models Match DeepSeek V4 Flash](#item-3) ⭐️ 8.0/10
4. [Rust Security Team Warns of Targeted Attacks on Prominent Rustaceans](#item-4) ⭐️ 8.0/10
5. [Claude Code adds AGENTS.md support in version 2.1.277](#item-5) ⭐️ 7.0/10
6. [Cloudflare saves another 100TB of RAM using math and Rust](#item-6) ⭐️ 7.0/10
7. [Xcode 27.1 Beta Adds iPhone Duo Development Support](#item-7) ⭐️ 7.0/10
8. [US troop deaths in Iran war exceed Pentagon count by at least four](#item-8) ⭐️ 7.0/10
9. [NHANES CHD risk model with leakage audit and calibration fix](#item-9) ⭐️ 7.0/10
10. [OpenJev landing page sparks debate on Jev semantic decoding](#item-10) ⭐️ 6.0/10
11. [Reddit proposal: augment driving datasets with synthetic edge cases](#item-11) ⭐️ 6.0/10
12. [Reddit user seeks studies isolating back-and-forth LLM interaction from one-way sharing and self-refinement](#item-12) ⭐️ 6.0/10
13. [uv 0.12.16 Adds Hash Verification for Downloaded Packages](#item-13) ⭐️ 5.0/10
14. [Cloudflare Quick Tunnels Gets New Landing Page, Sparks Criticism](#item-14) ⭐️ 5.0/10
15. [Minimal Phone 2: A Refined Minimalist Android Phone Draws Skepticism](#item-15) ⭐️ 5.0/10
16. [Simon Willison Compares Ignoring LLMs to Ignoring Jurassic Park](#item-16) ⭐️ 5.0/10
17. [AWS Principal Applied Scientist James Gung Hosts Reddit AMA](#item-17) ⭐️ 5.0/10
18. [Reddit user asks how mid-tier AI journals compare to top conferences like NeurIPS](#item-18) ⭐️ 5.0/10
19. [Simon Willison Highlights Pelican Bicycle Scene in Who Framed Roger Rabbit](#item-19) ⭐️ 3.0/10
20. [AAAI-27 Phase 1 Results Thread on Reddit](#item-20) ⭐️ 3.0/10

---

<a id="item-1"></a>
## [Android 17 Adds New APIs Without Releasing Them to AOSP](https://grapheneos.social/@GrapheneOS/117282080803799576) ⭐️ 8.0/10

Android 17 is reportedly the first Android version since the 3.x era to introduce new APIs without releasing them to the Android Open Source Project (AOSP). GrapheneOS highlighted this change, noting that the new APIs appeared only in a Pixel-exclusive update rather than being upstreamed to the public AOSP codebase. This shift raises concerns about Google's commitment to keeping Android truly open source, since third-party projects like GrapheneOS depend on timely AOSP releases to build privacy- and security-focused alternatives. If new APIs remain Pixel-exclusive, custom ROMs and OEMs may fall behind, potentially fragmenting the Android ecosystem. According to community discussion, Google ships four Pixel updates per year including documentation and SDKs, but only delivers 'real' Android source-code updates to OEMs and the public every half-year. The first and third quarterly release patches each year now appear to be Pixel-exclusive, meaning new APIs can land in Pixel SDKs before reaching AOSP.

hackernews · theanonymousone · Sep 18, 19:03 · [Discussion](https://news.ycombinator.com/item?id=49758736)

**Background**: The Android Open Source Project (AOSP) is the free and open-source codebase primarily licensed under the Apache License, from which Google and third parties build Android distributions. GrapheneOS is a non-profit, open-source mobile OS focused on privacy and security, built on AOSP and officially supported on Google Pixel devices. Historically, Google has released Android source code to AOSP alongside or shortly after Pixel updates, allowing projects like GrapheneOS to incorporate the latest features and security patches.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Android_(operating_system)">Android (operating system) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/GrapheneOS">GrapheneOS</a></li>
<li><a href="https://source.android.com/">Android Open Source Project</a></li>

</ul>
</details>

**Discussion**: Commenters expressed frustration with Google's perceived roadblocks against GrapheneOS, with some arguing Google regrets Android being open source. Others clarified that the core issue is not a single Pixel-exclusive API but the pattern of first and third quarterly patches being Pixel-exclusive, while some praised GrapheneOS and hoped Google would not crush it.

**Tags**: `#Android`, `#AOSP`, `#GrapheneOS`, `#Open Source`, `#Google`

---

<a id="item-2"></a>
## [Photon-Emission-Guided Laser Fault Injection Bypasses RP2350 Secure Debug](https://donjon.ledger.com/blog/rp2350-secure-debug-laser-fault-injection/) ⭐️ 8.0/10

Researchers at Ledger Donjon demonstrated a photon-emission-guided laser fault injection attack that restores Secure debug access on the RP2350 A4 microcontroller by flipping two bits in the debug enable register. The attack combines differential photon-emission microscopy to localize the target register with SWD-guided laser pulses, requiring physical access, destructive chip preparation, and roughly $250,000 in lab equipment. This is a significant hardware security result because the RP2350 was marketed with secure boot and permanent debug-disable features intended to resist exactly this kind of tampering, and the RP2350's secure enclave had made it attractive as a Yubikey alternative. It underscores that physical attackers with sufficient resources can still defeat modern microcontroller security, reinforcing the ongoing arms race between secure hardware designers and fault-injection researchers. The attack specifically targets the RP2350 A4 stepping and requires destructive preparation to expose the silicon die, plus approximately $250,000 in laboratory equipment for the initial discovery and documentation. Community commenters note that replication in a home lab is feasible for under $25,000, and likely under $10,000, using cheaper tools such as the PicoEMP instead of professional-grade equipment.

hackernews · synack · Sep 18, 16:54 · [Discussion](https://news.ycombinator.com/item?id=49757050)

**Background**: Laser fault injection (LFI) is a physical attack technique that fires precisely focused laser pulses at an exposed silicon die to cause targeted transistors to malfunction at specific moments during a cryptographic or security operation. Photon-emission microscopy (PEM) is a failure-analysis technique that detects faint light emitted by switching transistors, allowing researchers to localize active circuit regions without probing. The RP2350 is Raspberry Pi's microcontroller featuring a secure enclave, secure boot, and one-time-programmable (OTP) debug-disable settings designed to prevent unauthorized access to internal secrets.

<details><summary>References</summary>
<ul>
<li><a href="https://donjon.ledger.com/blog/rp2350-secure-debug-laser-fault-injection/">Photon-Emission-Guided Laser Fault Injection Enables RP2350 ...</a></li>
<li><a href="https://github.com/raspberrypi/rp2350_hacking_challenge">GitHub - raspberrypi/rp2350_hacking_challenge</a></li>
<li><a href="https://threatcluster.io/cluster/laser-fault-injection-vulnerability-in-rp2350-microcontrolle-17a268d3">Laser Fault Injection Vulnerability in RP2350 Microcontroller</a></li>

</ul>
</details>

**Discussion**: Commenters broadly appreciated the technical depth of the write-up while debating practicality: one noted the $250k figure reflects discovery and documentation costs, and that replication is doable under $10k with tools like the PicoEMP, citing a similar MPC5566 attack replicated with a $50 tool versus a $5,000 one. Others framed the result as part of an inevitable arms race between safe-crackers and safe-builders, and one remarked on the impressive scale of using chip photon emission for imaging, reminiscent of early DRAM imaging discoveries.

**Tags**: `#hardware-security`, `#fault-injection`, `#RP2350`, `#embedded-security`, `#laser-attack`

---

<a id="item-3"></a>
## [Cactus Needle 3: 8-29MB Automation Models Match DeepSeek V4 Flash](https://cactuscompute.com/needle) ⭐️ 8.0/10

Cactus Compute released Needle 3, a family of ultra-small automation models (8-29MB, 25-121M parameters at 2-bit) that focus on tool calls and structured JSON output rather than chat. The 20-layer model scores 86.0 on Mobile Actions, beating LFM2.5 1.2B (82.4), Qwen3.5 0.8B (76.0), and Apple's on-device model (57.6), and the company claims DeepSeek V4 Flash-grade performance on narrow tasks after finetuning. This shows that extremely small models can handle structured automation tasks at a fraction of the size of general-purpose LLMs, enabling on-device tool calling in low-power environments like cars, homes, and industrial PLCs. It also signals a shift toward task-specific, tunable models rather than monolithic chat models for production automation. Needle 3 uses Intelligence Laddering, where each layer (2 to 20) is a deployable subnetwork from one set of weights, and replaces the dense FFN with a Monarch Hadamard MLP that costs O(d√d) parameters instead of O(d²). It adds case-insensitive regex triggers, calibrated confidence scores, multilingual support (EN, FR, ES, DE, NL, IT, PL), and runs on macOS, Linux, Windows, Android, iOS, watchOS, tvOS, WebAssembly, and WASI.

hackernews · HenryNdubuaku · Sep 18, 00:11 · [Discussion](https://news.ycombinator.com/item?id=49748553)

**Background**: Needle is a family of tiny language models designed specifically for automation: calling tools and emitting structured JSON, not open-ended conversation. Intelligence Laddering means a single trained network can be sliced into smaller subnetworks at inference time, trading accuracy for speed and size. The Monarch Hadamard MLP is a structured matrix technique that compresses the feed-forward layer by replacing dense matrices with Kronecker products of smaller matrices, drastically reducing parameters while preserving expressiveness.

<details><summary>References</summary>
<ul>
<li><a href="https://cactuscompute.com/blog/hadamard-mlp">The Hadamard MLP: Channel Mixing for Almost No Parameters | Cactus</a></li>
<li><a href="https://proceedings.mlr.press/v162/dao22a/dao22a.pdf">Monarch: Expressive Structured Matrices for Efﬁcient and Accurate Training</a></li>
<li><a href="https://github.com/HarryR/z80ai">GitHub - HarryR/z80ai: Z80-μLM is a 2 - bit quantized language model ...</a></li>

</ul>
</details>

**Discussion**: Commenters found the model promising for low-power use cases like voice assistants and industrial automation, but noted limitations: indirect commands often fail, and the thermostat sometimes responds in the wrong direction. Several suggested adding a confidence threshold to the demo, since bad responses tend to have low confidence scores.

**Tags**: `#small language models`, `#automation`, `#tool calls`, `#structured output`, `#edge AI`

---

<a id="item-4"></a>
## [Rust Security Team Warns of Targeted Attacks on Prominent Rustaceans](https://simonwillison.net/2026/Sep/17/targeted-attacks-on-rustaceans/) ⭐️ 8.0/10

On September 17, 2026, Adam Harvey and the crates security team published a warning about an ongoing social-engineering campaign targeting rust-lang members and owners of popular crates, aiming to compromise their devices and accounts so attackers can publish malware. The campaign uses fake video-call invitations for jobs, projects, or contracts to trick targets into installing a purported missing audio codec or executing a command placed on the clipboard. This is an active supply-chain threat against the Rust ecosystem, and the same trick already succeeded last month in a supply-chain attack on the arrayref crate, showing that maintainer accounts are a high-value entry point into software used by countless downstream projects. Because almost every piece of software depends on open source, any developer with publishing rights in a dependency network is a potential vector, so the warning is actionable for the entire open-source community. The attack relies on social engineering rather than a technical vulnerability: targets are invited to a video call framed as a positive opportunity, then pressured to install software or run a clipboard-supplied command. The Rust security team's warning follows the confirmed August 20, 2026 supply-chain attack on the arrayref crate, and Simon Willison suggests dependency cooldowns—delaying upgrades to new package releases by a few days—as a practical defense.

rss · Simon Willison · Sep 17, 23:59

**Background**: A supply chain attack targets less-secure elements in the software supply chain—such as a maintainer's account or a small dependency—to inject malicious code into the larger software that depends on it. Social engineering is the use of psychological pressure, such as a fake job offer or phishing, to influence people into performing actions or divulging information. In the Rust ecosystem, crates are packages published to crates.io, and whoever controls a crate's publishing rights can push code to every project that depends on it.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Supply_chain_attack">Supply chain attack</a></li>
<li><a href="https://en.wikipedia.org/wiki/Social_engineering_attack">Social engineering attack</a></li>
<li><a href="https://crates.io/crates">crates.io: Rust Package Registry</a></li>

</ul>
</details>

**Tags**: `#security`, `#supply-chain`, `#rust`, `#open-source`, `#social-engineering`

---

<a id="item-5"></a>
## [Claude Code adds AGENTS.md support in version 2.1.277](https://code.claude.com/docs/en/changelog) ⭐️ 7.0/10

Starting in version 2.1.277, Claude Code will check for and use an AGENTS.md file when no CLAUDE.md is present in a folder. This support is implemented as a built-in "mod" built on Claude Code's upcoming customization system, with source available on GitHub. This addresses a significant interoperability gap between Claude Code and other AI coding agents like Codex that already use the AGENTS.md standard, making it easier for developers who use multiple tools to maintain a single set of project instructions. The high community engagement and public criticism from figures like Shopify CEO Tobi Lütke show that cross-agent compatibility is becoming a major expectation in the developer tools ecosystem. The AGENTS.md support only activates when no CLAUDE.md exists, and community members note that Claude Code still does not detect skills located in .agents/skills directories. The feature is built on the mods system, meaning users will eventually be able to create custom versions of project instructions themselves.

hackernews · datadrivenangel · Sep 18, 21:00 · [Discussion](https://news.ycombinator.com/item?id=49760187)

**Background**: AGENTS.md is a simple, open Markdown format used by over 60,000 open-source projects to give AI coding agents project-specific context and instructions, functioning like a README for agents. CLAUDE.md is Anthropic's equivalent file that Claude Code reads automatically at the start of each session. As developers increasingly use multiple AI coding agents, having a shared instruction file reduces duplication and inconsistency across tools.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/agentsmd/agents.md">GitHub - agentsmd/agents.md: AGENTS.md — a simple, open format for guiding coding agents</a></li>
<li><a href="https://agents.md/">AGENTS.md</a></li>
<li><a href="https://academy.claude.com/courses/claude-code-101/the-claude-md-file">The CLAUDE.md file · Claude Code 101 · Claude Academy</a></li>

</ul>
</details>

**Discussion**: Community reaction is mixed: many appreciate the interoperability improvement but criticize it as the "absolute bare minimum," noting that symlink workarounds are now unnecessary. Commenters also highlight remaining gaps such as .agents/skills not being detected, and Shopify CEO Tobi Lütke publicly threatened to ban Claude Code at Shopify until it reads AGENTS.md and .agents/skills.

**Tags**: `#Claude Code`, `#AGENTS.md`, `#AI coding agents`, `#developer tools`, `#interoperability`

---

<a id="item-6"></a>
## [Cloudflare saves another 100TB of RAM using math and Rust](https://blog.cloudflare.com/saving-100-tb-of-ram-with-math/) ⭐️ 7.0/10

Cloudflare published a blog post detailing how it used mathematical optimizations, including a smaller ketama-style ring and a more compact Rust hash struct, to save an additional 100TB of RAM across its infrastructure. The company rolled out the change gradually, temporarily keeping both the old and new cacheable load balancer representations in memory during the transition. At Cloudflare's scale, shaving 100TB of RAM translates into substantial cost savings and more headroom for other workloads, and the write-up offers a reusable playbook for engineers optimizing large distributed systems. The accompanying Hacker News discussion highlights broader tensions between aggressive optimization and long-term code maintainability. The optimization involved shrinking the hash representation used for the cacheable load balancer, with the Rust section focusing on a struct that stores hashes; one commenter noted that 2 bytes per hash matters only because there is a hash for every task on every computer. Cloudflare deliberately avoided a single global flip because a bad change could have caused an apocalyptic increase in origin traffic.

hackernews · f311a · Sep 18, 18:51 · [Discussion](https://news.ycombinator.com/item?id=49758580)

**Background**: Cloudflare operates a massive global edge network that handles a large share of internet traffic, so even small per-request memory overheads multiply into terabytes across its fleet. Hash rings are a common technique for distributing load across servers, and their memory footprint depends on how many entries and how many bytes per entry are stored. Rust is increasingly used in such performance-critical infrastructure for its memory safety and low-level control.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.cloudflare.com/saving-100-tb-of-ram-with-math/">Saving another 100 TB of RAM with math (and Rust) | Cloudflare Blog</a></li>
<li><a href="https://leventov.medium.com/hash-table-tradeoffs-cpu-memory-and-variability-22dc944e6b9a">Hash table tradeoffs: CPU, memory, and variability | by Roman Leventov | Medium</a></li>

</ul>
</details>

**Discussion**: Commenters largely praised the writing style and the impressiveness of the optimizations, with one noting they preferred it to many recent Cloudflare blog posts. Others raised concerns about codebase complexity and impenetrable silos, questioned whether the hash savings were truly necessary, and joked that the freed RAM would simply be consumed by AI inference.

**Tags**: `#cloudflare`, `#memory-optimization`, `#distributed-systems`, `#hashing`, `#engineering`

---

<a id="item-7"></a>
## [Xcode 27.1 Beta Adds iPhone Duo Development Support](https://developer.apple.com/documentation/xcode-release-notes/xcode-27_1-release-notes) ⭐️ 7.0/10

Apple released the first Xcode 27.1 beta on September 18, 2026, adding updated SDKs and a simulator that supports the iPhone Duo's foldable poses and orientations. This allows developers to build and test apps for Apple's first foldable iPhone ahead of its October 23, 2026 release. This release gives developers roughly a month to adapt their apps to a fundamentally new form factor before the iPhone Duo reaches customers, a significant platform shift for the iOS ecosystem. Poorly optimized apps at launch could hurt early user experience and pressure developers to update quickly. Xcode 27.1 beta requires Apple silicon Macs running macOS 26.6 or later, and Apple bundles a /uikit-app-modernization skill to help developers adopt layouts for the iPhone Duo. The simulator specifically supports the device's new poses and orientations, which is critical for testing foldable-specific UI behavior.

hackernews · CameronBanga · Sep 18, 18:39 · [Discussion](https://news.ycombinator.com/item?id=49758419)

**Background**: The iPhone Duo is Apple's first foldable iPhone, announced on September 9, 2026, featuring an outer display and a large inner display when unfolded. Xcode is Apple's integrated development environment, and its beta releases typically precede new hardware launches so developers can prepare apps in advance. Foldable devices introduce new layout and orientation challenges that differ from traditional slab phones.

<details><summary>References</summary>
<ul>
<li><a href="https://www.macrumors.com/2026/09/18/apple-releases-xcode-27-1-beta-iphone-duo-support/">Apple Releases Xcode 27 . 1 Beta With iPhone Duo... - MacRumors</a></li>
<li><a href="https://9to5mac.com/2026/09/18/apple-releases-xcode-27-1-beta-enabling-iphone-duo-app-development/">Apple releases Xcode 27 . 1 beta , enabling iPhone Duo app... - 9to5Mac</a></li>
<li><a href="https://en.wikipedia.org/wiki/IPhone_Duo">IPhone Duo</a></li>

</ul>
</details>

**Discussion**: Developers on Hacker News expressed a mix of excitement and concern: some noted the short window between simulator availability and customer launch, expecting many apps to look broken initially, while others worried about app optimization and older apps showing oddities on the new form factor. One commenter shared screenshots of compiling their app, and another raised concerns about Xcode 27.1 not running on older macOS versions like Mavericks.

**Tags**: `#Xcode`, `#iOS Development`, `#Apple`, `#iPhone Duo`, `#Developer Tools`

---

<a id="item-8"></a>
## [US troop deaths in Iran war exceed Pentagon count by at least four](https://www.reuters.com/world/middle-east/us-troop-deaths-iran-war-exceed-pentagon-count-by-least-four-washington-post-2026-09-18/) ⭐️ 7.0/10

A Reuters and Washington Post investigation published on September 18, 2026, reports that US troop deaths during the Iran war exceed the Pentagon's official count by at least four, citing unidentified officials. The report also notes that not all of the undisclosed deaths were directly tied to the months-long conflict, but involved US personnel stationed in the Middle East amid ongoing hostilities. The discrepancy raises serious questions about government transparency and the accuracy of official casualty reporting during an active conflict, potentially eroding public trust in the Pentagon and the administration. It could also intensify congressional scrutiny and public debate over the conduct and human cost of the US-Iran war. The investigation relies on unidentified officials and does not specify the exact circumstances of the additional deaths, leaving open the question of whether personnel who died in the Middle East from causes unrelated to combat should be classified as war fatalities. The Pentagon has not publicly confirmed or disputed the higher figure.

hackernews · wslh · Sep 18, 22:35 · [Discussion](https://news.ycombinator.com/item?id=49761178)

**Background**: The United States and Iran have been engaged in a months-long military conflict, and the Pentagon regularly publishes official casualty figures that shape public perception of the war. Investigative journalism has historically played a key role in uncovering gaps between official statements and actual events, as seen in past conflicts like Vietnam and Iraq. Reuters and the Washington Post are major news organizations whose joint reporting adds credibility to the findings.

**Discussion**: Commenters drew historical parallels to the Iraq War era, with one noting that in both 2006 and 2026 a president embroiled the country in an unpopular Middle East war and lied about it. Others debated whether deaths of US personnel in the Middle East from non-combat causes should count as war fatalities, and some criticized the media focus by pointing to other alleged atrocities and unrelated events.

**Tags**: `#geopolitics`, `#military`, `#investigative-journalism`, `#government-transparency`, `#war`

---

<a id="item-9"></a>
## [NHANES CHD risk model with leakage audit and calibration fix](https://www.reddit.com/r/MachineLearning/comments/1wjp062/classifying_coronary_heart_disease_risk_from/) ⭐️ 7.0/10

A developer built a machine learning project predicting self-reported, physician-diagnosed coronary heart disease (CHD) from four cycles of NHANES data (2011-2012 to 2017-2018), covering about 21,500 adults after cleaning. The project compares logistic regression, random forest, and gradient boosting, and includes a full leakage audit plus a sigmoid recalibration step that fixed badly miscalibrated probabilities (mean predicted risk ~30% vs. actual 4%). This work highlights two critical but often overlooked issues in healthcare machine learning: data leakage from questionnaire variables that directly encode other cardiovascular diagnoses, and poor probability calibration in imbalanced clinical datasets. By openly documenting the leakage effect (PR-AUC jumping from 0.23 to 0.51 when leaky features were included) and fixing calibration, the project provides a practical template for more trustworthy clinical prediction models. Final held-out test results show ROC-AUC 0.875 and PR-AUC 0.239 for logistic regression, with random forest and gradient boosting performing similarly; age alone achieves 0.83 AUC, and PPV at the chosen threshold is only 0.13, meaning most positive predictions are wrong given the ~4% CHD prevalence. The decision threshold was frozen on the development set before touching the test set, and features like smoking status, diabetes, and blood pressure medication use are not yet included.

reddit · r/MachineLearning · /u/YouJonaa · Sep 18, 12:36

**Background**: NHANES (National Health and Nutrition Examination Survey) is a nationally representative survey conducted by the National Center for Health Statistics that combines interviews, physical examinations, and laboratory tests to assess the health and nutritional status of U.S. adults and children. Data leakage in machine learning occurs when a model uses information during training that would not be available at prediction time, leading to overly optimistic performance; a 2023 review found it to be a widespread failure mode affecting at least 294 academic publications across 17 disciplines. Model calibration refers to how well predicted probabilities match actual outcome rates, and methods like sigmoid (Platt) scaling are commonly used to correct miscalibrated classifiers.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Leakage_(machine_learning)">Leakage (machine learning) - Wikipedia</a></li>
<li><a href="https://scikit-learn.org/stable/modules/calibration.html">1.16. Probability calibration — scikit-learn 1.9.1 documentation</a></li>
<li><a href="https://www.sgim.org/resource/national-health-nutrition-examination-survey-nhanes/">National Health & Nutrition Examination Survey ( NHANES ) – SGIM</a></li>

</ul>
</details>

**Tags**: `#machine-learning`, `#healthcare`, `#data-leakage`, `#model-calibration`, `#NHANES`

---

<a id="item-10"></a>
## [OpenJev landing page sparks debate on Jev semantic decoding](https://openjev.com/) ⭐️ 6.0/10

OpenJev, a promotional site for a runtime-defined semantic decoding service, hit the front page of Hacker News with 530 points and 238 comments. Commenters criticized the site's cluttered design while sharing alternative Jev implementations, including a vLLM patch that turns DiffusionGemma into Jev and links to open-source models, papers, and datasets. The discussion highlights growing interest in structured output and semantic decoding as alternatives to full autoregressive generation, with community members questioning whether specialized models like Jev offer a real technical moat over existing structured-output paradigms. It also shows how open-source reproductions can quickly emerge around closed commercial services. A commenter noted that a vLLM patch to turn DiffusionGemma into Jev achieves similar latency and eval scores on a DGX Spark, while a Qwen36 model clearly lost to both. Others pointed to an open-sourced Jev architecture with model, paper, and dataset, and questioned how Jev differs from OpenAI's structured output, noting that the OpenJev project reproduces the interface pattern but not Jev's undisclosed model or training.

hackernews · ilreb · Sep 18, 09:42 · [Discussion](https://news.ycombinator.com/item?id=49752041)

**Background**: Jev is a closed service from TypeSafe that performs runtime-defined semantic decisions, meaning it picks among user-provided choices rather than generating free-form text. This differs from typical LLM structured output, where a model generates tokens constrained by a grammar or schema. The OpenJev project aims to reproduce Jev's interface pattern using open models, but not its proprietary model or training. vLLM is a popular open-source inference engine that supports structured outputs via backends like xgrammar and guidance.

<details><summary>References</summary>
<ul>
<li><a href="https://mohammedshehu.com/jev-typesafe-ai/">What Is Jev? How to Implement Typesafe AI’s Decision Model (Practical Guide)</a></li>
<li><a href="https://daily.dev/posts/jev-means-structured-output-is-interesting-again-zbs61p1nf">Jev means structured output is interesting again | daily.dev</a></li>
<li><a href="https://docs.vllm.ai/en/latest/features/structured_outputs/">Structured Outputs - vLLM</a></li>

</ul>
</details>

**Discussion**: Commenters widely criticized the OpenJev landing page as a cluttered, low-quality 'vibecoded' site, with some expressing general fatigue with LLM-generated websites. Others contributed substantive technical discussion, sharing a vLLM patch for a legitimate Jev implementation, linking to open-source models, papers, and datasets, and debating whether Jev is meaningfully different from existing structured output approaches. A key concern was that OpenJev reproduces only the interface, not the actual Jev model.

**Tags**: `#LLM`, `#structured-output`, `#semantic-decoding`, `#vLLM`, `#open-source`

---

<a id="item-11"></a>
## [Reddit proposal: augment driving datasets with synthetic edge cases](https://www.reddit.com/r/MachineLearning/comments/1wjnj4a/augmenting_large_datasets_to_have_more_edge_case/) ⭐️ 6.0/10

A Reddit user (u/danson729) proposed augmenting large labeled autonomous driving datasets by transforming clear daytime footage into rare conditions such as night, fog, rain, and glare, using physics-based effects where possible and constrained generative models for what physics cannot handle. The goal is to keep labels intact while matching the target camera quality (e.g., a cheap dashcam at night in the rain with heavy compression). Edge cases like night, fog, and rain are exactly where perception models fail most, yet they are rare in real driving data, so synthetic augmentation could improve robustness without the cost and risk of collecting rare real-world footage. This matters for autonomous driving practitioners and anyone doing domain adaptation, since it targets the sim-to-real and source-to-target gap directly. The proposal emphasizes keeping labels intact throughout the transformation, using physics-based effects for fog, rain, and low-light noise, and constrained generative models for dusk lighting, headlight glare, and wet roads, followed by matching the target camera's quality. The author frames it as adapting a large labeled dataset A to look like target domain B where the model will actually run, and is explicitly asking for feedback rather than presenting results.

reddit · r/MachineLearning · /u/danson729 · Sep 18, 11:24

**Background**: Domain adaptation in autonomous driving addresses the mismatch between the data a model is trained on (the source domain, often clear daytime footage) and the conditions it encounters in deployment (the target domain, such as adverse weather). Data augmentation is a common technique to close this gap, and prior work has explored physics-based simulation of adverse weather as well as constrained generative models for image synthesis. The idea here combines both approaches in a pipeline that transforms existing labeled data rather than collecting new data.

<details><summary>References</summary>
<ul>
<li><a href="https://www.labelvisor.com/domain-adaptation-for-autonomous-driving/">Domain adaptation for autonomous driving | Labelvisor</a></li>
<li><a href="https://arxiv.org/abs/2307.09676">[2307.09676] Domain Adaptation based Object Detection for...</a></li>
<li><a href="https://www.emergentmind.com/topics/kitti-weather-benchmark">KITTI-Weather Benchmark for Autonomous Driving</a></li>

</ul>
</details>

**Tags**: `#data augmentation`, `#domain adaptation`, `#autonomous driving`, `#edge cases`, `#generative models`

---

<a id="item-12"></a>
## [Reddit user seeks studies isolating back-and-forth LLM interaction from one-way sharing and self-refinement](https://www.reddit.com/r/MachineLearning/comments/1wjm0rx/what_studies_isolate_backandforth_llm_interaction/) ⭐️ 6.0/10

A Reddit user on r/MachineLearning has posted a detailed research question asking whether back-and-forth interaction between two different LLMs (GPT-4.1 and Claude Sonnet 4.6) improves task success beyond one-way sharing, independent aggregation, and self-refinement under a controlled resource budget. The user has designed a 576-pipeline experiment across twelve tasks and eight families but has not yet made any model calls, seeking existing literature before spending roughly $110 in API costs. This question targets a core methodological gap in multi-agent LLM research: many studies claim dialogue or debate helps, but few isolate the effect of genuine back-and-forth interaction from confounds like extra serial refinement or generic metacognitive prompting. A rigorous answer would help practitioners decide whether multi-agent dialogue is worth its cost, and the user's protocol design could serve as a template for controlled evaluation. The proposed interaction is a fixed four-step sequence (X drafts, Y responds, X revises, Y revises), with comparators including independent drafts plus budgeted aggregation, one-way sharing in both directions, self-refinement over multiple calls, generic reminders with a controller, and the same dialogue schedule with a single model to test heterogeneity. Budget accounting covers accumulated input context, generation, controllers, and final synthesis, and the user notes that equal token counts do not equal equal compute.

reddit · r/MachineLearning · /u/breadstickdingdong · Sep 18, 10:01

**Background**: Multi-agent LLM systems, where multiple language models collaborate or debate to solve a task, have become a popular research direction, but recent work such as controlled studies of multi-agent debate and comparisons of debate versus voting suggests that debate does not consistently outperform simpler single-agent or aggregation baselines. A key methodological challenge is that dialogue conditions often receive more total compute, more serial refinement steps, or different prompts than their baselines, making it hard to attribute any improvement to interaction itself. The user's proposed experiment aims to control for these confounds by equalizing resource budgets and including a single-model dialogue condition.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2511.07784v1">Can LLM Agents Really Debate? A Controlled Study of Multi-Agent Debate in Logical Reasoning</a></li>
<li><a href="https://arxiv.org/html/2508.17536v1">Debate or Vote: Which Yields Better Decisionsin Multi-Agent Large Language Models?</a></li>
<li><a href="https://arxiv.org/abs/2511.02755">[2511.02755] Controlling Performance and Budget of a ... Self-Resource Allocation in Multi-Agent LLM Systems Multi-LLM-Agents Debate - Performance, Efficiency, and ... MultiAgentBench : Evaluating the Collaboration and ... GitHub - Skytliang/Multi-Agents-Debate: MAD: The first work ... [PDF] Controlling Performance and Budget of a Centralized ...</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#multi-agent`, `#collaboration`, `#research-question`, `#evaluation`

---

<a id="item-13"></a>
## [uv 0.12.16 Adds Hash Verification for Downloaded Packages](https://github.com/astral-sh/uv/releases/tag/0.12.16) ⭐️ 5.0/10

astral-sh/uv released version 0.12.16 on 2026-09-17, adding verification of downloaded wheels and source distributions against hashes supplied by package indexes, plus hash support for build-constraint dependencies. The release also adds Pyodide 314.0.7, 0.29.5, and 0.27.8, and includes several preview features and bug fixes. Hash verification of downloaded artifacts strengthens supply-chain security by ensuring packages match what the index published, protecting users from tampered or corrupted downloads. This matters for teams using uv in CI/CD pipelines where reproducibility and integrity are critical. The hash verification applies to wheels and source distributions downloaded from package indexes, and build-constraint dependencies can now include hashes for verifying downloaded build dependencies. The release also fixes several panic scenarios, including malformed index URLs, proxy URLs without a host, and unsupported Git URL schemes in lockfiles.

github · astral-releases-bot[bot] · Sep 18, 01:01

**Background**: uv is an extremely fast Python package and project manager from Astral, written in Rust, that provides a unified interface for installing Python versions, managing dependencies, creating virtual environments, and running scripts. Wheels are the standard binary distribution format for Python packages, and source distributions (sdists) are the source-code equivalent. Package indexes such as PyPI publish hashes for these artifacts, which tools can use to verify integrity during installation.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.astral.sh/uv/">uv is an extremely fast Python package and project manager , written...</a></li>
<li><a href="https://packaging.python.org/en/latest/specifications/binary-distribution-format/">Binary distribution format - Python Packaging User Guide</a></li>
<li><a href="https://pyodide.org/en/stable/index.html">Pyodide — Version 314.0.6</a></li>

</ul>
</details>

**Tags**: `#python`, `#package-manager`, `#uv`, `#release-notes`, `#supply-chain-security`

---

<a id="item-14"></a>
## [Cloudflare Quick Tunnels Gets New Landing Page, Sparks Criticism](https://try.cloudflare.com/) ⭐️ 5.0/10

Cloudflare has launched a new landing page at try.cloudflare.com for its Quick Tunnels feature, which allows users to expose local development environments to the internet without an account. The page highlights instant, secure access with no DNS or certificate configuration, but the feature itself has existed for over five years. The new landing page has drawn attention to Cloudflare's maintenance of the tunnel product, with critics pointing to long-standing bugs and questioning whether a simple page update for an old feature deserves front-page attention. This highlights broader concerns about how major cloud providers prioritize and maintain developer tools. Quick Tunnels generate a random subdomain on each run and are intended for testing and development only, not production use. Community members noted that a macOS service installation bug has remained unfixed since 2021, and some criticized the new page's design for poor font color contrast.

hackernews · jcbhmr · Sep 18, 14:18 · [Discussion](https://news.ycombinator.com/item?id=49754785)

**Background**: Cloudflare Tunnel (formerly Argo Tunnel) is a secure tunneling service launched in 2018 that connects internal resources to Cloudflare's network without opening inbound ports. Quick Tunnels is a lightweight, anonymous version that requires no account or DNS configuration, making it a popular alternative to tools like ngrok for quickly sharing localhost. The service is built on Cloudflare's global network and is often used for real-time previews and development testing.

<details><summary>References</summary>
<ul>
<li><a href="https://try.cloudflare.com/">Cloudflare Quick Tunnels</a></li>
<li><a href="https://developers.cloudflare.com/cloudflare-one/networks/connectors/cloudflare-tunnel/">Cloudflare Tunnel · Cloudflare One docs</a></li>
<li><a href="https://gist.github.com/randyburden/cbda4da88bc4e6cd9e17d59ecf03dcf9">Cloudflare Quick Tunnels - ngrok alternative for exposing localhost...</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters were largely critical, noting that Quick Tunnels have existed for over five years and that a new landing page for an old product may not warrant front-page attention. Some pointed to unresolved bugs, such as a macOS service installation issue open since 2021, and questioned Cloudflare's commitment to the product. Others compared it to Tailscale's Tailcat and appreciated the no-account requirement.

**Tags**: `#Cloudflare`, `#tunnels`, `#networking`, `#Hacker News`, `#discussion`

---

<a id="item-15"></a>
## [Minimal Phone 2: A Refined Minimalist Android Phone Draws Skepticism](https://minimalcompany.com/) ⭐️ 5.0/10

The Minimal Company announced the Minimal Phone 2, a smaller and more refined version of its original minimalist Android phone, featuring a better QWERTY thumb keyboard, a premium aluminum body, and improved software. The announcement generated 162 upvotes and 155 comments on Hacker News, but much of the discussion was critical rather than enthusiastic. The Minimal Phone 2 tests whether there is a viable market for a deliberately limited Android device aimed at reducing doomscrolling, a niche that has grown crowded with e-ink phones, flip phones, and dumbed-down handsets. Its reception suggests that simply running full Android with a smaller form factor may not satisfy users who want a genuinely different, less distracting operating system. The company has not clearly disclosed which version of Android the phone runs, a gap that commenters flagged as a dealbreaker for purchase decisions. The device keeps full Android app compatibility, meaning users must rely on self-control rather than system-level restrictions to limit usage.

hackernews · nashashmi · Sep 18, 02:00 · [Discussion](https://news.ycombinator.com/item?id=49749369)

**Background**: The Minimal Phone is a minimalist Android phone with an E Ink display and a QWERTY thumb keyboard, made by The Minimal Company, a Southern California consumer electronics firm founded in 2023. The first model tested whether users would accept a slower, monochrome screen in exchange for fewer distractions. The second generation aims to refine that formula with a smaller body, better keyboard, and aluminum construction, but it still runs standard Android rather than a custom minimalist OS.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Minimal_Phone">Minimal Phone</a></li>
<li><a href="https://minimalcompany.com/pages/mp02">MINIMAL PHONE 2 - MP02 – Minimal Company</a></li>
<li><a href="https://www.digitaltrends.com/phones/minimal-phone-2-looks-like-a-deliberate-antidote-to-doomscrolling/">Minimal Phone 2 looks like a deliberate antidote to ...</a></li>

</ul>
</details>

**Discussion**: Commenters were largely critical, with one lamenting that every new minimalist phone is just marketing wrapped around a kneecapped Android device and wishing for a BlackBerry-like alternative with a different OS. Others complained about missing Android version details, criticized 2.5D screen edges as reducing usable width, and argued that full Android compatibility means the phone still requires self-control rather than solving distraction.

**Tags**: `#minimalist phone`, `#Android`, `#hardware`, `#product launch`, `#digital wellbeing`

---

<a id="item-16"></a>
## [Simon Willison Compares Ignoring LLMs to Ignoring Jurassic Park](https://simonwillison.net/2026/Sep/18/probably-gonna-eat-you/) ⭐️ 5.0/10

Simon Willison published a short note on September 18, 2026, arguing that a computer scientist who refuses to find anything interesting about LLMs right now is like a geneticist who refuses to find anything interesting about a newly opened Jurassic Park. The quip captures the current AI moment: LLMs and generative AI have become so consequential that dismissing them as uninteresting is increasingly seen as a professional blind spot, and Willison's framing may resonate with researchers and engineers deciding how much attention to give the field. The post is a single-sentence opinion snippet tagged llms, ai, and generative-ai, not a technical deep-dive or announcement; its value lies in the framing rather than in new data or benchmarks.

rss · Simon Willison · Sep 18, 19:21

**Background**: Large language models (LLMs) are AI models, typically neural networks trained on vast amounts of text, that handle natural language tasks such as generation, translation, and question answering. Generative AI is the broader subfield that uses such models to produce text, images, audio, code, and other data, and it has expanded rapidly since the AI boom of the 2020s. Simon Willison is a well-known software developer and commentator who frequently writes about LLMs and their practical implications.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Generative_AI">Generative AI</a></li>

</ul>
</details>

**Tags**: `#llms`, `#ai`, `#generative-ai`, `#commentary`, `#industry-trends`

---

<a id="item-17"></a>
## [AWS Principal Applied Scientist James Gung Hosts Reddit AMA](https://www.reddit.com/r/MachineLearning/comments/1wjuki0/im_a_principal_applied_scientist_at_aws_who/) ⭐️ 5.0/10

James Gung, a Principal Applied Scientist at AWS who joined Amazon in 2021, hosted a Reddit AMA on r/MachineLearning to discuss his career path and work on AI services including Amazon Bedrock, Lex, Q Business, and Amazon Quick. He answered questions about internships, interviews, and daily life as an applied scientist during a one-hour session starting at 11:00 AM ET. This AMA offers a rare insider perspective on what it's like to work as an applied scientist at AWS, one of the largest cloud and AI providers, which can help students and engineers understand career paths in applied AI. It also sheds light on the teams behind widely used services like Bedrock and Lex that many developers rely on to build generative AI and conversational applications. Gung's research spans task-oriented dialogue, agent evaluation, conversation simulation, and proactive agents, and he previously worked on conversational AI at Amelia after earning a PhD in Computer Science from the University of Colorado Boulder. He noted he cannot discuss unannounced products, financials, competitors, internal tools, legal matters, pricing, or customer data, and he was speaking from personal experience rather than as an official Amazon spokesperson.

reddit · r/MachineLearning · /u/Amazon_Careers · Sep 18, 16:13

**Background**: Amazon Bedrock is a fully managed AWS service launched in 2023 that provides a unified API to access foundation models from multiple AI companies for building generative AI applications. Amazon Lex is an AWS service for building conversational interfaces using voice and text, and it powers the Amazon Alexa virtual assistant. An AMA (Ask Me Anything) is a public Q&A format popular on Reddit where users ask a host questions on a chosen topic.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Amazon_Bedrock">Amazon Bedrock</a></li>
<li><a href="https://en.wikipedia.org/wiki/Amazon_Lex">Amazon Lex</a></li>
<li><a href="https://aws.amazon.com/bedrock/">Amazon Bedrock – Build genAI applications and agents at ...</a></li>

</ul>
</details>

**Tags**: `#AWS`, `#Applied Scientist`, `#Career Advice`, `#AI Services`, `#Amazon Bedrock`

---

<a id="item-18"></a>
## [Reddit user asks how mid-tier AI journals compare to top conferences like NeurIPS](https://www.reddit.com/r/MachineLearning/comments/1wjnruv/how_competitive_are_journals_compared_to_top_ai/) ⭐️ 5.0/10

A Reddit user on r/MachineLearning, posting as /u/ATHii-127, described receiving NeurIPS scores of 2/3/3 (3/4/4) and asked how the review standards and acceptance difficulty of mid-tier AI journals such as Pattern Recognition, Neurocomputing, Knowledge-Based Systems, Neural Networks, and Expert Systems with Applications compare to top conferences like NeurIPS, CVPR, and ICLR. The paper in question concerns attention mechanisms for Vision Transformers, with a modification to the attention module as its main contribution. This question reflects a widespread dilemma in the machine learning community: with top conferences like NeurIPS, CVPR, and ICLR receiving record submission volumes and low acceptance rates, many researchers are turning to journals as an alternative venue, and understanding the relative difficulty of these venues affects where work gets published and how careers progress. The discussion is relevant to graduate students and researchers deciding whether to resubmit to another conference or pivot to a journal. The user explicitly rules out top-tier journals such as TPAMI, IJCV, and TMLR, and is instead targeting journals perceived as a step below, including Pattern Recognition, Neurocomputing, Knowledge-Based Systems, Neural Networks, and Expert Systems with Applications. The NeurIPS scores cited (2/3/3 with confidence 3/4/4) suggest a borderline-to-negative outcome, and the user expects rejection before official results are released.

reddit · r/MachineLearning · /u/ATHii-127 · Sep 18, 11:36

**Background**: NeurIPS (Conference on Neural Information Processing Systems), CVPR (Conference on Computer Vision and Pattern Recognition), and ICLR (International Conference on Learning Representations) are among the highest-impact venues in AI and machine learning research, and ICLR is often described alongside NeurIPS and ICML as one of the three primary conferences in the field. These conferences use peer-review scoring systems, and papers that fall below the acceptance threshold are commonly redirected by authors to journals. Journals such as Pattern Recognition, Neurocomputing, and Expert Systems with Applications are Elsevier-published venues with broader scope and generally different review timelines and acceptance criteria than top conferences.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/International_Conference_on_Learning_Representations">International Conference on Learning Representations</a></li>
<li><a href="https://en.wikipedia.org/wiki/Conference_on_Computer_Vision_and_Pattern_Recognition">Conference on Computer Vision and Pattern Recognition - Wikipedia</a></li>
<li><a href="https://neurips.cc/">2026 Conference</a></li>

</ul>
</details>

**Tags**: `#academic publishing`, `#peer review`, `#AI conferences`, `#journals`, `#machine learning`

---

<a id="item-19"></a>
## [Simon Willison Highlights Pelican Bicycle Scene in Who Framed Roger Rabbit](https://simonwillison.net/2026/Sep/18/the-creative-spirit-of-who-framed-roger-rabbit/) ⭐️ 3.0/10

Simon Willison shared a clip from the 1988 film Who Framed Roger Rabbit showing a pelican riding a bicycle, crediting Cypress Frankenfeld for pointing out the sequence. He noted that the pelican is animated while the bicycle is a real prop, with water-filled wheels for stability and cable-guided movement. The post is a lighthearted appreciation of practical filmmaking craft rather than a technical news item, offering a small window into how live-action and animation were blended before digital tools. It resonates with readers interested in the history of visual effects and the ingenuity of physical production techniques. The bicycle in the scene was a real bicycle whose wheels were reportedly filled with water to keep it stable, and it was set running and guided by a cable while the animated pelican was composited over it. The film is directed by Robert Zemeckis, with animation directed by Richard Williams.

rss · Simon Willison · Sep 18, 14:36

**Background**: Who Framed Roger Rabbit is a 1988 American fantasy comedy directed by Robert Zemeckis that combines live-action and animation, loosely based on Gary K. Wolf's novel Who Censored Roger Rabbit?. It is widely praised for integrating animated characters with live-action performances in a way that was integral to the storytelling, rather than appearing tacked on. The film's animation was led by Richard Williams and produced with involvement from Steven Spielberg.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Who_Framed_Roger_Rabbit">Who Framed Roger Rabbit - Wikipedia</a></li>
<li><a href="https://www.ebsco.com/research-starters/film/who-framed-roger-rabbit-merges-animation-live-action">Who Framed Roger Rabbit Merges Animation with Live Action | Film | Research Starters | EBSCO Research</a></li>
<li><a href="https://www.syfy.com/syfy-wire/why-roger-rabbit-an-animated-and-legal-marvel-would-be-impossible-today">Who Framed Roger Rabbit's animation director Richard Williams did the impossible</a></li>

</ul>
</details>

**Tags**: `#film`, `#animation`, `#pop-culture`, `#trivia`, `#blog`

---

<a id="item-20"></a>
## [AAAI-27 Phase 1 Results Thread on Reddit](https://www.reddit.com/r/MachineLearning/comments/1wjhiyu/aaai27_phase_1_results_d/) ⭐️ 3.0/10

A Reddit user posted a thread on r/MachineLearning inviting others to share updates on AAAI-27 Phase 1 results, which are expected on September 24. The thread is intended as a place for researchers to post when they start receiving notifications. AAAI is one of the top-tier AI conferences, so its acceptance decisions directly affect the publication plans, careers, and travel schedules of many machine learning researchers. A shared thread helps authors gauge when notifications are going out and compare outcomes across the community. AAAI-27 uses a two-phase reviewing process for its Main Track: Phase 1 consists of two reviews supplemented by one AI-generated, non-decisional review, and the conference itself will be held February 16-23, 2027 in Montréal, Canada. The Reddit post contains no technical content beyond the expected notification date.

reddit · r/MachineLearning · /u/BeneficialFish04 · Sep 18, 05:36

**Background**: The AAAI Conference on Artificial Intelligence is an annual international academic conference organized by the Association for the Advancement of Artificial Intelligence, first held in 1980 at Stanford University. It is widely regarded as one of the leading AI conferences, ranking alongside venues such as NeurIPS, ICML, and ICLR. Like those conferences, AAAI uses AI-assisted algorithms to help assign submitted papers to reviewers, and its submission deadlines typically fall in late August or early September, with the conference held the following February.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AAAI_Conference_on_Artificial_Intelligence">AAAI Conference on Artificial Intelligence</a></li>
<li><a href="https://aaai.org/conference/aaai/aaai-27/">AAAI - 27 - AAAI</a></li>
<li><a href="http://wikicfp.com/cfp/program?id=3">AAAI : National Conference on Artificial Intelligence 2027 2026 2025 ..</a></li>

</ul>
</details>

**Discussion**: The thread is a low-activity community post with no substantive comments summarized, serving mainly as a placeholder for researchers to report when AAAI-27 Phase 1 notifications arrive.

**Tags**: `#AAAI`, `#conference`, `#academic`, `#machine learning`, `#community`

---