---
layout: default
title: "Horizon Summary: 2026-07-02 (EN)"
date: 2026-07-02
lang: en
---

> From 21 items, 17 important content pieces were selected

---

1. [Virginia Bans Sale of Geolocation Data](#item-1) ⭐️ 8.0/10
2. [Linux 6.9 LUKS suspend fails to wipe encryption keys](#item-2) ⭐️ 8.0/10
3. [Podman v6.0.0 Released with Enhanced Networking](#item-3) ⭐️ 8.0/10
4. [Immich 3.0 Released: Major Update for Self-Hosted Photos](#item-4) ⭐️ 8.0/10
5. [PeerTube: Decentralized Video Platform Gains Traction](#item-5) ⭐️ 7.0/10
6. [How to Ask Strangers for Help Effectively](#item-6) ⭐️ 7.0/10
7. [Simon Willison Releases llm-coding-agent Alpha](#item-7) ⭐️ 7.0/10
8. [Simon Willison uses DSPy to optimize Datasette Agent SQL prompts](#item-8) ⭐️ 7.0/10
9. [Understand to Participate: Key to AI Coding Collaboration](#item-9) ⭐️ 7.0/10
10. [Improving machine-translated novels via style transfer](#item-10) ⭐️ 7.0/10
11. [SentryCode: Open-Source Kernel-Level Auditor for AI Coding Agents](#item-11) ⭐️ 7.0/10
12. [Gnosys Improves Safety Classifiers Under Label Scarcity](#item-12) ⭐️ 7.0/10
13. [Exapunks: A Retrospective on Zachtronics' Programming Puzzle Game](#item-13) ⭐️ 6.0/10
14. [Paper Fishing: Unethical Authorship in Academia](#item-14) ⭐️ 6.0/10
15. [ML PhD Seeks Math Foundation Book Recommendations](#item-15) ⭐️ 6.0/10
16. [How ML conference paper selections work](#item-16) ⭐️ 6.0/10
17. [Beginner Asks About Replacing Transformer with Mamba in Fast BLT](#item-17) ⭐️ 4.0/10

---

<a id="item-1"></a>
## [Virginia Bans Sale of Geolocation Data](https://www.hunton.com/privacy-and-cybersecurity-law-blog/virginia-bans-sale-of-geolocation-data) ⭐️ 8.0/10

Virginia Governor Abigail Spanberger signed S.B. 338 into law on April 13, 2026, amending the Virginia Consumer Data Protection Act (VCDPA) to prohibit the sale of consumers' precise geolocation data, effective July 1, 2026. This ban makes Virginia the third state to prohibit the sale of geolocation data, reflecting a growing trend in state-level privacy regulation. It addresses public concerns about data misuse, such as tracking visits to Planned Parenthood or insurance companies monitoring driving behavior. The ban applies to 'controllers' under the VCDPA and defines 'sale' broadly as the exchange of personal data for monetary or other valuable consideration. Enforcement challenges include jurisdictional issues for out-of-state companies and the practical difficulty of policing data resale.

hackernews · toomuchtodo · Jul 2, 21:03 · [Discussion](https://news.ycombinator.com/item?id=48767347)

**Background**: Geolocation data reveals a person's precise location and can be used for targeted advertising, surveillance, or discrimination. The VCDPA, enacted in 2021, was Virginia's first comprehensive privacy law, and this amendment adds specific protections for sensitive location data. Other states like California and Maryland have similar laws.

<details><summary>References</summary>
<ul>
<li><a href="https://epic.org/virginia-governor-signs-bill-banning-sale-of-precise-location-data/">Virginia Governor Signs Bill Banning Sale of Precise Location Data</a></li>
<li><a href="https://www.hunton.com/privacy-and-cybersecurity-law-blog/virginia-bans-sale-of-geolocation-data">Virginia Bans Sale of Geolocation Data</a></li>
<li><a href="https://www.regulatoryoversight.com/2026/04/virginia-becomes-third-state-to-ban-sale-of-consumers-precise-geolocation-data/">Virginia Becomes Third State to Ban Sale of Consumers' Precise Geolocation Data | Regulatory Oversight</a></li>

</ul>
</details>

**Discussion**: Commenters generally support the ban but raise enforcement concerns, such as how to handle out-of-state companies selling data collected in Virginia. They also highlight real-world abuses, like anti-abortion ads using location data from Planned Parenthood visits, underscoring the need for strong enforcement.

**Tags**: `#privacy`, `#geolocation`, `#regulation`, `#data protection`

---

<a id="item-2"></a>
## [Linux 6.9 LUKS suspend fails to wipe encryption keys](https://mathstodon.xyz/@iblech/116769502749142438) ⭐️ 8.0/10

Since Linux kernel 6.9, the LUKS suspend operation (cryptsetup luksSuspend) no longer wipes disk-encryption keys from memory, a regression that could expose master keys during suspend-to-RAM. This regression undermines a key security feature of LUKS, potentially allowing attackers with physical access to extract encryption keys from RAM during sleep. It affects all Linux users relying on LUKS disk encryption, though the practical risk depends on threat models. The bug was introduced in Linux 6.9 and affects the luksSuspend command, which is designed to suspend a LUKS device and wipe its encryption key from kernel memory. The regression means the key remains in memory during suspend-to-RAM, contrary to the documented behavior.

hackernews · IngoBlechschmid · Jul 2, 15:25 · [Discussion](https://news.ycombinator.com/item?id=48763035)

**Background**: LUKS (Linux Unified Key Setup) is a disk encryption specification that protects data at rest. The luksSuspend operation is used to temporarily suspend an encrypted device (e.g., before hibernation) by blocking I/O and wiping the master key from memory. Suspend-to-RAM (sleep) keeps RAM powered, so any data in memory, including encryption keys, remains accessible if an attacker gains physical access.

<details><summary>References</summary>
<ul>
<li><a href="https://www.man7.org/linux//man-pages/man8/cryptsetup-luksSuspend.8.html">cryptsetup-luksSuspend (8) - Linux manual page - man7.org</a></li>
<li><a href="https://man.archlinux.org/man/core/cryptsetup/cryptsetup-luksSuspend.8.en">cryptsetup-luksSuspend (8) — Arch manual pages</a></li>
<li><a href="https://www.mankier.com/8/cryptsetup-luksSuspend">cryptsetup-luksSuspend: suspends an active device and wipes ...</a></li>

</ul>
</details>

**Discussion**: Community comments show mixed views: some argue the bug is overblown since luksSuspend is not officially supported by the kernel, while others note that security regressions like this are easy to miss because everything still works. Some users point out that during normal sleep, the encryption key is already in memory, so the bug may not change the practical risk for many.

**Tags**: `#Linux`, `#security`, `#LUKS`, `#kernel`, `#encryption`

---

<a id="item-3"></a>
## [Podman v6.0.0 Released with Enhanced Networking](https://blog.podman.io/2026/07/introducing-podman-v6-0-0/) ⭐️ 8.0/10

Podman v6.0.0 has been released, introducing major improvements including new networking features that enhance performance and usability. As a leading Docker alternative, this release strengthens Podman's position in the container ecosystem, offering users a daemonless, rootless, and more secure container management experience. The new networking features are particularly praised by the community, and the release continues to support rootless containers and Quadlet for systemd integration.

hackernews · soheilpro · Jul 2, 14:23 · [Discussion](https://news.ycombinator.com/item?id=48762098)

**Background**: Podman is a daemonless container engine that allows users to run containers without a central daemon, improving security and simplicity. It is often compared to Docker and is popular for its rootless capabilities and compatibility with Docker commands and compose files.

<details><summary>References</summary>
<ul>
<li><a href="https://www.redhat.com/en/topics/containers/what-is-podman">What is Podman?</a></li>
<li><a href="https://sanj.dev/post/docker-vs-podman-comparison/">Docker vs Podman: Rootless Networking, Benchmarks & Runtime ...</a></li>
<li><a href="https://dev.to/mechcloud_academy/docker-vs-podman-an-in-depth-comparison-2025-2eia">Docker vs Podman: An In-Depth Comparison (2026)</a></li>

</ul>
</details>

**Discussion**: Community comments are overwhelmingly positive, with users praising ease of migration from Docker, the daemonless architecture, and Quadlet. Some discussion noted macOS support and UI issues, but overall sentiment is highly favorable.

**Tags**: `#Podman`, `#containers`, `#Docker alternative`, `#devops`, `#open source`

---

<a id="item-4"></a>
## [Immich 3.0 Released: Major Update for Self-Hosted Photos](https://github.com/immich-app/immich/discussions/29439) ⭐️ 8.0/10

Immich 3.0, a major version of the self-hosted photo and video management solution, has been released with improvements and strong community support. This release solidifies Immich as a leading open-source alternative to Google Photos and Apple Photos, offering users full control over their data and privacy. The update includes performance enhancements and feature refinements, though specific changelog details are not provided in the announcement. The community discussion highlights ongoing concerns about iOS photo sync reliability.

hackernews · hashier · Jul 2, 14:13 · [Discussion](https://news.ycombinator.com/item?id=48761944)

**Background**: Immich is a high-performance, self-hosted photo and video management solution that can be deployed via Docker. It provides mobile apps for iOS and Android with automatic backup, face recognition, album sharing, and map view, making it a popular privacy-focused alternative to cloud services.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/immich-app/immich">GitHub - immich -app/ immich : High performance self - hosted photo ...</a></li>
<li><a href="https://xtom.com/blog/self-hosted-photo-management-apps-ditch-google-icloud-photos/">The 15 Best Self - Hosted Photo Management Apps... | xTom</a></li>
<li><a href="https://selfhostedguides.com/immich-photo-management/">Immich : Self - Hosted Google Photos Alternative — Selfhosted Guides</a></li>

</ul>
</details>

**Discussion**: Users express strong satisfaction with Immich, calling it a 'no-brainer replacement' for Apple Photos or Google Photos when combined with a VPN like Tailscale. However, one user reports persistent issues with iOS photo sync, where the app filled device storage and failed to complete uploads even after days of foreground operation.

**Tags**: `#self-hosting`, `#photo management`, `#open source`, `#privacy`

---

<a id="item-5"></a>
## [PeerTube: Decentralized Video Platform Gains Traction](https://github.com/Chocobozzz/PeerTube) ⭐️ 7.0/10

PeerTube, a free and open-source decentralized video platform using ActivityPub federation and peer-to-peer technology, has grown to over 600,000 hosted videos and 150,000 users, offering an alternative to centralized platforms like YouTube. This matters because PeerTube challenges the dominance of centralized video platforms by distributing hosting and playout load across instances, enhancing privacy and reducing reliance on big tech, though it still faces hurdles in monetization and content discovery. PeerTube uses peer-to-peer technology in the browser to distribute playout load among viewers, but it does not handle discovery or monetization natively; each instance is independently operated, and federation via ActivityPub allows cross-instance video sharing.

hackernews · doener · Jul 2, 11:17 · [Discussion](https://news.ycombinator.com/item?id=48759634)

**Background**: PeerTube is a free software project launched by Framasoft in 2018. It uses the ActivityPub protocol to federate independent video hosting servers (instances), allowing users on different instances to follow and interact with each other's content. Unlike YouTube, no single entity controls the network, and each instance admin sets their own moderation and storage policies.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/PeerTube">PeerTube - Wikipedia</a></li>
<li><a href="https://github.com/Chocobozzz/PeerTube">GitHub - Chocobozzz/PeerTube: ActivityPub-federated video streaming platform using P2P directly in your web browser · GitHub</a></li>
<li><a href="https://joinpeertube.org/">What is PeerTube? | JoinPeerTube</a></li>

</ul>
</details>

**Discussion**: Community comments highlight practical concerns: professional YouTubers note the lack of monetization makes it unsustainable for high-quality content creation, while others point out that PeerTube only handles hosting and playout, not discovery or ads. Some users appreciate it for open-source tutorials but acknowledge the audience is still small.

**Tags**: `#decentralization`, `#video hosting`, `#federation`, `#open source`, `#PeerTube`

---

<a id="item-6"></a>
## [How to Ask Strangers for Help Effectively](https://pradyuprasad.com/writings/how-to-ask-for-help/) ⭐️ 7.0/10

A detailed guide on asking for help from strangers, emphasizing proof of work, brevity, and understanding the recipient's perspective, has been published and gained significant community traction. This advice is crucial for professionals and job seekers who often need to network with strangers; mastering these techniques can significantly increase response rates and build valuable connections. Key points include showing proof of work upfront, keeping requests brief, and tailoring the ask to the recipient's context. The guide also warns against common mistakes like overly long messages or lack of personalization.

hackernews · FigurativeVoid · Jul 2, 13:19 · [Discussion](https://news.ycombinator.com/item?id=48761118)

**Background**: Asking strangers for help is a common but challenging task in professional networking. Many people struggle because they fail to respect the recipient's time or demonstrate their own effort. This guide provides actionable strategies to overcome these hurdles.

**Discussion**: Commenters largely agreed with the advice, adding that proof of work must be genuine and deep, not superficial. Some emphasized that personal estimation of how often people are asked for help is often inaccurate, so understanding the recipient's baseline is key.

**Tags**: `#communication`, `#career`, `#networking`, `#soft-skills`

---

<a id="item-7"></a>
## [Simon Willison Releases llm-coding-agent Alpha](https://simonwillison.net/2026/Jul/2/llm-coding-agent/#atom-everything) ⭐️ 7.0/10

Simon Willison released llm-coding-agent 0.1a0, an alpha coding agent built on his LLM library, inspired by Claude Code, with tools for reading, editing files, and executing commands. This release demonstrates a practical application of LLMs for software development, potentially streamlining developer workflows by automating file editing and command execution directly from the terminal. The agent includes tools like edit_file, execute_command, list_files, read_file, and search_files, and can be run via 'uvx --prerelease=allow --with llm-coding-agent llm code'.

rss · Simon Willison · Jul 2, 19:33

**Background**: Simon Willison's LLM library is a CLI tool and Python library that provides an abstraction layer over hundreds of LLMs. Claude Code is an agentic coding tool by Anthropic that reads codebases, edits files, and runs commands. This project uses Willison's python-lib-template-repository to scaffold the library.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/simonw/llm">GitHub - simonw/llm: Access large language models from the command-line · GitHub</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent , Terminal, IDE</a></li>
<li><a href="https://github.com/simonw/python-lib-template-repository">GitHub - simonw/ python - lib - template - repository : GitHub template...</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#coding agent`, `#Python`, `#AI tools`, `#open source`

---

<a id="item-8"></a>
## [Simon Willison uses DSPy to optimize Datasette Agent SQL prompts](https://simonwillison.net/2026/Jul/2/dspy-datasette-agent-prompts/#atom-everything) ⭐️ 7.0/10

Simon Willison used DSPy to evaluate and improve the SQL system prompts for Datasette Agent, an AI assistant for Datasette. He delegated the task to Claude Code on the web, which tested prompts with GPT-4.1 mini and nano and identified several promising improvements. This demonstrates a practical, automated approach to prompt optimization that can improve the reliability and accuracy of LLM-powered SQL agents. It shows how developers can systematically refine system prompts without manual trial and error, potentially reducing errors like column-name guessing and retry loops. The optimization revealed that the original prompt's schema listing only gave table names, and the advice not to call describe_table if already known caused column-name guessing and error-retry loops. Suggested fixes include including column names in the schema listing or softening that advice.

rss · Simon Willison · Jul 2, 18:25

**Background**: DSPy is a framework for automatically optimizing prompts and LLM pipelines using a metric and a dataset, eliminating manual prompt tuning. Datasette Agent is an open-source plugin for Datasette that provides an AI assistant for exploring and querying SQLite databases. Claude Code on the web allows users to delegate coding tasks to Claude that run on Anthropic-managed cloud infrastructure without active supervision.

<details><summary>References</summary>
<ul>
<li><a href="https://agent.datasette.io/">Datasette Agent: an AI assistant for Datasette to help explore and analyze data in SQLite</a></li>
<li><a href="https://code.claude.com/docs/en/web-quickstart">Get started with Claude Code on the web - Claude Code Docs</a></li>

</ul>
</details>

**Tags**: `#DSPy`, `#prompt engineering`, `#AI agents`, `#SQL`, `#Datasette`

---

<a id="item-9"></a>
## [Understand to Participate: Key to AI Coding Collaboration](https://simonwillison.net/2026/Jul/2/understand-to-participate/#atom-everything) ⭐️ 7.0/10

Simon Willison highlights Geoffrey Litt's concept of 'understand to participate' as essential for collaborating with AI coding agents without accumulating cognitive debt. This concept addresses the growing challenge of cognitive debt in AI-assisted software development, where developers risk losing understanding of code generated by agents, impacting productivity and code quality. Geoffrey Litt presented this idea at the AIE conference, arguing that developers must understand code deeply enough to actively participate in the creative process with AI agents.

rss · Simon Willison · Jul 2, 17:07

**Background**: Cognitive debt refers to the erosion of shared understanding of a software system over time, leading to inadequate mental models for safe changes. As AI coding agents generate large code changes, developers may lose track of how the system works, accumulating cognitive debt.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/cognitive-debt-software-engineering-oren-chapo-6qw7f/">Cognitive Debt in Software Engineering - LinkedIn</a></li>
<li><a href="https://arxiv.org/abs/2603.22106">From Technical Debt to Cognitive and Intent Debt: Rethinking ... From Technical Debt to Cognitive and Intent Debt: - arXiv.org How Generative and Agentic AI Shift Concern from Technical ... Cognitive debt: The hidden risk in AI-driven software development Understanding Cognitive Debt in Engineering Teams From Technical Debt to Cognitive and Intent Debt - ACM Queue</a></li>
<li><a href="https://devops.com/coding-agent-teams-the-next-frontier-in-ai-assisted-software-development/">Coding Agent Teams: The Next Frontier in AI-Assisted Software Development - DevOps.com</a></li>

</ul>
</details>

**Tags**: `#AI-assisted coding`, `#cognitive debt`, `#software engineering`, `#developer productivity`

---

<a id="item-10"></a>
## [Improving machine-translated novels via style transfer](https://www.reddit.com/r/MachineLearning/comments/1ulrdw9/improving_machinetranslated_novels_via_style/) ⭐️ 7.0/10

A Reddit user proposes using unsupervised style transfer to polish machine-translated webnovels, referencing STRAP and other methods, and seeks advice on balancing faithfulness and fluency. This project addresses a practical need for improving the readability of machine-translated fiction, which is often plagued by awkward phrasing. Success could benefit the large community of webnovel readers and translators. The approach is unsupervised due to lack of parallel data, focusing on sentence-level style transfer with potential paragraph-level context needed for coherence. Domain-specific terms like 'terminology' must be preserved.

reddit · r/MachineLearning · /u/Divine_Invictus · Jul 2, 19:04

**Background**: Style transfer in NLP aims to rewrite text in a different style while preserving content. Unsupervised methods like STRAP generate pseudo-parallel data to fine-tune language models. Machine-translated novels often suffer from 'translationese'—unnatural phrasing that retains source language structure.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/martiansideofthemoon/style-transfer-paraphrase">GitHub - martiansideofthemoon/style-transfer-paraphrase ...</a></li>
<li><a href="https://ar5iv.labs.arxiv.org/html/2010.05700">[2010.05700] Reformulating Unsupervised Style Transfer as ...</a></li>
<li><a href="https://aclanthology.org/2020.emnlp-main.55.pdf">Reformulating Unsupervised Style Transfer as Paraphrase ...</a></li>

</ul>
</details>

**Tags**: `#style transfer`, `#machine translation`, `#NLP`, `#unsupervised learning`

---

<a id="item-11"></a>
## [SentryCode: Open-Source Kernel-Level Auditor for AI Coding Agents](https://www.reddit.com/r/MachineLearning/comments/1ul7ap2/sentrycode_realtime_auditor_honeytokens_for_ai/) ⭐️ 7.0/10

SentryCode, an open-source kernel-level auditing tool, has been released to monitor AI coding agents for privacy violations using honeytokens and covert channel detection. As AI coding agents become more prevalent, concerns about telemetry and data exfiltration grow; SentryCode provides a novel, zero-false-positive approach to detect data breaches and covert channels, enhancing trust in local AI tools. SentryCode logs file, network, and cue activity, uses honeypot tokens for zero-false-positive data breach detection, detects steganographically encrypted covert channels, provides tamper-proof audit logs, and supports policy enforcement—all running locally without outbound connections.

reddit · r/MachineLearning · /u/cyh-c · Jul 2, 03:48

**Background**: Honeytokens are decoy data placed in systems to detect unauthorized access; covert channels are hidden communication paths that can exfiltrate data. Kernel-level auditing tools monitor system calls at the OS kernel level, providing deep visibility into process behavior. SentryCode combines these techniques to specifically address privacy risks from AI coding agents that may perform telemetry or environmental scanning.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Honeytoken">Honeytoken</a></li>
<li><a href="https://github.com/rencete/covert-channel-detector">GitHub - rencete/covert-channel-detector: Detection of covert ... [2604.14987] AI-Enabled Covert Channel Detection in RF ... A Survey of Network Covert Channel: Construction and Detection AI-Enabled Covert Channel Detection in RF Receiver Architectures An Improved Approach to DNS Covert Channel Detection ... - MDPI A Case Study on the Detection of Hash-Chain-based Covert ...</a></li>
<li><a href="https://chanakar.substack.com/p/linux-security-superpower-auditd-guide">Mastering auditd: The Essential Guide to Linux Kernel-Level ...</a></li>

</ul>
</details>

**Tags**: `#AI Security`, `#Open Source`, `#Privacy`, `#Auditing`, `#Honeytokens`

---

<a id="item-12"></a>
## [Gnosys Improves Safety Classifiers Under Label Scarcity](https://www.reddit.com/r/MachineLearning/comments/1ul3ohk/making_optimization_work_when_labels_are_scarce_r/) ⭐️ 7.0/10

Gnosys Labs introduced an autonomous model engineer that improves safety classifiers when ground truth labels are scarce, outperforming both the starting classifier and the GEPA prompt optimizer on the ToxicChat benchmark across two runs. This approach addresses a critical bottleneck in deploying AI classifiers for content moderation, fraud detection, and risk scoring, where obtaining human-verified labels is expensive and slow, enabling more reliable optimization with limited supervision. Gnosys fuses a small verified label set with a large unlabeled pool to create a calibrated quality estimate, then optimizes against that estimate rather than raw labels; in the headline run with 3,000 labels, it achieved 0.777 harm caught vs. 0.731 for the starting classifier and 0.702 for GEPA.

reddit · r/MachineLearning · /u/Kody--- · Jul 2, 00:59

**Background**: Label scarcity is a common challenge in machine learning, especially for tasks requiring expensive human judgments like toxicity detection. Traditional prompt optimizers like GEPA improve whatever evaluation signal they are given, but with very few labels, they risk fitting noise. Gnosys acts as an autonomous model engineer that judges signal trustworthiness and engineers a better objective before optimizing.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2310.17389">[2310.17389] ToxicChat: Unveiling Hidden Challenges of ... ToxicChat: A Benchmark for Content Moderation in Real-world ... ToxicChat: Unveiling Hidden Challenges of Toxicity Detection ... [2310.17389] ToxicChat: Unveiling Hidden Challenges of ... TOXIC C : Unveiling Hidden Challenges of Toxicity Detection ... lmsys/toxic-chat · Datasets at Hugging Face ToxicChat Dataset - Papersgraph</a></li>
<li><a href="https://github.com/gepa-ai/gepa">GitHub - gepa-ai/gepa: Optimize prompts, code, and more with ...</a></li>
<li><a href="https://pypi.org/project/gnosyslabs/">Python client for the Gnosys Labs autonomous experimentation...</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#label scarcity`, `#prompt optimization`, `#safety classifier`, `#active learning`

---

<a id="item-13"></a>
## [Exapunks: A Retrospective on Zachtronics' Programming Puzzle Game](https://www.zachtronics.com/exapunks/) ⭐️ 6.0/10

A Hacker News post discusses the 2018 programming puzzle game Exapunks by Zachtronics, with community comments highlighting the developer's new game UVS_Nirmana by Coincidence Games and sharing gameplay strategies. Exapunks remains a beloved title in the programming game genre, and the discussion provides context on Zachtronics' legacy and Zach Barth's continued work under Coincidence Games, offering insights into the evolution of programming puzzle games. Exapunks was released in early access on August 9, 2018, and fully launched on October 22, 2018. It features a custom puzzle creation tool called Axiom VirtualNetwork+, written in JavaScript.

hackernews · yu3zhou4 · Jul 2, 18:41 · [Discussion](https://news.ycombinator.com/item?id=48765663)

**Background**: Exapunks is a programming puzzle game set in an alternate 1997, where players control software agents called EXAs to hack networks. Zachtronics is known for engineering puzzle games like TIS-100 and SHENZHEN I/O, which teach assembly-like programming concepts. The developer, Zach Barth, later founded Coincidence Games, which released the spacecraft engineering puzzle game UVS_Nirmana.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Exapunks">Exapunks - Wikipedia</a></li>
<li><a href="https://www.zachtronics.com/exapunks/">EXAPUNKS - Zachtronics</a></li>
<li><a href="https://store.steampowered.com/app/716490/EXAPUNKS/">Save 50% on EXAPUNKS on Steam Exapunks - Wikipedia EXAPUNKS - Zachtronics EXAPUNKS by Zachtronics Steam Community :: Guide :: Dan's Exapunks Solutions -50% EXAPUNKS on GOG.com Exapunks Review - by Felix Roth - Corerunner</a></li>

</ul>
</details>

**Discussion**: Commenters praised Exapunks and other Zachtronics games for capturing the essence of programming fun. One user noted that the game taught them assembly isn't scary, influencing their career. Another shared a concept for a game blending Zachtronics-style puzzles with Starcraft and Factorio elements.

**Tags**: `#gaming`, `#programming`, `#puzzle`, `#zachtronics`

---

<a id="item-14"></a>
## [Paper Fishing: Unethical Authorship in Academia](https://www.reddit.com/r/MachineLearning/comments/1ulgunh/what_do_you_think_about_paper_fishing_d/) ⭐️ 6.0/10

A PhD student in Germany reports a colleague who adds his name to others' papers without contributing, a practice known as 'paper fishing,' and questions whether it is normalized in academia. This highlights the ethical issue of gift authorship, which undermines research integrity and can lead to unfair career advancement, affecting trust in academic publishing. The colleague reportedly does no research work and relies on paper fishing to meet progress requirements for funding renewal, while others claim such practices are common in academia.

reddit · r/MachineLearning · /u/impressivestatus21 · Jul 2, 12:26

**Background**: Gift authorship, also known as guest authorship, occurs when someone is listed as an author without making a substantial contribution. This is considered a questionable research practice (QRP) by ethics committees like COPE. The practice can distort credit and accountability in research.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aje.com/arc/ghost-authorship-gift-authorship-guest-authorship">Ghost Authorship, Gift Authorship, Guest Authorship – 3 ...</a></li>
<li><a href="https://publicationethics.org/news-opinion/gift-authorship">Gift authorship - COPE: Committee on Publication Ethics</a></li>
<li><a href="https://journals.sagepub.com/doi/10.1177/17470161241262244">Gift and ghost authorship and the use of authorship ...</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion likely includes diverse viewpoints, with some condemning the practice as unethical and others acknowledging its prevalence, while debating whether it is truly normalized or just tolerated in certain environments.

**Tags**: `#academia`, `#ethics`, `#research culture`, `#machine learning`

---

<a id="item-15"></a>
## [ML PhD Seeks Math Foundation Book Recommendations](https://www.reddit.com/r/MachineLearning/comments/1ulmy9g/booksresources_to_improve_mathematical/) ⭐️ 6.0/10

A mid-to-late stage ML PhD student posted on Reddit asking for book recommendations to strengthen mathematical foundations in linear algebra, probability theory, and functional analysis, citing shaky fundamentals from learning as they go. This discussion highlights a common challenge for ML researchers: the need for solid mathematical foundations to advance in research, and the community's response can guide many others facing similar gaps. The user mentions considering 'Linear Algebra Done Right' for linear algebra, a primer on RKHS for functional analysis, and re-reading PRML (Pattern Recognition and Machine Learning) by Christopher Bishop, while seeking recommendations for probability theory.

reddit · r/MachineLearning · /u/mvreich · Jul 2, 16:24

**Background**: Many ML PhD students learn mathematics on the fly, leading to gaps in foundational knowledge. Books like 'Linear Algebra Done Right' and PRML are standard references, while functional analysis is often encountered through kernel methods and RKHS theory.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Reproducing_kernel_Hilbert_space">Reproducing kernel Hilbert space - Wikipedia</a></li>
<li><a href="https://www.microsoft.com/en-us/research/publication/pattern-recognition-machine-learning/">Pattern Recognition and Machine Learning - Microsoft Research</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#mathematics`, `#resources`, `#PhD`

---

<a id="item-16"></a>
## [How ML conference paper selections work](https://www.reddit.com/r/MachineLearning/comments/1ulnstb/how_papers_are_selected_for_best_paper_oral_or/) ⭐️ 6.0/10

A Reddit user asked how papers are selected for Best Paper, Oral, or Highlight presentations at major ML/CV conferences like CVPR, NeurIPS, and ICLR, sparking a discussion on the opaque selection process. Understanding the selection criteria helps researchers tailor their submissions and sets expectations, while also promoting transparency in academic publishing. The selection typically involves area chairs (ACs), senior area chairs (SACs), program chairs, or a separate award committee, and decisions are based on reviewer scores, novelty, impact, and AC discussions, often using the original reviewed version rather than the camera-ready.

reddit · r/MachineLearning · /u/National-Resident244 · Jul 2, 16:55

**Background**: Major ML/CV conferences receive thousands of submissions and use a peer-review system where each paper is reviewed by multiple reviewers. After reviews, area chairs lead discussions and make recommendations, while senior chairs and program chairs make final decisions on accept/reject and special designations like Oral or Best Paper.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.neurips.cc/2025/11/26/announcing-the-neurips-2025-best-paper-awards/">Announcing the NeurIPS 2025 Best Paper Awards – NeurIPS Blog</a></li>
<li><a href="https://neuripsconf.medium.com/announcing-the-neurips-2020-award-recipients-73e4d3101537">Announcing the NeurIPS 2020 award recipients | by Neural... | Medium</a></li>

</ul>
</details>

**Discussion**: The Reddit thread likely contains answers from experienced researchers explaining the multi-tiered review process, with some noting that ACs often have significant influence and that scores alone are not decisive.

**Tags**: `#conference`, `#paper selection`, `#machine learning`, `#CVPR`, `#NeurIPS`

---

<a id="item-17"></a>
## [Beginner Asks About Replacing Transformer with Mamba in Fast BLT](https://www.reddit.com/r/MachineLearning/comments/1ulngy8/has_anyone_tried_this_approach_with_fast_byte/) ⭐️ 4.0/10

A Reddit user asked whether anyone has tried replacing the transformer in the entropy model of the Fast Byte Latent Transformer (BLT) paper with a Mamba model, citing Mamba's linear-time complexity advantage. This question highlights a potential research direction to combine tokenizer-free byte-level models with efficient state-space architectures, which could lead to faster and more scalable language models. The Fast BLT paper introduces techniques to speed up byte-level transformers, while Mamba is a state-space model that achieves O(n) complexity. The user is a machine learning beginner and did not provide any experimental results or detailed analysis.

reddit · r/MachineLearning · /u/SoloLeveller07 · Jul 2, 16:43

**Background**: Fast Byte Latent Transformer (Fast BLT) is a tokenizer-free language model that processes raw bytes, addressing the bottleneck of standard byte-level transformers. Mamba is a recent architecture based on state-space models that offers linear-time inference and lower memory usage compared to transformers. Entropy models are used in compression and language modeling to predict the probability distribution of the next token or byte.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2605.08044">Fast Byte Latent Transformer</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mamba_(deep_learning_architecture)">Mamba (deep learning architecture) - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2312.00752">[2312.00752] Mamba: Linear-Time Sequence Modeling with ... What is a Mamba model - GeeksforGeeks Mamba (deep learning architecture) - Wikipedia A Visual Guide to Mamba and State Space Models What is a Mamba model? - IBM Core Model Architecture | state-spaces/mamba | DeepWiki</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#transformers`, `#Mamba`, `#entropy model`

---