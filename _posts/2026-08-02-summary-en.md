---
layout: default
title: "Horizon Summary: 2026-08-02 (EN)"
date: 2026-08-02
lang: en
---

> From 21 items, 14 important content pieces were selected

---

1. [Karpathy's Pelican Benchmark Sparks Debate on AI Physical Understanding](#item-1) ⭐️ 8.0/10
2. [Kakehashi: Experimental Userspace Runs macOS Binaries on Linux ARM](#item-2) ⭐️ 8.0/10
3. [F*: A General-Purpose Proof-Oriented Programming Language](#item-3) ⭐️ 8.0/10
4. [Open Letters Debate AI Open-Weight Models and Safety](#item-4) ⭐️ 8.0/10
5. [eBay Harassment Campaign Leads to $56M Payout and Prison Sentences](#item-5) ⭐️ 7.0/10
6. [Context Degradation in LLMs: Research Insights and Practical Habits](#item-6) ⭐️ 7.0/10
7. [CausalVLBench: New Benchmark for Visual Causal Reasoning in LVLMs](#item-7) ⭐️ 7.0/10
8. [Meshdiff: Client-Side STL Comparison Tool in Browser](#item-8) ⭐️ 6.0/10
9. [Seeking Pipeline Advice for Converting Textbook Figures into Editable Assets](#item-9) ⭐️ 6.0/10
10. [RISC OS Open Celebrates 20 Years of Open Source Development](#item-10) ⭐️ 5.0/10
11. [NeurIPS 2026 Reviewers and ACs Unresponsive After Early Rebuttals](#item-11) ⭐️ 5.0/10
12. [Conference Reviews: Demanding Too Much?](#item-12) ⭐️ 5.0/10
13. [Simon Willison's July 2026 Sponsors-Only Newsletter Released](#item-13) ⭐️ 4.0/10
14. [ARR August Cycle Submission Count Raises Venue Identification Questions](#item-14) ⭐️ 3.0/10

---

<a id="item-1"></a>
## [Karpathy's Pelican Benchmark Sparks Debate on AI Physical Understanding](https://twitter.com/karpathy/status/2083749667410727319) ⭐️ 8.0/10

Andrej Karpathy tweeted about a new benchmark called 'Pelican', which uses the task of generating an SVG of a pelican on a bicycle to evaluate AI models' understanding of the physical world. The tweet has sparked a high-engagement discussion on Hacker News and Twitter. This benchmark highlights a shift from simple image generation to more complex tasks that require physical world understanding, which is crucial for advancing AI capabilities. It provides a new way to measure progress in AI models, potentially influencing future research and development directions. The benchmark specifically asks models to generate an SVG of a pelican on a bicycle, which requires understanding of object relationships and physical plausibility. Karpathy noted that while the SVG pelican has a ground truth that can be eyeballed, more complex benchmarks like playable games are harder to evaluate at scale.

hackernews · delichon · Aug 2, 04:05 · [Discussion](https://news.ycombinator.com/item?id=49140998)

**Background**: AI models have traditionally been evaluated on tasks like image classification or text generation, but recent benchmarks aim to test deeper understanding of the physical world. This is part of a broader trend where researchers like Yann LeCun are investing in world models and architectures like JEPA to achieve physical understanding, moving beyond next-token prediction.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49140998">Karpathy’s Pelican | Hacker News</a></li>
<li><a href="https://x.com/karpathy/status/2083948654377996480">Andrej Karpathy on X: "More on the pelican on the bicycle ...</a></li>
<li><a href="https://arxiv.org/html/2512.01989">PAI- Bench : A Comprehensive Benchmark For Physical AI</a></li>

</ul>
</details>

**Discussion**: The community discussion is mixed: some express concern that the benchmark implies the 'pelican on a bicycle' problem is solved, while others see it as a useful qualitative measure for future progress. Some users note that models like Anthropic's may be specifically trained for three.js code generation, making such benchmarks less indicative of general physical understanding. There is also humorous commentary about going one layer deeper with recursive SVG generation.

**Tags**: `#AI`, `#benchmarking`, `#Karpathy`, `#physical understanding`, `#machine learning`

---

<a id="item-2"></a>
## [Kakehashi: Experimental Userspace Runs macOS Binaries on Linux ARM](https://github.com/wie-project/kakehashi) ⭐️ 8.0/10

Kakehashi, an experimental userspace translation layer, has demonstrated working prototypes that run macOS CLI binaries natively on Linux ARM64, including 7-Zip, curl, and Xcode tools. It loads Darwin Mach-O binaries, maps a freestanding libSystem, and translates BSD syscalls without using a JIT. This project could enable running macOS software on Linux ARM hardware, expanding compatibility and potentially reducing the need for macOS-specific hardware. It addresses a long-standing gap in cross-platform binary compatibility, similar to what Wine/Proton did for Windows apps, and could benefit developers and users on ARM Linux systems. The current implementation is CLI-first and lacks a JIT, resulting in performance overhead; for example, 7-Zip runs about 5.2x slower than native Linux. The project is at an early stage, with a clear optimization plan to reduce this gap, and it focuses on translating BSD syscalls and providing a freestanding libSystem.

hackernews · vlad_kalinkin · Aug 2, 16:26 · [Discussion](https://news.ycombinator.com/item?id=49145937)

**Background**: macOS binaries are Mach-O executables that rely on Darwin's kernel interfaces and libraries, making them incompatible with Linux. Projects like Darling aim to provide a compatibility layer for macOS on Linux, but ARM64 support is still in development. Kakehashi takes a different approach by focusing on userspace translation for ARM64, potentially complementing or competing with existing efforts.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/wie-project/kakehashi">GitHub - wie-project/kakehashi: Userspace macOS translation ...</a></li>
<li><a href="https://news.ycombinator.com/item?id=49145937">Show HN: Kakehashi – Experimental userspace to run macOS binaries on Linux ARM | Hacker News</a></li>
<li><a href="https://www.darlinghq.org/">Darling | macOS translation layer for Linux</a></li>

</ul>
</details>

**Discussion**: The HN community expressed strong interest, with users comparing Kakehashi to Darling and suggesting potential collaboration. Some raised questions about feasibility and the complexity of the approach, while others hoped for future applications like running Audio Unit plugins on Linux.

**Tags**: `#macOS`, `#Linux`, `#ARM`, `#binary compatibility`, `#userspace`

---

<a id="item-3"></a>
## [F*: A General-Purpose Proof-Oriented Programming Language](https://fstar-lang.org/) ⭐️ 8.0/10

F* is a general-purpose, proof-oriented programming language that integrates formal verification into the development process, allowing programmers to write programs together with machine-checked proofs of their properties. The language has gained attention for its ability to express external library calls while incrementally migrating existing C codebases, as highlighted in community discussions. F* matters because it offers a practical approach to formal verification, which is crucial for developing secure and reliable software, especially in critical systems. Its active community and real-world applications, such as migrating C codebases, indicate growing interest and potential for broader adoption in the industry. F* is pronounced 'F star' and is designed for dependently typed programming, where types can encode program specifications, and type-checking ensures correctness. The language has been used in projects like Steel, which is a proof-oriented programming language built on F* for concurrent separation logic, demonstrating its capability in handling concurrency and imperative code.

hackernews · ducktective · Aug 2, 12:31 · [Discussion](https://news.ycombinator.com/item?id=49143925)

**Background**: Formal verification is a technique used to prove the correctness of software using mathematical methods, often through specification languages and proof systems. F* is a proof-oriented programming language that integrates these techniques directly into the programming process, allowing developers to write programs and proofs together. This approach is particularly valuable in security-critical and safety-critical systems where bugs can have severe consequences.

<details><summary>References</summary>
<ul>
<li><a href="https://fstar-lang.org/">F *: A Proof - Oriented Programming Language</a></li>
<li><a href="https://www.linkedin.com/pulse/f-general-purpose-proof-oriented-programming-language-kusho-4bipc">F * : A general-purpose proof - oriented programming language</a></li>
<li><a href="https://www.linuxlinks.com/f-general-purpose-proof-oriented-programming-language/">F * - general-purpose, proof - oriented programming language</a></li>

</ul>
</details>

**Discussion**: Community comments show a mix of positive feedback and constructive criticism. Some users appreciate F*'s ability to handle external libraries and incremental migration from C, while others criticize the lack of code examples on the homepage, making it hard for newcomers to understand the syntax and benefits. There is also curiosity about its industry usage and applicability for functional programming enthusiasts.

**Tags**: `#formal verification`, `#programming language`, `#proof-oriented`, `#functional programming`, `#security`

---

<a id="item-4"></a>
## [Open Letters Debate AI Open-Weight Models and Safety](https://simonwillison.net/2026/Aug/2/open-letters/#atom-everything) ⭐️ 8.0/10

Simon Willison summarized recent open letters on AI development, including a Microsoft-led letter supporting open-weight models signed by 235 companies, and a separate letter from 1,324 AI employees calling for paced AI development. These letters reflect a significant industry divide over AI regulation, with major players like Microsoft, NVIDIA, and OpenAI advocating for open models, while Anthropic and others warn of risks. The outcome could shape US AI policy and the future of open-weight models. The Microsoft-led letter explicitly supports distillation, a technique where models train on other models' outputs, and argues against conflating it with misappropriation. Notably, Anthropic did not sign and instead published its own position, calling for a crackdown on industrial-scale distillation operations.

rss · Simon Willison · Aug 2, 04:16

**Background**: Open-weight models are AI models whose learned parameters are publicly released, allowing others to download, use, and sometimes modify them. This contrasts with closed models, which are kept proprietary. The debate centers on whether open weights foster innovation and safety through transparency or pose risks of misuse and concentration of power.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Open-weight_model">Open-weight model</a></li>
<li><a href="https://simonwillison.net/tags/ai/">Simon Willison on ai</a></li>

</ul>
</details>

**Tags**: `#AI`, `#open-source`, `#policy`, `#open-weight models`, `#industry`

---

<a id="item-5"></a>
## [eBay Harassment Campaign Leads to $56M Payout and Prison Sentences](https://www.ft.com/content/06ec1b03-d4af-40cf-b12a-4ba5a410f6d2) ⭐️ 7.0/10

eBay has agreed to pay $56 million to a Massachusetts couple after its security team conducted a harassment campaign against them. Several former eBay security executives, including Senior Director Jim Baugh, received prison sentences for their roles in the scheme. This case highlights serious ethical and security failures within a major tech company, raising questions about corporate accountability and the misuse of internal security resources. It serves as a cautionary tale for other companies about the legal and reputational consequences of targeting critics. The harassment campaign involved seven members of eBay's security team, including former police captains, who sent threatening messages, delivered live spiders and cockroaches, and conducted surveillance. Jim Baugh was sentenced to 57 months in prison, while Brian Gilbert received time served and a $20,000 fine.

hackernews · JumpCrisscross · Aug 2, 19:19 · [Discussion](https://news.ycombinator.com/item?id=49147435)

**Background**: The victims, David and Ina Steiner, published a newsletter critical of eBay. In response, eBay's security team launched a campaign to intimidate them, which included sending disturbing packages and monitoring their activities. The case underscores the importance of ethical oversight in corporate security operations.

**Discussion**: Commenters expressed skepticism that this campaign was limited to one couple, questioning whether eBay targeted other critics. Some referenced similar corporate misconduct cases, while others noted eBay's high seller fees as a separate concern.

**Tags**: `#eBay`, `#harassment`, `#legal`, `#corporate ethics`, `#security`

---

<a id="item-6"></a>
## [Context Degradation in LLMs: Research Insights and Practical Habits](https://www.reddit.com/r/MachineLearning/comments/1vdsgcj/context_degradation_in_llms_what_the_papers/) ⭐️ 7.0/10

A Reddit post synthesizes recent research on context degradation in large language models and offers practical habits for long analysis sessions. The post highlights that performance degrades as context length increases, a phenomenon known as 'context rot'. This matters because context degradation affects the reliability of LLMs in real-world applications, especially in long-horizon tasks like coding agents and scientific analysis. Understanding and mitigating this issue is crucial for practitioners who rely on LLMs for complex, extended interactions. The post references research showing that all tested frontier models degrade as context grows, with mechanisms including attention dilution and information overload. Practical habits include context compaction, structured note-taking, and multi-agent architectures, as suggested by Anthropic's context engineering cookbook.

reddit · r/MachineLearning · /u/usernamehere93 · Aug 2, 20:20

**Background**: Large language models (LLMs) process input sequences of tokens, and their performance can degrade when the input context becomes very long. This phenomenon, sometimes called 'context rot', has been observed across various models and can impact tasks that require maintaining information over extended interactions. Techniques like context compaction and structured note-taking aim to mitigate these effects by managing what information is retained.

<details><summary>References</summary>
<ul>
<li><a href="https://www.morphllm.com/context-rot">Context Rot: Why LLMs Degrade as Context Grows (Complete ...</a></li>
<li><a href="https://arxiv.org/html/2601.11564v1">Context Discipline and Performance Correlation: Analyzing LLM ...</a></li>
<li><a href="https://www.trychroma.com/research/context-rot">Context Rot: How Increasing Input Tokens Impacts LLM ...</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#context degradation`, `#machine learning`, `#practical tips`

---

<a id="item-7"></a>
## [CausalVLBench: New Benchmark for Visual Causal Reasoning in LVLMs](https://www.reddit.com/r/MachineLearning/comments/1vdd7ty/r_causalvlbench_benchmarking_visual_causal/) ⭐️ 7.0/10

Researchers introduced CausalVLBench, a new benchmark for evaluating visual causal reasoning in large vision-language models (LVLMs). It covers three tasks: causal structure inference, intervention target prediction, and counterfactual prediction, tested under zero-shot and few-shot settings. This benchmark addresses an underexplored capability of LVLMs, providing a standardized way to measure and compare their causal reasoning abilities. It could drive progress in making these models more reliable for tasks requiring understanding of cause-and-effect from visual data. The benchmark is detailed in the paper arXiv:2506.11034, which formulates causal reasoning in LVLMs as inferring causal mechanisms from visual cues. It evaluates models under zero-shot and few-shot settings, offering a comprehensive assessment of visual causal reasoning.

reddit · r/MachineLearning · /u/moschles · Aug 2, 09:07

**Background**: Large vision-language models (LVLMs) like GPT-4V and CLIP combine visual and textual understanding, but their causal reasoning abilities have been less studied compared to text-only LLMs. Causal reasoning involves understanding cause-effect relationships, which is crucial for tasks like predicting outcomes of interventions or imagining counterfactual scenarios. This benchmark aims to systematically evaluate these abilities in LVLMs.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2506.11034">[2506.11034] CausalVLBench: Benchmarking Visual Causal Reasoning in Large Vision-Language Models</a></li>
<li><a href="https://arxiv.org/html/2506.11034v2">CausalVLBench: Benchmarking Visual Causal Reasoning in Large Vision-Language Models</a></li>

</ul>
</details>

**Tags**: `#benchmark`, `#vision-language models`, `#causal reasoning`, `#evaluation`

---

<a id="item-8"></a>
## [Meshdiff: Client-Side STL Comparison Tool in Browser](https://meshdiff.com/) ⭐️ 6.0/10

Meshdiff is a new browser-based tool that allows users to visually compare two versions of an STL file entirely on the client side, without uploading data to a server. The tool displays three synchronized viewports (front, top, and side) to highlight geometric differences between the meshes. This tool addresses a practical need in 3D printing and CAD workflows, where tracking changes between file versions is common. Its client-side, local-first approach enhances privacy and convenience, aligning with a growing trend of powerful in-browser applications powered by WebAssembly and Three.js. The tool supports STL files, which are widely used in 3D printing and CAD, and provides a visual comparison without requiring server-side processing. Community members have suggested adding synchronized rotation controls and GitHub integration for automated previews in pull requests.

hackernews · projscope · Aug 2, 11:34 · [Discussion](https://news.ycombinator.com/item?id=49143479)

**Background**: STL (stereolithography) is a file format that describes the surface geometry of a 3D object as a triangulated mesh, commonly used in 3D printing and CAD. Comparing different versions of such files is essential for detecting design changes, but traditional tools often require desktop software or server uploads. Meshdiff leverages modern browser capabilities to perform this task locally, ensuring data privacy and ease of use.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/STL_(file_format)">STL (file format)</a></li>
<li><a href="https://www.adobe.com/creativecloud/file-types/image/vector/stl-file.html">STL files explained | Learn about the STL file format | Adobe</a></li>
<li><a href="https://meshdev.sourceforge.net/">MeshDev - Mesh Comparison Software</a></li>

</ul>
</details>

**Discussion**: The community response is positive, with users praising the tool's utility and local-first approach. Suggestions include adding synchronized viewport rotation and integrating the tool as a GitHub PR trigger for 3D file previews. Some users also noted the acronym confusion with the Standard Template Library (STL).

**Tags**: `#3D printing`, `#STL`, `#browser tool`, `#visualization`, `#CAD`

---

<a id="item-9"></a>
## [Seeking Pipeline Advice for Converting Textbook Figures into Editable Assets](https://www.reddit.com/r/MachineLearning/comments/1vdlj8j/looking_for_the_right_pipeline_to_convert/) ⭐️ 6.0/10

A Reddit user is asking for technical advice on building a human-assisted pipeline to convert scanned academic textbook figures into structured, editable digital assets by detecting figures, extracting and removing embedded labels, and storing geometry for frontend control. This discussion highlights a practical challenge in document understanding that combines figure detection, OCR, and image inpainting, with implications for educational technology and digital publishing. The community's suggestions could guide cost-effective, human-in-the-loop solutions for large-scale textbook digitization. The user emphasizes cost constraints, preferring lightweight or traditional CV methods over expensive multimodal LLMs, and notes that the workflow will be human-assisted to correct errors. The main technical hurdle is removing embedded labels while preserving the underlying illustration, which may require image inpainting techniques.

reddit · r/MachineLearning · /u/Afraid_Reviewer · Aug 2, 15:50

**Background**: Document layout analysis involves detecting and classifying regions such as figures, tables, and text in scanned pages. OCR (Optical Character Recognition) is used to extract text, while image inpainting fills in missing or removed areas. The user's goal is to create interactive educational content by making figures editable, which requires separating labels from artwork and storing geometric data for frontend rendering.

<details><summary>References</summary>
<ul>
<li><a href="https://www.researchgate.net/publication/352260370_A_Survey_of_Graphical_Page_Object_Detection_with_Deep_Neural_Networks">(PDF) A Survey of Graphical Page Object Detection with Deep Neural...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Geometric_feature_learning">Geometric feature learning - Wikipedia</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S2773186325001549">Image feature extraction techniques: A comprehensive review</a></li>

</ul>
</details>

**Discussion**: No comments were provided in the news item, so community sentiment is unavailable.

**Tags**: `#document understanding`, `#computer vision`, `#OCR`, `#figure extraction`, `#pipeline`

---

<a id="item-10"></a>
## [RISC OS Open Celebrates 20 Years of Open Source Development](https://www.riscosopen.org/news/articles/2026/06/20/twenty-years-of-risc-os-open) ⭐️ 5.0/10

RISC OS Open, the community-driven project managing the open-source RISC OS operating system, celebrated its twentieth anniversary on June 20, 2026. The milestone highlights the continued development and dedication of the community to this niche ARM-based OS. This anniversary underscores the longevity and resilience of RISC OS, a unique non-POSIX operating system that has survived Acorn's demise and continues to attract hobbyists and embedded developers. It demonstrates the power of community-driven open-source projects in preserving and evolving legacy software. RISC OS Open Limited (ROOL) manages the source code, which was open-sourced in 2018, and the project is run largely on a voluntary basis. The OS is known for its fast boot times on Raspberry Pi and its modular design, and it continues to be developed on version 5.0.

hackernews · AlexeyBrin · Aug 2, 12:36 · [Discussion](https://news.ycombinator.com/item?id=49143967)

**Background**: RISC OS was originally designed by Acorn Computers in 1987 for their ARM-based Archimedes personal computers. After Acorn's demise, the intellectual property passed through several hands, and in 2006 RISC OS Open was formed to facilitate publishing the sources. The OS is notable for being designed specifically for ARM from the start, and it remains a lightweight, modular alternative to mainstream operating systems.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/RISC_OS">RISC OS - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/RISC_OS_Open">RISC OS Open - Wikipedia</a></li>
<li><a href="https://www.riscosopen.org/content/">RISC OS Open: Welcome</a></li>

</ul>
</details>

**Discussion**: Community comments reflect nostalgia and technical appreciation. One user fondly recalled developing software for RISC OS, noting it was where they cut their teeth as an open-source developer. Others highlighted the OS's fast boot on Raspberry Pi and pointed to programming resources, while another expressed surprise at the project's longevity given the small user base.

**Tags**: `#RISC OS`, `#Open Source`, `#Retro Computing`, `#ARM`, `#Community`

---

<a id="item-11"></a>
## [NeurIPS 2026 Reviewers and ACs Unresponsive After Early Rebuttals](https://www.reddit.com/r/MachineLearning/comments/1vdu92a/neurips_2026_acs_and_reviewers_have_disappeared_d/) ⭐️ 5.0/10

Authors report that after submitting rebuttals early via the 'Rebuttal' button before the official discussion period (Jul 27 AoE), they received no responses from reviewers or ACs, and no notifications were triggered for rebuttals on papers they were reviewing. The issue persists even after the discussion period opened, with about one day left in the discussion window. This highlights a potential systemic flaw in the NeurIPS 2026 review process, where early rebuttals may be overlooked, undermining the fairness and effectiveness of the discussion phase. It affects authors' chances for oral/spotlight decisions and could erode trust in the conference's peer review system. The authors tried meta-comments visible to all, individual nudges to reviewers, and emails to PCs, but still received silence. Some users report metareviews already contain decisions (all rejections), while others have metareviews that seem optimistic but lack reviewer engagement.

reddit · r/MachineLearning · /u/extricableforsythia · Aug 2, 21:33

**Background**: NeurIPS is a top-tier machine learning conference that uses a peer review process where authors submit rebuttals to reviewer comments during a designated discussion period. The official guidelines state that rebuttals can be posted until August 3rd AOE, and both the 'Rebuttal' and 'official comment' buttons are treated equivalently. However, the system may not have sent notifications for early submissions, causing authors to miss out on engagement.

<details><summary>References</summary>
<ul>
<li><a href="https://neurips.cc/Conferences/2026/ReviewerGuidelines">2026 Reviewer Guidelines - neurips.cc</a></li>
<li><a href="https://x.com/NeurIPSConf/status/2081991451236319328">A clarification on the timeframe for rebuttals and author ...</a></li>
<li><a href="https://singularitymoments.com/content/neurips-2026-why-the-review-process-is-breaking-under-the-weight-of-ai/">NeurIPS 2026: Why the review process is breaking under the ...</a></li>

</ul>
</details>

**Discussion**: The community expresses frustration and concern, with some noting that metareviews already contain decisions (mostly rejections) while others see optimistic metareviews but no reviewer engagement. There is a sense of helplessness and questioning of the process's fairness, with some wondering whether to keep hope or give up.

**Tags**: `#NeurIPS`, `#peer review`, `#conference`, `#rebuttal`, `#community`

---

<a id="item-12"></a>
## [Conference Reviews: Demanding Too Much?](https://www.reddit.com/r/MachineLearning/comments/1vdl461/conference_reviews_asking_too_much_d/) ⭐️ 5.0/10

A researcher on Reddit questions whether conference reviewers' demands for extensive additions, often extending beyond the paper's stated scope, are appropriate, and suggests such papers might be better suited for journals. The author also mentions having to retract a paper due to concerns that a conference publication would block a planned journal publication. This discussion highlights a common tension in academic publishing between conference and journal expectations, affecting researchers' publication strategies and career progression. It underscores the need for clearer guidelines and better alignment between review demands and publication venues. The author notes that top-tier conferences often require additions to go into supplemental materials or appendices due to page limits. They question whether such expanded papers should instead be submitted to journals, which typically allow longer formats and more flexibility.

reddit · r/MachineLearning · /u/examachine · Aug 2, 15:33

**Background**: Conference papers are typically shorter and more structured, with strict page limits (e.g., 6-8 pages for IEEE full papers), while journals allow more extensive content. Supplemental materials are used to add depth without exceeding page limits, but they may not be fully reviewed. Publishing a conference paper can sometimes conflict with later journal publication, depending on the venue's policies on extended versions.

<details><summary>References</summary>
<ul>
<li><a href="https://conferences.ieeeauthorcenter.ieee.org/become-an-ieee-conference-author/types-of-ieee-conference-papers/">Types of IEEE Conference Papers - IEEE Author Center Conferences</a></li>
<li><a href="https://www.iconf.com/news/824">Conference Paper Word Count and Page Limit: What You Need to ...</a></li>
<li><a href="https://marss-conference.org/submission/journal-publication-after-conference/">Journal publication after MARSS – MARSS 2026 Hangzhou, China</a></li>

</ul>
</details>

**Tags**: `#academic publishing`, `#conference reviews`, `#research process`, `#machine learning`

---

<a id="item-13"></a>
## [Simon Willison's July 2026 Sponsors-Only Newsletter Released](https://simonwillison.net/2026/Aug/2/july-newsletter/#atom-everything) ⭐️ 4.0/10

Simon Willison announced the release of his July 2026 sponsors-only monthly newsletter, accessible to GitHub sponsors. The newsletter covers topics including AI model releases (GPT-5.6 Sol/Terra/Luna, Claude Opus 5, Kimi K3, DeepSeek-V4-Flash-0731), accidental cyberattacks by AI models, and his renewed interest in MCP. This newsletter provides early access to curated insights on cutting-edge AI developments, which is valuable for practitioners and enthusiasts who follow Simon Willison's analysis. It also highlights the growing trend of creators using sponsorship models to monetize exclusive content. The newsletter is available to sponsors, with a $10/month sponsorship to stay a month ahead of the free copy. A preview of the June newsletter is linked for potential subscribers. The topics include specific model names and a mention of MCP (Model Context Protocol), an open standard for AI integration.

rss · Simon Willison · Aug 2, 04:12

**Background**: Simon Willison is a well-known developer and AI enthusiast who publishes a monthly newsletter summarizing notable AI developments. MCP (Model Context Protocol) is an open standard introduced by Anthropic in November 2024 to standardize how AI applications connect to external systems. The newsletter covers recent model releases such as GPT-5.6 and Kimi K3, reflecting the rapid pace of AI advancement.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>
<li><a href="https://openai.com/index/gpt-5-6/">GPT-5.6: Frontier intelligence that scales with your ambition | OpenAI</a></li>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K 3 Tech Blog: Open Frontier Intelligence</a></li>

</ul>
</details>

**Tags**: `#newsletter`, `#AI`, `#MCP`, `#Simon Willison`

---

<a id="item-14"></a>
## [ARR August Cycle Submission Count Raises Venue Identification Questions](https://www.reddit.com/r/MachineLearning/comments/1vdgpha/arr_august_cycle_d/) ⭐️ 3.0/10

A researcher on r/MachineLearning asked whether the low submission count (under 500) in the ARR August cycle can indicate the intended venue, such as EACL 2027, or if it is simply due to incomplete submissions. The question highlights uncertainty about the reliability of the counter for venue identification. This matters because ARR is a central peer-review platform for NLP, and understanding submission patterns helps researchers gauge competition and plan submissions. The question reflects broader community interest in how ARR cycles align with specific conference deadlines, which affects submission strategies. The ARR August cycle has a submission deadline of August 3, 2026, for EACL 2027, according to the EACL 2027 website. ARR runs 8-week review cycles with deadlines on the 15th of every second month, but the counter may not be fully updated until after the deadline.

reddit · r/MachineLearning · /u/New_Glove_2098 · Aug 2, 12:22

**Background**: ACL Rolling Review (ARR) is a peer-review platform for the Association for Computational Linguistics, where authors submit papers that are reviewed and then can be committed to a venue. The submission count on the ARR dashboard is often used by authors to gauge the number of submissions, but it may not be reliable until the cycle closes. EACL 2027 is the 20th conference of the European Chapter of the ACL, scheduled for March 2027 in Athens, Greece.

<details><summary>References</summary>
<ul>
<li><a href="https://aclrollingreview.org/dates">Dates and Venues – ACL Rolling Review – A peer review platform for...</a></li>
<li><a href="https://2027.eacl.org/calls/papers/">EACL 2027 Call for Papers</a></li>
<li><a href="https://2027.eacl.org/">2027.eacl.org - The 20th Conference of the European Chapter</a></li>

</ul>
</details>

**Tags**: `#ARR`, `#submission`, `#EACL`, `#NLP`, `#academic publishing`

---