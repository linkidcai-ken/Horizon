---
layout: default
title: "Horizon Summary: 2026-07-13 (EN)"
date: 2026-07-13
lang: en
---

> From 22 items, 19 important content pieces were selected

---

1. [Apple SpeechAnalyzer API Benchmarked Against Whisper](#item-1) ⭐️ 8.0/10
2. [Open Data Rescues Climate.gov After Government Removal](#item-2) ⭐️ 8.0/10
3. [Telegram's t.me domain suspended due to legal actions](#item-3) ⭐️ 8.0/10
4. [Samsung Health Threatens Data Deletion for AI Opt-Out](#item-4) ⭐️ 8.0/10
5. [DOOMQL: Doom-like game powered by SQLite queries](#item-5) ⭐️ 8.0/10
6. [CoT as Scaling Trap; Latent Reasoning Next](#item-6) ⭐️ 8.0/10
7. [Reddit Debate: What Is Continual Learning and Why for AGI?](#item-7) ⭐️ 8.0/10
8. [GPUHedge cuts serverless GPU cold start p95 latency from 117s to 30s](#item-8) ⭐️ 8.0/10
9. [Open-source tool filters arXiv papers by research interest](#item-9) ⭐️ 8.0/10
10. [Jacobian Lens Workspace Entropy Tested on Qwen3-4B](#item-10) ⭐️ 8.0/10
11. [Build and Ship Apple Apps Without Xcode](#item-11) ⭐️ 7.0/10
12. [Real Token Costs of Frontier AI Models Compared](#item-12) ⭐️ 7.0/10
13. [Sega CD Silpheed: FMV Engineering Deep Dive](#item-13) ⭐️ 7.0/10
14. [Datasette Code Frequency Chart Shows AI Agent Impact](#item-14) ⭐️ 7.0/10
15. [AI Agents Should Never Be Directly Responsible Individuals](#item-15) ⭐️ 7.0/10
16. [Prompt-Engineering Paper on Mode Collapse Accepted to ICML](#item-16) ⭐️ 6.0/10
17. [LLMs and CS PhD Completion Times](#item-17) ⭐️ 5.0/10
18. [shot-scraper 1.11: Improved Server Startup and JS File Option](#item-18) ⭐️ 3.0/10
19. [ECCV 2026 Authorized Delegate Policy Clarification](#item-19) ⭐️ 3.0/10

---

<a id="item-1"></a>
## [Apple SpeechAnalyzer API Benchmarked Against Whisper](https://get-inscribe.com/blog/apple-speech-api-benchmark.html) ⭐️ 8.0/10

Apple introduced the SpeechAnalyzer API at WWDC 2025, replacing the older SFSpeechRecognizer, and a benchmark shows it is substantially faster than Whisper Large-V2 with only slightly lower accuracy. This API could disrupt many paid speech-to-text apps that rely on Whisper, as Apple may integrate it natively into macOS, offering a free, on-device, privacy-preserving alternative. The benchmark tested SpeechAnalyzer against Whisper Large-V2 on a math lecture, finding it substantially faster and only slightly worse in accuracy, making it very usable for live transcription.

hackernews · get-inscribe · Jul 13, 16:06 · [Discussion](https://news.ycombinator.com/item?id=48894752)

**Background**: Speech recognition converts audio to text. Apple's new SpeechAnalyzer API is an on-device solution for iOS 26 and macOS, replacing the older SFSpeechRecognizer. Whisper is an open-source model by OpenAI widely used for transcription.

<details><summary>References</summary>
<ul>
<li><a href="https://developer-mdn.apple.com/videos/play/wwdc2025/277/">Bring advanced speech -to-text to your app with... - Apple Developer</a></li>
<li><a href="https://www.argmaxinc.com/blog/apple-and-argmax">Apple SpeechAnalyzer and Argmax WhisperKit - Argmax</a></li>
<li><a href="https://asibiont.com/en/blog/apple-speechanalyzer-protiv-whisper-chto-izmenilos-v-mire-vibe-coding-v-2026-godu">Apple 's New SpeechAnalyzer API Benchmarked... — ASI Biont Blog</a></li>

</ul>
</details>

**Discussion**: Commenters note that Whisper is no longer state-of-the-art, with better models like Nvidia's Nemotron and Parakeet, Mistral's Voxtral, and Cohere Transcribe available. Some predict Apple's native integration will hurt paid Whisper wrappers, while others share positive experiences with alternatives like Willow.

**Tags**: `#speech recognition`, `#Apple`, `#benchmark`, `#ASR`, `#Whisper`

---

<a id="item-2"></a>
## [Open Data Rescues Climate.gov After Government Removal](https://werd.io/climate-gov-was-destroyed-open-data-saved-it/) ⭐️ 8.0/10

A blog post details how open data initiatives preserved climate.gov data after it was removed from government websites, demonstrating the resilience of decentralized archiving. This event underscores the importance of open data and civic tech in ensuring public access to government-funded information, especially in politically sensitive areas like climate science. The saved data relies on donations for ongoing maintenance, raising questions about long-term sustainability. The community discussion also explores using decentralized systems like IPFS for government publications.

hackernews · benwerd · Jul 13, 19:57 · [Discussion](https://news.ycombinator.com/item?id=48897945)

**Background**: Open data refers to data that is freely available for anyone to access, use, and share. Civic tech uses technology to improve government-citizen relationships. Decentralized archiving distributes data across multiple nodes to prevent single points of failure.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Open_data">Open data - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Civic_technology">Civic technology</a></li>
<li><a href="https://mona.ws/en/articles/foreseeing-the-future/archiving-transactions">Transaction Archiving in a Decentralized Environment: Challenges...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed gratitude for the data rescue but questioned how the site will stay relevant without government funding. Some advocated for decentralized archiving as a default for government static content, while others noted the challenge of dynamic services.

**Tags**: `#open data`, `#climate data`, `#government transparency`, `#archiving`, `#civic tech`

---

<a id="item-3"></a>
## [Telegram's t.me domain suspended due to legal actions](https://www.whois.com/whois/t.me) ⭐️ 8.0/10

Telegram's short URL domain t.me has been suspended, as shown by WHOIS records indicating serverHold and clientRenewProhibited status codes. The suspension likely stems from legal or regulatory investigations by Russia, France, or India. This suspension could disrupt access to millions of Telegram links shared via t.me, affecting users and businesses relying on the platform. It highlights the vulnerability of centralized domain registrations and the power of registrars and registries in enforcing legal actions. The domain is on serverHold, meaning the .me registry (not GoDaddy) took the action, and clientRenewProhibited indicates a legal dispute or pending deletion. Telegram's reliance on GoDaddy as registrar surprised many, given GoDaddy's history of opaque suspensions.

hackernews · Tiberium · Jul 13, 19:52 · [Discussion](https://news.ycombinator.com/item?id=48897878)

**Background**: Domain suspension can occur when a registrar or registry receives a legal order or detects policy violations. ICANN's EPP status codes like serverHold indicate the domain is not resolving, while clientRenewProhibited prevents renewal. Telegram is under investigation in multiple countries for issues like extremism and exam cheating.

<details><summary>References</summary>
<ul>
<li><a href="https://www.icann.org/resources/pages/epp-status-codes-2014-06-16-en">EPP Status Codes | What Do They Mean, and Why Should... - ICANN</a></li>
<li><a href="https://en.wikipedia.org/wiki/WHOIS">WHOIS - Wikipedia</a></li>
<li><a href="https://lookup.icann.org/">ICANN Lookup</a></li>

</ul>
</details>

**Discussion**: Commenters expressed surprise that Telegram used GoDaddy, known for lack of transparency. Some noted the serverHold status indicates registry-level action, not registrar. Others highlighted the irony of launching a Telegram channel just before the suspension, and shared insights on ICANN status codes.

**Tags**: `#Telegram`, `#domain suspension`, `#ICANN`, `#GoDaddy`, `#legal investigation`

---

<a id="item-4"></a>
## [Samsung Health Threatens Data Deletion for AI Opt-Out](https://neow.in/cWsyMTV3) ⭐️ 8.0/10

Samsung Health has updated its privacy policy to require users to consent to their health data being used for AI training, or face permanent deletion of their account and all associated data. This policy forces users to choose between losing their health history or allowing their sensitive biometric data to be used for AI training, raising significant privacy and data rights concerns. The data categories targeted include sleep, medications, medical records, and cycle tracking details. Users who opt out will lose access to core syncing functionality and face account deletion.

hackernews · bundie · Jul 13, 20:01 · [Discussion](https://news.ycombinator.com/item?id=48897991)

**Background**: Samsung Health is a health-tracking app used with Galaxy Watches and other devices. Many tech companies use user data to train AI models, but typically offer an opt-out without data deletion. This policy is unusually coercive.

<details><summary>References</summary>
<ul>
<li><a href="https://www.androidheadlines.com/2026/07/samsung-health-ai-data-training-deletion-policy.html">Samsung Health to Delete Data If Users Opt Out of AI</a></li>
<li><a href="https://9to5google.com/2026/07/13/samsung-health-ai-training-data-consent/">Samsung Health will delete your data without AI training consent</a></li>
<li><a href="https://www.howtogeek.com/samsung-health-requires-ai-training-consent/">Samsung is pushing users to train AI with their personal ...</a></li>

</ul>
</details>

**Discussion**: Commenters express frustration, with one noting the app already has ads and bugs. Another sarcastically suggests data deletion might be a benefit. Some compare it to Google's similar practices, criticizing the user-hostile approach.

**Tags**: `#privacy`, `#Samsung`, `#health data`, `#AI training`, `#data rights`

---

<a id="item-5"></a>
## [DOOMQL: Doom-like game powered by SQLite queries](https://simonwillison.net/2026/Jul/13/doomql/#atom-everything) ⭐️ 8.0/10

Peter Gostev built DOOMQL, a Doom-like first-person shooter where SQLite serves as the game engine, handling movement, collision, enemies, and rendering entirely through SQL queries, including a ray tracer implemented via a recursive CTE. This project demonstrates an unconventional and creative use of SQLite, pushing the boundaries of what a database can do and inspiring new approaches to game development and database-driven rendering. The game is implemented as a Python terminal script and creates a SQLite database that can be explored with Datasette; Simon Willison extended it with a Datasette App that displays the game view and a tactical minimap, refreshed every second.

rss · Simon Willison · Jul 13, 22:34

**Background**: SQLite is the most widely deployed database engine, known for its lightweight, serverless architecture. Doom is a landmark 1993 first-person shooter that popularized the genre. DOOMQL was built with GPT-5.6 Sol, an advanced AI model from OpenAI focused on cybersecurity and long-horizon tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sqlite.org/">SQLite Home Page</a></li>
<li><a href="https://openai.com/index/previewing-gpt-5-6-sol/">Previewing GPT - 5 . 6 Sol : a next-generation model | OpenAI</a></li>

</ul>
</details>

**Tags**: `#sqlite`, `#game development`, `#ai-assisted`, `#python`, `#creative coding`

---

<a id="item-6"></a>
## [CoT as Scaling Trap; Latent Reasoning Next](https://www.reddit.com/r/MachineLearning/comments/1uviru5/chain_of_thought_is_a_scaling_trap_the_next_wave/) ⭐️ 8.0/10

A Reddit post argues that Chain-of-Thought (CoT) reasoning is a scaling trap due to faithfulness and cost issues, and proposes latent reasoning methods like Coconut, HRM, and RecursiveMAS as the next wave, while noting the black box interpretability problem. This critique challenges the dominant CoT paradigm in LLM reasoning, highlighting a shift toward latent computation that could reduce cost and latency but raises governance concerns for high-stakes applications. Coconut enables continuous latent thoughts for breadth-first search; HRM uses hierarchical recurrence for deep reasoning with few parameters; RecursiveMAS passes latent embeddings between agents. BDH (Dragon Hatchling) achieves 97.4% accuracy on Sudoku without CoT, aiming to combine latent iteration with stateful memory.

reddit · r/MachineLearning · /u/meowsterpieces · Jul 13, 17:50

**Background**: Chain-of-Thought (CoT) prompting improves LLM reasoning by generating intermediate steps in natural language. However, it serializes computation into tokens, increasing cost and latency, and the trace may not faithfully reflect the model's internal reasoning. Latent reasoning methods perform computation in hidden states, outputting language only at the end, potentially improving efficiency but reducing interpretability.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2412.06769">[2412.06769] Training Large Language Models to Reason in a Continuous Latent Space</a></li>
<li><a href="https://arxiv.org/abs/2506.21734">[2506.21734] Hierarchical Reasoning Model - arXiv.org Hierarchical Reasoning Model - arXiv.org Images What is a hierarchical reasoning model (HRM)? - IBM GitHub - Malaeu/hrm: Hierarchical Reasoning Model Official ... Paper page - Hierarchical Reasoning Model - Hugging Face The Era of Hierarchical Reasoning Models?</a></li>
<li><a href="https://recursivemas.github.io/">RecursiveMAS</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion includes diverse viewpoints: some agree CoT is a costly interface artifact, while others argue it remains useful for interpretability. Several commenters emphasize the need for outer-loop verification (e.g., DAGs, unit tests) to address the black box problem, and some question whether latent methods can scale to general language tasks.

**Tags**: `#LLM reasoning`, `#Chain-of-Thought`, `#latent reasoning`, `#AI interpretability`, `#scaling`

---

<a id="item-7"></a>
## [Reddit Debate: What Is Continual Learning and Why for AGI?](https://www.reddit.com/r/MachineLearning/comments/1uvm2p4/whats_your_take_on_continual_learning_d/) ⭐️ 8.0/10

A Reddit discussion questions the definition and importance of continual learning for AGI, citing claims by Dario Amodei (continual learning by 2026) and Demis Hassabis (most important unsolved breakthrough). This debate highlights the lack of consensus on a core AGI capability, affecting research direction, funding, and timeline predictions. The post notes that continual learning is framed variously as solving catastrophic forgetting, online learning, lifelong learning, or meta-learning, with shifting goalposts.

reddit · r/MachineLearning · /u/watercolorer2024 · Jul 13, 19:47

**Background**: Continual learning aims to enable AI models to learn new tasks without forgetting previous ones, a challenge known as catastrophic forgetting. It is considered a missing piece for AGI, as current models are typically trained on static datasets and then frozen.

<details><summary>References</summary>
<ul>
<li><a href="https://chrhenning.com/blog/2025/agi-misses-continual-learning/">Continual Learning - The Missing Piece of AGI | Christian Henning</a></li>
<li><a href="https://en.wikipedia.org/wiki/Catastrophic_forgetting">Catastrophic forgetting</a></li>
<li><a href="https://arxiv.org/abs/2311.05241">[2311.05241] When Meta-Learning Meets Online and Continual ... When Meta-Learning Meets Online and Continual Learning: A Survey When Meta-Learning Meets Online and Continual Learning: A ... When Meta-Learning Meets Online and Continual Learning: A ... Reconciling meta-learning and continual learning with online ... Meta Learning and Continual Learning | by Prathamesh Gadekar ... Meta Learning and Continual Learning in Adaptive AI Systems ...</a></li>

</ul>
</details>

**Discussion**: The discussion reflects a mix of skepticism and curiosity, with some arguing that continual learning is overhyped and poorly defined, while others see it as a fundamental bottleneck. Commenters call for clearer benchmarks and frameworks.

**Tags**: `#continual learning`, `#AGI`, `#machine learning`, `#catastrophic forgetting`, `#meta-learning`

---

<a id="item-8"></a>
## [GPUHedge cuts serverless GPU cold start p95 latency from 117s to 30s](https://www.reddit.com/r/MachineLearning/comments/1uvlb6h/gpuhedge_hedging_serverless_gpu_providers/) ⭐️ 8.0/10

GPUHedge, an open-source hedging library for serverless GPU providers, reduces p95 cold start latency from 116.6 seconds to 29.4 seconds by launching requests on a primary provider and conditionally switching to a backup after 10 seconds. Cold start latency is a major pain point for serverless GPU inference, often causing delays of over a minute for large models; GPUHedge offers a practical, provider-agnostic solution that can significantly improve user experience and reduce costs. The benchmark used a 17 GB AI model on RunPod as primary and Cerebrium as backup, with a 10-second hedge threshold; the approach reduced requests over 60 seconds from 11/36 to 0/36 and lowered modeled active-compute cost from $0.0114 to $0.0083 per request.

reddit · r/MachineLearning · /u/Putrid_Construction3 · Jul 13, 19:20

**Background**: Serverless GPU providers allow users to run AI inference without managing infrastructure, but they suffer from cold start latency—the time to load a model onto a GPU when no warm instance is available. This can range from 30 seconds to several minutes for large models. Hedging is a technique used in distributed systems to reduce tail latency by issuing redundant requests to multiple providers and using the first successful response.

<details><summary>References</summary>
<ul>
<li><a href="https://www.paralleliq.ai/blog/gpu-ops-serverless-cold-start">Serverless GPU Cold Start Latency: Causes and Solutions</a></li>
<li><a href="https://lyceum.technology/magazine/serverless-gpu-cold-start-latency-comparison/index.html">Serverless GPU Cold Start Latency: Architecture Comparison</a></li>

</ul>
</details>

**Tags**: `#serverless GPU`, `#cold start`, `#hedging`, `#machine learning`, `#open source`

---

<a id="item-9"></a>
## [Open-source tool filters arXiv papers by research interest](https://www.reddit.com/r/MachineLearning/comments/1uvcdf7/hundreds_of_papers_hit_arxiv_every_day_and_maybe/) ⭐️ 8.0/10

A developer released Research Radar, an open-source tool that daily fetches new arXiv papers, scores abstracts against a user-defined research interest file, and summarizes top papers using LLMs. This tool addresses the common pain point of information overload in research, saving researchers 30-60 minutes daily by surfacing only relevant papers, and its model-agnostic design allows use with local or cloud LLMs. The tool uses a two-pass scoring: a cheap model scores abstracts 1-10, then a strong model deep-reads top papers (40-70k tokens each) to generate summaries and relation to user's work; it supports Telegram digest and costs are benchmarked in the repo.

reddit · r/MachineLearning · /u/usedtobreath · Jul 13, 13:59

**Background**: arXiv is a preprint repository hosting over 2 million papers across sciences, with about 24,000 new submissions monthly. Researchers often struggle to filter relevant papers from daily feeds. Research Radar automates this by combining arXiv's RSS/API with LLM-based relevance scoring.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ArXiv_(identifier)">ArXiv (identifier)</a></li>
<li><a href="https://info.arxiv.org/help/api/index.html">arXiv API Access - arXiv info</a></li>
<li><a href="https://info.arxiv.org/help/api/user-manual.html">arXiv API User's Manual - arXiv info arxiv · PyPI arxiv-docs/source/help/api/user-manual.md at develop - GitHub arxiv API documentation - lukasschwab.me arxiv-docs/source/help/api/basics.md at develop - GitHub arXiv API — Free Public API | Public APIs Directory</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion was positive, with users praising the tool's practicality and asking technical questions about model calibration and cost. The author engaged actively, explaining design choices and inviting feedback.

**Tags**: `#arXiv`, `#research tool`, `#open source`, `#NLP`, `#paper filtering`

---

<a id="item-10"></a>
## [Jacobian Lens Workspace Entropy Tested on Qwen3-4B](https://www.reddit.com/r/MachineLearning/comments/1uv5l75/evaluating_jspace_entropy_as_an_error_predictor/) ⭐️ 8.0/10

A researcher evaluated Jacobian Lens workspace entropy as an error predictor on Qwen3-4B across 7 datasets with ~11,400 examples, finding it complements output confidence on factual tasks but fails on misconception detection and is highly task-dependent. This study provides rigorous empirical evidence that workspace entropy is not a general-purpose hallucination detector, narrowing its practical use to specific factual retrieval scenarios, which is important for AI safety and model reliability research. The evaluation used Qwen3-4B on TriviaQA, PopQA, NQ-Open, TruthfulQA, HotpotQA, GSM8K, and CommonSenseQA; workspace entropy improved error-routing precision on PopQA but was weaker than output confidence on TruthfulQA, and thresholds calibrated on one dataset failed on others.

reddit · r/MachineLearning · /u/dasjomsyeet · Jul 13, 08:27

**Background**: Jacobian Lens is an interpretability technique developed by Anthropic that reads out what an internal activation is disposed to make the model say, providing a window into the model's internal representations. Workspace entropy refers to the entropy of the probability distribution over tokens in this internal workspace, which was hypothesized to indicate uncertainty or hallucination. Qwen3-4B is an open-source 4-billion-parameter language model from Alibaba Cloud.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/anthropics/jacobian-lens">GitHub - anthropics/jacobian-lens: Companion code for the global workspace interpretability paper · GitHub</a></li>
<li><a href="https://huggingface.co/Qwen/Qwen3-4B">Qwen/ Qwen 3 - 4 B · Hugging Face</a></li>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen</a></li>

</ul>
</details>

**Tags**: `#interpretability`, `#AI safety`, `#language models`, `#error detection`, `#Jacobian Lens`

---

<a id="item-11"></a>
## [Build and Ship Apple Apps Without Xcode](https://scottwillsey.com/building-and-shipping-mac-and-ios-apps-without-ever-opening-xcode/) ⭐️ 7.0/10

A developer demonstrates a complete workflow to build, sign, notarize, and ship Mac and iOS apps using Claude Code and command-line tools, without ever opening Xcode. This approach enables CI/CD pipelines and AI-assisted development for Apple platforms, potentially reducing reliance on Xcode's GUI and opening up new automation possibilities. The workflow uses Claude Code to generate scripts that handle archiving, Developer ID-signing, notarization, stapling, and installation, with loud failure on any step. It requires running the agent on the Mac, not in a sandbox.

hackernews · speckx · Jul 13, 18:22 · [Discussion](https://news.ycombinator.com/item?id=48896665)

**Background**: Xcode is Apple's integrated development environment (IDE) for macOS, iOS, watchOS, and tvOS apps. However, many build and signing tasks can be performed via command-line tools (xcodebuild, codesign, altool) without the GUI. Claude Code is Anthropic's agentic coding tool that can edit files, run commands, and automate workflows.

<details><summary>References</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://developer.apple.com/documentation/xcode/installing-the-command-line-tools">Installing the command-line tools - Apple Developer</a></li>

</ul>
</details>

**Discussion**: Commenters express mixed feelings: some praise the workflow's convenience, while others raise security concerns about running AI agents outside a sandbox, citing incidents like xAI uploading SSH keys. Alternative tools like xtool (for Linux) and Axiom are mentioned as complementary approaches.

**Tags**: `#iOS development`, `#CI/CD`, `#AI-assisted development`, `#Xcode alternatives`, `#security`

---

<a id="item-12"></a>
## [Real Token Costs of Frontier AI Models Compared](https://playcode.io/blog/real-price-of-frontier-models) ⭐️ 7.0/10

An analysis on Playcode.io reveals that OpenAI's tokenizer is up to 2x more efficient than Anthropic's, leading to significantly lower effective costs per token for users. This matters because developers and businesses choosing between frontier models may face hidden cost differences beyond listed prices, impacting budget planning and model selection. The analysis shows that for a ~90k LOC C++ codebase, GPT uses 1.12M tokens while Claude uses 2.2M tokens; for a ~30k LOC TypeScript codebase, GPT uses 260K tokens versus Claude's 437K tokens.

hackernews · ianberdin · Jul 13, 18:32 · [Discussion](https://news.ycombinator.com/item?id=48896800)

**Background**: Frontier AI models like GPT-4o and Claude charge per token, but tokenizers split text into tokens with varying efficiency. A more efficient tokenizer means fewer tokens for the same input, reducing actual cost. OpenAI's o200k_base tokenizer has been in use since GPT-4o launched, while Anthropic's tokenizer is reportedly less efficient.

<details><summary>References</summary>
<ul>
<li><a href="https://llm-calculator.com/blog/tokenization-performance-benchmark/">Tokenization Speed and Efficiency Benchmarks (July 2025)</a></li>

</ul>
</details>

**Discussion**: Community comments confirm the efficiency gap, with users reporting GPT's tokenizer being 1.6x to 2x better than Claude's depending on data type. Some also note that OpenAI documents its tokenizer, which is an improvement over Anthropic's lack of transparency.

**Tags**: `#AI pricing`, `#LLM costs`, `#tokenizers`, `#OpenAI`, `#Anthropic`

---

<a id="item-13"></a>
## [Sega CD Silpheed: FMV Engineering Deep Dive](https://fabiensanglard.net/silpheed/index.html) ⭐️ 7.0/10

Fabien Sanglard published a technical analysis of how Silpheed on the Sega CD used pre-rendered full motion video (FMV) and clever hardware tricks to simulate 3D graphics, despite the console lacking 3D capabilities. This article reveals the ingenious engineering behind one of the Sega CD's most visually impressive games, offering valuable insights into retro game development and the creative constraints of early 1990s hardware. The game exploited the Sega CD's tile-based graphics, limited palette, and the Mega-CD ASIC's font registers to achieve high-quality animation with only a 12.5 MHz CPU and 150 KB/s CD bandwidth. It used pre-rendered computer animation as a scrolling background, with player and enemy sprites overlaid on top.

hackernews · ibobev · Jul 13, 14:52 · [Discussion](https://news.ycombinator.com/item?id=48893639)

**Background**: The Sega CD was an add-on for the Sega Genesis that played CD-based games and added hardware like a faster CPU and a custom graphics chip for sprite scaling and rotation. Full motion video (FMV) games were common on the platform, but most were criticized for limited interactivity. Silpheed stood out by creating an illusion of 3D polygonal graphics through carefully crafted FMV sequences.

<details><summary>References</summary>
<ul>
<li><a href="https://fabiensanglard.net/silpheed/">The art and engineering of Sega CD Silpheed</a></li>
<li><a href="https://en.wikipedia.org/wiki/Silpheed">Silpheed - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Sega_CD">Sega CD - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters praised the article's technical depth and shared personal experiences with the game. One user noted the article might be slightly incorrect about the sound setup, explaining that the Mega Drive I has a sound input on the expansion port that mixes CD audio. Another commenter pointed to impressive demoscene productions on the same hardware.

**Tags**: `#retro gaming`, `#game development`, `#Sega CD`, `#technical deep-dive`, `#graphics`

---

<a id="item-14"></a>
## [Datasette Code Frequency Chart Shows AI Agent Impact](https://simonwillison.net/2026/Jul/13/datasette-code-frequency/#atom-everything) ⭐️ 7.0/10

Simon Willison shared a GitHub code frequency chart of his Datasette project, showing a massive spike in code additions and deletions in 2026 that he attributes to AI coding agents like Opus 4.8, GPT-5.5, Fable 5, and GPT-5.6 Sol. This provides concrete, visual evidence of how advanced AI coding agents can dramatically boost a developer's output, fueling ongoing debates about AI's role in software development and productivity. The largest spike shows 37,022 additions and -9,528 deletions in a single week in 2026, far exceeding any previous activity since the project began in 2018. The chart, titled "Additions and deletions per week," covers from 2018 through 2026.

rss · Simon Willison · Jul 13, 21:45

**Background**: Datasette is an open-source tool for exploring and publishing data, created by Simon Willison. GitHub's code frequency chart visualizes additions and deletions per week in a repository. AI coding agents are large language models that can autonomously write and modify code, with models like Opus 4.5 and GPT-5.5 representing cutting-edge capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://datasette.io/">Datasette: An open source multi-tool for exploring and publishing data</a></li>
<li><a href="https://github.com/simonw/datasette">GitHub - simonw/datasette: An open source multi-tool for exploring and publishing data · GitHub</a></li>
<li><a href="https://docs.github.com/en/repositories/viewing-activity-and-data-for-your-repository/about-repository-graphs">About repository graphs - GitHub Docs</a></li>

</ul>
</details>

**Tags**: `#AI-assisted coding`, `#developer productivity`, `#open source`, `#data visualization`

---

<a id="item-15"></a>
## [AI Agents Should Never Be Directly Responsible Individuals](https://simonwillison.net/2026/Jul/12/directly-responsible-individuals/#atom-everything) ⭐️ 7.0/10

Simon Willison argues that AI agents should never be designated as Directly Responsible Individuals (DRIs) because they cannot be held accountable for outcomes. This distinction is crucial for organizational accountability as AI agents become more autonomous; it reinforces the principle that only humans can bear ultimate responsibility. Willison references the GitLab handbook definition of DRI and cites IBM's 1979 training slide stating that a computer must never make a management decision because it cannot be held accountable.

rss · Simon Willison · Jul 12, 23:57

**Background**: Directly Responsible Individual (DRI) is a concept popularized at Apple, referring to the person ultimately accountable for a project's success or failure. GitLab's handbook defines DRIs as individuals who own specific projects or initiatives. The term is widely used in tech companies to clarify ownership and accountability.

<details><summary>References</summary>
<ul>
<li><a href="https://handbook.gitlab.com/handbook/people-group/directly-responsible-individuals/">Directly Responsible Individuals (DRI) | The GitLab Handbook</a></li>
<li><a href="https://tettra.com/article/directly-responsible-individuals-guide/">Directly Responsible Individuals : The What, How and Why of DRIs</a></li>
<li><a href="https://www.bitesizelearning.co.uk/resources/directly-responsible-individual-dri-apple">Using the Directly Responsible Individual ( DRI ) concept at work...</a></li>

</ul>
</details>

**Tags**: `#accountability`, `#AI agents`, `#organizational culture`, `#software engineering`

---

<a id="item-16"></a>
## [Prompt-Engineering Paper on Mode Collapse Accepted to ICML](https://www.reddit.com/r/MachineLearning/comments/1uv1xb3/promptengineering_paper_accepted_to_icml_r/) ⭐️ 6.0/10

A paper titled 'Verbalized Sampling: How to Mitigate Mode Collapse and Unlock LLM Diversity' was accepted to ICML 2025, proposing a simple prompt-engineering trick to increase output diversity without retraining. This acceptance sparks debate about whether prompt-engineering papers, which often lack theoretical rigor, belong at top-tier machine learning conferences like ICML, potentially reshaping the field's standards. The technique, called Verbalized Sampling, involves modifying the prompt to encourage more diverse responses, recovering up to 66% of diversity according to some reports, but the paper provides no rigorous theoretical analysis.

reddit · r/MachineLearning · /u/Mean_Revolution1490 · Jul 13, 05:00

**Background**: Mode collapse in LLMs refers to the phenomenon where aligned models produce a narrow set of responses, often due to reinforcement learning from human feedback (RLHF). Prompt engineering involves crafting inputs to guide model behavior without changing model weights. ICML is a top-tier conference for machine learning research.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2510.01171">Verbalized Sampling: How to Mitigate Mode Collapse and Unlock LLM...</a></li>
<li><a href="https://www.analyticsvidhya.com/blog/2025/10/verbalized-sampling/">RIP Prompt Engineering: The New Skill is Verbalized Sampling</a></li>
<li><a href="https://www.emergentmind.com/topics/semantic-mode-collapse">Semantic Mode Collapse in Generative Models</a></li>

</ul>
</details>

**Discussion**: The Reddit post questions whether such a simple trick without theoretical depth belongs at ICML. Commenters are divided: some argue it's 'modern machine learning' and empirically valuable, while others agree it should be in less technical venues.

**Tags**: `#prompt engineering`, `#LLM`, `#ICML`, `#machine learning`, `#mode collapse`

---

<a id="item-17"></a>
## [LLMs and CS PhD Completion Times](https://www.reddit.com/r/MachineLearning/comments/1uvhr7a/fast_track_through_a_cs_phd_using_llms_for_paper/) ⭐️ 5.0/10

A Reddit user asks whether large language models (LLMs) are enabling CS PhD students to finish their degrees faster by simplifying paper writing and running experiments. If LLMs significantly reduce the time needed for writing and experimentation, it could reshape PhD timelines and productivity norms in CS research. The post is speculative and lacks concrete data or examples; it invites community discussion on whether observed trends match the hypothesis.

reddit · r/MachineLearning · /u/Alone_Reality3726 · Jul 13, 17:15

**Background**: A CS PhD typically involves coursework, original research, writing papers, and a dissertation. LLMs can assist with drafting, editing, and even generating code for experiments, potentially speeding up these tasks.

**Tags**: `#LLMs`, `#PhD`, `#CS research`, `#productivity`

---

<a id="item-18"></a>
## [shot-scraper 1.11: Improved Server Startup and JS File Option](https://simonwillison.net/2026/Jul/12/shot-scraper/#atom-everything) ⭐️ 3.0/10

shot-scraper 1.11 introduces a 30-second server startup timeout, replacing the previous one-second fixed delay, and adds a --js-file option for loading JavaScript from files or standard input. This release improves reliability for automated screenshot workflows that depend on a local server, reducing failures when servers take longer to start. The --js-file option enhances scripting flexibility for users who prefer external JavaScript files. The server polling mechanism now waits up to 30 seconds for port availability, addressing issue #197. The --js-file option supports local files, standard input, and gh:username/script shorthand, as an alternative to the existing --javascript argument.

rss · Simon Willison · Jul 12, 23:46

**Background**: shot-scraper is a command-line tool for taking automated screenshots of websites, built on Playwright. It supports single screenshots, multi-shot YAML configurations, and video capture, often used for documentation and web scraping. The server: mechanism allows running a temporary local server during multi or video sessions.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jul/12/shot-scraper/">Release: shot-scraper 1.11</a></li>
<li><a href="https://shot-scraper.datasette.io/">shot - scraper</a></li>

</ul>
</details>

**Tags**: `#release`, `#tooling`, `#web scraping`

---

<a id="item-19"></a>
## [ECCV 2026 Authorized Delegate Policy Clarification](https://www.reddit.com/r/MachineLearning/comments/1uv31uj/eccv_2026_meaning_of_authorized_delegate/) ⭐️ 3.0/10

A Reddit user whose paper was provisionally accepted to ECCV 2026 asks for clarification on the 'authorized delegate' policy, as none of the authors can attend in person due to US immigration issues. This highlights a common logistical challenge for international researchers, especially those with visa restrictions, and the need for clear conference policies on delegate presentation to avoid paper withdrawal. ECCV 2026 requires each paper to be presented in person by an author or an authorized delegate, and a full author registration (non-student, non-virtual) is required by July 17, 2026. The user asks whether a colleague already attending can serve as delegate, if the delegate needs separate registration, and how to formally notify the conference.

reddit · r/MachineLearning · /u/Latter-Sympathy7767 · Jul 13, 06:00

**Background**: ECCV (European Conference on Computer Vision) is a top-tier biennial computer vision conference. Many conferences require in-person presentation to ensure engagement and quality. 'Authorized delegate' typically means a person designated by the authors to present the paper, often a colleague from the same institution who is already registered. The exact definition and process vary by conference.

<details><summary>References</summary>
<ul>
<li><a href="https://eccv.ecva.net/Conferences/2026/SubmissionPolicies">ECCV 2026 Submission Policies</a></li>
<li><a href="https://eccv.ecva.net/Conferences/2026/CallForPapers">ECCV 2026 Call for Papers</a></li>

</ul>
</details>

**Tags**: `#ECCV`, `#conference policy`, `#academic publishing`

---