---
layout: default
title: "Horizon Summary: 2026-09-07 (EN)"
date: 2026-09-07
lang: en
---

> From 15 items, 15 important content pieces were selected

---

1. [LG Smart TVs Caught Logging Audio and Scanning Networks](#item-1) ⭐️ 8.0/10
2. [OpenAI Reveals Coding Agents Reshaping Research, RSI on the Horizon](#item-2) ⭐️ 8.0/10
3. [LLM-guided evolution improves 10 circle-packing solutions](#item-3) ⭐️ 8.0/10
4. [Yandex Proposes KV Cache as Agent Runtime for Interactive LLMs](#item-4) ⭐️ 8.0/10
5. [LLM Performance Drift: 31,352 Runs Reveal Temporal Variability](#item-5) ⭐️ 8.0/10
6. [Interactive Map Shows LA Building Construction from 1880 to 2026](#item-6) ⭐️ 7.0/10
7. [Caltech Hosts First Hackathon for Research-Level Math with AI](#item-7) ⭐️ 7.0/10
8. [Linux Kernel Git Server Overwhelmed by Abusive Crawlers](#item-8) ⭐️ 7.0/10
9. [OpenAI Chief Scientist Advocates for Defensive AI, Warns Against Reckless Racing](#item-9) ⭐️ 7.0/10
10. [Rustuna: High-Performance Rust Implementation of Optuna Released](#item-10) ⭐️ 7.0/10
11. [IEEE T-PAMI Paper Rejected Despite 'Excellent' Scores Due to Ghost Reviewer](#item-11) ⭐️ 7.0/10
12. [Browser-Based Video Compressor Built with WebAssembly FFMPEG and Claude Code](#item-12) ⭐️ 6.0/10
13. [Animated Mercator to Equal Earth Transition Built with GPT-6 Astra](#item-13) ⭐️ 6.0/10
14. [How Frontier LLMs and VLAs Are Shaping Learning-from-Demonstrations Research](#item-14) ⭐️ 6.0/10
15. [Radar Engineer Shares MLP Classifier for Automotive Radar Point Clouds](#item-15) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [LG Smart TVs Caught Logging Audio and Scanning Networks](https://www.youtube.com/watch?v=6IFVTcM28KA) ⭐️ 8.0/10

An investigation by Gamers Nexus revealed that LG smart TVs, including the flagship G5 OLED, log audio even when the screen is off and actively scan local networks for nearby devices such as smartphones and smartwatches. The findings were detailed in a 135-minute video and corroborated by multiple tech news outlets. This raises serious privacy concerns for the estimated 216 million LG smart TV users worldwide, as the devices may capture sensitive audio and network information without explicit user consent. It underscores the broader issue of smart devices collecting data in ways that users may not anticipate, potentially leading to regulatory scrutiny and a push for more transparent data practices. The investigation used Wireshark packet captures on retail LG OLED models, including the G5, and observed the TVs scanning the LAN for unrelated hardware. The TVs also captured microphone audio with the screen off, uploading data once reconnected to the internet. LG's terms of service reportedly require users to notify household members and guests about potential eavesdropping.

hackernews · treve · Sep 7, 00:22 · [Discussion](https://news.ycombinator.com/item?id=49592375)

**Background**: Smart TVs are internet-connected televisions that often include voice recognition and network features. While such features can enhance user experience, they also introduce privacy risks if data is collected and transmitted without clear consent. This investigation highlights the importance of understanding device capabilities and terms of service, as well as the potential legal implications under wiretap laws.

<details><summary>References</summary>
<ul>
<li><a href="https://cybersecuritynews.com/lg-smart-tvs-caught-scanning-networks/">LG Smart TVs Caught Scanning Networks and Logging Audio in Standby</a></li>
<li><a href="https://www.notebookcheck.net/LG-smart-TVs-caught-logging-audio-with-screen-off-and-snooping-on-local-devices.1391214.0.html">LG smart TVs caught logging audio with screen off and snooping on local ...</a></li>
<li><a href="https://cyberinsider.com/lg-smart-tvs-found-scanning-home-networks-for-nearby-devices/">LG Smart TVs found scanning home networks for nearby devices</a></li>

</ul>
</details>

**Discussion**: Community comments express outrage and concern, with users sharing experiences of disabling network functions or physically unplugging WiFi/BT chips. Some highlight the contractual obligation to inform guests about eavesdropping, while others question the legality under wiretap laws and call for accountability.

**Tags**: `#privacy`, `#smart TV`, `#LG`, `#security`, `#surveillance`

---

<a id="item-2"></a>
## [OpenAI Reveals Coding Agents Reshaping Research, RSI on the Horizon](https://simonwillison.net/2026/Sep/6/research-acceleration-the-view-inside-openai/) ⭐️ 8.0/10

OpenAI published a blog post detailing how coding agents have transformed their research workflows, with a chart showing daily AI spend per researcher surging from near zero in early 2026 to roughly $600 by late August. The post also introduces 'Recursive Self-Improvement' (RSI) as a key focus, alongside a companion essay by Chief Scientist Jakub Pachocki titled 'An Alien Mind.' This signals a major shift in AI research practices, as OpenAI's internal adoption of coding agents and focus on RSI could accelerate the pace of AI development industry-wide. It highlights the growing importance of agentic engineering and raises both opportunities and safety concerns about systems that can improve themselves. The chart shows a steep acceleration in late July 2026, which the author speculates may coincide with internal access to the model later released as GPT-6 Astra. The post does not expand the acronym RSI, assuming readers are familiar with the concept of recursive self-improvement.

rss · Simon Willison · Sep 6, 23:57

**Background**: Recursive self-improvement (RSI) is a hypothesized process where an AGI system rewrites its own code to enhance its capabilities, potentially leading to an intelligence explosion. Coding agents are AI tools that assist developers by writing or modifying code, and their use has grown rapidly in 2026, as reflected in OpenAI's internal data.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Recursive_self-improvement">Recursive self-improvement</a></li>
<li><a href="https://www.anthropic.com/institute/recursive-self-improvement">When AI builds itself \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#AI research`, `#coding agents`, `#recursive self-improvement`, `#agentic engineering`

---

<a id="item-3"></a>
## [LLM-guided evolution improves 10 circle-packing solutions](https://www.reddit.com/r/MachineLearning/comments/1w9xlyi/llmguided_program_evolution_improves_10_bestknown/) ⭐️ 8.0/10

An LLM-guided program evolution approach improved the best-known sum-of-radii for 10 values of N (101-114) on the Packomania csqv benchmark, with improvements of 2.4% to 5.4% achieved in 15 iterations at a total LLM cost of $27.72. The results were independently accepted by Packomania. This demonstrates a novel and cost-effective application of LLMs to evolve optimization algorithms, achieving concrete improvements on a recognized benchmark. It highlights the potential of LLM-guided program evolution as a general tool for solving complex optimization problems, which could impact fields like operations research and computational geometry. The approach starts from a simple seed solver and iteratively proposes algorithmic changes guided by a scoreboard and history, with each candidate scored by an independent verifier. The paper is available at arxiv.org/abs/2609.05093, and code and solutions are on GitHub at github.com/ucsandman/discovery-loop.

reddit · r/MachineLearning · /u/SIGH_I_CALL · Sep 7, 16:54

**Background**: Circle packing is a classic optimization problem where circles are arranged inside a container to maximize or minimize a certain objective, such as the sum of radii. Packomania is a well-known benchmark site for such problems. LLM-guided program evolution is a technique where a large language model iteratively proposes modifications to a program, which are then evaluated, allowing the algorithm to improve over time.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2609.05093">LLM - Guided Program Evolution for Circle Packing:Breaking 10...</a></li>
<li><a href="https://packomania.com/">Packomania (52C17)</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#program evolution`, `#optimization`, `#circle packing`, `#AI research`

---

<a id="item-4"></a>
## [Yandex Proposes KV Cache as Agent Runtime for Interactive LLMs](https://www.reddit.com/r/MachineLearning/comments/1w9myqc/kv_cache_as_an_agent_runtime_r/) ⭐️ 8.0/10

Yandex Research has proposed using KV cache manipulation as an agent runtime to achieve more interactive LLM systems, and released a blog post and a preview of an agent playing DOOM using a Qwen3.8-27B model. This introduces a novel axis for LLM agent design—model inference/runtime—alongside models and harnesses, potentially enabling more responsive and interactive AI applications. It could inspire further research into runtime-level optimizations for agent capabilities. The approach builds on prior work from the same lab, including Hogwild! Inference and AsyncReasoning, and leverages KV cache manipulation to modify the model's inference state. The preview demonstrates an agent interactively playing DOOM, highlighting the technique's potential for real-time control.

reddit · r/MachineLearning · /u/_puhsu · Sep 7, 09:03

**Background**: KV cache is a key-value cache used in transformer-based LLMs to store attention computations, enabling efficient autoregressive generation. Traditional agent designs focus on the model or the harness (e.g., frameworks like LangGraph), but this work suggests that manipulating the inference state itself could offer a middle ground for achieving interactivity without retraining or heavy abstraction.

<details><summary>References</summary>
<ul>
<li><a href="https://research.yandex.com/publications/hogwild-inference-parallel-llm-generation-via-concurrent-attention">Hogwild ! Inference : Parallel LLM Generation via Concurrent Attention</a></li>
<li><a href="https://arxiv.org/abs/2504.06261">Hogwild ! Inference : Parallel LLM Generation via Concurrent Attention</a></li>

</ul>
</details>

**Tags**: `#KV cache`, `#LLM agents`, `#inference`, `#interactive AI`, `#research`

---

<a id="item-5"></a>
## [LLM Performance Drift: 31,352 Runs Reveal Temporal Variability](https://www.reddit.com/r/MachineLearning/comments/1w9llr4/measuring_llm_performance_drift_observations_and/) ⭐️ 8.0/10

A study measured LLM performance drift using 31,352 repeated benchmark observations across 49 models, finding within-day standard deviation of 2.80 points and between-day daily median standard deviation of 8.43 points. The authors propose a longitudinal evaluation methodology instead of static leaderboards. This highlights that API-served LLM scores are not stable over time, challenging the reliability of static leaderboards for model comparison. It underscores the need for continuous monitoring and change detection in production ML systems. The methodology includes versioned benchmark configurations, repeated execution-based evaluation, separation of availability failures from valid outcomes, and tracking serving/version metadata. The authors also address benchmark contamination by withholding the exact live task bank while publishing methodology.

reddit · r/MachineLearning · /u/ionutvi · Sep 7, 07:44

**Background**: LLM benchmarks are typically static snapshots, but API-served models can change due to infrastructure updates, version changes, or silent behavior shifts. Longitudinal evaluation treats benchmarking as a time-series problem, measuring drift and variability over time. This approach is relevant for MLOps and production monitoring, where detecting performance degradation is critical.

<details><summary>References</summary>
<ul>
<li><a href="https://data-today.net/llm-performance-drift-benchmark-variance/">LLM performance drift : why your benchmark scores... | Data Today</a></li>
<li><a href="https://github.com/liyucheng09/llm-compressive">GitHub - liyucheng09/llm-compressive: Longitudinal Evaluation of LLMs via Data Compression · GitHub</a></li>
<li><a href="https://cameronrwolfe.substack.com/p/llm-bench">The Anatomy of an LLM Benchmark - Deep (Learning) Focus</a></li>

</ul>
</details>

**Discussion**: The Reddit post invites technical criticism on methodology, including questions about using daily medians vs. individual observations, distinguishing model drift from provider effects, and balancing benchmark transparency with contamination prevention. Community responses likely discuss these methodological challenges and suggest alternative approaches.

**Tags**: `#LLM`, `#benchmarking`, `#performance drift`, `#evaluation`, `#MLOps`

---

<a id="item-6"></a>
## [Interactive Map Shows LA Building Construction from 1880 to 2026](https://lax-skyline.parcelscope.net/) ⭐️ 7.0/10

An interactive map at lax-skyline.parcelscope.net visualizes the construction dates of buildings in Los Angeles from 1880 to 2026, allowing users to explore urban growth patterns over time. The map highlights the city's development and has sparked discussions about zoning policies and historical data. This visualization offers a unique perspective on Los Angeles' urban development, making it easier for residents, planners, and researchers to understand how zoning decisions and historical events have shaped the city. It also encourages public engagement with urban planning and data transparency. The map appears to be based on data from the Los Angeles County Assessor's portal, which records construction dates for existing properties. However, it only shows buildings that are still standing, which may underrepresent older neighborhoods that have been redeveloped.

hackernews · rustywasm · Sep 7, 18:52 · [Discussion](https://news.ycombinator.com/item?id=49601655)

**Background**: Los Angeles has a complex urban history, including a massive streetcar network that was largely dismantled in the mid-20th century, and significant zoning changes in the 1980s that limited housing density. The map's data source is the LA County Assessor's office, which tracks property characteristics for tax purposes.

**Discussion**: Commenters noted that the map only shows surviving buildings, making older periods appear emptier than they were, and pointed out that neighborhoods like Palms have been completely rebuilt. Others discussed LA's historical public transportation network and the impact of downzoning on housing affordability, with some suggesting that the map provides a valuable but incomplete picture of the city's development.

**Tags**: `#visualization`, `#urban planning`, `#Los Angeles`, `#history`, `#data`

---

<a id="item-7"></a>
## [Caltech Hosts First Hackathon for Research-Level Math with AI](https://mathathonchallenge.com/index.html) ⭐️ 7.0/10

Caltech undergraduate students are organizing the Mathathon, described as the first hackathon ever devoted to research-level mathematics, with a focus on promoting responsible AI use in mathematical discovery. The event invites participants to work on open mathematical problems over a 40-hour period. This event highlights a novel intersection of AI and mathematics, potentially setting a precedent for how hackathons can be used to advance research-level math. It also addresses the growing need for guidelines on responsible AI use in mathematical research, a topic of increasing debate in the community. The organizers are Caltech undergraduates acting independently, not representing Caltech or sponsors, and receive no monetary compensation; all funding goes to judges and participants. The event's FAQ outlines commitments to responsible AI use, and the format involves teams working on problems for 40 hours.

hackernews · astroanax · Sep 7, 09:26 · [Discussion](https://news.ycombinator.com/item?id=49596055)

**Background**: Hackathons are typically intensive, short-term events where participants collaborate on coding projects, often with a focus on software development. In mathematics, AI tools like large language models are increasingly used to assist with conjecture generation, proof checking, and exploring problems, but their integration into research raises questions about reliability and ethics. The Mathathon aims to explore these issues in a hackathon setting, encouraging participants to leverage AI responsibly.

<details><summary>References</summary>
<ul>
<li><a href="https://cctest.ai/en/articles/in-mathematical-discovery-finding-the-right-problem-may-be-the-real-bottleneck">How FAR Uses AI to Triage Open Math Problems - CCTest</a></li>
<li><a href="https://spectrum.ieee.org/ai-in-mathematics">AI in Mathematics Is Forcing Big Questions - IEEE Spectrum</a></li>
<li><a href="https://arxiv.org/html/2511.07420">ADVANCING MATHEMATICS RESEARCHWITH GENERATIVE AI</a></li>

</ul>
</details>

**Discussion**: Community comments include an AMA from an organizer clarifying the event's independent nature and funding model, and a recent Caltech grad noting the weak CS department as motivation for the event. Some commenters express skepticism about the hackathon format for LLM-based math progress, while others see it as a useful testbed for AI reasoning harnesses.

**Tags**: `#hackathon`, `#mathematics`, `#AI`, `#Caltech`, `#research`

---

<a id="item-8"></a>
## [Linux Kernel Git Server Overwhelmed by Abusive Crawlers](https://simonwillison.net/2026/Sep/7/creepy-crawlies/) ⭐️ 7.0/10

Konstantin Ryabitsev reported that git.kernel.org, the official Git server for the Linux kernel, now spends more CPU cycles rendering commit pages for scrapers than on all legitimate access, including git clones. At any given time, across five geo-distributed nodes, 14 CPU cores are dedicated solely to rendering git commits as HTML for these crawlers. This highlights a growing operational burden on critical open-source infrastructure caused by abusive web scrapers, which can degrade performance for legitimate users and increase costs. It underscores the need for better bot management and raises concerns for other projects that serve large numbers of crawlable pages, such as Datasette. The report specifically mentions that the CPU usage is for rendering commits as HTML, which is a resource-intensive operation. The problem is not that the information is secret—it is already accessible via Git—but that automated systems request millions of individually rendered web pages, causing excessive load.

rss · Simon Willison · Sep 7, 23:08

**Background**: git.kernel.org is the official hosting site for the Linux kernel source code, operated by the Linux Kernel Organization. It provides web interfaces for browsing commits and other data, which are convenient for humans but are also targeted by scrapers that harvest data at scale. The Linux kernel project has been exploring solutions like Anubis, a proof-of-work challenge system, to deter such abusive crawling.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kernel.org/">The Linux Kernel Archives</a></li>
<li><a href="https://en.wikipedia.org/wiki/Anubis_(software)">Anubis (software) - Wikipedia</a></li>
<li><a href="https://www.linux.se/tag/scrapers/">scrapers – Linux.se :Allt om Linux – på svenska.</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion likely includes debates about the scale of the problem, potential countermeasures, and the broader impact of AI training scrapers on web infrastructure. Some may argue that the issue is exaggerated or that better caching could help, while others emphasize the need for industry-wide standards on bot behavior.

**Tags**: `#crawling`, `#git`, `#Linux kernel`, `#web infrastructure`, `#scraping`

---

<a id="item-9"></a>
## [OpenAI Chief Scientist Advocates for Defensive AI, Warns Against Reckless Racing](https://simonwillison.net/2026/Sep/7/jakub-pachocki/) ⭐️ 7.0/10

Jakub Pachocki, OpenAI's Chief Scientist, publicly argued that powerful aligned AI is needed for defense against other AI threats, while cautioning that this necessity must not justify reckless acceleration of AI development. His remarks were excerpted from an OpenAI blog post titled 'An Alien Mind'. This statement from a top OpenAI leader signals a strategic emphasis on defensive AI applications, potentially shaping industry priorities and policy discussions. It highlights a growing tension between the urgency to build safeguards and the risks of uncontrolled AI advancement. Pachocki specifically mentioned securing infrastructure, protecting against rogue agents in real time, and inventing new protective measures as key defensive goals. He also emphasized that 'racing forward at all costs' is 'absurd' given the seriousness of the stakes, reflecting a nuanced position within OpenAI's leadership.

rss · Simon Willison · Sep 7, 22:26

**Background**: AI alignment refers to ensuring AI systems act in accordance with human intentions and values. OpenAI has recently launched initiatives like the Defense Factory and the $1 billion Daybreak Initiative to bolster cyber defense using AI, aligning with Pachocki's call for defensive systems.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/the-defense-factory/">Defense Factory | OpenAI</a></li>
<li><a href="https://cyberpress.org/openai-launches-1-billion-daybreak-initiative/">OpenAI Launches $1 Billion Daybreak Initiative for Critical Infrastructure Cyber Defense</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#OpenAI`, `#AI ethics`, `#AI policy`

---

<a id="item-10"></a>
## [Rustuna: High-Performance Rust Implementation of Optuna Released](https://www.reddit.com/r/MachineLearning/comments/1w9nyhz/rustuna_a_highperformance_rust_implementation_of/) ⭐️ 7.0/10

The Optuna team has released Rustuna, a high-speed, memory-efficient implementation of Optuna written in Rust. It is designed to be API-compatible with Optuna and has zero Python dependencies. This brings Optuna's hyperparameter optimization capabilities to the Rust ecosystem, offering performance and security benefits. It addresses pain points like memory footprint and supply chain risks, which is significant for production ML systems. Rustuna is available on GitHub at https://github.com/optuna/rustuna/ and is announced via a Medium blog post. It retains the familiar Optuna API and concept while optimizing memory management natively in Rust.

reddit · r/MachineLearning · /u/c-bata · Sep 7, 10:01

**Background**: Optuna is an open-source Python library for automatic hyperparameter tuning, first introduced in 2018 by Preferred Networks. Rust is a general-purpose programming language that emphasizes performance, type safety, concurrency, and memory safety. Rustuna aims to combine Optuna's optimization algorithms with Rust's efficiency and safety.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Optuna">Optuna - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Rust_(programming_language)">Rust ( programming language ) - Wikipedia</a></li>
<li><a href="https://github.com/optuna/optuna">GitHub - optuna/optuna: A hyperparameter optimization framework · GitHub</a></li>

</ul>
</details>

**Tags**: `#Rust`, `#Optuna`, `#Hyperparameter Optimization`, `#Machine Learning`, `#Open Source`

---

<a id="item-11"></a>
## [IEEE T-PAMI Paper Rejected Despite 'Excellent' Scores Due to Ghost Reviewer](https://www.reddit.com/r/MachineLearning/comments/1w9v43o/update_eic_confirmed_ghost_reviewerhow_to_get/) ⭐️ 7.0/10

A researcher reported that their IEEE T-PAMI paper, which received 'Excellent' scores from reviewers, was rejected due to a ghost reviewer, and the editor-in-chief (EIC) confirmed this irregularity. This incident was shared on Reddit, sparking discussions about the integrity of the peer review process. This case highlights a potential flaw in the peer review system of a top-tier journal like IEEE T-PAMI, which could undermine trust in academic publishing. It raises concerns about fairness and transparency, affecting researchers who rely on such venues for career advancement and knowledge dissemination. The paper reportedly received 'Excellent' scores from all assigned reviewers, yet was rejected due to an additional 'ghost reviewer' whose identity was not disclosed. The EIC confirmed the existence of this ghost reviewer, but the specific reasons for the rejection remain unclear, and the process lacks transparency.

reddit · r/MachineLearning · /u/cussealin · Sep 7, 15:22

**Background**: IEEE Transactions on Pattern Analysis and Machine Intelligence (T-PAMI) is a prestigious monthly peer-reviewed journal published by the IEEE Computer Society, focusing on pattern analysis and machine intelligence. Typically, the journal uses three reviewers, but this incident suggests an undisclosed additional reviewer influenced the decision, raising questions about standard review protocols.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/IEEE_Transactions_on_Pattern_Analysis_and_Machine_Intelligence">IEEE Transactions on Pattern Analysis and Machine Intelligence - Wikipedia</a></li>
<li><a href="https://manusights.com/blog/ieee-transactions-on-pattern-analysis-and-machine-intelligence-under-review">IEEE TPAMI Under Review: Status Meanings (2026)</a></li>

</ul>
</details>

**Discussion**: The Reddit community expressed shock and concern, with many questioning the legitimacy of ghost reviewers and calling for greater transparency in the review process. Some commenters shared similar experiences, while others debated potential reasons for such decisions, such as editorial bias or conflicts of interest.

**Tags**: `#academic publishing`, `#peer review`, `#IEEE T-PAMI`, `#research ethics`, `#machine learning`

---

<a id="item-12"></a>
## [Browser-Based Video Compressor Built with WebAssembly FFMPEG and Claude Code](https://simonwillison.net/2026/Sep/7/video-compressor/) ⭐️ 6.0/10

Simon Willison shared a browser-based video compressor tool that uses the WebAssembly build of FFMPEG, which he had Claude Fable 5.1 in Claude Code for web build for him. The tool generates multiple compressed versions of a video with presets ranging from Largest to Smallest, and the demo compressed a video to as small as 145 KB (48% of original) in about 11.8 seconds. This tool demonstrates the practical application of WebAssembly and AI-assisted coding, enabling developers and content creators to compress videos directly in the browser without server-side processing or installing FFMPEG. It highlights the growing trend of running complex multimedia tasks client-side and the increasing capability of AI tools like Claude Code to generate functional utilities from natural language requests. The tool offers five presets (Largest, Large, Medium, Small, Smallest) with output resolutions of 854×370 or 640×276, CRF quality settings from 22 to 28, and audio bitrates from 128 to 64 kbps. It also includes options for encoder speed, H.264 profile, 30 fps limit, stripping metadata, dropping audio, and encoding only the first 10 seconds, with each result showing the ffmpeg command used.

rss · Simon Willison · Sep 7, 18:29

**Background**: FFmpeg is a powerful command-line tool for handling video, audio, and other multimedia files, but it typically requires installation and command-line usage. WebAssembly (Wasm) allows C/C++ code to be compiled to run in web browsers, and projects like ffmpeg.wasm port FFmpeg to the browser, enabling client-side video processing. Claude Code is an AI-assisted coding tool by Anthropic that can generate code based on natural language prompts, and in this case, it helped build the video compressor tool.

<details><summary>References</summary>
<ul>
<li><a href="https://ffmpegwasm.netlify.app/docs/overview/">Overview | ffmpeg .wasm</a></li>
<li><a href="https://github.com/ffmpegwasm/ffmpeg.wasm">GitHub - ffmpegwasm/ ffmpeg .wasm: FFmpeg for browser, powered by...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>

</ul>
</details>

**Tags**: `#video compression`, `#WebAssembly`, `#FFMPEG`, `#Claude Code`, `#developer tools`

---

<a id="item-13"></a>
## [Animated Mercator to Equal Earth Transition Built with GPT-6 Astra](https://simonwillison.net/2026/Sep/7/equal-earth/) ⭐️ 6.0/10

Simon Willison released an animated D3 tool that smoothly transitions between the Mercator and Equal Earth map projections, built with GPT-6 Astra (medium) in ChatGPT Work. The tool was created in response to a recent UN vote encouraging the use of equal-area projections. This tool provides an intuitive visual comparison of two important map projections, helping users understand the distortions inherent in the widely used Mercator projection. It also showcases the potential of AI-assisted coding for creating interactive geospatial visualizations quickly. The tool is hosted at tools.simonwillison.net/equal-earth and uses D3.js to interpolate between projections. The transition is animated in a video preview, and the code was generated via a ChatGPT share link, highlighting a 'vibe-coding' approach.

rss · Simon Willison · Sep 7, 16:24

**Background**: The Mercator projection, introduced in 1569, preserves angles and shapes but severely distorts area, making landmasses near the poles appear much larger than they are. The Equal Earth projection, invented in 2018, is an equal-area pseudocylindrical projection that preserves relative sizes while maintaining a visually pleasing shape. In September 2026, the UN General Assembly voted on a resolution encouraging the use of equal-area projections, specifically noting Equal Earth, which may influence educational and technological applications.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Equal_Earth_map_projection">Equal Earth map projection</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mercator_projection">Mercator projection - Wikipedia</a></li>
<li><a href="https://observablehq.com/@d3/projection-transitions">Projection Transitions / D3 | Observable</a></li>

</ul>
</details>

**Tags**: `#geospatial`, `#d3`, `#data-visualization`, `#map-projections`, `#AI-assisted-coding`

---

<a id="item-14"></a>
## [How Frontier LLMs and VLAs Are Shaping Learning-from-Demonstrations Research](https://www.reddit.com/r/MachineLearning/comments/1w9lt31/roboticists_working_in_learningfromdemonstrations/) ⭐️ 6.0/10

A Reddit discussion in r/MachineLearning asks roboticists how recent advances in frontier LLMs and Vision-Language-Action models (VLAs) are influencing research in learning-from-demonstrations (LfD) and behavioral cloning (BC). The thread seeks community insights on whether these fields are converging or evolving independently. This discussion highlights a potential paradigm shift in robotics, where large pretrained models may replace or augment traditional imitation learning methods. The outcome could influence how future robotic policies are trained, making them more generalizable and capable of following natural language instructions. The post specifically asks about the impact of ViTs (Vision Transformers) and VLAs, and whether LfD/BC research is proceeding independently of frontier LLMs. No community responses are provided in the given content, so the discussion's value depends on the quality of replies, which are not available here.

reddit · r/MachineLearning · /u/moschles · Sep 7, 07:56

**Background**: Learning-from-demonstrations (LfD) and behavioral cloning (BC) are imitation learning techniques where robots learn policies from expert demonstrations. Behavioral cloning uses supervised learning to map observations to actions. Vision-Language-Action models (VLAs) are end-to-end models that take camera images and natural language instructions as input and directly output robot actions, leveraging pretrained LLMs and visual encoders to generalize across tasks and embodiments.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/cns-tech-prism-vlms-vlas-architecture-behind-robot-intelligence-n8koc">[CNS Tech Prism] VLMs and VLAs : The Architecture Behind Robot ...</a></li>
<li><a href="https://www.smashingrobotics.com/what-are-vision-language-action-models-in-robotics/">Vision Language Action Models in Robotics (September 2026 Guide)</a></li>
<li><a href="https://arxiv.org/html/2408.10568v1">Constrained Behavior Cloning for Robotic Learning</a></li>

</ul>
</details>

**Tags**: `#robotics`, `#learning-from-demonstrations`, `#behavioral cloning`, `#LLMs`, `#VLAs`

---

<a id="item-15"></a>
## [Radar Engineer Shares MLP Classifier for Automotive Radar Point Clouds](https://www.reddit.com/r/MachineLearning/comments/1w9m26u/automotive_radar_object_classification_p/) ⭐️ 6.0/10

A radar signal processing engineer trained a 5-class MLP classifier on RadarScenes radar point clouds, using per-scan histograms and class-weighted cross-entropy loss. The model achieved macro F1 scores ranging from 0.381 to 0.764 depending on the number of radar detections per instance. This work highlights practical challenges in automotive radar object classification, such as class imbalance and sequence bias, which are critical for developing robust perception systems in autonomous driving. The findings can guide other practitioners in designing more effective radar-based classifiers. The classifier uses a 3-layer MLP with 16-bin histograms as input, and the author found that split sensitivity caused more performance variation than architectural changes. Two-wheelers are often confused with pedestrians due to overlapping velocity distributions, and stationary two-wheelers are indistinguishable from pedestrians.

reddit · r/MachineLearning · /u/bruno_pinto90 · Sep 7, 08:10

**Background**: RadarScenes is a real-world radar point cloud dataset for automotive applications, providing data for tasks like object classification. Radar point clouds are sparse and noisy, and classifying objects such as cars, pedestrians, and two-wheelers is challenging due to varying detection counts and class imbalance. Class-weighted cross-entropy loss is a common technique to address imbalanced datasets by assigning higher weights to minority classes.

<details><summary>References</summary>
<ul>
<li><a href="https://www.researchgate.net/publication/359411890_RadarScenes_A_Real-World_Radar_Point_Cloud_Data_Set_for_Automotive_Applications">RadarScenes: A Real-World Radar Point Cloud Data Set for Automotive Applications | Request PDF</a></li>
<li><a href="https://arxiv.org/html/2104.02493v2">RadarScenes: A Real-World Radar Point Cloud Data Set for Automotive Applications</a></li>
<li><a href="https://www.emergentmind.com/topics/weighted-cross-entropy-loss">Weighted Cross-Entropy Loss Techniques</a></li>

</ul>
</details>

**Tags**: `#automotive radar`, `#machine learning`, `#classification`, `#radar point clouds`

---