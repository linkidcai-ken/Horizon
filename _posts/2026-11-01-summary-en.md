---
layout: default
title: "Horizon Summary: 2026-11-01 (EN)"
date: 2026-11-01
lang: en
---

> From 15 items, 13 important content pieces were selected

---

1. [Jepsen Finds Severe Transactional Anomalies in ParticleDB 1.1.4](#item-1) ⭐️ 9.0/10
2. [HackerTube: A YouTube-style Interface Built from Hacker News Video Recommendations](#item-2) ⭐️ 8.0/10
3. [Critical Linux TCP Use-After-Free Vulnerability CVE-2026-98432 (CVSS 9.8)](#item-3) ⭐️ 8.0/10
4. [Researchers exploit ChatGPT account takeover via preview and JSONP flaw](#item-4) ⭐️ 8.0/10
5. [Blog Post Argues Memory Latency, Not Bandwidth, Is the Real Bottleneck](#item-5) ⭐️ 7.0/10
6. [Molly Signal fork unmaintained for 3 months, contains vulnerabilities](#item-6) ⭐️ 7.0/10
7. [Anthropic Blocks Users for Training Larger Models, Sparking Debate](#item-7) ⭐️ 7.0/10
8. [Reddit user asks for cross-modal ML technique taxonomy](#item-8) ⭐️ 6.0/10
9. [Two-stage deep learning framework detects neonatal brain pathologies from MRI](#item-9) ⭐️ 6.0/10
10. [Gear: An Open-Source scikit-learn for Recursive Self-Improvement](#item-10) ⭐️ 6.0/10
11. [Reddit User Asks: Is Neuro-Evolution Relevant in Industry or Research?](#item-11) ⭐️ 5.0/10
12. [datasette-llm 0.1a9 auto-detects LLM default model](#item-12) ⭐️ 4.0/10
13. [Reddit user asks if sharing from-scratch LLM experiments is welcome](#item-13) ⭐️ 3.0/10

---

<a id="item-1"></a>
## [Jepsen Finds Severe Transactional Anomalies in ParticleDB 1.1.4](https://jepsen.io/analyses/particledb-1.1.4) ⭐️ 9.0/10

Jepsen's analysis of ParticleDB 1.1.4, a database claiming Postgres compatibility, uncovered frequent and profound transactional anomalies including lost committed writes, aborted reads, intermediate reads, and lost updates. The report also found that ParticleDB's claim of being 'formally proven' with a TLA+ proof was unsupported, as no TLA+ specification was available during the collaboration. This finding is significant because it reveals that a database marketed for AI agents and Postgres compatibility can lose data and violate basic consistency guarantees, potentially affecting any user relying on it for production workloads. Jepsen recommends users halt deployment immediately and migrate to more reliable databases, highlighting the risks of inadequate testing and false claims in database development. Jepsen documented 96 issues in ParticleDB, ranging from crashes and deadlocks to bizarre behaviors like partially-invisible rows that could not be deleted, WHERE 4 = 5 evaluating true, dropped tables re-emerging in distorted forms, and strings turning into integers. In versions 1.1.18.11.rc-7 through 1.1.18.11.rc-19, many queries using the Postgres interface threw 'Bad value for type long' errors, rendering the database largely unusable.

hackernews · aphyr · Oct 31, 13:39 · [Discussion](https://news.ycombinator.com/item?id=50316100)

**Background**: Jepsen is a well-known independent organization that performs rigorous safety and consistency testing of distributed systems, particularly databases, by simulating network partitions, process pauses, and other failures. Transactional anomalies such as G1a (Aborted Read), G1b (Intermediate Read), and P4 (Lost Update) are violations of isolation guarantees that can lead to data corruption and application errors. TLA+ is a formal specification language used to mathematically verify system properties, and claiming a TLA+ proof implies a high level of assurance.

<details><summary>References</summary>
<ul>
<li><a href="https://jepsen.io/analyses/particledb-1.1.4">Jepsen: ParticleDB 1.1.4</a></li>
<li><a href="https://news.ycombinator.com/item?id=50316100">Jepsen: ParticleDB 1.1.4 | Hacker News</a></li>
<li><a href="https://particledb.ai/">ParticleDB | The database for AI agents</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion was highly engaged, with commenters expressing shock at the severity of the findings and criticizing the database for being 'vibecoded'—developed without rigorous engineering. One commenter noted the dichotomy between software that is correct by construction and software that is incorrect by construction and relies on workarounds, while another highlighted the absurdity of issues like 'WHERE 4 = 5' and strings turning into integers.

**Tags**: `#databases`, `#distributed-systems`, `#formal-verification`, `#Jepsen`, `#transactional-consistency`

---

<a id="item-2"></a>
## [HackerTube: A YouTube-style Interface Built from Hacker News Video Recommendations](https://karpathy.bearblog.dev/hacker-tube/) ⭐️ 8.0/10

Andrej Karpathy launched HackerTube, a YouTube-style web interface that aggregates 6,454 videos recommended in Hacker News comments since 2007, sourced from 39,834 comments. The site is open source, and users are encouraged to fork and reuse the entire codebase, including a DATA.md file designed for AI agents to customize the experience. This project demonstrates an alternative to engagement-optimized algorithmic feeds, offering a curated, non-addictive browsing experience that prioritizes intellectual curiosity over clickbait. It sparks discussion about how social platforms could be redesigned to serve users' interests rather than maximizing time-on-site. The dataset covers videos recommended from 2007 to present, and the site includes an about page with instructions for forking and customizing via AI agents. Community feedback suggests adding a new-to-old sort option, which is noted as easy to implement.

hackernews · karpathy · Oct 31, 19:56 · [Discussion](https://news.ycombinator.com/item?id=50319510)

**Background**: Hacker News is a social news website run by Y Combinator, focused on computer science and entrepreneurship, where users submit and discuss links. Algorithmic feeds on platforms like YouTube are designed to maximize engagement, often leading to addictive behavior and clickbait. HackerTube leverages the community's curated recommendations to create a more intentional viewing experience.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hacker_News">Hacker News</a></li>
<li><a href="https://invidious.io/">Invidious - An open source alternative front-end to YouTube</a></li>

</ul>
</details>

**Discussion**: Commenters praised the refreshing, non-addictive browsing experience and the pure 'nerd content' free of influencer clickbait. Some expressed a desire for continuous updates and a new-to-old sort, while one noted that curated feeds often fail to satisfy their desire for expanding horizons and discovering unexpected perspectives.

**Tags**: `#Hacker News`, `#content curation`, `#YouTube alternative`, `#open source`, `#recommendation systems`

---

<a id="item-3"></a>
## [Critical Linux TCP Use-After-Free Vulnerability CVE-2026-98432 (CVSS 9.8)](https://atlasum.net/blog/cve-2026-98432-linux-ipv4-tcp-uaf) ⭐️ 8.0/10

A critical use-after-free vulnerability, CVE-2026-98432, has been discovered in the Linux kernel's IPv4 TCP handshake path, with a CVSS score of 9.8. The flaw arises when two processors act on related request and child sockets while both can still reference the same IP options object, and it was fixed upstream on October 15, 2026. This vulnerability affects a core networking component of Linux, potentially allowing remote code execution or denial of service, and impacts a vast number of servers and devices running Linux. However, exploitability over the internet is considered unlikely due to common router configurations that drop packets with IP options. Exploitation requires multiple CPU cores to process packets, so single-core systems or those with packet processing pinned to a single core are not affected. Dropping packets with IP options helps but is not a full mitigation according to Red Hat, and MPTCP is not a requirement for exploitation.

hackernews · oger · Oct 31, 19:16 · [Discussion](https://news.ycombinator.com/item?id=50319143)

**Background**: A use-after-free vulnerability occurs when a program continues to use a pointer after it has been freed, potentially allowing an attacker to execute arbitrary code or cause a crash. CVSS is a standardized severity score where 9.8 indicates critical severity, often remotely exploitable with no authentication. Linux's TCP/IP stack is fundamental to network communication, making vulnerabilities in this area particularly concerning.

<details><summary>References</summary>
<ul>
<li><a href="https://atlasum.net/blog/cve-2026-98432-linux-ipv4-tcp-uaf">Linux 's October 2026 TCP Use-After-Free: CVE - 2026 - 98432 — Atlas</a></li>
<li><a href="https://www.penligent.ai/hackinglabs/cve-2026-98432/">CVE - 2026 - 98432 Linux TCP Flaw, Ubuntu Patch and Mitigation Status</a></li>
<li><a href="https://getrff.com/blog/cve-2026-98432-linux-tcp-ip-options-block/">CVE - 2026 - 98432 : how to block the Linux TCP bug until Ubuntu and...</a></li>

</ul>
</details>

**Discussion**: Commenters clarified that this is a Linux-specific vulnerability, not affecting BSD, Mac, or Windows. They noted that exploitability over the internet is unlikely due to ISP routers dropping IP options packets, and that multi-core systems are required for exploitation. Some expressed frustration that major distributions like Ubuntu and RHEL had not yet patched, while others asked about the exact impact (RCE vs. DoS) and shared tips for monitoring CVEs.

**Tags**: `#security`, `#linux`, `#vulnerability`, `#tcp`, `#cve`

---

<a id="item-4"></a>
## [Researchers exploit ChatGPT account takeover via preview and JSONP flaw](https://www.parameter.ai/labs/we-found-a-gap-at-openai) ⭐️ 8.0/10

Parameter Labs discovered a vulnerability chain that allowed them to take over ChatGPT accounts by manipulating preview content and exploiting a JSONP endpoint. OpenAI confirmed both frontends rejected the reported messages, fixed the issue, and awarded a $5,000 bug bounty. This account takeover vulnerability highlights ongoing security challenges in AI chat platforms that handle rich content, potentially exposing user data and conversations. The disclosure and subsequent fix underscore the importance of bug bounty programs in securing widely used AI services. The exploit required the user to click a link, and OpenAI stated that both frontends rejected the reported messages, indicating some defensive layers were effective. The $5,000 bounty was considered low by some community members given the severity of the vulnerability.

hackernews · armcat · Oct 31, 10:30 · [Discussion](https://news.ycombinator.com/item?id=50314699)

**Background**: JSONP (JSON with Padding) is a technique for cross-origin data exchange that can be vulnerable to injection attacks if not properly secured, allowing attackers to steal sensitive data. OpenAI's bug bounty program rewards security researchers for responsibly disclosing vulnerabilities in its systems, including ChatGPT, APIs, and plugins.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/bug-bounty-program/">Announcing OpenAI ’s Bug Bounty Program | OpenAI</a></li>
<li><a href="https://www.cyberglossary.org/en/term/jsonp-vulnerability">What is JSONP Vulnerability ? Meaning, definition & examples</a></li>
<li><a href="https://securitycafe.ro/2017/01/18/practical-jsonp-injection/">Practical JSONP Injection – Security Café</a></li>

</ul>
</details>

**Discussion**: Commenters criticized the $5,000 bounty as too low, arguing it may discourage researchers from reporting serious flaws. Some also found the write-up confusing, particularly the explanation of how JSONP was bypassed, and noted related remote file system access issues in the ChatGPT desktop app.

**Tags**: `#security`, `#ChatGPT`, `#OpenAI`, `#vulnerability disclosure`, `#web security`

---

<a id="item-5"></a>
## [Blog Post Argues Memory Latency, Not Bandwidth, Is the Real Bottleneck](https://pivotlake.io/blog/its-the-memory-latency-stupid/) ⭐️ 7.0/10

A technical blog post titled 'It's the memory latency, stupid' explains that memory latency, not just bandwidth, is a critical performance bottleneck, and illustrates this with practical analysis and optimization approaches. The post gained traction on Hacker News with 109 upvotes and 34 comments. This matters because many developers focus on bandwidth when optimizing memory performance, but latency often dominates in real-world workloads, especially in systems with deep cache hierarchies and out-of-order execution. Understanding this distinction can lead to more effective optimizations and better system design. The article likely discusses how memory latency affects performance through cache misses and how techniques like prefetching, data locality optimization, and reducing pointer chasing can mitigate it. Community comments mention specific examples such as custom containers with inline allocation and object pools using index+generations to improve locality on embedded systems.

hackernews · ntur1337 · Oct 31, 18:38 · [Discussion](https://news.ycombinator.com/item?id=50318720)

**Background**: Memory latency is the time it takes for a CPU to access data from main memory, typically 60-100 nanoseconds, while bandwidth is the rate at which data can be transferred. Modern CPUs use caches to hide latency, but cache misses still stall execution. The article builds on classic performance analysis concepts, and commenters reference the well-known paper 'CPU Memory' by Stewart.

<details><summary>References</summary>
<ul>
<li><a href="https://pc-bottleneck.com/ram-speed-vs-latency/">RAM Speed vs Latency: Which Impacts Performance More?</a></li>
<li><a href="https://www.digitalcitizen.life/memory-latency-vs-bandwidth-how-they-affect-real-world-system-performance/">Memory Latency vs Bandwidth: How They Affect Real-World ...</a></li>

</ul>
</details>

**Discussion**: Commenters shared real-world anecdotes: one described optimizing an embedded system by using custom containers and object pools to improve locality, while another suggested using LLM agents to check assembly and PMUs. A critic argued the proposed solution is essentially a clustered hashmap and not orders of magnitude better, and another asked for an updated version of a classic memory latency paper.

**Tags**: `#memory-latency`, `#performance-optimization`, `#systems-programming`, `#cache`, `#profiling`

---

<a id="item-6"></a>
## [Molly Signal fork unmaintained for 3 months, contains vulnerabilities](https://piefed.world/post/1503394) ⭐️ 7.0/10

Molly, a popular independent Signal fork for Android, has not received updates for three months and is now vulnerable to known security issues. The community discussion highlights that the fork is lagging behind official Signal fixes, prompting users to seek alternatives or switch back to the official app. Molly users may be exposed to unpatched vulnerabilities, undermining the security guarantees that motivated them to use a privacy-focused fork. This raises broader questions about the sustainability and security trade-offs of third-party Signal clients. Molly previously distinguished itself with features like a passphrase-encrypted database and fully FOSS builds without proprietary blobs, and it typically updated every two weeks to track Signal. The current gap means missing fixes such as RingRTC call-teardown patches and Signal's blacklist of compromised eMudhra TLS intermediates.

hackernews · DeepLogin · Oct 31, 10:23 · [Discussion](https://news.ycombinator.com/item?id=50314666)

**Background**: Signal is a widely used end-to-end encrypted messaging app, and its source code is open, allowing developers to create forks like Molly that add features or remove proprietary components. Forks must independently merge upstream security patches, so any delay in maintenance can leave users exposed to known vulnerabilities. Molly has been popular among privacy enthusiasts for offering a fully FOSS alternative to the official Signal Android client.

<details><summary>References</summary>
<ul>
<li><a href="https://molly.im/">Molly is an improved Signal app for Android</a></li>
<li><a href="https://github.com/mollyim/mollyim-android">mollyim/mollyim-android: Enhanced and security-focused fork of Signal .</a></li>
<li><a href="https://signal.org/">Signal >> Home</a></li>

</ul>
</details>

**Discussion**: Commenters noted that official Signal now supports linking multiple devices to one account, removing a key reason to use Molly, and clarified that the official Signal APK self-updates. One user released a stopgap fork called Polly with recent fixes, while others debated Signal's pragmatic stance against third-party clients and its slow adoption of features like UnifiedPush.

**Tags**: `#Signal`, `#security`, `#privacy`, `#open-source`, `#Android`

---

<a id="item-7"></a>
## [Anthropic Blocks Users for Training Larger Models, Sparking Debate](https://twitter.com/jiahaoshao1/status/2116475922190922088) ⭐️ 7.0/10

A Hacker News discussion highlights reports that Anthropic has blocked users whose activity touches on training larger models, with commenters sharing anecdotes of account bans and inconsistent refusal behavior from Claude. This incident underscores growing concerns about AI provider policies and user trust, as professionals increasingly rely on LLM APIs and may face sudden account restrictions; it also fuels calls for a more open, standardized, and portable ecosystem of AI models. The user involved is reportedly based in Hong Kong, where Claude is geo-blocked, and likely accessed the service via VPN, which combined with model training work may have triggered Anthropic's classifiers; commenters also note inconsistent refusals, such as Claude declining to extract code or start a browser testing session for moral or policy reasons.

hackernews · pretext · Oct 31, 19:39 · [Discussion](https://news.ycombinator.com/item?id=50319358)

**Background**: Anthropic maintains a Usage Policy that prohibits certain activities, including using its models to train competing larger models. The company has updated its policy annually, with the 2026 version introducing new rules and a narrow ban on abusing Claude. Account bans can be triggered by automated classifiers detecting suspicious behavior, such as training-related queries over VPNs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/2026-usage-policy-update">2026 Usage Policy update \ Anthropic</a></li>
<li><a href="https://cellcog.ai/blog/anthropic-usage-policy-2026/">Anthropic Usage Policy 2026: Nov 12 Rules and Abuse Ban</a></li>

</ul>
</details>

**Discussion**: Commenters express frustration with Anthropic's opinionated and dogmatic approach, with some urging professionals to cultivate alternatives and push for ecosystem portability. Others share specific instances of Claude's inconsistent refusals, such as declining to extract code or start a browser session, while one commenter notes the Hong Kong geo-block and VPN use as a likely trigger for the ban.

**Tags**: `#AI policy`, `#Anthropic`, `#LLM providers`, `#account bans`, `#Hacker News discussion`

---

<a id="item-8"></a>
## [Reddit user asks for cross-modal ML technique taxonomy](https://www.reddit.com/r/MachineLearning/comments/1xkp8e9/are_there_fundamental_repeating_patterns_in_ml/) ⭐️ 6.0/10

A Reddit user on r/MachineLearning posted a discussion question asking whether there is an existing taxonomy or mental model that groups machine learning techniques by their underlying patterns—such as tokenization, masking, diffusion, and next-token prediction—rather than by modality like text, image, or audio. If such a taxonomy exists or could be developed, it would help researchers organize papers across subfields and transfer techniques more efficiently, potentially accelerating cross-pollination between NLP, vision, and audio research. The user specifically points to examples like tokenization, masked language modeling (MLM), masked autoencoders (MAE), audio masking, diffusion models, and next-token/next-frame prediction as instances of repeating patterns across modalities, and seeks a way to group research papers accordingly.

reddit · r/MachineLearning · /u/OkCampaign8400 · Nov 1, 00:07

**Background**: Masked language modeling (MLM) is a pretraining technique in NLP where parts of a text are masked and the model learns to predict the missing tokens, as used in BERT. Masked autoencoders (MAE) apply a similar idea to images by masking random patches and reconstructing missing pixels, showing a clear cross-modal pattern. Diffusion models, which learn to reverse a noise-adding process, have been successfully applied to image, audio, and even text generation, further illustrating how a single paradigm can span modalities.

<details><summary>References</summary>
<ul>
<li><a href="https://mbrenndoerfer.com/writing/masked-language-modeling-bidirectional-understanding-bert">Masked Language Modeling - Interactive</a></li>
<li><a href="https://arxiv.org/abs/2111.06377">[2111.06377] Masked Autoencoders Are Scalable Vision Learners</a></li>
<li><a href="https://en.wikipedia.org/wiki/Diffusion_model_(machine_learning)">Diffusion model (machine learning)</a></li>

</ul>
</details>

**Tags**: `#machine-learning`, `#taxonomy`, `#cross-modal`, `#research-patterns`, `#discussion`

---

<a id="item-9"></a>
## [Two-stage deep learning framework detects neonatal brain pathologies from MRI](https://www.reddit.com/r/MachineLearning/comments/1xkcy83/hierarchical_detection_of_neonatal_brain/) ⭐️ 6.0/10

A research paper shared on r/MachineLearning presents a hierarchical two-stage deep learning pipeline that emulates clinical reasoning to detect neonatal brain pathologies from paired T1-weighted and T2-weighted MRI scans. Automated detection could support earlier diagnosis of neonatal brain injuries, where timely intervention is critical, and the hierarchical design may help disentangle confounding effects of preterm birth from true pathology. The framework uses a two-stage hierarchical classification approach on paired T1- and T2-weighted neonatal MRI, but the Reddit post is a bare link with no substantive discussion, so details on dataset size, accuracy, and clinical validation remain unverified from the post alone.

reddit · r/MachineLearning · /u/rottoneuro · Oct 31, 15:21

**Background**: Neonatal brain pathologies such as hypoxic-ischemic encephalopathy are a leading cause of mortality and disability, and MRI is key for early detection. However, preterm birth produces imaging patterns that can confound automated diagnosis, motivating hierarchical or two-stage models that first separate broad categories before fine-grained classification.

<details><summary>References</summary>
<ul>
<li><a href="https://www.frontiersin.org/journals/neuroimaging/articles/10.3389/fnimg.2026.1981436/full">Frontiers | Hierarchical detection of neonatal brain pathologies using...</a></li>
<li><a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=7371651">Hierarchical Detection of Neonatal Brain Pathologies Using... :: SSRN</a></li>
<li><a href="https://jbiochemtech.com/article/diagnosis-of-neonatal-brain-pathologies-analysis-of-the-effectiveness-of-deep-learning-algorithms-a-bhr8s3fkrhe8xbm?html">Diagnosis of Neonatal Brain Pathologies : Analysis of the...</a></li>

</ul>
</details>

**Tags**: `#deep-learning`, `#medical-imaging`, `#MRI`, `#neonatal-health`, `#research-paper`

---

<a id="item-10"></a>
## [Gear: An Open-Source scikit-learn for Recursive Self-Improvement](https://www.reddit.com/r/MachineLearning/comments/1xkeq7d/i_built_a_scikitlearn_for_rsi_p/) ⭐️ 6.0/10

The author released Gear, an open-source meta-learning framework that separates search, execution, and evaluation to make RSI methods like GEPA, RRSI, and Harness² easier to implement and compare. A working GEPA variant with shared failure diagnosis and staged evaluation improved pass rates on AutomationBench Marketing (27.0% to 40.0%), AutomationBench Support (17.0% to 25.0%), and Terminal-Bench 2.1 (52.8% to 62.9%) using GPT 5.6 Luna at medium reasoning effort. This framework could standardize how recursive self-improvement and meta-learning approaches are built and benchmarked, similar to how scikit-learn standardized classical machine learning. It may benefit researchers and engineers working on agent optimization, prompt evolution, and automated AI research by providing a common abstraction for comparing methods. At max effort on Marketing, Luna with the optimized harness reached 88.88% objective completion versus 84.08% for Astra + Codex, though strict task pass rates were 53% versus 57%, indicating the advantage was in partial completion. With the same optimized harness at max effort, Luna's estimated API cost averaged $0.0568 per task versus $1.1858 for Astra, a 95.21% reduction excluding optimization and infrastructure costs.

reddit · r/MachineLearning · /u/Pale-Training-6944 · Oct 31, 16:33

**Background**: Recursive self-improvement (RSI) refers to an AI system iteratively designing more capable successors, and recent work applies it to improving prompts, tools, and agent workflows. GEPA is a genetic-Pareto prompt optimization algorithm that uses iterative reflection, mutation, and Pareto-aware selection to evolve high-performing variants with minimal evaluations. Gear aims to provide a unified framework for such methods, separating the search for promising changes from execution and evaluation to address sampling, evaluation, and diversity challenges familiar from reinforcement learning and evolutionary search.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Recursive_self-improvement">Recursive self-improvement - Wikipedia</a></li>
<li><a href="https://github.com/gepa-ai/gepa">GitHub - gepa-ai/gepa: Optimize prompts, code, and more with ...</a></li>
<li><a href="https://arxiv.org/abs/2507.19457">GEPA: Reflective Prompt Evolution Can Outperform ...</a></li>

</ul>
</details>

**Tags**: `#meta-learning`, `#reinforcement-learning`, `#agent-optimization`, `#open-source`, `#benchmarking`

---

<a id="item-11"></a>
## [Reddit User Asks: Is Neuro-Evolution Relevant in Industry or Research?](https://www.reddit.com/r/MachineLearning/comments/1xkh5bw/is_neuroevolution_relevant_d/) ⭐️ 5.0/10

A Reddit user on r/MachineLearning shared their experiments using neuro-evolution to train AI to play various games and asked whether the technique is actually used in industry or research, and whether it relates to reinforcement learning. This question reflects a common uncertainty among practitioners about the practical relevance of neuro-evolution, a niche but historically significant approach that has influenced reinforcement learning and continues to appear in areas like game AI and evolutionary robotics. Neuro-evolution uses evolutionary algorithms to optimize neural network weights and topologies, and is particularly suited to sequential decision tasks with large or continuous state and action spaces, as well as partially observable environments (POMDPs).

reddit · r/MachineLearning · /u/tapopalis · Oct 31, 18:09

**Background**: Neuro-evolution is a form of artificial intelligence that applies evolutionary algorithms to generate artificial neural networks, their parameters, and rules. It is most commonly used in artificial life, general game playing, and evolutionary robotics, and has been shown to be a strong alternative to classic reinforcement learning methods in some benchmarks. A well-known algorithm in this space is NEAT (NeuroEvolution of Augmenting Topologies), which evolves both the weights and structures of networks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Neuroevolution">Neuroevolution - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Neuroevolution_of_augmenting_topologies">Neuroevolution of augmenting topologies</a></li>
<li><a href="https://nn.cs.utexas.edu/?neuroevolution">NNRG Areas - Neuroevolution</a></li>

</ul>
</details>

**Tags**: `#neuro-evolution`, `#reinforcement-learning`, `#machine-learning`, `#research`, `#industry`

---

<a id="item-12"></a>
## [datasette-llm 0.1a9 auto-detects LLM default model](https://simonwillison.net/2026/Oct/31/datasette-llm/) ⭐️ 4.0/10

datasette-llm 0.1a9 now automatically picks up the default model configured in Simon Willison's LLM CLI tool, so users can start Datasette Agent without explicitly setting a default model. Previously, running Datasette Agent required an extra flag such as `-s plugins.datasette-agent.default_model gpt-6-astra`. This small UX improvement lowers the setup friction for Datasette Agent, an AI assistant that writes and runs SQL queries against Datasette-hosted data. It makes the Datasette and LLM toolchain feel more cohesive for developers who already use LLM as their model interface. The release is an alpha version (0.1a9) of a niche plugin, and the change only affects default model resolution; users who want a specific non-default model can still configure it explicitly. The example command `uvx --with datasette-agent datasette content.db --internal internal.db` now works without the model flag.

rss · Simon Willison · Oct 31, 22:10

**Background**: Datasette is a tool for exploring and publishing data, often backed by SQLite. Datasette Agent is an AI assistant built on Datasette that can answer questions by writing and executing SQL queries. LLM is a CLI tool and Python library for interacting with many large language models, and datasette-llm is a plugin that provides a standard interface for Datasette plugins to use LLM models, including model management and API key handling.

<details><summary>References</summary>
<ul>
<li><a href="https://agent.datasette.io/">Datasette Agent : an AI assistant for Datasette to help explore and...</a></li>
<li><a href="https://github.com/simonw/llm">GitHub - simonw/llm: Access large language models from the ...</a></li>
<li><a href="https://github.com/datasette/datasette-llm">GitHub - datasette/datasette-llm: LLM integration plugin for ...</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#llm`, `#datasette-agent`, `#release`, `#developer-tools`

---

<a id="item-13"></a>
## [Reddit user asks if sharing from-scratch LLM experiments is welcome](https://www.reddit.com/r/MachineLearning/comments/1xkgtly/is_it_okay_to_share_my_experiments_implementing/) ⭐️ 3.0/10

A Reddit user has built and trained an ~8M parameter LLM from scratch in PyTorch and is asking whether sharing their blog series documenting the process—covering transformer building, 60,000 training steps, and upcoming KV caching and PagedAttention implementations—would be welcome in r/MachineLearning. This post reflects a growing trend of practitioners building small LLMs from scratch as educational labs, and if shared, such detailed experiment logs could provide valuable learning material for others in the community. The user's LLM is only ~8M parameters, making it feasible to train on modest hardware, and the planned implementations of KV caching and PagedAttention are key inference optimization techniques often used in production LLM serving.

reddit · r/MachineLearning · /u/the-random-guy-2002 · Oct 31, 17:57

**Background**: KV caching stores previously computed key and value tensors during autoregressive generation to avoid redundant computation, significantly speeding up inference. PagedAttention, introduced in 2023, manages KV cache memory in non-contiguous blocks inspired by OS virtual memory, reducing memory waste and enabling efficient serving of large language models. Orca is a family of techniques for efficient LLM serving, including continuous batching and iteration-level scheduling.

<details><summary>References</summary>
<ul>
<li><a href="https://martinlwx.github.io/en/llm-inference-optimization-kv-cache/">LLM inference optimization (1): KV Cache - MartinLwx's Blog</a></li>
<li><a href="https://en.wikipedia.org/wiki/PagedAttention">PagedAttention</a></li>
<li><a href="https://sapling.ai/llm/orca">The LLM Index: Orca | Sapling</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#research-implementation`, `#community-guidelines`, `#PyTorch`, `#meta-post`

---