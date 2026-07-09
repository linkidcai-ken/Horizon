---
layout: default
title: "Horizon Summary: 2026-07-09 (EN)"
date: 2026-07-09
lang: en
---

> From 21 items, 18 important content pieces were selected

---

1. [OpenAI Releases GPT-5.6 with Three Sizes](#item-1) ⭐️ 9.0/10
2. [EU Parliament Passes Chat Control 1.0 Mass Scanning](#item-2) ⭐️ 9.0/10
3. [Bun Rewritten from Zig to Rust](#item-3) ⭐️ 9.0/10
4. [Postgres rewritten in Rust passes all regression tests](#item-4) ⭐️ 8.0/10
5. [Meta Launches Muse Spark 1.1 with Paid API](#item-5) ⭐️ 8.0/10
6. [OpenAI Launches GPT-Live Voice Mode with GPT-5.5 Delegation](#item-6) ⭐️ 8.0/10
7. [Running GLM 5.2 on a 32GB RAM Laptop](#item-7) ⭐️ 7.0/10
8. [Tencent's Hy3: Small Model Rivals DeepSeek Flash V4](#item-8) ⭐️ 7.0/10
9. [No Leap Second at End of 2026](#item-9) ⭐️ 7.0/10
10. [U.S. Army logistics fragile in next war](#item-10) ⭐️ 7.0/10
11. [TLS Certificates for Internal Services Done Right](#item-11) ⭐️ 7.0/10
12. [IMGNet: Face Verification via Sign Patterns, Not Cosine](#item-12) ⭐️ 7.0/10
13. [Damn Interesting launches funding drive to sustain site](#item-13) ⭐️ 6.0/10
14. [LLM-Meta-AI 0.1 Plugin Released for Muse-Spark-1.1](#item-14) ⭐️ 6.0/10
15. [Why Conferences Outshine Journals in ML Research](#item-15) ⭐️ 6.0/10
16. [Talos-XII: Hand-written autograd and RL in Rust for gacha simulation](#item-16) ⭐️ 6.0/10
17. [Show HN: 18 Words – A Timed Word Game](#item-17) ⭐️ 5.0/10
18. [llm 0.31.1 Fixes JSON Error with Empty Tool Call Arguments](#item-18) ⭐️ 3.0/10

---

<a id="item-1"></a>
## [OpenAI Releases GPT-5.6 with Three Sizes](https://openai.com/index/gpt-5-6/) ⭐️ 9.0/10

OpenAI released GPT-5.6, a new frontier model available in three sizes: Luna, Terra, and Sol, achieving state-of-the-art results on the ARC-AGI-3 benchmark with Sol scoring 7.8%. GPT-5.6 sets a new SOTA on ARC-AGI-3, a benchmark designed to measure human-like agentic intelligence, marking a significant step toward more capable AI agents. Its improved intent understanding and image handling also enhance practical usability for developers. The three models have knowledge cutoff of February 16, 2026, and are priced per million tokens: Luna $1/$6, Terra $2.50/$15, Sol $5/$30. GPT-5.6 Sol is the first verified frontier model to beat an ARC-AGI-3 game.

hackernews · logickkk1 · Jul 9, 17:04 · [Discussion](https://news.ycombinator.com/item?id=48849066)

**Background**: Frontier AI models are the most advanced general-purpose models at a given time, capable of reasoning, multimodal generation, and agentic workflows. ARC-AGI-3 is an interactive reasoning benchmark that challenges AI agents to explore novel environments, infer goals, and plan actions, measuring progress toward artificial general intelligence.

<details><summary>References</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>
<li><a href="https://arxiv.org/abs/2603.24621">[2603.24621] ARC-AGI-3: A New Challenge for Frontier Agentic Intelligence</a></li>

</ul>
</details>

**Discussion**: Comments highlight that GPT-5.6 Sol achieves SOTA on ARC-AGI-3, with some users noting that OpenAI excluded Fable 5 from comparisons because it refused most biology questions. There is also discussion comparing GPT-5.6 with Claude Code for coding tasks, and mixed sentiment about OpenAI's openness versus Anthropic's closed approach.

**Tags**: `#AI`, `#OpenAI`, `#GPT-5.6`, `#LLM`, `#ARC-AGI`

---

<a id="item-2"></a>
## [EU Parliament Passes Chat Control 1.0 Mass Scanning](https://www.patrick-breyer.de/en/eu-parliament-greenlights-chat-control-1-0-breyer-our-children-lose-out/) ⭐️ 9.0/10

The European Parliament has passed Chat Control 1.0, allowing voluntary mass scanning of private messages on platforms like Gmail, Snapchat, and Skype until April 2028, despite a majority of voting MEPs opposing it. The rejection motion failed to reach the required absolute majority of 361 votes. This legislation significantly expands warrantless surveillance of private communications for 450 million EU citizens, raising serious privacy and encryption concerns. The procedural maneuver used to pass it undermines democratic legitimacy and could set a precedent for future mass surveillance laws. Chat Control 1.0 applies only to services without end-to-end encryption or where platforms can access messages server-side; end-to-end encrypted services remain unaffected. The law is voluntary for companies, but critics argue it normalizes mass scanning and could lead to mandatory requirements later.

hackernews · rapnie · Jul 9, 11:03 · [Discussion](https://news.ycombinator.com/item?id=48843923)

**Background**: Chat Control refers to EU proposals to combat child sexual abuse material (CSAM) by scanning private messages. Chat Control 1.0, initially agreed in 2021, allows voluntary scanning by US tech companies. A more controversial Chat Control 2.0, which would mandate scanning of encrypted messages, is still under debate.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control">Chat Control - Wikipedia</a></li>
<li><a href="https://www.patrick-breyer.de/en/posts/chat-control/">Chat Control: The EU's CSAM scanner proposal</a></li>
<li><a href="https://www.techtimes.com/articles/320010/20260709/eu-parliament-passes-chat-control-default-314-meps-couldnt-block-scanning-law.htm">EU Parliament Passes Chat Control by Default: 314 MEPs Couldn't Block Scanning Law</a></li>

</ul>
</details>

**Discussion**: Commenters expressed outrage at the procedural trick used to pass the law, noting that the vote was held just before summer break with many MEPs absent, and required an absolute majority to reject. They see this as a democratic failure and a step toward totalitarian governance, with some calling it a 'blame-laundering mechanism' for unpopular laws.

**Tags**: `#privacy`, `#EU legislation`, `#surveillance`, `#encryption`, `#digital rights`

---

<a id="item-3"></a>
## [Bun Rewritten from Zig to Rust](https://simonwillison.net/2026/Jul/8/rewriting-bun-in-rust/#atom-everything) ⭐️ 9.0/10

Jarred Sumner announced the complete rewrite of the Bun JavaScript runtime from Zig to Rust, driven by memory safety concerns and a desire to reduce bugs. The rewrite was accomplished in 11 days using AI coding agents, with an estimated cost of $165,000 in API tokens. This rewrite demonstrates that large-scale software rewrites, once considered too risky, are now feasible with AI assistance. It also highlights Rust's growing dominance in systems programming due to its memory safety guarantees, potentially influencing future runtime development. The Bun test suite, written in TypeScript, served as a conformance suite to validate the Rust port. The new Rust-based Bun has been live in Claude Code since June 17, 2026, with 10% faster startup on Linux and no noticeable regressions.

rss · Simon Willison · Jul 8, 23:57

**Background**: Bun is a JavaScript runtime, package manager, and test runner designed as a drop-in replacement for Node.js, originally written in Zig. Zig is a system programming language that requires manual memory management, which led to bugs like use-after-free and double-free. Rust, in contrast, enforces memory safety at compile time through its ownership system and RAII (Resource Acquisition Is Initialization), eliminating entire classes of memory bugs.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bun_(software)">Bun (software) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Memory_safety">Memory safety - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Bun`, `#Rust`, `#Zig`, `#runtime`, `#software engineering`

---

<a id="item-4"></a>
## [Postgres rewritten in Rust passes all regression tests](https://github.com/malisper/pgrust) ⭐️ 8.0/10

A project called pgrust has rewritten PostgreSQL in Rust using LLMs, and it now passes 100% of the PostgreSQL regression tests. This demonstrates the potential of LLMs to assist in large-scale code rewrites, but also raises concerns about code review, license compatibility, and trust in AI-generated code. The project generated 7101 commits in less than a month, making traditional commit-history review infeasible. The license was changed from the PostgreSQL license to AGPL, sparking debate about compatibility.

hackernews · SweetSoftPillow · Jul 9, 06:18 · [Discussion](https://news.ycombinator.com/item?id=48841676)

**Background**: PostgreSQL is a 30-year-old relational database with a comprehensive regression test suite covering SQL operations and extended capabilities. The pgrust project aims to build a better version by leveraging modern techniques and Rust's safety guarantees.

<details><summary>References</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/regress.html">PostgreSQL: Documentation: 18: Chapter 31. Regression Tests</a></li>
<li><a href="https://medium.com/@haseeb_sohail/how-i-evaluate-llm-code-quality-reviewing-ai-generated-code-at-scale-db8c4f150107">How I Evaluate LLM Code Quality: Reviewing AI-Generated Code at Scale | by Muhammad Haseeb Sohail | Medium</a></li>
<li><a href="https://www.qt.io/software-insights/are-llms-better-than-humans">Code Quality: Are LLMs Better Than Humans?</a></li>

</ul>
</details>

**Discussion**: The author explained the project's goal of using LLMs to rearchitect Postgres. Commenters questioned how to review AI-generated code, expressed distrust in AI rewrites, and raised license compatibility concerns between the original PostgreSQL license and AGPL.

**Tags**: `#Postgres`, `#Rust`, `#LLM`, `#database`, `#rewrite`

---

<a id="item-5"></a>
## [Meta Launches Muse Spark 1.1 with Paid API](https://ai.meta.com/blog/introducing-muse-spark-meta-model-api/) ⭐️ 8.0/10

Meta has released Muse Spark 1.1, a multimodal reasoning model designed for agentic tasks, and introduced its first paid API tier for developers, priced at $1.25 per million input tokens and $4.25 per million output tokens. This marks Meta's first commercial AI model offering, directly competing with OpenAI and Anthropic at roughly one-quarter of their rates, potentially disrupting the AI pricing landscape and making advanced agentic AI more accessible. Muse Spark 1.1 features a 1M-token context window, major gains in tool use, computer use, coding, and multimodal understanding, and runs in 'Thinking' mode within Meta AI. New users receive $20 in free credits.

hackernews · ot · Jul 9, 14:10 · [Discussion](https://news.ycombinator.com/item?id=48846184)

**Background**: Agentic AI models are designed to autonomously perform tasks using tools, code, and computer interfaces, going beyond simple chat. Meta previously released open-weight models like Llama, but Muse Spark 1.1 is its first paid API, signaling a strategic shift toward monetizing its AI research.

<details><summary>References</summary>
<ul>
<li><a href="https://ai.meta.com/blog/introducing-muse-spark-meta-model-api/">Introducing Muse Spark 1.1</a></li>
<li><a href="https://www.datacamp.com/blog/muse-spark-1-1">Muse Spark 1.1: Meta's Agentic Model and API | DataCamp</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-07-09/meta-starts-charging-for-ai-with-muse-spark-1-1-agentic-model">Meta Starts Charging for AI With Muse Spark 1.1 Agentic Model - Bloomberg</a></li>

</ul>
</details>

**Discussion**: Community members like GodelNumbering criticized the benchmark methodology, noting that resource caps were overridden, which disqualifies results. Simonw shared a practical plugin for LLM, while Tiberium called the pricing 'insane' for being cheap. Jacobgold suggested Meta should continue as a 'spoiler' by releasing open-weight models to commoditize coding models.

**Tags**: `#AI`, `#Meta`, `#agentic model`, `#machine learning`, `#open source`

---

<a id="item-6"></a>
## [OpenAI Launches GPT-Live Voice Mode with GPT-5.5 Delegation](https://simonwillison.net/2026/Jul/8/introducing-gptlive/#atom-everything) ⭐️ 8.0/10

OpenAI has introduced GPT-Live, an upgraded voice mode for ChatGPT that uses a new model capable of delegating complex tasks to GPT-5.5 in the background while maintaining conversation flow. This upgrade significantly improves real-time AI interaction by enabling seamless delegation of complex queries without interrupting the conversation, making voice mode more useful for brainstorming and multitasking. GPT-Live is available in the iPhone app and can handle tasks like web search and deep reasoning by delegating to GPT-5.5. The previous voice mode was based on an older GPT-4o model with a 2024 knowledge cutoff.

rss · Simon Willison · Jul 8, 23:20

**Background**: GPT-5.5, codenamed 'Spud', is a large language model released by OpenAI in April 2026. It achieved notable benchmark scores and has been used in various applications, including code security. GPT-Live leverages this model to enhance voice mode capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.5">GPT-5.5</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion highlighted the impressive delegation feature but also noted a bug where the model would interrupt and laugh at user statements, which OpenAI reportedly addressed.

**Tags**: `#OpenAI`, `#GPT-Live`, `#voice mode`, `#AI`, `#ChatGPT`

---

<a id="item-7"></a>
## [Running GLM 5.2 on a 32GB RAM Laptop](https://github.com/JustVugg/colibri) ⭐️ 7.0/10

A developer created Colibrì, a lightweight inference engine that runs the 744B-parameter GLM 5.2 model on a 32GB RAM laptop using int4 quantization and on-demand expert streaming from disk, achieving 0.1 tokens per second. This demonstrates that large Mixture-of-Experts models can be run on consumer hardware without a GPU, making advanced LLMs accessible to more users and enabling local inference with privacy benefits. Colibrì is a single C file (~1300 lines) with no runtime dependencies on Python or BLAS, and it uses an LRU cache for streaming experts from disk. The model activates only ~40B parameters per token, with ~11GB of routed experts changing per token.

hackernews · vforno · Jul 9, 08:05 · [Discussion](https://news.ycombinator.com/item?id=48842459)

**Background**: GLM 5.2 is a large language model with 744 billion parameters using a Mixture-of-Experts architecture, where only a subset of parameters are activated per token. Int4 quantization reduces model size by compressing weights to 4-bit integers, and streaming experts from disk trades speed for memory usage.

**Discussion**: Commenters discussed similar approaches, including mmap-based loading and Medusa heads for speculative decoding, and raised concerns about SSD wear from constant disk streaming. Some noted that 0.1 tok/s is too slow for interactive use but could be useful for batch processing overnight.

**Tags**: `#LLM`, `#optimization`, `#local-inference`, `#GLM`, `#quantization`

---

<a id="item-8"></a>
## [Tencent's Hy3: Small Model Rivals DeepSeek Flash V4](https://hy.tencent.com/research/hy3) ⭐️ 7.0/10

Tencent has released Hy3, a small language model that achieves performance comparable to DeepSeek Flash V4 and even surpasses V4 Pro on some benchmarks, despite its compact size. Hy3's strong performance at a small size makes it a promising candidate for local deployment and cost-effective inference, potentially shifting the landscape of accessible AI models. Hy3 is slightly larger than DeepSeek V4 Flash but reportedly matches or exceeds V4 Pro on certain benchmarks; it is available via OpenRouter with a free tier until July 21st.

hackernews · andai · Jul 9, 15:27 · [Discussion](https://news.ycombinator.com/item?id=48847552)

**Background**: Small language models (SLMs) are designed to run efficiently on consumer hardware, enabling local inference without cloud dependency. Hy3 competes in the same niche as DeepSeek's Flash series, which are optimized for speed and low resource usage.

**Discussion**: Community members note Hy3's surprising capability for its size and discuss its potential for local use, but some question its utility given pricing parity with DeepSeek-hosted Flash V4. There is curiosity about its performance under heavy quantization.

**Tags**: `#AI/ML`, `#language model`, `#Tencent`, `#open-source`, `#model comparison`

---

<a id="item-9"></a>
## [No Leap Second at End of 2026](https://datacenter.iers.org/data/latestVersion/bulletinC.txt) ⭐️ 7.0/10

The International Earth Rotation and Reference Systems Service (IERS) announced that no leap second will be introduced at the end of December 2026, keeping the UTC-TAI offset at -37 seconds and the UTC-GPS offset at -18 seconds. This decision affects time-sensitive systems worldwide, including financial networks, telecommunications, and satellite navigation, which rely on precise UTC offsets. It also continues the ongoing debate about leap seconds' impact on software engineering and the potential shift to a leap-second-free time scale. The announcement confirms that Earth's rotation has not deviated enough to require a leap second adjustment. The next possible leap second insertion could occur in June or December 2027, depending on future observations.

hackernews · ChrisArchitect · Jul 9, 14:16 · [Discussion](https://news.ycombinator.com/item?id=48846281)

**Background**: Leap seconds are occasionally added to Coordinated Universal Time (UTC) to keep it within 0.9 seconds of mean solar time, which is based on Earth's rotation. Earth's rotation is irregular due to tidal friction, geological activity, and weather patterns, making long-term predictions difficult. The last leap second was added on December 31, 2016.

**Discussion**: Community comments expressed curiosity about the unpredictability of Earth's rotation, with users asking about geological and weather influences. There was also discussion about the impact on UNIX timestamps and the constant offsets between TAI, GPS, and UTC. A humorous comment suggested using jet engines to adjust time.

**Tags**: `#leap second`, `#timekeeping`, `#UTC`, `#UNIX timestamps`, `#Earth rotation`

---

<a id="item-10"></a>
## [U.S. Army logistics fragile in next war](https://mwi.westpoint.edu/the-glass-backbone-why-the-armys-logistics-will-break-in-the-next-war/) ⭐️ 7.0/10

An article from Modern War Institute argues that the U.S. Army's logistics are dangerously fragile due to over-reliance on just-in-time supply chains, which would break under the strain of a major conflict. This vulnerability could cripple U.S. military operations in a future high-intensity war, as logistics are the backbone of sustained combat. The article challenges the Army's modernization priorities and calls for a shift toward more resilient supply chains. The article criticizes the outdated 'tooth-to-tail ratio' concept, which undervalues logistics personnel and infrastructure. It warns that just-in-time logistics, effective in peacetime, become a liability in contested environments where supply lines are targeted.

hackernews · baud147258 · Jul 9, 13:24 · [Discussion](https://news.ycombinator.com/item?id=48845442)

**Background**: Military logistics involves the planning and execution of moving and sustaining forces, including supply, transportation, and maintenance. The U.S. Army has long prioritized combat units over support units, a ratio known as 'tooth-to-tail.' Just-in-time logistics minimizes inventory but assumes safe supply lines, which may not hold in a peer conflict.

**Discussion**: Commenters largely agree with the article's thesis, drawing historical parallels to Fabian strategy and noting that adversaries like Iran and Russia understand logistics vulnerabilities. Some argue that new technologies like SpaceX's Starship could bypass traditional logistics, but others counter that such systems are unproven in war.

**Tags**: `#military logistics`, `#infrastructure`, `#systems thinking`, `#strategy`

---

<a id="item-11"></a>
## [TLS Certificates for Internal Services Done Right](https://tuxnet.dev/posts/tls-for-internal-services/) ⭐️ 7.0/10

A new guide on managing TLS certificates for internal services has sparked debate, with experts advocating for ACME DNS-01 challenges over split-horizon DNS to reduce complexity and long-term maintenance. This matters because many organizations struggle with certificate management for internal services, and the debate highlights practical trade-offs between security, simplicity, and operational overhead that affect real-world deployments. The guide recommends avoiding split-horizon DNS and instead using DNS-01 challenges with Let's Encrypt, which allows internal services to obtain publicly trusted certificates without exposing internal hostnames or requiring complex DNS mirroring.

hackernews · mrl5 · Jul 9, 14:57 · [Discussion](https://news.ycombinator.com/item?id=48846995)

**Background**: Split-horizon DNS provides different DNS responses based on the requester's network, often used to give internal IPs for internal users and public IPs for external users. However, maintaining two sets of DNS records can become tedious. ACME DNS-01 challenges allow certificate issuance by proving control over a domain's DNS records, enabling internal services to use public certificates without split DNS.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Split-horizon_DNS">Split-horizon DNS</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree that split-horizon DNS is a headache and prefer DNS-01 challenges with Let's Encrypt, though some note that self-signed certificates would be easier if OS trust stores were universally respected. Others use public zones with internal IPs and VPNs to avoid leakage concerns.

**Tags**: `#TLS`, `#certificates`, `#internal services`, `#DNS`, `#ACME`

---

<a id="item-12"></a>
## [IMGNet: Face Verification via Sign Patterns, Not Cosine](https://www.reddit.com/r/MachineLearning/comments/1urxvxh/i_built_imgnet_a_face_verification_model_that/) ⭐️ 7.0/10

IMGNet introduces a face verification model that replaces cosine similarity with a sliding window sign pattern matching approach, achieving 96.27% on LFW with a 10.58 MB model trained on CASIA-WebFace. This work challenges the default use of cosine similarity in metric learning, showing that sign pattern matching can achieve competitive results with a much smaller model, potentially enabling more efficient and interpretable face verification systems. The model uses three metrics (IMG Sign Score, AMP IMG Score, Chain Score) sharing one threshold, and a voting system (2/3 or 3/3 pass = MATCH). When applied to ArcFace embeddings without retraining, IMG Sign Score achieves 99.58% on LFW, only 0.24% below ArcFace+Cosine.

reddit · r/MachineLearning · /u/img-_- · Jul 9, 18:00

**Background**: Face verification typically compares embedding vectors using cosine similarity or Euclidean distance. Cosine similarity measures the angle between two vectors, but IMGNet argues that locally consistent sign patterns across embedding dimensions may be more robust and efficient.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/cosine-similarity">What Is Cosine Similarity? | IBM</a></li>
<li><a href="https://arxiv.org/html/2504.16318v1">Semantics at an Angle: When Cosine Similarity Works Until It Doesn't - arXiv</a></li>
<li><a href="https://datascience.stackexchange.com/questions/129996/an-old-question-cosine-or-euclidean-to-compute-similarity-of-embeddings">An old question: Cosine or Euclidean to compute similarity of embeddings?</a></li>

</ul>
</details>

**Tags**: `#face verification`, `#deep learning`, `#computer vision`, `#metric learning`

---

<a id="item-13"></a>
## [Damn Interesting launches funding drive to sustain site](https://www.damninteresting.com/a-possible-future/) ⭐️ 6.0/10

The creator of Damn Interesting, a long-running blog of fascinating stories, announced a funding drive to sustain the site. The blog has been running for years and is seeking community support to continue. This highlights the challenges faced by independent, high-quality content creators in sustaining their work without relying on ads or paywalls. The community's nostalgic response underscores the blog's cultural impact on the 'generally interesting' genre that influenced many podcasts. The funding drive is modest in amount, reflecting the site's niche but dedicated audience. The blog's thorough, long-form articles and occasional interactive simulations (e.g., orbital mechanics) set it apart from typical content.

hackernews · mzur · Jul 9, 15:25 · [Discussion](https://news.ycombinator.com/item?id=48847511)

**Background**: Damn Interesting is a blog that publishes in-depth, well-researched articles on a wide range of fascinating topics. It has been running for many years and has a loyal readership, but like many independent sites, it struggles with sustainable funding.

**Discussion**: Commenters expressed nostalgia and appreciation for the blog, with many sharing personal memories and noting its influence on the podcasting genre. The creator clarified that they did not self-promote on Hacker News, showing humility.

**Tags**: `#blogging`, `#community`, `#funding`, `#history`

---

<a id="item-14"></a>
## [LLM-Meta-AI 0.1 Plugin Released for Muse-Spark-1.1](https://simonwillison.net/2026/Jul/9/llm-meta-ai/#atom-everything) ⭐️ 6.0/10

The llm-meta-ai 0.1 plugin has been released, enabling the LLM command-line tool to run prompts against Meta's new muse-spark-1.1 model. This plugin expands the LLM ecosystem by adding support for Meta's latest model, allowing users to easily experiment with a different family of models from a single tool. The plugin is version 0.1, indicating an initial release that may have limited features or stability. It specifically targets the muse-spark-1.1 model, which is part of Meta's new Muse Spark series.

rss · Simon Willison · Jul 9, 16:12

**Background**: LLM is a command-line tool by Simon Willison that provides a unified interface to run prompts against various large language models. Plugins like llm-meta-ai extend its capabilities to support additional models from different providers.

**Tags**: `#llm`, `#meta`, `#plugin`, `#release`, `#ai`

---

<a id="item-15"></a>
## [Why Conferences Outshine Journals in ML Research](https://www.reddit.com/r/MachineLearning/comments/1urqqk6/journals_vs_conferences_ml_research_r/) ⭐️ 6.0/10

A Reddit discussion highlights that ICML and NeurIPS have become more prestigious than traditional journals in machine learning research over the past two to three years. This shift reflects the fast-paced nature of AI research, where rapid dissemination and high visibility at conferences are valued over the slower, more rigorous journal process. The post attributes the trend to the AI boom, which demands faster delivery of results, and notes that conferences have higher and faster acceptance rates compared to journals.

reddit · r/MachineLearning · /u/hg_wallstreetbets · Jul 9, 13:44

**Background**: In many scientific fields, journals are the primary venue for publishing research, with rigorous peer review. However, in machine learning, top conferences like ICML and NeurIPS have become the dominant publication venues due to their fast review cycles and high impact.

**Tags**: `#machine learning`, `#research culture`, `#conferences`, `#journals`

---

<a id="item-16"></a>
## [Talos-XII: Hand-written autograd and RL in Rust for gacha simulation](https://www.reddit.com/r/MachineLearning/comments/1urvxgb/talosxii_handwritten_autograd_small_rlmlp_stack/) ⭐️ 6.0/10

Talos-XII is a CLI simulator for Arknights: Endfield's gacha system that uses hand-written neural networks and reinforcement learning, without any external ML frameworks like PyTorch or ndarray. It trains small MLPs, a Dueling DQN, and a PPO actor-critic with a custom autograd engine and SIMD dispatch. This project demonstrates that a full ML stack—autograd, neural networks, and RL—can be built from scratch in Rust for a specific domain, achieving performance with SIMD and parallelism. It offers a lightweight alternative to heavy frameworks for niche applications like game probability modeling. The project includes a custom autograd engine with matmul, conv2d, pooling, and gradient-checked backward passes, runtime SIMD dispatch (scalar, AVX2, AVX-512, NEON), and Rayon-parallelized simulations. It also features an experimental ACHF component that blends dense and sparse paths with a gradient-sensitive gate and Sinkhorn projection.

reddit · r/MachineLearning · /u/zay0kami · Jul 9, 16:52

**Background**: Gacha systems in games use random pulls with pity mechanics to guarantee rewards after a certain number of attempts. Traditional probability tables cannot easily answer conditional questions like pull decisions based on current pity. Reinforcement learning can model such sequential decision problems, but typically requires heavy frameworks like PyTorch.

**Tags**: `#Rust`, `#reinforcement learning`, `#autograd`, `#gacha`, `#simulation`

---

<a id="item-17"></a>
## [Show HN: 18 Words – A Timed Word Game](https://18words.com/) ⭐️ 5.0/10

A new timed word game called 18 Words was launched on Hacker News, where players guess words from scrambled letters within a time limit. The game has sparked community discussion about game design choices, particularly the timer and scoring system, which could influence future word game development. The game presents 18 words, each with a 30-second timer; if the timer expires, the game ends. Community members have suggested adding a relax mode, a shuffle button, and allowing players to continue after missing a word with a reduced score.

hackernews · pompomsheep · Jul 9, 12:48 · [Discussion](https://news.ycombinator.com/item?id=48845049)

**Background**: Word games like this are popular on Hacker News, often receiving feedback on mechanics and user experience. The developer actively engages with the community to refine the game.

**Discussion**: The community generally appreciates the game's design but strongly requests a timer-free relax mode and a shuffle button to improve playability. Some users prefer a scoring system that allows continuing after mistakes.

**Tags**: `#word game`, `#game design`, `#user feedback`, `#hacker news`

---

<a id="item-18"></a>
## [llm 0.31.1 Fixes JSON Error with Empty Tool Call Arguments](https://simonwillison.net/2026/Jul/9/llm/#atom-everything) ⭐️ 3.0/10

llm 0.31.1 fixes a bug where OpenAI Chat Completion endpoints could return a JSON error when tool calls have empty arguments. This fix improves reliability for users of llm who rely on tool calling with OpenAI-compatible providers, ensuring that empty arguments do not break workflows. The bug was discovered while testing the llm-meta-ai plugin, and the fix is referenced in GitHub issue #1521.

rss · Simon Willison · Jul 9, 16:06

**Background**: llm is a command-line tool for interacting with large language models. Tool calling allows models to invoke external functions, and empty arguments can cause parsing errors in some providers.

**Tags**: `#llm`, `#bug-fix`, `#openai`

---