---
layout: default
title: "Horizon Summary: 2026-09-01 (EN)"
date: 2026-09-01
lang: en
---

> From 19 items, 16 important content pieces were selected

---

1. [Google Removes MV2 Extensions from Chrome Web Store, Including uBlock Origin](#item-1) ⭐️ 8.0/10
2. [Sliding-Window Attention Outperforms Linear Attention on Long-Context Reasoning](#item-2) ⭐️ 8.0/10
3. [GNNs on Dynamic Graphs Suffer Temporal Leakage; SynthFin-AML Enforces Causal Boundaries](#item-3) ⭐️ 8.0/10
4. [Turning Security Cameras into an Automatic Bird Identification System](#item-4) ⭐️ 7.0/10
5. [Apple Surprised by AI-Driven Demand for Mac Mini and Mac Studio](#item-5) ⭐️ 7.0/10
6. [ChatGPT Work Skill Reference Site Highlights Playwright Browser Control](#item-6) ⭐️ 7.0/10
7. [Military Commissary Freezer Failures Spark Hacking Speculation](#item-7) ⭐️ 7.0/10
8. [Wrapture: New Python Library Extends Monkeypatching to Testing and Tracing](#item-8) ⭐️ 7.0/10
9. [Entropic Scree: New Tool to Assess Signal in Dirty Data](#item-9) ⭐️ 7.0/10
10. [Playa Phone: A Burning Man Art Project Connects Strangers via Vintage Payphone](#item-10) ⭐️ 6.0/10
11. [Walkable ASCII Cyberpunk City in a Single HTML File](#item-11) ⭐️ 6.0/10
12. [RavynOS: Pre-alpha open-source OS aiming for macOS compatibility](#item-12) ⭐️ 6.0/10
13. [Professor's Advice on Cold Emailing for PhD Positions](#item-13) ⭐️ 6.0/10
14. [uv 0.12.8 Released with Performance and Preview Features](#item-14) ⭐️ 5.0/10
15. [Monthly Hiring and Job Seeker Thread for ML Community](#item-15) ⭐️ 3.0/10
16. [User Seeks Examples of Well-Designed ML Posters for ECCV 2026](#item-16) ⭐️ 3.0/10

---

<a id="item-1"></a>
## [Google Removes MV2 Extensions from Chrome Web Store, Including uBlock Origin](https://webiterate.dev/google-removed-extensions-ublock-origin-108/) ⭐️ 8.0/10

Google has removed all Manifest V2 (MV2) extensions from the Chrome Web Store, including the popular ad-blocker uBlock Origin. This move completes the transition to Manifest V3, which began years ago and was fully enforced by 2025. This change significantly impacts Chrome users who relied on MV2-based ad-blockers like uBlock Origin, which offer more robust filtering than MV3 alternatives. It raises security concerns for less tech-savvy users who may be exposed to malicious ads, and it is driving many users to switch to Firefox or other browsers. Chrome disabled all MV2 extensions in July 2025, and the final developer flag to re-enable them was removed in Chrome 151, which reached stable on July 28, 2026. uBlock Origin users on Chrome are advised to switch to uBlock Origin Lite, while Firefox continues to support the full version.

hackernews · twapi · Aug 31, 21:10 · [Discussion](https://news.ycombinator.com/item?id=49514878)

**Background**: Manifest V2 (MV2) was the previous extension platform for Chrome, allowing extensions like uBlock Origin to use powerful webRequest API for blocking network requests. Manifest V3 (MV3) restricts this API, favoring declarativeNetRequest, which limits ad-blocking capabilities. Google began phasing out MV2 in 2024, with a full removal by 2025, citing security and performance improvements.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.chrome.com/docs/extensions/develop/migrate">Migrate to Manifest V3 | Chrome for Developers</a></li>
<li><a href="https://toolbistro.com/radar/ublock-origin-alternatives">uBlock Origin Alternatives After Chrome Kills MV2 | ToolBistro</a></li>
<li><a href="https://www.neowin.net/news/google-chrome-is-killing-all-ublock-origin-bypasses-microsoft-edge-opera-to-follow/">Google Chrome is killing all uBlock Origin bypasses ... - Neowin</a></li>

</ul>
</details>

**Discussion**: Community comments express strong dissatisfaction with Google's decision, with many users highlighting security risks for less tech-savvy individuals who may fall for malicious ads. Several users have already switched to Firefox, praising its support for uBlock Origin, and some express distrust of Google's control over the web.

**Tags**: `#Chrome`, `#Manifest V2`, `#Ad-blocking`, `#Privacy`, `#Browser`

---

<a id="item-2"></a>
## [Sliding-Window Attention Outperforms Linear Attention on Long-Context Reasoning](https://www.reddit.com/r/MachineLearning/comments/1w3j1vw/slidingwindow_attention_beats_linear_on/) ⭐️ 8.0/10

A new arXiv preprint (2608.28444) claims that Sliding Window Attention (SWA) with attention sinks achieves 2 to 10 times higher performance than linear attention variants on long-context reasoning benchmarks such as Needle-in-a-Haystack and BABILong. The authors recommend switching to SWA instead of post-training linear models. This finding challenges a major research direction in efficient attention mechanisms, suggesting that simpler baselines have been overlooked. If validated, it could redirect research efforts and save significant computational resources spent on post-training linear attention models. The paper compares SWA with sinks against post-trained linear attention models across multiple LLMs and downstream tasks. The authors note that linear attention may require training from scratch or extensive post-training to match SWA, while SWA needs no post-training and maintains low memory usage.

reddit · r/MachineLearning · /u/Justgototheeffinmoon · Aug 31, 16:35

**Background**: Standard transformer attention has quadratic computational cost with sequence length, which is problematic for long contexts. Linear attention variants aim to reduce this to linear complexity via kernel approximations, but they often require post-training to perform well. Sliding window attention restricts attention to a local window, reducing cost, and attention sinks are special tokens that stabilize training and inference by absorbing excess attention.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2608.28444v1">Sliding - window beats linear attention</a></li>
<li><a href="https://carnotresearch.medium.com/let-the-chaos-sink-in-481c8a37471e">Let the Chaos Sink In. Balancing attention in transformers | Medium</a></li>
<li><a href="https://arxiv.org/abs/2406.10149">[2406.10149] BABILong: Testing the Limits of LLMs with Long Context Reasoning-in-a-Haystack</a></li>

</ul>
</details>

**Tags**: `#attention mechanisms`, `#long-context`, `#LLM efficiency`, `#arXiv`, `#benchmarking`

---

<a id="item-3"></a>
## [GNNs on Dynamic Graphs Suffer Temporal Leakage; SynthFin-AML Enforces Causal Boundaries](https://www.reddit.com/r/MachineLearning/comments/1w3imxy/your_gnn_is_probably_just_an_overcomplicated_mlp/) ⭐️ 8.0/10

The post introduces SynthFin-AML v10.0, a synthetic anti-money laundering dataset with 100k nodes and 1.2M edges, designed to enforce strict causal boundaries via a 3-snapshot temporal split. It also benchmarks LightGBM against GraphSAGE, showing GraphSAGE achieves PR-AUC 0.881 vs LightGBM's 0.848 on the strict temporal split. This addresses a critical evaluation flaw in GNN research on dynamic graphs, where standard random splits cause temporal leakage and inflated performance. By providing a benchmark with strict causal boundaries, it sets a higher standard for evaluation, potentially improving the reliability of GNN models in financial fraud detection and other temporal domains. The dataset ensures fraud and retail transaction amounts share the same lognormal distribution (μ=8.517, σ=0.8) to prevent distribution leakage. The 3-snapshot split uses train edges ≤ Day 7, validation ≤ Day 8, and test ≤ Day 10, physically disjointing temporal windows to bound the receptive field. The benchmark has been submitted to PyTorch Geometric as PR #10774.

reddit · r/MachineLearning · /u/Glabmayt2075 · Aug 31, 16:21

**Background**: Graph Neural Networks (GNNs) are widely used for learning on graph-structured data, but when applied to dynamic graphs (e.g., financial transaction networks), standard training with random splits can cause temporal leakage: the model sees future edges during training, leading to overly optimistic performance. This happens because message-passing aggregates information from neighbors that may include edges occurring after the prediction time. The SynthFin-AML dataset aims to mitigate this by enforcing strict causal boundaries, ensuring that evaluation reflects true generalization.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2512.06932v1">Hidden Leaks in Time Series Forecasting: How Data Leakage ... Stealing Training Graphs from Graph Neural Networks Batch-agnostic dynamic GNN for mitigating temporal ... MSPipe: Efficient Temporal GNN Training via Retrofitting temporal GNN training with decoder-only ... machine learning - How does temporal data leakage happen ... MSPipe: Efficient Temporal GNN Training via Staleness-Aware ...</a></li>
<li><a href="https://huggingface.co/datasets/ovvaliyev/synthfin-aml">ovvaliyev/ synthfin - aml · Datasets at Hugging Face</a></li>
<li><a href="https://github.com/valiyevoktay-cmd/synthfin-aml-">GitHub - valiyevoktay-cmd/ synthfin - aml -: A graph-native Anti-Money...</a></li>

</ul>
</details>

**Tags**: `#GNN`, `#temporal leakage`, `#dynamic graphs`, `#anti-money laundering`, `#dataset`

---

<a id="item-4"></a>
## [Turning Security Cameras into an Automatic Bird Identification System](https://jasontucker.blog/how-i-turned-my-security-cameras-into-an-automatic-bird-identification-system-with-birdnet-go/) ⭐️ 7.0/10

A blog post describes how to repurpose security cameras into an automatic bird identification system using BirdNET-Go, which analyzes audio from camera microphones to identify bird species in real time. The post includes practical setup details and has sparked significant community engagement. This DIY project demonstrates a novel, accessible application of embedded AI for wildlife monitoring, potentially inspiring hobbyists and researchers to repurpose existing infrastructure for ecological observation. It highlights the growing trend of local, privacy-preserving AI inference on edge devices. BirdNET-Go is a self-hosted, real-time soundscape analyzer that runs on a Raspberry Pi and supports audio from soundcards or network streams, including RTSP feeds from cameras. The system can also identify bats, and the author notes that it works with various camera brands, though some users report challenges with audio quality and sampling rates.

hackernews · speckx · Aug 31, 16:47 · [Discussion](https://news.ycombinator.com/item?id=49511856)

**Background**: BirdNET is an AI-powered sound identification tool developed by the Cornell Lab of Ornithology, capable of recognizing bird species from audio recordings. BirdNET-Go is a community implementation that runs locally on devices like Raspberry Pi, enabling real-time, offline analysis. Security cameras with built-in microphones can provide a convenient audio source for such systems.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/tphakala/birdnet-go">GitHub - tphakala/birdnet-go: Self-hosted realtime soundscape ...</a></li>
<li><a href="https://birdnet.cornell.edu/">BirdNET – AI-Powered Sound ID</a></li>
<li><a href="https://jasontucker.blog/how-i-turned-my-security-cameras-into-an-automatic-bird-identification-system-with-birdnet-go/">How I Turned My Security Cameras Into an Automatic Bird Identification System with BirdNet-Go</a></li>

</ul>
</details>

**Discussion**: Community members shared their own implementations, such as using Unifi doorbell cams, Aqara cameras, and portable BirdNET-Pi setups. Some discussed technical challenges like wind noise and sampling rate limitations, while others suggested improvements like using e-ink displays for visualization. Overall sentiment was positive and enthusiastic.

**Tags**: `#BirdNET`, `#DIY`, `#Computer Vision`, `#Audio Recognition`, `#Embedded AI`

---

<a id="item-5"></a>
## [Apple Surprised by AI-Driven Demand for Mac Mini and Mac Studio](https://www.macrumors.com/2026/08/30/apple-unexpected-mac-mini-and-studio-demand/) ⭐️ 7.0/10

Apple is reportedly caught off guard by strong demand for Mac Mini and Mac Studio, driven by local AI workloads. The company lacked a dedicated engineering team for business customers or an enterprise AI strategy, according to the article. This signals a shift towards on-device AI, where users prefer local processing for privacy, latency, and cost reasons. It highlights an unexpected product-market fit that could influence Apple's future hardware and AI strategy. The demand is attributed to local AI workloads such as running LLMs and training models. Apple reportedly did not anticipate this demand, lacking dedicated enterprise support, which contrasts with the growing trend of AI PCs with NPUs.

hackernews · thm · Aug 31, 12:41 · [Discussion](https://news.ycombinator.com/item?id=49508982)

**Background**: On-device AI runs workloads directly on hardware, reducing cloud costs and latency while improving privacy. Modern devices often include NPUs for this purpose, and Mac Mini models with M-series chips are popular for local AI due to their performance and memory bandwidth.

<details><summary>References</summary>
<ul>
<li><a href="https://www.microsoft.com/en-us/surface/business/business-planning-and-strategy-center/on-device-ai-business-workflows">On-Device AI for Business: Faster, Smarter Workflows ...</a></li>
<li><a href="https://www.deloitte.com/us/en/services/consulting/services/hybrid-ai.html">On-Device AI | Deloitte US</a></li>
<li><a href="https://www.apple.com/mac-mini/">Mac mini - Apple</a></li>

</ul>
</details>

**Discussion**: Commenters are skeptical, with some calling it marketing, while others share practical experiences of local AI training being faster and cheaper for experiments. There is also curiosity about whether local setups can match cloud subscriptions, and concern that AI enthusiasts are driving up prices for regular consumers.

**Tags**: `#Apple`, `#AI hardware`, `#local AI`, `#Mac Mini`, `#Mac Studio`

---

<a id="item-6"></a>
## [ChatGPT Work Skill Reference Site Highlights Playwright Browser Control](https://codex-tool-reference.simonw.chatgpt.site/) ⭐️ 7.0/10

A new reference site, codex-tool-reference.simonw.chatgpt.site, catalogs ChatGPT Work skills, with the standout being a control-browser skill that instructs ChatGPT Work to launch a Playwright instance via Node.js REPL and run `nodeRepl.write(await browser.documentation())` to obtain usage instructions. This skill provides a practical method for AI agents to control real browsers, enabling more interactive and dynamic web automation tasks. It highlights the growing ecosystem of reusable skills for ChatGPT Work, which could significantly enhance developer productivity and expand the capabilities of AI assistants. The skill leverages Playwright, an open-source browser automation framework by Microsoft, and uses a Node.js REPL to interact with the browser. The `browser.documentation()` method returns detailed instructions on how to use the browser, which ChatGPT Work then follows to perform tasks.

hackernews · ijidak · Aug 31, 14:07 · [Discussion](https://news.ycombinator.com/item?id=49510000)

**Background**: ChatGPT Work skills are reusable workflows that allow users to automate recurring tasks and ensure consistent outputs. Playwright is a popular open-source library for browser testing and web scraping, supporting Chromium, Firefox, and WebKit with a single API. The reference site serves as a collection of such skills, providing developers with ready-made solutions for common automation needs.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Playwright_(software)">Playwright (software) - Wikipedia</a></li>
<li><a href="https://github.com/microsoft/playwright">GitHub - microsoft/playwright: Playwright is a framework for Web Testing and Automation. It allows testing Chromium, Firefox and WebKit with a single API. · GitHub</a></li>
<li><a href="https://help.openai.com/en/articles/20001066-skills-in-chatgpt">Skills in ChatGPT - OpenAI Help Center</a></li>

</ul>
</details>

**Discussion**: Simon Willison highlighted the control-browser skill as the most interesting, noting its use of Playwright and the `browser.documentation()` method. Another commenter questioned how this differs from Codex, while others pointed out UI issues on the site and mused about the common aesthetic of AI-generated websites.

**Tags**: `#ChatGPT`, `#AI tools`, `#browser automation`, `#Playwright`, `#developer tools`

---

<a id="item-7"></a>
## [Military Commissary Freezer Failures Spark Hacking Speculation](https://signalandsilence.substack.com/p/i-think-someone-hacked-the-commissary) ⭐️ 7.0/10

A blog post speculates that simultaneous failures of freezers at multiple military commissaries may be the result of a cyberattack, prompting discussions about potential DoD network infiltration. The Pentagon has acknowledged a 'possible refrigeration disruption' at some Defense Commissary Agency commissaries. This matters because it highlights the vulnerability of military infrastructure to cyber threats, including industrial control systems (ICS) that manage physical equipment like refrigeration. If confirmed, it could signal a new class of attacks targeting military logistics and supply chains, with potential ripple effects on readiness and morale. The incidents reportedly affected at least six military installations, with failures occurring near-simultaneously. The blog post notes that the timing and pattern are suspicious, but no official confirmation of a hack has been made, and alternative explanations like misconfiguration or update errors are possible.

hackernews · jcurbo · Aug 31, 11:45 · [Discussion](https://news.ycombinator.com/item?id=49508506)

**Background**: Military commissaries are retail stores on military bases that sell groceries and household goods to service members and their families. Industrial control systems (ICS) and supervisory control and data acquisition (SCADA) systems are used to monitor and control physical equipment, including refrigeration units. These systems have known vulnerabilities, such as legacy software and weak access controls, making them potential targets for cyberattacks.

<details><summary>References</summary>
<ul>
<li><a href="https://signalandsilence.substack.com/p/i-think-someone-hacked-the-commissary">I Think the Military Commissary Freezers Were Hacked</a></li>
<li><a href="https://www.schneier.com/blog/archives/2026/08/is-someone-hacking-dod-refrigerators.html">Is Someone Hacking DoD Refrigerators? - Schneier on Security</a></li>
<li><a href="https://www.levelblue.com/blogs/spiderlabs-blog/unveiling-the-dark-side-common-attacks-and-vulnerabilities-in-industrial-control-systems/">Unveiling the Dark Side: Common Attacks and Vulnerabilities in Industrial Control Systems</a></li>

</ul>
</details>

**Discussion**: Commenters are divided: some, like mark-r, suggest the incident might be a deliberate proof of DoD network infiltration, while others, like CobaltFire, argue it's more likely a misconfiguration or update error, noting the concerning timing. 0xWTF draws parallels to a vulnerability hinted at in a 2014 book, and peterabbitcook shares personal experience with insecure PLCs, supporting the plausibility of a hack. codingdave cautions against jumping to conclusions, suggesting the author should first consider the number of refrigerators and baseline failure rates.

**Tags**: `#cybersecurity`, `#military`, `#IoT`, `#industrial control systems`, `#speculation`

---

<a id="item-8"></a>
## [Wrapture: New Python Library Extends Monkeypatching to Testing and Tracing](https://simonwillison.net/2026/Aug/31/introducing-wrapture/) ⭐️ 7.0/10

Graham Dumpleton, creator of wrapt, has released a new Python library called Wrapture that extends wrapt's monkeypatching capabilities to enable both tracing and testing of functions and methods. The library, still in its early weeks, includes OpenTelemetry support and a configuration-based mechanism for adding tracing to existing projects. Wrapture offers a novel approach to testing and observability in Python, potentially serving as an alternative to unittest.mock and simplifying the integration of tracing into existing codebases. Its development as a fully AI-driven project also highlights the growing role of AI assistants in software engineering. Wrapture allows wrapping any function or method to trace all access or override return values, and includes a TOML-based configuration for capturing traces to JSON lines. The project is very young, just a few weeks old, and was entirely written by an AI assistant under Graham's direction, which he distinguishes from 'vibe coding' by emphasizing careful engineering and design.

rss · Simon Willison · Aug 31, 23:59

**Background**: Monkeypatching is a technique in Python that allows modifying the behavior of functions or classes at runtime, often used for testing or adding instrumentation. wrapt is a well-known library that provides a transparent object proxy to safely apply monkeypatching, and Wrapture builds on these ideas to unify testing and tracing. OpenTelemetry is an observability framework for generating and collecting telemetry data, and Wrapture's support for it enables easy integration with existing monitoring systems.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/GrahamDumpleton/wrapt">GitHub - GrahamDumpleton/wrapt: A Python module for decorators, wrappers and monkey patching. · GitHub</a></li>
<li><a href="https://wrapt.readthedocs.io/">wrapt — wrapt 2.3.0 documentation</a></li>
<li><a href="https://grahamdumpleton.me/posts/2026/09/unit-testing-with-wrapture/">Unit testing with wrapture - Graham Dumpleton</a></li>

</ul>
</details>

**Tags**: `#Python`, `#testing`, `#tracing`, `#monkeypatching`, `#library`

---

<a id="item-9"></a>
## [Entropic Scree: New Tool to Assess Signal in Dirty Data](https://www.reddit.com/r/MachineLearning/comments/1w3br9c/how_to_assess_if_there_is_a_strong_signal_in_your/) ⭐️ 7.0/10

A new tabular data diagnostic tool called Entropic Scree has been released, which estimates signal strength, signal-to-noise ratio (SNR), intrinsic rank, and linear sufficiency in high-dimensional, real-world datasets using a transformed mutual information metric. The R function is already available, with Python and R packages to be released soon. This tool addresses a common pain point in applied machine learning: dealing with dirty, high-dimensional data. By providing a more robust diagnostic than traditional PCA-based methods, it could help practitioners better decide whether their data contains enough signal for modeling, potentially improving model performance and saving time. The method evaluates a transformed mutual information metric instead of linear variance, rank order, or Euclidean distance, making it less reliant on strong parametric or distance assumptions. It also serves as a practical diagnostic for the 'From Garbage to Gold' framework, which describes when uncurated, error-prone data can be used directly for accurate predictions.

reddit · r/MachineLearning · /u/Chocolate_Milk_Son · Aug 31, 12:02

**Background**: Mutual information is a measure of the mutual dependence between two random variables, quantifying how much information one variable provides about another. Traditional dimensionality reduction techniques like PCA rely on linear variance and Euclidean distance, which may fail on dirty, high-dimensional data. Entropic Scree aims to overcome these limitations by using an information-theoretic approach.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/tjleestjohn/Entropic-Scree">GitHub - tjleestjohn/ Entropic - Scree : Overcome the limits of standard...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mutual_information">Mutual information - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#data quality`, `#mutual information`, `#dimensionality reduction`, `#diagnostics`, `#tabular data`

---

<a id="item-10"></a>
## [Playa Phone: A Burning Man Art Project Connects Strangers via Vintage Payphone](https://playaphone.com/) ⭐️ 6.0/10

A hacker news post highlighted the Playa Phone, a vintage payphone art installation at Burning Man that allows participants to make calls. The project's creator, aaron42net, engaged with the community in the comments, answering questions about the project. This project exemplifies the interactive and community-driven spirit of Burning Man, fostering spontaneous human connections in a tech-saturated world. It also sparked discussions about the event's culture and the role of technology in social interaction, resonating with a broader audience interested in art, community, and technology. The Playa Phone is a vintage payphone set up at Burning Man, allowing participants to make calls. The project's creator, aaron42net, is active in the community and answered questions in the comments. A livestream of the event was also shared, with a note about a potential naming discrepancy on the map.

hackernews · cutoff · Aug 31, 14:52 · [Discussion](https://news.ycombinator.com/item?id=49510514)

**Background**: Burning Man is an annual week-long event in the Nevada desert that emphasizes community, art, self-expression, and self-reliance. It features large-scale art installations and interactive projects, often created by participants. The Playa Phone is one such project, blending nostalgia with the event's ethos of radical inclusion and gifting.

**Discussion**: The community discussion was largely positive, with the creator engaging directly. One user shared a heartwarming story of getting married after stopping at the phone booth, while another promoted a similar app for spontaneous calls. There was also a question about whether Burning Man is fun, reflecting a cynical view of the event's demographics, and a livestream link was shared.

**Tags**: `#burning man`, `#art project`, `#community`, `#interactive`, `#hackernews`

---

<a id="item-11"></a>
## [Walkable ASCII Cyberpunk City in a Single HTML File](https://www.youtube.com/watch?v=3YtygAx_C6A) ⭐️ 6.0/10

A developer has created a walkable 3D ASCII cyberpunk city that runs entirely in a single HTML file, with recent updates adding traffic, interiors, and skyscrapers. The project is showcased in a video and has gained attention on Hacker News. This project demonstrates the creative potential of browser-based ASCII art, offering a unique aesthetic that appeals to nostalgic and creative coding communities. It highlights how modern web technologies can render complex scenes without heavy dependencies, potentially inspiring similar hobbyist projects. The city is rendered using ASCII characters in a fixed-width font, likely via a canvas or DOM manipulation, and includes interactive elements like walking and traffic. The developer has released multiple update videos, but the GitHub project may not match the latest video content, as noted by a commenter.

hackernews · keithcarolus · Aug 31, 18:21 · [Discussion](https://news.ycombinator.com/item?id=49512975)

**Background**: ASCII art is a technique that uses printable characters to create images, often rendered in monospace fonts to maintain alignment. In web browsers, developers can leverage HTML, CSS, and JavaScript to create dynamic ASCII art, as opposed to traditional terminal-based approaches. This project is part of a broader trend of creative coding in the browser, where constraints like single-file HTML push the boundaries of what can be achieved with minimal resources.

<details><summary>References</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=DSRooHo_HSI">ASCII City Update 2: Traffic & Detail Update - YouTube</a></li>
<li><a href="https://github.com/tweakyourpc/ascii-city">GitHub - tweakyourpc/ascii-city: A 3D city renderer that ...</a></li>
<li><a href="https://www.neowin.net/news/developer-builds-a-fully-walkable-3d-city-entirely-out-of-ascii-characters/">Developer builds a fully walkable 3D city entirely out of ...</a></li>

</ul>
</details>

**Discussion**: Community comments are generally positive, with one user praising the browser-based approach for ASCII art and another expressing nostalgia. However, some users noted issues with rendering differences in their own experience, and one flagged the post as a duplicate.

**Tags**: `#ASCII art`, `#creative coding`, `#browser graphics`, `#cyberpunk`, `#HTML`

---

<a id="item-12"></a>
## [RavynOS: Pre-alpha open-source OS aiming for macOS compatibility](https://ravynos.com/) ⭐️ 6.0/10

RavynOS, a pre-alpha open-source operating system based on Darwin, FreeBSD, and Apple open-source components, has been highlighted in recent community discussions. The project aims to provide macOS compatibility while maintaining the freedom of open source. This project is significant because it attempts to combine the user experience of macOS with the openness of FreeBSD, potentially offering an alternative for users who want macOS-like functionality without Apple's hardware or licensing. It also contributes to the ongoing effort of open-source reimplementation of proprietary systems, similar to ReactOS and Darling. RavynOS is in pre-alpha stage, meaning it is not yet stable or feature-complete. The project's FAQ addresses legal concerns by citing precedents like ReactOS and GNUstep, and it uses Discord for community communication, which some users find limiting.

hackernews · Bluestein · Aug 31, 16:19 · [Discussion](https://news.ycombinator.com/item?id=49511534)

**Background**: Darwin is the open-source core of Apple's operating systems, derived from NeXTSTEP, FreeBSD, and other BSD code, along with Apple's own contributions. FreeBSD is a widely used open-source Unix-like OS descended from BSD. RavynOS builds on these foundations to create a macOS-compatible environment, similar to how ReactOS aims for Windows compatibility.

<details><summary>References</summary>
<ul>
<li><a href="https://ravynos.com/">ravynOS - Finesse of macOS. Freedom of Open Source.</a></li>
<li><a href="https://en.wikipedia.org/wiki/Darwin_(operating_system)">Darwin (operating system) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/FreeBSD">FreeBSD - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community comments show mixed reactions: some question the unique benefits of Darwin over other BSDs, others note the lack of screenshots on the website, and some express frustration with Discord as the primary communication channel. There is also a reference to previous discussions on Hacker News, indicating ongoing interest.

**Tags**: `#operating systems`, `#open source`, `#Darwin`, `#FreeBSD`, `#macOS compatibility`

---

<a id="item-13"></a>
## [Professor's Advice on Cold Emailing for PhD Positions](https://www.reddit.com/r/MachineLearning/comments/1w3bwci/cold_emailing_profs_about_phd_positions_read_this/) ⭐️ 6.0/10

A professor shared a list of common mistakes to avoid when cold emailing about PhD positions, including sending mass emails, vague research interests, and misrepresenting workshop papers as conference papers. This advice is crucial for prospective PhD applicants, as it can significantly improve their chances of getting a positive response from potential supervisors. It also highlights the importance of genuine research interest and honesty in academic communication. The professor specifically advises against using LLMs to outsource thinking, as it leads to generic research directions. They also emphasize checking supervisors' websites for specific contact instructions, as ignoring them can result in emails being sent to spam.

reddit · r/MachineLearning · /u/tariban · Aug 31, 12:09

**Background**: Cold emailing professors is a common practice in many countries for PhD recruitment. Foundational ML research focuses on core algorithms and methodologies rather than specific application domains, which is why the professor notes that many applicants' applied interests may not align with their research.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tiktok.com/discover/cold-emailing-professors">Cold Emailing Professors | TikTok</a></li>
<li><a href="https://www.linkedin.com/posts/sanya-jain-your-grad-coach-181835223_when-is-the-right-time-to-cold-email-professors-activity-7225913537393569793-mdf0">How to Cold Email Professors for a PhD in the USA | LinkedIn</a></li>
<li><a href="https://academia.stackexchange.com/questions/206643/is-it-appropriate-to-cold-email-professors-in-search-of-a-postdoc-position">physics - Is it appropriate to cold email professors in search of...</a></li>

</ul>
</details>

**Tags**: `#PhD applications`, `#academic advice`, `#cold emailing`, `#career guidance`

---

<a id="item-14"></a>
## [uv 0.12.8 Released with Performance and Preview Features](https://github.com/astral-sh/uv/releases/tag/0.12.8) ⭐️ 5.0/10

uv 0.12.8 was released on 2026-08-31, introducing preview features for content-addressed caching, performance improvements for concurrent downloads and lockfile processing, and several bug fixes. Notable enhancements include deduplicating identical files within and across cached wheels, and preventing concurrent uv processes from downloading the same remote wheel more than once. This release matters because it improves the efficiency and reliability of uv, a popular Python package manager, benefiting developers who rely on it for fast dependency resolution and installation. The content-addressed cache preview feature could significantly reduce disk usage and download times, while the lockfile processing speedups enhance performance for large projects. The content-addressed cache preview feature deduplicates identical files within and across cached wheels, and includes optimizations like reusing the hashing buffer and bulk reading hard-link counts on macOS. Performance improvements include preventing concurrent downloads of the same wheel, indexing packages during lockfile traversal, and reducing marker interner work for warm resolutions.

github · astral-automations-bot[bot] · Aug 31, 22:18

**Background**: uv is a fast Python package and project manager written in Rust, known for its speed and efficiency. Content-addressed storage (CAS) is a method where data is stored and retrieved based on its content, not its location, which helps in deduplication and efficient caching. Lockfiles are files that record the exact versions of dependencies to ensure reproducible builds.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Content-addressable_storage">Content-addressable storage - Wikipedia</a></li>
<li><a href="https://docs.astral.sh/uv/concepts/tools/">Tools | uv - Astral</a></li>
<li><a href="https://devsecopsschool.com/blog/lockfile/">What is Lockfile? Meaning, Architecture, Examples, Use Cases ...</a></li>

</ul>
</details>

**Tags**: `#uv`, `#Python`, `#package manager`, `#performance`, `#release`

---

<a id="item-15"></a>
## [Monthly Hiring and Job Seeker Thread for ML Community](https://www.reddit.com/r/MachineLearning/comments/1w30ti8/d_monthly_whos_hiring_and_who_wants_to_be_hired/) ⭐️ 3.0/10

A new monthly thread has been posted on r/MachineLearning for job postings and job seekers, providing templates for both hiring and seeking positions. This thread centralizes job opportunities and candidate resumes within the machine learning community, facilitating networking and career moves for professionals in the field. The thread includes specific templates: for hiring, use 'Hiring: [Location], Salary:[], [Remote | Relocation], [Full Time | Contract | Part Time]' and for job seekers, 'Want to be Hired: [Location], Salary Expectation:[], [Remote | Relocation], [Full Time | Contract | Part Time]' with a resume link. It reminds users that the community is geared towards experienced professionals.

reddit · r/MachineLearning · /u/AutoModerator · Aug 31, 02:30

**Background**: Reddit's r/MachineLearning is a popular forum for machine learning practitioners. Monthly hiring threads are a common feature in many professional subreddits to organize job-related posts and reduce clutter. The templates help standardize information for easier browsing.

**Tags**: `#jobs`, `#machine learning`, `#community`

---

<a id="item-16"></a>
## [User Seeks Examples of Well-Designed ML Posters for ECCV 2026](https://www.reddit.com/r/MachineLearning/comments/1w39buv/good_machine_learning_posters_d/) ⭐️ 3.0/10

A Reddit user posted a request on r/MachineLearning asking for examples of well-designed machine learning or computer vision posters to inspire their own poster for ECCV 2026. The post is a simple, low-scored inquiry with no technical depth. This post highlights the practical need for effective poster design in academic conferences, which can significantly impact how research is communicated and received. Although the post itself is low priority, it reflects a common challenge for researchers preparing for major conferences like ECCV. The user specifically mentions ECCV 2026, a major computer vision conference, indicating a forward-looking timeline. The request is generic, asking for 'cool examples' without specifying any particular style, topic, or format, which may limit the usefulness of responses.

reddit · r/MachineLearning · /u/National-Resident244 · Aug 31, 10:04

**Background**: Academic conferences like ECCV (European Conference on Computer Vision) often require researchers to present their work as posters. A well-designed poster can effectively convey complex ideas visually, aiding in networking and feedback. However, many researchers struggle with poster design, leading to requests for examples and best practices.

**Tags**: `#machine learning`, `#posters`, `#conference`, `#computer vision`

---