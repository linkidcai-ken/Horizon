---
layout: default
title: "Horizon Summary: 2026-06-20 (EN)"
date: 2026-06-20
lang: en
---

> From 18 items, 17 important content pieces were selected

---

1. [SMPTE Makes Its Standards Freely Accessible](#item-1) ⭐️ 8.0/10
2. [AI-Powered Plagiarism of 'The Dictionary of Obscure Sorrows'](#item-2) ⭐️ 8.0/10
3. [Cloudflare Temporary Accounts for AI Agents](#item-3) ⭐️ 8.0/10
4. [DVD-JEPA: Open-Source Minimal JEPA World Model](#item-4) ⭐️ 8.0/10
5. [Time Series Modeling Needs Dynamical Systems Perspective](#item-5) ⭐️ 8.0/10
6. [Open Handbook on LLM Inference at Scale](#item-6) ⭐️ 8.0/10
7. [minFLUX: A Minimal PyTorch Implementation of FLUX Diffusion Models](#item-7) ⭐️ 8.0/10
8. [F-15 Strike Eagle II Reverse Engineering Seeks Testers](#item-8) ⭐️ 7.0/10
9. [CSSQuake: Classic Game Recreated in CSS and HTML](#item-9) ⭐️ 7.0/10
10. [Build Your Own LLM Workshop Released on YouTube](#item-10) ⭐️ 7.0/10
11. [Should ML PhDs Graduate Without Top-Tier Papers?](#item-11) ⭐️ 7.0/10
12. [TSAuditor: A Tool to Catch Time-Series Data Pitfalls](#item-12) ⭐️ 7.0/10
13. [Global PM2.5 Forecaster Overcomes Variance Trap](#item-13) ⭐️ 7.0/10
14. [UHF X11 Brings X11 Window System to Apple Vision Pro](#item-14) ⭐️ 6.0/10
15. [StartupWiki Launches as Free Crunchbase Alternative](#item-15) ⭐️ 5.0/10
16. [Seeking Python Packages for PSO and GA Optimization](#item-16) ⭐️ 5.0/10
17. [How to Access Books3 Dataset for Research](#item-17) ⭐️ 3.0/10

---

<a id="item-1"></a>
## [SMPTE Makes Its Standards Freely Accessible](https://www.smpte.org/blog/smpte-makes-its-standards-freely-accessible-openingstandards-library-to-the-global-media-technology-community) ⭐️ 8.0/10

SMPTE has announced that all its media technology standards are now freely accessible to the public, and it is modernizing its development process by adopting GitHub workflows and HTML-based authoring. This move removes financial barriers to critical standards like SMPTE timecode and VC-1, fostering innovation and interoperability in media production and distribution. It aligns with the broader industry trend toward open standards, potentially accelerating adoption of new technologies. The transition includes adopting GitHub for version control and issue tracking, moving to structured HTML-based authoring, and implementing an integrated publishing pipeline. Previously, standards like SMPTE 430.10 cost money to access.

hackernews · zdw · Jun 20, 17:01 · [Discussion](https://news.ycombinator.com/item?id=48610827)

**Background**: SMPTE (Society of Motion Picture and Television Engineers) develops many widely used media technology standards, such as SMPTE timecode for frame labeling and VC-1 video codec. Historically, accessing these standards required purchasing PDFs, which limited their reach. By making them freely available and modernizing development with open-source tools, SMPTE aims to increase community participation and speed up standardization.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Category:SMPTE_standards">Category:SMPTE standards - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Society_of_Motion_Picture_and_Television_Engineers">Society of Motion Picture and Television Engineers - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/SMPTE_timecode">SMPTE timecode - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters largely applauded the move, with lambdaone comparing it to the IETF's successful no-cost standards model. geerlingguy questioned why any standards body wouldn't do this by default, while andersthuesen recalled having to buy the SMPTE 430.10 standard in the past.

**Tags**: `#standards`, `#media technology`, `#open access`, `#SMPTE`, `#open source`

---

<a id="item-2"></a>
## [AI-Powered Plagiarism of 'The Dictionary of Obscure Sorrows'](https://waxy.org/2026/06/the-wholesale-plagiarism-of-obscure-sorrows/) ⭐️ 8.0/10

An article on Waxy.org reveals that a website called Qontour plagiarized the entire book 'The Dictionary of Obscure Sorrows' by John Koenig, reproducing its full text verbatim, likely using AI to create a knock-off site. This incident highlights the growing problem of AI-enabled content theft, where plagiarists can easily copy and republish entire works, and underscores the challenges creators face in enforcing copyright through DMCA takedowns against anonymous entities. The plagiarized site reproduced the book's 800-word foreword and all 311 neologisms verbatim, and the perpetrator is identified as Prompt Digital Inc (DBA Qontour), an anonymous entity. The original author, John Koenig, is pursuing legal action.

hackernews · ridesisapis · Jun 20, 18:05 · [Discussion](https://news.ycombinator.com/item?id=48611411)

**Background**: The Dictionary of Obscure Sorrows is a word-construction project by John Koenig that coins neologisms for emotions not yet described in language. It was launched as a website and YouTube channel, and later published as a printed book in 2021 by Simon & Schuster. The DMCA (Digital Millennium Copyright Act) provides a notice-and-takedown process for copyright holders to request removal of infringing content from online platforms.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/The_Dictionary_of_Obscure_Sorrows">The Dictionary of Obscure Sorrows</a></li>
<li><a href="https://copyrightalliance.org/education/copyright-law-explained/the-digital-millennium-copyright-act-dmca/dmca-notice-takedown-process/">DMCA Notice & Takedown Process | Copyright Alliance</a></li>

</ul>
</details>

**Discussion**: Commenters expressed frustration with platform enforcement, noting that Google and Apple are often unhelpful without a court order. Some pointed out that DMCA takedowns are designed for such cases, but anonymity of infringers complicates enforcement. One commenter humorously coined a new 'obscure sorrow' for the situation.

**Tags**: `#plagiarism`, `#AI`, `#copyright`, `#DMCA`, `#creator rights`

---

<a id="item-3"></a>
## [Cloudflare Temporary Accounts for AI Agents](https://blog.cloudflare.com/temporary-accounts/) ⭐️ 8.0/10

Cloudflare introduced temporary accounts that allow AI agents and developers to deploy Workers for 60 minutes using `wrangler deploy --temporary`, with the option to claim the account permanently. This feature enables ephemeral deployments for AI agents, PR previews, and code review, reducing friction for experimentation while expanding Cloudflare's serverless ecosystem. Temporary deployments expire after 60 minutes unless claimed; Cloudflare applies rate limits and abuse prevention checks to prevent misuse of ephemeral infrastructure.

hackernews · farhadhf · Jun 20, 11:19 · [Discussion](https://news.ycombinator.com/item?id=48608394)

**Background**: Cloudflare Workers is a serverless computing platform that runs code on the edge network. Ephemeral environments are short-lived, isolated deployments often used for testing and previews. AI agents are software systems that use AI to autonomously perform tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://developers.cloudflare.com/workers/">Overview · Cloudflare Workers docs</a></li>
<li><a href="https://ephemeralenvironments.io/">Ephemeral Environments</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent</a></li>

</ul>
</details>

**Discussion**: Community members praised the feature for enabling free scratch deployments and PR previews, but raised concerns about hard billing caps and abuse prevention. Simon Willison highlighted the lack of hard billing caps as a major missing feature.

**Tags**: `#cloudflare`, `#serverless`, `#ai-agents`, `#deployment`, `#ephemeral`

---

<a id="item-4"></a>
## [DVD-JEPA: Open-Source Minimal JEPA World Model](https://www.reddit.com/r/MachineLearning/comments/1uatlzx/dvdjepa_an_opensource_fullyreproducible_jepa/) ⭐️ 8.0/10

DVD-JEPA is a minimal, fully reproducible implementation of the Joint-Embedding Predictive Architecture (JEPA) that learns to predict future representations rather than pixels, demonstrated on a bouncing DVD logo in a 16×16 box. This work provides an accessible, browser-based demonstration of JEPA, a key self-supervised learning paradigm proposed by Yann LeCun, and shows its utility for anomaly detection with a simple predictive monitor. A linear probe recovers the logo's exact (x,y) position from the frozen 32-dimensional latent space to within 0.73 pixels, and the model can dream future frames for ~20 steps before latent drift. The entire system runs client-side in a browser with ~40 lines of JavaScript.

reddit · r/MachineLearning · /u/NielsRogge · Jun 20, 10:52

**Background**: JEPA (Joint-Embedding Predictive Architecture) is a self-supervised learning method that predicts abstract representations (embeddings) of future data rather than reconstructing pixels, allowing the model to discard unpredictable details. It was introduced by Yann LeCun in 2022 and has been extended to images (I-JEPA) and video (V-JEPA). DVD-JEPA is a minimal implementation that uses a context encoder, an EMA target encoder, and a latent predictor trained without labels or a decoder.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Joint_Embedding_Predictive_Architecture">Joint Embedding Predictive Architecture</a></li>
<li><a href="https://arxiv.org/abs/2301.08243">[2301.08243] Self-Supervised Learning from Images with a Joint-Embedding Predictive Architecture</a></li>
<li><a href="https://rohitbandaru.github.io/blog/JEPA-Deep-Dive/">Deep Dive into Yann LeCun’s JEPA | Rohit Bandaru</a></li>

</ul>
</details>

**Discussion**: The Reddit community praised the work for its clarity, reproducibility, and clever demonstration, with many noting it makes JEPA concepts accessible. Some commenters discussed the potential for scaling to more complex environments and the significance of the anomaly detection application.

**Tags**: `#world model`, `#JEPA`, `#self-supervised learning`, `#video prediction`, `#anomaly detection`

---

<a id="item-5"></a>
## [Time Series Modeling Needs Dynamical Systems Perspective](https://www.reddit.com/r/MachineLearning/comments/1uark0u/time_series_modeling_needs_a_dynamical_systems/) ⭐️ 8.0/10

A position paper at ICML 2026 argues that time series modeling should adopt a dynamical systems perspective, proposing five concrete recommendations including generalized teacher forcing, pretraining on dynamical system simulations, and moving back to modern RNNs. This perspective could enable true out-of-domain generalization and long-term prediction, addressing fundamental limitations of current time series models. It also offers a mechanistic understanding of time series properties that is transferable across domains. The paper compares custom-trained and foundation models for time series and dynamical systems reconstruction, and suggests that proper training techniques are more important than model architecture. It also highlights topological shifts as the hard problem in forecasting.

reddit · r/MachineLearning · /u/DangerousFunny1371 · Jun 20, 08:47

**Background**: Time series modeling typically focuses on short-term forecasting without capturing the underlying dynamical rules. Dynamical systems reconstruction (DSR) aims to infer the governing equations from observed data, enabling long-term behavior prediction and out-of-domain generalization. Chaotic systems, common in nature, contain rich temporal structure that standard models often miss.

**Discussion**: The Reddit discussion includes diverse viewpoints, with some commenters supporting the shift to RNNs and dynamical systems theory, while others question the practicality of pretraining on simulations and the dismissal of transformers. There is general agreement that the paper raises important open problems.

**Tags**: `#time series`, `#dynamical systems`, `#machine learning`, `#forecasting`, `#ICML`

---

<a id="item-6"></a>
## [Open Handbook on LLM Inference at Scale](https://www.reddit.com/r/MachineLearning/comments/1uavduv/an_open_handbook_on_llm_inference_at_scale_gpu/) ⭐️ 8.0/10

An open, in-progress handbook on LLM inference at scale has been released, covering GPU internals, KV cache, batching, and production frameworks like vLLM, SGLang, and TensorRT-LLM. The author has just added a chapter on GPU execution and memory internals with mermaid diagrams. This resource helps engineers and researchers understand the bottlenecks in LLM inference, enabling them to optimize deployment and reduce costs. It bridges the gap between theoretical knowledge and production practice. The handbook is a personal learning project hosted on GitHub, with the author actively seeking community feedback via issues and PRs. It includes detailed explanations of GPU memory hierarchy, KV cache management, and comparisons of serving frameworks.

reddit · r/MachineLearning · /u/YouFirst295 · Jun 20, 12:27

**Background**: LLM inference at scale requires efficient use of GPU memory, especially the KV cache which grows with batch size and sequence length. Frameworks like vLLM use paged attention to manage KV cache, while TensorRT-LLM uses CUDA graph fusion for peak performance. Understanding these internals is key to reducing latency and increasing throughput.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bentoml.com/blog/what-is-gpu-memory-and-why-it-matters-for-llm-inference">What is GPU Memory and Why it Matters for LLM Inference</a></li>
<li><a href="https://northflank.com/blog/vllm-vs-tensorrt-llm-and-how-to-run-them">vLLM vs TensorRT-LLM: Key differences, performance, and how to run them | Blog — Northflank</a></li>
<li><a href="https://www.spheron.network/blog/vllm-vs-tensorrt-llm-vs-sglang-benchmarks/">vLLM vs TensorRT-LLM vs SGLang: H100 Benchmarks (2026) | Spheron Blog</a></li>

</ul>
</details>

**Tags**: `#LLM inference`, `#GPU internals`, `#vLLM`, `#TensorRT-LLM`, `#open source`

---

<a id="item-7"></a>
## [minFLUX: A Minimal PyTorch Implementation of FLUX Diffusion Models](https://www.reddit.com/r/MachineLearning/comments/1ub1db3/studying_flux_in_diffusers_library_was_hard_so_i/) ⭐️ 8.0/10

A developer released minFLUX, a minimal PyTorch implementation of FLUX.1 and FLUX.2 diffusion models, with line-by-line mappings to HuggingFace diffusers and training/inference loops. This simplifies studying FLUX's architecture, which is otherwise complex in the official diffusers library, and highlights key differences between FLUX.1 and FLUX.2, aiding researchers and practitioners. minFLUX includes VAE, transformer, flow matching with velocity MSE loss, Euler ODE solver for inference, and shared utilities like RoPE and timestep embeddings. FLUX.2 improves transformer blocks, modulation, FFN, VAE normalization, and position IDs over FLUX.1.

reddit · r/MachineLearning · /u/Other-Eye-8152 · Jun 20, 16:50

**Background**: FLUX is a family of text-to-image diffusion models that use a hybrid architecture of multimodal and parallel diffusion transformer blocks, scaled to 12B parameters. Flow matching is a generative modeling framework that combines aspects of diffusion models and continuous normalizing flows, often using an Euler ODE solver for sampling. The official HuggingFace diffusers library provides implementations but is heavily abstracted, making it difficult to study core components.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2507.09595v1">Demystifying Flux Architecture</a></li>
<li><a href="https://medium.com/@drmarcosv/how-does-flux-work-the-new-image-generation-ai-that-rivals-midjourney-7f81f6f354da">How does Flux work? The new image generation AI that rivals Midjourney | by Marcos V. Conde | Medium</a></li>
<li><a href="https://mlg.eng.cam.ac.uk/blog/2024/01/20/flow-matching.html">An introduction to Flow Matching · Cambridge MLG Blog</a></li>

</ul>
</details>

**Discussion**: The community praised the project for its clarity and educational value, with many noting the difficulty of navigating the official diffusers code. Some discussed the architectural differences between FLUX.1 and FLUX.2, and a few suggested adding support for other FLUX variants.

**Tags**: `#diffusion models`, `#FLUX`, `#PyTorch`, `#open source`, `#machine learning`

---

<a id="item-8"></a>
## [F-15 Strike Eagle II Reverse Engineering Seeks Testers](https://neuviemeporte.github.io/f15-se2/2026/06/20/needyou.html) ⭐️ 7.0/10

The F-15 Strike Eagle II reverse engineering project has completed converting the DOS game's assembly code to binary-equivalent C code and is now seeking testers to find bugs before porting to Linux and Windows. This project preserves a classic DOS game by enabling native play on modern platforms without emulation, ensuring the game's long-term accessibility and the four freedoms for its community. The project uses a two-step approach: first full reverse to assembler, then conversion to binary-equivalent C code while still running on DOS, with porting to Linux/Windows to follow. Testers need version 451.03 of the game and DOSBox or real DOS.

hackernews · LowLevelMahn · Jun 20, 15:10 · [Discussion](https://news.ycombinator.com/item?id=48609766)

**Background**: Reverse engineering old DOS games is challenging due to real-mode segmented memory and limited tooling. Converting assembly to C allows the game to be compiled for modern operating systems, offering better performance and integration than emulation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reddit.com/r/programming/comments/1crelua/dos_game_f15_strike_eagle_ii_reverse/">DOS game "F-15 Strike Eagle II" reverse engineering/reconstruction war stories - Ghidra to the rescue : r/programming</a></li>
<li><a href="https://news.ycombinator.com/item?id=40347662">DOS game “F-15 Strike Eagle II” reverse engineering/reconstruction war stories | Hacker News</a></li>
<li><a href="https://github.com/frranck/asm2c">GitHub - frranck/asm2 c : Tool to convert DOS Assembly code to C code</a></li>

</ul>
</details>

**Discussion**: Community sentiment is positive, with appreciation for preservation efforts and the four freedoms. Some question the value of decompilation over emulation, but others note that native ports avoid emulation overhead and enable deeper modifications.

**Tags**: `#reverse engineering`, `#game preservation`, `#DOS`, `#porting`, `#retro computing`

---

<a id="item-9"></a>
## [CSSQuake: Classic Game Recreated in CSS and HTML](https://cssquake.com/) ⭐️ 7.0/10

CSSQuake is a technical demo that recreates the classic game Quake using only CSS and HTML, powered by the PolyCSS engine, and is playable in a web browser. This project demonstrates the surprising capabilities of CSS for 3D rendering and game logic, pushing the boundaries of what is possible with web technologies and inspiring creative experimentation. Despite being called CSSQuake, the demo actually requires JavaScript to run, and it runs slower than the original Quake on a Pentium-133 PC from the 1990s.

hackernews · msalsas · Jun 20, 10:49 · [Discussion](https://news.ycombinator.com/item?id=48608223)

**Background**: Quake is a landmark first-person shooter game released in 1996, known for its advanced 3D graphics. CSS (Cascading Style Sheets) is a web technology used for styling HTML elements, not typically used for game rendering. This project uses PolyCSS, a CSS-based rendering engine, to simulate the game's visuals and logic.

<details><summary>References</summary>
<ul>
<li><a href="https://cssquake.com/">cssQuake - Powered by PolyCSS</a></li>

</ul>
</details>

**Discussion**: Commenters are impressed by the technical achievement but note that the game runs slower than the original and requires JavaScript, with some pointing out gameplay differences from the original Quake.

**Tags**: `#CSS`, `#game development`, `#retro computing`, `#web technology`, `#technical demo`

---

<a id="item-10"></a>
## [Build Your Own LLM Workshop Released on YouTube](https://www.reddit.com/r/MachineLearning/comments/1uazlnd/hi_reddit_i_posted_my_build_your_own_llm_workshop/) ⭐️ 7.0/10

Justin Angel released a comprehensive workshop video on YouTube that teaches how to build a large language model from scratch, covering everything from machine learning fundamentals to transformer architecture and training, with no math or ML prerequisites. This resource lowers the barrier for newcomers to understand and build LLMs, providing a hands-on, code-driven approach that includes Excel examples for intuition. It addresses a growing demand for accessible, practical education in the rapidly evolving field of generative AI. The workshop includes sections on tokenizers, embeddings, attention mechanisms (MHA, GQA, MQA, MLA), and training techniques like instruction tuning and reinforcement learning. It also covers advanced topics such as torch.compile() fused kernels and SwiGLU activation functions.

reddit · r/MachineLearning · /u/JustinAngel · Jun 20, 15:36

**Background**: Large language models (LLMs) like GPT-4 and LLaMA are built on transformer architectures that use attention mechanisms and feed-forward networks. Building an LLM from scratch requires understanding concepts like weight initialization (e.g., Kaiming, Glorot), normalization (e.g., RMSNorm, LayerNorm), and optimization. This workshop aims to demystify these concepts using slides, Excel, and code.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@s_boudefel/exploring-swiglu-the-activation-function-powering-modern-llms-9697f88221e7">Exploring SwiGLU : The Activation Function Powering Modern LLMs | by Selssabil | Medium</a></li>
<li><a href="https://en.wikipedia.org/wiki/Weight_initialization">Weight initialization - Wikipedia</a></li>
<li><a href="https://gist.github.com/purohit10saurabh/cbf5759e17061b7819ab7e52498b1f62">tinytorchcompile: torch . compile in a nutshell — operator fusion of...</a></li>

</ul>
</details>

**Discussion**: The Reddit community reacted positively, with users appreciating the no-prerequisites approach and the inclusion of Excel examples for intuition. Some commenters noted the comprehensive coverage and praised the instructor's teaching style.

**Tags**: `#LLM`, `#Machine Learning`, `#Tutorial`, `#Deep Learning`, `#Transformers`

---

<a id="item-11"></a>
## [Should ML PhDs Graduate Without Top-Tier Papers?](https://www.reddit.com/r/MachineLearning/comments/1uazlhg/would_you_let_an_ml_phd_student_graduate_without/) ⭐️ 7.0/10

A Reddit user asks whether an ML PhD advisor should let a student graduate with solid work but no publications in top-tier venues like NeurIPS, ICML, ICLR, or CVPR, only three first-author A-level papers. This debate highlights the tension between publication metrics and thesis quality in ML PhD programs, affecting student careers, advisor decisions, and academic culture. The student has been in the program for four years, has a coherent thesis direction, and three first-author A-level papers, but no top-tier venue publications. The question assumes the thesis itself is solid.

reddit · r/MachineLearning · /u/Hope999991 · Jun 20, 15:36

**Background**: In machine learning, top-tier conferences like NeurIPS, ICML, ICLR, and CVPR are highly competitive and often considered essential for academic career progression. Many PhD programs implicitly require such publications for graduation, though formal requirements vary. A-level papers refer to reputable but not top-tier venues.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2510.09586v1">Vision Language Models: A Survey of 26K Papers (CVPR, ICLR, NeurIPS 2023–2025)</a></li>
<li><a href="https://algoverseairesearch.org/blog/icml-iclr-aaai-student-guide">Beyond NeurIPS: A Student's Guide to ICML, ICLR, AAAI, and Other AI Conferences | Algoverse AI Research</a></li>
<li><a href="https://wiki.eventhosts.cc/">Welcome to Event Hosts Wiki | Wiki.EventHosts NeurIPS/ICML/ICLR/CVPR and more</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion (not provided in detail) likely includes diverse opinions: some argue that solid work without top-tier pubs should suffice, while others emphasize the importance of top-tier publications for career prospects. The original post's score of 7.0 suggests strong engagement.

**Tags**: `#PhD`, `#machine learning`, `#publications`, `#academia`, `#career`

---

<a id="item-12"></a>
## [TSAuditor: A Tool to Catch Time-Series Data Pitfalls](https://www.reddit.com/r/MachineLearning/comments/1ub15wf/tsauditor_a_timeseries_auditing_framework_p/) ⭐️ 7.0/10

A practitioner released tsauditor, an open-source Python library that detects chronological breaks, data leakage, and sequential anomalies in time-series datasets. The tool provides evidence and suggested fixes for each issue. Time-series data issues like leakage and broken chronology are common but often overlooked, leading to overly optimistic model performance. TSAuditor helps practitioners catch these problems early, improving model reliability and saving debugging time. TSAuditor is lightweight, available on PyPI, and can be used without defining a domain. It includes an example notebook with side-by-side comparisons against standard profiling tools.

reddit · r/MachineLearning · /u/severecaseofsarcarsm · Jun 20, 16:41

**Background**: Time-series data requires careful handling because chronological order matters; shuffling or leaking future information into training data can produce misleadingly high accuracy. Common pitfalls include missing data that is not random (e.g., a contiguous block of missing days) and data leakage where future data inadvertently influences past predictions. Standard profiling tools often fail to detect these issues, as they treat each row independently.

<details><summary>References</summary>
<ul>
<li><a href="https://pypi.org/project/tsauditor/">A data quality auditing library for time - series tabular data in financial...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Leakage_(machine_learning)">Leakage (machine learning) - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/data-leakage-machine-learning">What is Data Leakage in Machine Learning? | IBM</a></li>

</ul>
</details>

**Tags**: `#time-series`, `#data auditing`, `#ML pipeline`, `#data quality`, `#tool`

---

<a id="item-13"></a>
## [Global PM2.5 Forecaster Overcomes Variance Trap](https://www.reddit.com/r/MachineLearning/comments/1uar4vc/built_a_global_aq_pm25_forecaster_ml_model_p/) ⭐️ 7.0/10

A practitioner built an end-to-end PM2.5 forecasting pipeline for the US, UK, India, and Australia using over 1.6 million rows of OpenAQ and NASA weather data, and introduced a horizon-aligned architecture that decouples forecast horizons to overcome the variance trap. This work addresses a common failure in time series forecasting—the variance trap—where naive baselines outperform ML models in chaotic environments, and provides a practical solution that reduces MASE below 1.0 globally, even at a 30-day horizon. The horizon-aligned architecture uses strict autoregressive lag vectors specific to each horizon (h=1, 7, 14, 30) and a 3-day rolling volatility matrix that ends at the inference boundary to prevent data leakage. The current model uses scikit-learn Gradient Boosting Regressor, with plans to migrate to XGBoost or LightGBM.

reddit · r/MachineLearning · /u/Divyanshailani · Jun 20, 08:20

**Background**: The variance trap occurs when a forecasting model fails to anticipate sudden shifts in chaotic environments, leading to a Mean Absolute Scaled Error (MASE) greater than 1.0, meaning a naive carryover guess outperforms the model. MASE compares forecast errors to those of a naive benchmark; values below 1.0 indicate the model is better than the benchmark.

<details><summary>References</summary>
<ul>
<li><a href="https://abouttrading.substack.com/p/the-biasvariance-tradeoff-in-time">The Bias–Variance Tradeoff in Time Series Forecasting</a></li>
<li><a href="https://medium.com/@ashishdce/mean-absolute-scaled-error-mase-in-forecasting-8f3aecc21968">Mean Absolute Scaled Error ( MASE ) in Forecasting | Medium</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#time series forecasting`, `#air quality`, `#gradient boosting`

---

<a id="item-14"></a>
## [UHF X11 Brings X11 Window System to Apple Vision Pro](https://www.lispm.net/apps/uhf-x11/) ⭐️ 6.0/10

UHF X11 is a new app that ports the classic X11 windowing system to Apple's VisionOS, allowing users to run 2D and 3D X11 applications on the Apple Vision Pro headset in a spatial computing environment. This project demonstrates the flexibility of spatial computing by bridging legacy Unix graphical interfaces with modern mixed reality hardware, potentially enabling developers to experiment with X11 applications in immersive environments. UHF X11 supports OpenGL clients via GLX rendering over X11, though compatibility varies. The app is built specifically for VisionOS and Apple Vision Pro, and may not be available in all regional App Stores.

hackernews · zdw · Jun 20, 17:04 · [Discussion](https://news.ycombinator.com/item?id=48610853)

**Background**: The X Window System (X11) is a network-transparent windowing system for bitmap displays, common on Unix-like operating systems since the 1980s. VisionOS is Apple's extended reality operating system for the Apple Vision Pro headset, which blends digital content with the physical world. Spatial computing refers to 3D human-computer interaction that takes place in real-world environments.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/X_Windowing_System">X Windowing System</a></li>
<li><a href="https://en.wikipedia.org/wiki/VisionOS">VisionOS</a></li>
<li><a href="https://en.wikipedia.org/wiki/Spatial_computing">Spatial computing</a></li>

</ul>
</details>

**Discussion**: Community comments are mixed: some find the project amusing and creative, while others express skepticism about X11's longevity compared to visionOS. One user notes the unavailability in the German App Store, and another asks about Linux AR headset alternatives.

**Tags**: `#X11`, `#VisionOS`, `#Apple Vision Pro`, `#spatial computing`, `#retro computing`

---

<a id="item-15"></a>
## [StartupWiki Launches as Free Crunchbase Alternative](https://startupwiki.tech/) ⭐️ 5.0/10

StartupWiki, a free and open startup database inspired by Wikipedia, has been launched to provide easy access to startup information without accounts or subscriptions. This project addresses the need for a free, accessible startup database, challenging paid platforms like Crunchbase and potentially democratizing startup research for founders, investors, and enthusiasts. The database currently includes startup profiles, search and filtering, company categorization, and a public API in progress, but early tests show limited coverage with many startups missing.

hackernews · shpran · Jun 20, 15:59 · [Discussion](https://news.ycombinator.com/item?id=48610224)

**Background**: Crunchbase is a leading startup database that compiles data via AI, community contributions, and live sources, but its advanced features require a subscription. StartupWiki aims to be a free, community-driven alternative similar to Wikipedia, relying on AI and user input for data, though reliability concerns have been raised.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Crunchbase">Crunchbase</a></li>
<li><a href="https://en.wikipedia.org/wiki/Category:Startup_databases">Category:Startup databases - Wikipedia</a></li>
<li><a href="https://grokipedia.com/page/List_of_startup_discovery_platforms">List of startup discovery platforms</a></li>

</ul>
</details>

**Discussion**: Community feedback highlights data coverage and reliability issues: users found many startups missing, and the VERIFIED badge lacks provenance links, raising skepticism. Suggestions include scraping investor portfolios and exposing an API for AI-driven data acquisition.

**Tags**: `#startups`, `#database`, `#open-source`, `#data`

---

<a id="item-16"></a>
## [Seeking Python Packages for PSO and GA Optimization](https://www.reddit.com/r/MachineLearning/comments/1ub81us/python_packages_for_particle_swarms_genetic/) ⭐️ 5.0/10

A Reddit user is asking for recommendations on Python packages for particle swarm optimization (PSO) and genetic algorithms (GA) to replace a constrained Levenberg-Marquardt optimizer for curve-fitting. They discovered scikit-opt and want community feedback on its usability and alternatives. This discussion highlights the practical need for robust, easy-to-use optimization libraries in Python, especially for complex curve-fitting tasks where traditional methods like Levenberg-Marquardt may fail. The outcome could guide practitioners toward better tools for avoiding local minima. The user's current optimizer is constrained Levenberg-Marquardt, which is slow and prone to local minima. They are not concerned about speed or GPU support initially, but prioritize easy data visualization. Scikit-opt is an open-source Python library (MIT license) that implements PSO, GA, simulated annealing, and more.

reddit · r/MachineLearning · /u/bwllc · Jun 20, 21:28

**Background**: Particle swarm optimization (PSO) and genetic algorithms (GA) are population-based metaheuristics used for global optimization, often effective for non-convex problems where gradient-based methods like Levenberg-Marquardt get stuck. Scikit-opt is a Python package that provides a unified interface for several swarm intelligence algorithms, similar to scikit-learn's API style.

<details><summary>References</summary>
<ul>
<li><a href="https://scikit-opt.github.io/scikit-opt/">scikit-opt</a></li>
<li><a href="https://github.com/guofei9987/scikit-opt">GitHub - guofei9987/scikit-opt: Genetic Algorithm, Particle Swarm Optimization, Simulated Annealing, Ant Colony Optimization Algorithm,Immune Algorithm, Artificial Fish Swarm Algorithm, Differential Evolution and TSP(Traveling salesman) · GitHub</a></li>
<li><a href="https://quantsrus.github.io/post/constraints-in-levenberg-marquardt-least-squares-optimization/">Constraints in the Levenberg - Marquardt least-squares optimization</a></li>

</ul>
</details>

**Tags**: `#optimization`, `#particle swarm`, `#genetic algorithms`, `#Python`, `#scikit-opt`

---

<a id="item-17"></a>
## [How to Access Books3 Dataset for Research](https://www.reddit.com/r/MachineLearning/comments/1uaoomx/how_to_access_books3_dataset_for_research/) ⭐️ 3.0/10

A Reddit user asked how to access the Books3 dataset for research purposes, highlighting ongoing interest in this controversial dataset. Books3 is a key training dataset for many large language models, but its copyrighted content raises legal and ethical concerns, making access a sensitive issue for researchers. Books3 contains over 191,000 copyrighted books compiled from the pirate website Bibliotik, and is part of the larger Pile dataset. Researchers seeking access must navigate copyright restrictions and potential legal risks.

reddit · r/MachineLearning · /u/xolmnyc · Jun 20, 05:55

**Background**: The Books3 dataset was created by EleutherAI as part of The Pile, a large-scale curated dataset for training language models. It has been widely used but also criticized for including copyrighted material without permission, leading to lawsuits and discussions about fair use in AI training.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/The_Pile_(dataset)">The Pile (dataset) - Wikipedia</a></li>
<li><a href="https://www.theatlantic.com/technology/archive/2025/09/dataset-books3/683662/">AI Watchdog: Books3 - The Atlantic</a></li>

</ul>
</details>

**Tags**: `#dataset`, `#books3`, `#machine learning`

---