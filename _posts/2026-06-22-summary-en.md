---
layout: default
title: "Horizon Summary: 2026-06-22 (EN)"
date: 2026-06-22
lang: en
---

> From 14 items, 11 important content pieces were selected

---

1. [Valve Launches Steam Machine with Fair Reservation System](#item-1) ⭐️ 9.0/10
2. [Half of LG Smart TV Apps Contain Proxy SDKs](#item-2) ⭐️ 8.0/10
3. [Moebius: 0.2B inpainting model rivals 10B performance](#item-3) ⭐️ 8.0/10
4. [Police Chiefs Abusing Flock LPR to Stalk Women](#item-4) ⭐️ 8.0/10
5. [Canada Plans Up to 10 New Nuclear Reactors in 15 Years](#item-5) ⭐️ 7.0/10
6. [Mitchell Hashimoto Pledges $400k to Zig Software Foundation](#item-6) ⭐️ 7.0/10
7. [sqlite-utils 4.0rc1 Adds Migrations and Nested Transactions](#item-7) ⭐️ 7.0/10
8. [Hugging Face Revives Papers with Code with New Features](#item-8) ⭐️ 7.0/10
9. [Seeking Syntax-Robust NLI for Diffusion LLM Outputs](#item-9) ⭐️ 7.0/10
10. [Oak: A Git Alternative Designed for AI Agents](#item-10) ⭐️ 6.0/10
11. [User Seeks Local Speech Annotation Tool with HITL](#item-11) ⭐️ 4.0/10

---

<a id="item-1"></a>
## [Valve Launches Steam Machine with Fair Reservation System](https://store.steampowered.com/news/group/45479024/view/685257114654870245) ⭐️ 9.0/10

Valve launched the Steam Machine on June 29, 2026, a new gaming PC running SteamOS, with a randomized reservation system to combat scalping and ensure fair access. This launch marks Valve's return to dedicated gaming hardware with an open platform philosophy, potentially reshaping the PC gaming landscape by offering a console-like experience with PC flexibility. The Steam Machine is reported to be over six times faster than the Steam Deck in some aspects, and it comes in 512GB and 2TB versions. The reservation system accepts signups over several days without incentive to be first, aiming to reduce bot activity.

hackernews · theschwa · Jun 22, 17:09 · [Discussion](https://news.ycombinator.com/item?id=48632884)

**Background**: Steam Machines were first introduced in 2015 as a line of small form-factor gaming PCs running SteamOS, but they were discontinued by 2018 due to low adoption. Valve's new Steam Machine is a single, unified design released in 2026, building on the success of the Steam Deck and emphasizing open hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Steam_Machine">Steam Machine</a></li>
<li><a href="https://store.steampowered.com/sale/steammachine">Steam Machine</a></li>
<li><a href="https://www.vice.com/en/article/steam-machine-pre-orders-might-go-live-soon-as-reservation-system-leaks/">Steam Machine Pre-Orders Might Go Live Soon As Reservation ...</a></li>

</ul>
</details>

**Discussion**: Community comments are largely positive, praising the fair reservation system and open platform. Users appreciate the ability to install other operating systems and see the launch as a signal of Linux gaming support, though some note missing price and spec details.

**Tags**: `#gaming`, `#hardware`, `#valve`, `#steam`, `#pc-gaming`

---

<a id="item-2"></a>
## [Half of LG Smart TV Apps Contain Proxy SDKs](https://spur.us/blog/smart-tv-apps-residential-proxy-sdks) ⭐️ 8.0/10

Spur scanned 6,038 LG and Samsung smart TV apps and found 2,058 (about 34%) contained residential proxy SDKs, with nearly half of LG apps affected. This turns millions of smart TVs into potential proxy exit nodes, enabling fraud, credential stuffing, and privacy violations without user consent. The SDKs can be configured to ignore screen-on and call states, meaning the TV relays traffic even while actively used. Top flagged apps include those from Desoline and Bright Data, both based in Israel.

hackernews · microcode · Jun 22, 20:48 · [Discussion](https://news.ycombinator.com/item?id=48635954)

**Background**: Residential proxy SDKs allow apps to route third-party traffic through the user's home IP address, making it appear as legitimate residential traffic. This is often used for web scraping or bypassing geo-restrictions, but when embedded in smart TVs without clear disclosure, it poses serious privacy risks.

<details><summary>References</summary>
<ul>
<li><a href="https://spur.us/blog/smart-tv-apps-residential-proxy-sdks">Nearly Half of LG Smart TV Apps Contain Residential Proxy SDKs</a></li>
<li><a href="https://securityarsenal.com/blog/bright-data-sdk-abuse-smart-tvs-and-mobile-devices-hijacked-for-ai-scraping">Bright Data SDK Abuse: Smart TVs and Mobile Devices Hijacked for AI ...</a></li>
<li><a href="https://cybersecuritynews.com/free-apps-turning-smart-tvs-into-proxies/">Free Apps on Samsung and LG Smart TVs Secretly Turning Your Devices ...</a></li>

</ul>
</details>

**Discussion**: Commenters strongly advise never connecting smart TVs to the internet, suggesting VLAN isolation or using external devices like Apple TV. Some express revulsion at the privacy violations, while others note that commercial displays are a safer alternative.

**Tags**: `#smart TV`, `#privacy`, `#security`, `#SDK`, `#LG`

---

<a id="item-3"></a>
## [Moebius: 0.2B inpainting model rivals 10B performance](https://hustvl.github.io/Moebius/) ⭐️ 8.0/10

Researchers released Moebius, a 0.2B parameter image inpainting model that claims to match the performance of 10B-level models, along with a browser-based ONNX demo. This breakthrough could democratize high-quality image inpainting by making it feasible on consumer hardware, reducing computational costs by orders of magnitude. The model is limited to 512x512 output and inpainted regions may appear smoother than surroundings; it struggles with novel objects.

hackernews · DSemba · Jun 22, 13:53 · [Discussion](https://news.ycombinator.com/item?id=48630171)

**Background**: Image inpainting fills missing or damaged parts of an image. Large models (10B parameters) achieve high quality but require massive compute. Moebius uses extreme compression and a specialized design to overcome the representation bottleneck.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/papers/2606.19195">Paper page - Moebius: 0.2B Lightweight Image Inpainting ...</a></li>
<li><a href="https://arxiv.org/abs/2606.19195">[2606.19195] Moebius: 0.2B Lightweight Image Inpainting ...</a></li>
<li><a href="https://hustvl.github.io/Moebius/">Moebius: 0.2B Lightweight Image Inpainting Framework with 10B ...</a></li>

</ul>
</details>

**Discussion**: Community members praised the efficiency but noted visible quality gaps compared to 10B models, especially in smoothness and novel objects. Some requested specialized versions for manga inpainting.

**Tags**: `#image inpainting`, `#deep learning`, `#computer vision`, `#efficient models`, `#ONNX`

---

<a id="item-4"></a>
## [Police Chiefs Abusing Flock LPR to Stalk Women](https://ipvm.com/reports/police-chiefs-track) ⭐️ 8.0/10

A report reveals that police chiefs have used Flock license plate readers to stalk women, demonstrating the urgent need for warrant requirements before such surveillance tools can be queried. This abuse of surveillance technology by law enforcement leaders undermines public trust and highlights the real-world consequences of warrantless surveillance, potentially influencing policy debates on privacy and civil liberties. The report documents multiple cases where police chiefs used Flock's automatic license plate reader (ALPR) data to track women's movements without a warrant, raising serious Fourth Amendment concerns.

hackernews · jhonovich · Jun 22, 19:13 · [Discussion](https://news.ycombinator.com/item?id=48634694)

**Background**: Flock Safety is a company that sells ALPR cameras that capture license plate data and store it in a searchable database. Law enforcement agencies often use these systems to solve crimes, but critics argue they enable mass surveillance without proper oversight. The Fourth Amendment generally requires a warrant for searches, but exceptions exist for data in plain view or voluntarily shared.

<details><summary>References</summary>
<ul>
<li><a href="https://www.law.cornell.edu/wex/electronic_surveillance">electronic surveillance | Wex | US Law | LII / Legal Information Institute</a></li>
<li><a href="https://stateofsurveillance.org/news/surveillance-accountability-act-massie-boebert-warrant-requirement-hr8470-2026/">Two Republicans File a Bill Requiring Warrants Before Government Surveillance - State of Surveillance</a></li>

</ul>
</details>

**Discussion**: Commenters expressed outrage and concern, with some noting that similar abuse could happen to anyone and urging readers to contact their local ACLU. Others debated the trade-off between crime-solving benefits and privacy risks, while one commenter pointed out that the police chief also stalked a man.

**Tags**: `#surveillance`, `#privacy`, `#police abuse`, `#civil liberties`, `#technology ethics`

---

<a id="item-5"></a>
## [Canada Plans Up to 10 New Nuclear Reactors in 15 Years](https://www.cbc.ca/news/politics/federal-nuclear-strategy-9.7244509) ⭐️ 7.0/10

The Canadian government announced a strategy to build up to 10 new nuclear reactors over the next 15 years, leveraging its uranium reserves and CANDU reactor expertise. This expansion could significantly boost Canada's clean energy capacity, supporting net-zero goals and providing reliable baseload power to complement intermittent renewables like solar and wind. The plan includes small modular reactors (SMRs) and traditional CANDU designs, with potential applications in oil sands operations to reduce CO2 emissions. The Darlington New Nuclear Project is already underway.

hackernews · geox · Jun 22, 19:06 · [Discussion](https://news.ycombinator.com/item?id=48634585)

**Background**: Canada is one of the few countries that offers complete nuclear reactor technology and services, with CANDU reactors operating both domestically and internationally. The country also holds some of the world's largest uranium reserves, giving it a strategic advantage in nuclear energy development.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/CANDU_reactor">CANDU reactor - Wikipedia</a></li>
<li><a href="https://natural-resources.canada.ca/energy-sources/nuclear-energy-uranium/canadian-nuclear-energy-technology">The Canadian Nuclear Energy Technology - Natural Resources Canada</a></li>
<li><a href="https://www.atkinsrealis.com/en/projects/candu-technology">CANDU technology: helping Ontario achieve Net Zero</a></li>

</ul>
</details>

**Discussion**: Commenters largely support the plan, citing Canada's uranium reserves, CANDU safety record, and need for baseload power. Some express skepticism about legislative delays, while others highlight potential industrial uses like powering oil sands operations.

**Tags**: `#nuclear energy`, `#Canada`, `#energy policy`, `#CANDU`, `#clean energy`

---

<a id="item-6"></a>
## [Mitchell Hashimoto Pledges $400k to Zig Software Foundation](https://mitchellh.com/writing/zig-donation-2026) ⭐️ 7.0/10

Mitchell Hashimoto, creator of the Ghostty terminal emulator, has pledged an additional $400,000 to the Zig Software Foundation to support the development of the Zig programming language. The donation is tied to Zig's principled stance against accepting contributions generated by large language models (LLMs). This significant donation provides crucial financial support for Zig, a promising systems programming language, and reinforces the project's controversial policy against LLM-generated contributions, which has sparked broader debate in the open-source community. It also highlights the growing influence of Ghostty, a terminal emulator written in Zig, which has boosted the language's visibility. The pledge is for the year 2026, following a previous $400,000 donation in 2024. Mitchell Hashimoto is the founder of HashiCorp and creator of Ghostty, a GPU-accelerated terminal emulator written in Zig that has gained significant traction.

hackernews · tosh · Jun 22, 13:43 · [Discussion](https://news.ycombinator.com/item?id=48630020)

**Background**: Zig is a general-purpose systems programming language designed as a modern alternative to C, emphasizing simplicity, performance, and safety. The Zig Software Foundation (ZSF) is a non-profit that funds the language's development. The project's policy against LLM-generated contributions stems from concerns that such contributions increase maintainer burden without fostering genuine contributor growth, a stance that has drawn both support and criticism.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>
<li><a href="https://ziglang.org/">Home ⚡ Zig Programming Language</a></li>
<li><a href="https://openclawradar.com/article/zig-anti-llm-policy-rationale">Zig's Strict Anti- LLM Contribution Policy Explained</a></li>

</ul>
</details>

**Discussion**: Community comments largely praised the donation and Mitchell's contributions, with many highlighting Ghostty's quality and its role in promoting Zig. Some commenters also discussed Zig's anti-LLM policy, with one noting that it makes sense for the language's careful design process, while others debated the broader implications of LLM use in open source.

**Tags**: `#Zig`, `#open-source`, `#donation`, `#programming-languages`

---

<a id="item-7"></a>
## [sqlite-utils 4.0rc1 Adds Migrations and Nested Transactions](https://simonwillison.net/2026/Jun/21/sqlite-utils-40rc1/#atom-everything) ⭐️ 7.0/10

Simon Willison released sqlite-utils 4.0rc1, the first release candidate for version 4, which introduces built-in database migrations and nested transaction support via the db.atomic() context manager. This update brings essential database management features to a widely-used Python library and CLI tool, making it easier for developers to handle schema changes and complex transactional logic in SQLite without external dependencies. The migration system is a port of the existing sqlite-migrate package and does not support reverse migrations; errors must be fixed by adding new migrations. The nested transactions use SQLite savepoints, allowing atomic operations within a transaction.

rss · Simon Willison · Jun 21, 23:35

**Background**: sqlite-utils is a Python library and CLI tool that provides higher-level operations on top of Python's built-in sqlite3 module, such as table transformations and automatic table creation from JSON. Migrations help manage incremental schema changes, while nested transactions allow partial rollbacks within a larger transaction.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/21/sqlite-utils-40rc1/">sqlite-utils 4.0rc1 adds migrations and nested transactions</a></li>
<li><a href="https://github.com/simonw/sqlite-migrate">GitHub - simonw/sqlite-migrate: A simple database migration system for SQLite, based on sqlite-utils · GitHub</a></li>
<li><a href="https://pypi.org/project/sqlite-migrate/">sqlite-migrate · PyPI</a></li>

</ul>
</details>

**Tags**: `#Python`, `#SQLite`, `#database`, `#migrations`, `#open source`

---

<a id="item-8"></a>
## [Hugging Face Revives Papers with Code with New Features](https://www.reddit.com/r/MachineLearning/comments/1ucm508/some_new_updates_to_papers_with_code_p/) ⭐️ 7.0/10

Hugging Face has revived Papers with Code (paperswithcode.co) with new features including SOTA badges, a trending score that combines GitHub star velocity and Hugging Face artifact activity, support for external evaluations, and expanded benchmarks like ImageNet-10% and 3D semantic segmentation. These updates improve research discovery and benchmarking, making it easier for the ML community to track state-of-the-art results and build on each other's work, which is crucial for accelerating progress in AI. The new trending score now incorporates Hugging Face artifact activity (models, datasets, Spaces) in addition to GitHub stars, and external evaluations allow viewing third-party benchmark results not originally in the paper. The platform also moved to a new domain (paperswithco.de) and continues to add more benchmarks from legacy data.

reddit · r/MachineLearning · /u/NielsRogge · Jun 22, 14:29

**Background**: Papers with Code is a platform that aggregates machine learning papers with associated code and benchmarks, helping researchers compare results. It was originally created by Ben Eysenbach and later acquired by Meta, but had fallen into disrepair. Hugging Face took over the project to revive it as a community resource.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/Papers_with_Code">Papers with Code</a></li>
<li><a href="https://paperswithcode.co/">Trending AI research papers with code , datasets, methods, and...</a></li>

</ul>
</details>

**Discussion**: The Reddit community reacted positively, with many expressing excitement about the revival and the new features. Some users requested additional benchmarks or features, and the Hugging Face team member responded actively to feedback.

**Tags**: `#machine learning`, `#papers with code`, `#open source`, `#benchmarking`, `#Hugging Face`

---

<a id="item-9"></a>
## [Seeking Syntax-Robust NLI for Diffusion LLM Outputs](https://www.reddit.com/r/MachineLearning/comments/1ucy7p3/syntactically_robust_nli_for_semantics_of/) ⭐️ 7.0/10

A researcher on Reddit is asking for literature on syntax-robust Natural Language Inference (NLI) to evaluate the semantic correctness of syntactically imperfect text generated by diffusion LLMs. This highlights a gap in current NLI research, as diffusion LLMs produce more syntactic noise than autoregressive models, complicating semantic evaluation. Addressing this could improve the reliability of automated evaluation for emerging diffusion-based language models. The user notes that state-of-the-art diffusion LLMs (except possibly LLaDA) struggle with syntactic correctness compared to autoregressive LLMs, and asks whether existing NLI methods are robust to such noise. The post has a score of 7 and includes community suggestions for relevant papers.

reddit · r/MachineLearning · /u/RepresentativeBee600 · Jun 22, 21:51

**Background**: Autoregressive LLMs (e.g., GPT) generate text token by token sequentially, while diffusion LLMs generate text by iteratively denoising from random noise. NLI is a task that determines whether a hypothesis is entailed, contradicted, or neutral given a premise, and has been used to evaluate the factual correctness of LLM outputs. However, NLI models are often sensitive to syntactic perturbations, which are more common in diffusion LLM outputs.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2604.16787">When Informal Text Breaks NLI: Tokenization Failure ...</a></li>
<li><a href="https://www.sciencedirect.com/science/article/abs/pii/S0950705124012425">Bridge to better understanding: Syntax extension with virtual linking-phrase for natural language inference - ScienceDirect</a></li>
<li><a href="https://timkellogg.me/blog/2025/02/17/diffusion">LLaDA: LLMs That Don't Gaslight You - Tim Kellogg</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion is substantive, with users suggesting relevant papers and approaches, indicating community validation of the research direction. Some comments point to existing work on NLI robustness to informal text and syntax extension methods.

**Tags**: `#NLI`, `#LLM`, `#syntax robustness`, `#diffusion models`, `#semantic evaluation`

---

<a id="item-10"></a>
## [Oak: A Git Alternative Designed for AI Agents](https://oak.space/oak/oak) ⭐️ 6.0/10

Oak is a new version control system built specifically for AI agents, using virtual mounts to allow agents to work on large repos without a full clone, enabling parallel task handling and reducing repo size. It claims to be up to 95% faster than Git for snapshots and eliminates the need for commit messages. As AI agents become more involved in software development, traditional version control systems like Git may become bottlenecks due to large repo sizes and sequential workflows. Oak aims to address these issues, potentially enabling more efficient agent-driven development and reducing token usage for LLM-based agents. Oak is still early-stage, lacking Windows support, CI, issues, and comments features. It uses virtual mounts similar to Google's internal system and Microsoft's VFS for Git, but is designed as a standalone VCS rather than a Git extension.

hackernews · zdgeier · Jun 22, 15:37 · [Discussion](https://news.ycombinator.com/item?id=48631726)

**Background**: Version control systems like Git track changes to files over time, but require a full copy of the repository to work, which can be large and slow for AI agents that need to operate on many tasks simultaneously. Virtual mounts allow files to be fetched on demand, reducing storage and bandwidth. Oak is designed to be a faster, agent-friendly alternative to Git.

<details><summary>References</summary>
<ul>
<li><a href="https://oak.space/">Version control at the speed of agents · oak</a></li>
<li><a href="https://en.wikipedia.org/wiki/List_of_version-control_software">List of version-control software - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Version_control">Version control - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community comments are mixed: some praise the lazy mount concept as innovative and similar to Google's internal system, while others question whether a new VCS is needed given Git's ubiquity and the fact that AI models already know Git well. Skepticism exists about token efficiency and compatibility with existing Git ecosystems.

**Tags**: `#version control`, `#AI agents`, `#git alternative`, `#developer tools`

---

<a id="item-11"></a>
## [User Seeks Local Speech Annotation Tool with HITL](https://www.reddit.com/r/MachineLearning/comments/1ucuohi/recommendations_for_speech_annotation_tools_d/) ⭐️ 4.0/10

A Reddit user requested recommendations for a locally installable speech annotation platform that supports human-in-the-loop (HITL) workflows, including automatic transcription, manual correction, and model fine-tuning. This query highlights a growing need for privacy-preserving, offline annotation tools in speech AI development, as many existing solutions are cloud-based. Addressing this gap could accelerate adoption of HITL practices in resource-constrained environments. The user specifically wants a platform that is not an online service, implying concerns about data privacy or internet dependency. The request includes automatic transcription followed by manual correction and model fine-tuning, which is a typical HITL pipeline for speech recognition.

reddit · r/MachineLearning · /u/neuralbeans · Jun 22, 19:40

**Background**: Human-in-the-loop (HITL) machine learning combines AI automation with human oversight to improve model accuracy and handle ambiguous cases. Speech annotation tools are used to transcribe and label audio data for training speech recognition models. Local installable tools offer data privacy and offline operation, unlike cloud-based services.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Human-in-the-loop">Human-in-the-loop - Wikipedia</a></li>
<li><a href="https://github.com/inboxpraveen/Speech-Annotation-Tool">GitHub - inboxpraveen/ Speech - Annotation - Tool : Review, correct, and...</a></li>
<li><a href="https://app.audino.in/">Audino Annotation Tool</a></li>

</ul>
</details>

**Tags**: `#speech annotation`, `#human-in-the-loop`, `#tool recommendation`

---