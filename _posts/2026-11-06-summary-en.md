---
layout: default
title: "Horizon Summary: 2026-11-06 (EN)"
date: 2026-11-06
lang: en
---

> From 24 items, 20 important content pieces were selected

---

1. [OpenSSH 'sshole' Authentication Bypass Flaw Hits musl-based Systems](#item-1) ⭐️ 9.0/10
2. [Claude Code leaks user email addresses via HTTP requests](#item-2) ⭐️ 8.0/10
3. [Hugging Face Releases Comprehensive MoE Training Handbook with Megatron-LM](#item-3) ⭐️ 8.0/10
4. [MS Paint Remote Code Execution Vulnerability CVE-2026-83844](#item-4) ⭐️ 7.0/10
5. [Servo's September update adds <progress> and rounded rectangles](#item-5) ⭐️ 7.0/10
6. [trainlint: Static AST Checker Catches 14 Silent ML Bugs](#item-6) ⭐️ 7.0/10
7. [DialFork benchmark targets procedural hallucination in conversational LLM agents](#item-7) ⭐️ 7.0/10
8. [Kagi opens search to everyone without an account](#item-8) ⭐️ 6.0/10
9. [Blogger Revives Hackintosh with AI Assistance, Sparking Debate](#item-9) ⭐️ 6.0/10
10. [Salon Publishes Farewell Piece, Sparking Debate on Journalism's Decline](#item-10) ⭐️ 6.0/10
11. [Motorola Signature 27 launches with official GrapheneOS support at $1,599](#item-11) ⭐️ 6.0/10
12. [Blog Post Urges Archiving YouTube Videos Before They Disappear](#item-12) ⭐️ 6.0/10
13. [Opinion: Tech Companies Still Fail to Understand Users Despite Data Collection](#item-13) ⭐️ 6.0/10
14. [Sparse Predictive Hierarchies Fail to Match Backprop on Chess Prediction Task](#item-14) ⭐️ 6.0/10
15. [Animated explainer shows how LLMs pick next token with real Qwen2.5-0.5B probabilities](#item-15) ⭐️ 6.0/10
16. [ML PhD publication expectations: how many papers are 'productive' now?](#item-16) ⭐️ 5.0/10
17. [Student asks: separate models or one global model for demand forecasting across 40 locations?](#item-17) ⭐️ 5.0/10
18. [Window Sweaters: A Whimsical macOS App for Knitted Window Borders](#item-18) ⭐️ 4.0/10
19. [Reddit Thread Invites ICLR 2027 Review Results Sharing](#item-19) ⭐️ 4.0/10
20. [Paul Ford: Browsers Are Powerful and Getting Cheaper](#item-20) ⭐️ 3.0/10

---

<a id="item-1"></a>
## [OpenSSH 'sshole' Authentication Bypass Flaw Hits musl-based Systems](https://sshhole.com/) ⭐️ 9.0/10

A critical OpenSSH authentication bypass vulnerability, dubbed 'sshole', allows attackers to log in without valid credentials on systems using musl libc (such as Alpine Linux) when password authentication is enabled and an account's password hash is set to '*'. The flaw arises from improper handling of special characters like '*' in crypt hashes, causing the crypt() comparison to incorrectly succeed. This vulnerability affects widely used lightweight Linux distributions like Alpine Linux, OpenWrt, and Buildroot, potentially exposing countless servers and embedded devices to unauthorized access. It highlights the dangers of in-band signaling in security-critical code and underscores the need for careful handling of special values in authentication systems. The bypass occurs because crypt() returns a hash starting with '*' when given an invalid salt, and OpenSSH compares this result to the stored hash '*', which is commonly used to indicate a disabled password. The vulnerability is specific to musl libc implementations; glibc-based systems are not affected in the same way, and musl has previously worked around similar issues but missed this path.

hackernews · josemrb · Nov 5, 12:19 · [Discussion](https://news.ycombinator.com/item?id=50378228)

**Background**: OpenSSH is a widely used suite for secure remote login and file transfer, and it relies on the system's crypt() function to verify passwords. The crypt() function hashes a password with a salt and returns a string that should match the stored hash; special values like '*' or '!' in the password field traditionally indicate that password login is disabled. musl libc is a lightweight C standard library alternative to glibc, commonly used in container-friendly distributions like Alpine Linux.

<details><summary>References</summary>
<ul>
<li><a href="https://thehackernews.com/2026/11/openssh-issues-emergency-fix-for-flaw.html">OpenSSH Issues Emergency Fix for Flaw Letting Long Passwords...</a></li>
<li><a href="https://alpinelinux.org/posts/2026-11-05-openssh-password-authentication-bypass/">Security advisory: openssh -server password... | Alpine Linux</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/openssh-flaw-lets-attackers-log-into-password-disabled-linux-accounts/">OpenSSH flaw lets attackers log into password-disabled Linux accounts</a></li>

</ul>
</details>

**Discussion**: Commenters widely criticized the use of in-band signaling, with one noting that '*' should never have been used as a special value for 'no password' or 'error while hashing'. Others pointed out that musl had previously worked around similar issues but missed this path, and some expressed disappointment that musl made convenience changes to core crypto functions without sufficient auditing.

**Tags**: `#security`, `#openssh`, `#authentication`, `#vulnerability`, `#crypt`

---

<a id="item-2"></a>
## [Claude Code leaks user email addresses via HTTP requests](https://github.com/anthropics/claude-code/issues/107757) ⭐️ 8.0/10

A GitHub issue reported that Claude Code was sending users' email addresses and other identifiers to third-party websites in the User-Agent header during web searches, and Anthropic has since shipped a built-in privacy plugin to block this behavior. This privacy leak affects developers using a widely adopted AI coding tool and has already led to reports of targeted spam, highlighting the risks of agentic tools exposing personal data to arbitrary websites. The leak occurred because Claude Code and its subagents embedded identifiers such as names, company names, and email addresses into User-Agent strings for curl requests; the fix is included in version 2.1.317 and later and can be toggled via /plugins.

hackernews · motoroco · Nov 5, 22:17 · [Discussion](https://news.ycombinator.com/item?id=50385272)

**Background**: Claude Code is Anthropic's agentic coding tool that runs in the terminal and IDE, capable of executing commands and making web requests. HTTP request headers, particularly the User-Agent, often carry identifying information that can be used to track or profile users. This incident shows how AI agents that autonomously make network requests can inadvertently leak personal data.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/anthropics/claude-code/issues/107757">Bug Report: Privacy violation in User-Agent header</a></li>
<li><a href="https://github.com/anthropics/claude-code/releases">Releases · anthropics/ claude - code · GitHub</a></li>
<li><a href="https://funwithtext.com/blog/http-headers-that-leak-identity.html">15 HTTP Headers That Leak Your Identity</a></li>

</ul>
</details>

**Discussion**: Commenters reported receiving personalized spam after switching to Claude Code, and one user shared examples of subagents embedding names and company details in User-Agent headers. Some expressed distrust of Anthropic's data handling, while a maintainer confirmed the issue and pointed to the new privacy plugin.

**Tags**: `#privacy`, `#AI coding tools`, `#Claude Code`, `#security`, `#data leakage`

---

<a id="item-3"></a>
## [Hugging Face Releases Comprehensive MoE Training Handbook with Megatron-LM](https://www.reddit.com/r/MachineLearning/comments/1xorgq0/the_ultimate_moe_training_handbook_training/) ⭐️ 8.0/10

Nouamane, a researcher at Hugging Face, released a detailed handbook for training Mixture-of-Experts (MoE) models with Megatron-LM, covering hardware setup, layer internals, serving, and reinforcement learning. The handbook includes 55 figures, scripts, and a consolidated list of recommended flags, drawing from approximately 800k GH200 GPU-hours on the Alps cluster at CSCS. This handbook fills a gap for practitioners who have trained dense models and want to transition to MoE, providing practical guidance and code-level insights that can accelerate adoption of MoE architectures in the open-source community. It also offers a rare glimpse into the training choices of frontier MoE models, backed by citations and real-world experiments. The handbook is structured into chapters: a Megatron-LM runbook (Chapter 2), a deep dive into MoE layer components with code and recommendations (Chapter 3), and serving/RL considerations (Chapter 4). Chapters 3 and 4 require no GPU, and the authors clearly label simulations versus real-run results.

reddit · r/MachineLearning · /u/Norlax_42 · Nov 5, 19:13

**Background**: Mixture-of-Experts (MoE) is a neural network architecture where multiple expert networks specialize in different regions of the input space, and a gating network routes each input to a subset of experts. This allows models to scale parameters efficiently while keeping computation manageable. Megatron-LM is NVIDIA's open-source framework for training large language models, offering GPU-optimized techniques and distributed training support. Load balancing is a critical challenge in MoE training to prevent routing collapse and ensure even expert utilization.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://github.com/NVIDIA/Megatron-LM">GitHub - NVIDIA/Megatron-LM: Ongoing research training ...</a></li>
<li><a href="https://huggingface.co/blog/NormalUhr/moe-balance">A Review on the Evolvement of Load Balancing Strategy in MoE ...</a></li>

</ul>
</details>

**Tags**: `#Mixture-of-Experts`, `#Megatron-LM`, `#Model Training`, `#Deep Learning`, `#Hugging Face`

---

<a id="item-4"></a>
## [MS Paint Remote Code Execution Vulnerability CVE-2026-83844](https://www.cve.org/CVERecord?id=CVE-2026-83844) ⭐️ 7.0/10

A remote code execution vulnerability, CVE-2026-83844, was disclosed in MS Paint for Windows 11, affecting versions from 11.0.0.0 up to but not including 11.2605.91.0, with Microsoft naming Paint 11.2609.401.0 as the fix. The patch is distributed through the Microsoft Store rather than Windows Update, causing confusion as some users report the Store still offering the old version. This vulnerability is notable because MS Paint, a simple image editor, is not typically expected to expose a network-facing attack surface, and its high severity (CVSS 8.1) means attackers could potentially execute malicious code remotely. The confusing patch distribution through the Microsoft Store rather than Windows Update leaves many users unsure whether they are protected. The vulnerability is an out-of-bounds read in Microsoft Paint that could allow an attacker to execute malicious code, and Microsoft classifies it as high severity with a CVSS score of 8.1. Users should check their Paint version and update via the Microsoft Store, as Windows Update may not show the fix.

hackernews · kuberwastaken · Nov 5, 20:43 · [Discussion](https://news.ycombinator.com/item?id=50384233)

**Background**: Remote code execution (RCE) is a critical vulnerability class that lets an attacker run arbitrary code on a target system remotely, often without authentication. MS Paint has been updated independently of Windows since spring 2021, which is why this fix arrives through the Microsoft Store rather than the operating system's update mechanism. The CVE record describes an unauthenticated attacker sending a specially crafted packet over the network to an affected service, raising questions about why Paint would have such a service.

<details><summary>References</summary>
<ul>
<li><a href="https://windowsforum.com/news/cve-2026-83844-windows-11-paint-rce-fix-confusion-and-how-to-check-your-version.451018/">CVE-2026-83844: Windows 11 Paint RCE Fix Confusion and How to ...</a></li>
<li><a href="https://windowsreport.com/microsoft-paint-security-flaw-could-let-hackers-execute-malicious-code-but-the-fix-is-hard-to-find/">Microsoft Paint Security Flaw Could Let Hackers Execute ...</a></li>
<li><a href="https://www.free-codecs.com/news/windows-11-paint-has-a-remote-hacking-bug-how-to-check-your-version-and-get-the-fix.htm">Windows 11 Paint Security Bug: How to Check and Get the Fix</a></li>

</ul>
</details>

**Discussion**: Commenters expressed disbelief that MS Paint could have a remote code execution vulnerability, with one asking 'WHY ON HELL paint has a remote code execution' and another joking about waiting for a Raymond Chen write-up. Others shared practical mitigation details, noting that Windows Update did not show the fix and that they had to get it from the Microsoft Store, while some pointed out that only specific versions are affected.

**Tags**: `#security`, `#vulnerability`, `#windows`, `#cve`, `#microsoft`

---

<a id="item-5"></a>
## [Servo's September update adds <progress> and rounded rectangles](https://servo.org/blog/2026/11/05/september-in-servo/) ⭐️ 7.0/10

Servo's September 2026 update introduces support for the HTML <progress> element and rounded rectangles, along with other improvements, as detailed in the project's monthly blog post. These additions fill basic web platform gaps, making Servo more usable for everyday browsing and demonstrating steady progress by the volunteer-driven project toward a viable alternative browser engine. The update also includes support for the :checked pseudo-class, and community members note that Servo received 527 commits in the period compared to over 20,000 for Chromium, highlighting the disparity in development resources.

hackernews · iamnothere · Nov 5, 14:34 · [Discussion](https://news.ycombinator.com/item?id=50379576)

**Background**: Servo is an experimental browser engine written in Rust, originally developed by Mozilla and now governed by Linux Foundation Europe with contributions from Igalia and the community. It aims to leverage Rust's memory safety and concurrency features to build a highly parallel rendering engine. The <progress> element is a standard HTML tag for displaying task completion, and rounded rectangles are a common CSS styling feature.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Servo_browser_engine">Servo browser engine</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/progress">HTML progress indicator element - HTML | MDN</a></li>
<li><a href="https://servo.org/">Servo aims to empower developers with a lightweight...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed admiration for Servo's Rust-based design and volunteer efforts, but some were surprised that basic features like <progress> and :checked were missing until now. Others shared practical experiences, noting that Servo's pre-built releases make it easier to use on Android, and one developer described Chrome's poor performance with many progress bars compared to Firefox.

**Tags**: `#servo`, `#browser-engine`, `#rust`, `#open-source`, `#web-rendering`

---

<a id="item-6"></a>
## [trainlint: Static AST Checker Catches 14 Silent ML Bugs](https://www.reddit.com/r/MachineLearning/comments/1xonrvy/trainlint_static_checks_for_ml_bugs_that_dont/) ⭐️ 7.0/10

A developer released trainlint, an open-source static analysis tool that parses Python code with ast to detect 14 common machine learning bugs that do not raise exceptions, such as fitting preprocessing before splitting data, leaving eval() on during training, and using softmax before CrossEntropyLoss. The tool requires no data, model, or GPU, and its author validated it on pytorch/examples, finding 20 real issues out of 22 flagged. Silent ML bugs like data leakage and eval-mode errors can inflate validation scores and waste significant debugging time, so a lightweight static checker that catches them before runtime could improve code quality for PyTorch and scikit-learn practitioners. It addresses a gap where traditional linters and unit tests fail because these mistakes produce no errors, only misleadingly good results. The tool matches names and reads one file at a time, only understands PyTorch and scikit-learn, and has no recall numbers; the author notes it will fail on code that names splits unusually. The leakage demonstration is striking: selecting top 20 features on the full dataset before 5-fold CV yields 85% accuracy on random labels, while doing selection inside a Pipeline yields 48%, proving the gap is pure leakage.

reddit · r/MachineLearning · /u/Possible-Active-1903 · Nov 5, 16:54

**Background**: Data leakage occurs when information from outside the training set influences model training, leading to overly optimistic performance estimates; a common example is fitting scalers or feature selectors on the full dataset before cross-validation. PyTorch models have train and eval modes that change the behavior of layers like dropout and batch normalization, and forgetting to switch modes can silently degrade results. Mixed-precision training with fp16 autocast typically requires a GradScaler to prevent gradient underflow, and using softmax before CrossEntropyLoss double-applies the normalization.

<details><summary>References</summary>
<ul>
<li><a href="https://www.geeksforgeeks.org/machine-learning/data-leakage/">Data Leakage - GeeksforGeeks</a></li>
<li><a href="https://stackoverflow.com/questions/60018578/what-does-model-eval-do-in-pytorch">What does model.eval () do in pytorch? - Stack Overflow Code sample</a></li>
<li><a href="https://apxml.com/courses/advanced-pytorch/chapter-3-optimization-training-strategies/mixed-precision-training">Mixed-Precision Training (AMP) in PyTorch</a></li>

</ul>
</details>

**Tags**: `#static-analysis`, `#machine-learning`, `#data-leakage`, `#developer-tools`, `#pytorch`

---

<a id="item-7"></a>
## [DialFork benchmark targets procedural hallucination in conversational LLM agents](https://www.reddit.com/r/MachineLearning/comments/1xofjrn/dialfork_a_benchmark_for_procedural_hallucination/) ⭐️ 7.0/10

Researchers from Idiap Research Institute and Logitech released DialFork, a benchmark that measures 'procedural hallucination'—where conversational agents make correct tool calls but fail to follow the required dialogue procedure. Built by forking conformant dialogues at controlled turn positions and injecting four hallucination types, it yields 36,278 dialogues across 24 tasks in 12 domains, validated by 30 human annotators. This introduces a third evaluation axis alongside factual accuracy and correct tool use, addressing a failure mode that is easy to miss but critical for deployed conversational agents. It provides the agent-evaluation community with a first-of-its-kind benchmark and public leaderboard to track progress on procedural fidelity. The benchmark defines three tasks: turn-level drift detection (including streaming), dialogue-level procedural distance, and set-level distribution comparison, each with its own leaderboard track on Hugging Face. Initial results from embedding-based distances, streaming detectors, and zero-shot LLMs leave substantial room for improvement, and all data, code, predictions, and human judgments are open.

reddit · r/MachineLearning · /u/sergbur · Nov 5, 10:44

**Background**: LLM agents are increasingly used in conversational settings where they must follow multi-step procedures—asking questions, confirming details, and reporting results—not just call tools correctly. Hallucination research has traditionally focused on factual errors and incorrect tool use, but procedural hallucination occurs when an agent's utterances drift from the required sequence even though each turn is fluent and factual. DialFork simulates this by replaying correct dialogues and injecting controlled deviations at known turn positions, enabling precise measurement of where and how far an agent drifts.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2610.21561">[2610.21561] DialFork: Going Beyond Factuality to Evaluate ...</a></li>
<li><a href="https://cctest.ai/en/articles/dialfork-tests-whether-agents-follow-the-conversation-procedure">DialFork Benchmarks Procedural Hallucination in AI Agents ...</a></li>

</ul>
</details>

**Tags**: `#LLM agents`, `#benchmark`, `#hallucination`, `#evaluation`, `#conversational AI`

---

<a id="item-8"></a>
## [Kagi opens search to everyone without an account](https://kagi.com/changelog#11820) ⭐️ 6.0/10

Kagi, the paid ad-free search engine, announced that anyone can now use its search directly from kagi.com without creating an account, receiving 50 free searches, with 100 more available after signing up for a free account. This lowers the barrier to trying Kagi, which has been a paid-only service, and could attract users frustrated with Google's ad-heavy results and privacy practices, intensifying competition among alternative search engines. After the initial 50 free searches, users can create a free account for 100 more, while paid plans start at $5 per month; Kagi's AI features remain opt-in and users can hide AI-generated images by default.

hackernews · elashri · Nov 5, 20:03 · [Discussion](https://news.ycombinator.com/item?id=50383740)

**Background**: Kagi is a paid, ad-free search engine developed by Kagi Inc. in Palo Alto, California, named after the Japanese word for 'key'. It aggregates results from multiple search engines while stripping ads and trackers, and its business model relies on subscriptions rather than advertising. The move comes as users increasingly seek privacy-focused alternatives to Google, such as DuckDuckGo and Brave Search.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kagi_(search_engine)">Kagi (search engine)</a></li>
<li><a href="https://kagi.com/">Kagi Search - Better search results. No ads.</a></li>
<li><a href="https://www.youtube.com/watch?v=Nr9BqrJzWSk">Kagi Search Now Works With No Account: 50 Free Searches Kagi drops its sign-up wall just as frustration over Google’s ... Kagi Blog - Celebrating 50K users with Kagi free search ... Kagi on X: "You can now try Kagi Search out of the box → no ... Kagi Search free alternative? : r/degoogle - Reddit</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters largely praised Kagi's search quality and features like custom site rankings, with some long-time subscribers sharing positive experiences. A notable request was for a DNS-enforced SafeSearch option, which has been in feedback since May 2022, to prevent Kagi from being blocked on filtered networks. Others expressed interest in trying Kagi due to frustration with Google and discussed alternatives like Ecosia and Qwant.

**Tags**: `#search-engines`, `#kagi`, `#privacy`, `#product-update`, `#hacker-news`

---

<a id="item-9"></a>
## [Blogger Revives Hackintosh with AI Assistance, Sparking Debate](https://www.naut.ca/blog/2026/11/05/the-hackintosh-reborn-with-ai/) ⭐️ 6.0/10

A blog post titled 'The Hackintosh Reborn' describes using AI tools to revive the Hackintosh practice of running macOS on non-Apple hardware, and it generated a 93-comment Hacker News discussion. This shows how AI-assisted development can lower the barrier to niche technical projects like Hackintosh, while the discussion highlights broader tensions between Apple's hardware dominance, macOS lock-in, and Linux alternatives. The article body is not provided, so details of the AI-assisted method are unclear; the discussion also touches on Asahi Linux's goal to support Apple silicon (including a hoped-for M5) and the observation that ARM Macs can run Switch games natively.

hackernews · rubatuga · Nov 5, 19:08 · [Discussion](https://news.ycombinator.com/item?id=50383057)

**Background**: A Hackintosh is a non-Apple computer configured to run macOS, a practice that became widespread after Apple's 2005 transition to Intel x86 processors but was expected to fade with Apple's shift to its own ARM-based silicon. AI-assisted software development uses large language models and AI agents to help with coding, debugging, and documentation. x86 is the dominant instruction set for desktop and laptop PCs, while ARM dominates mobile and is increasingly used in Apple laptops.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hackintosh">Hackintosh</a></li>
<li><a href="https://en.wikipedia.org/wiki/X86_architecture">X86 architecture</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI-assisted_software_development">AI-assisted software development - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters largely praised Apple's hardware while expressing frustration with macOS, with several wishing they could run Linux on MacBooks and hoping Asahi Linux will support future chips like the M5. One commenter called ARM Macs running Switch games natively a sign of the end of x86, and another argued Apple's value now lies in hardware rather than software.

**Tags**: `#hackintosh`, `#apple-hardware`, `#linux`, `#x86`, `#ai-assisted-development`

---

<a id="item-10"></a>
## [Salon Publishes Farewell Piece, Sparking Debate on Journalism's Decline](https://www.salon.com/2026/11/05/goodbye-from-salon/) ⭐️ 6.0/10

Salon, the pioneering online magazine founded in 1995, has published a farewell piece on its website, signaling its closure or end of operations. The announcement prompted a Hacker News discussion with 428 points and 159 comments about the long decline of newsroom jobs and the economics of online publishing. Salon's closure marks a cultural and industry milestone, as one of the first digital-native publications to gain mainstream influence has now shut down. It underscores the broader hollowing-out of journalism, where newsroom employment has fallen sharply and independent online publishers struggle to sustain profitable operations. Community comments note that newsroom jobs fell 60% between 2008 and 2020, with the biggest losses in beat reporting such as foreign bureaus, statehouse reporters, and regional specialty beats. One commenter who runs a long-standing online publication described only a brief window of modest profitability from 2012 to 2020, followed by an extreme drought in recent years.

hackernews · mkeeter · Nov 5, 20:03 · [Discussion](https://news.ycombinator.com/item?id=50383739)

**Background**: Salon was founded in 1995 as one of the first online-only magazines, known for publishing literary and political journalism and launching the careers of many writers. The digital transition eroded the advertising revenue that traditionally funded newsrooms, and platforms like Google and social media reshaped how audiences find news. In recent years, AI-generated search summaries and changing consumer habits have further reduced traffic to independent publishers.

<details><summary>References</summary>
<ul>
<li><a href="https://journonews.com/newsroom-employment-decline-accelerates-journalism-industry-faces-existential-crisis-as-revenue-models-collapse/">Newsroom Employment Decline Accelerates; Journalism Industry ...</a></li>
<li><a href="https://www.elizabethgrieco.com/u-s-newsroom-employment-dropped-40-percent-since-2008-driven-by-losses-at-newspapers/">U.S. Newsroom Employment Dropped 40 Percent Since 2008 ...</a></li>
<li><a href="https://thinkinsights.net/digital-transformation/industry-analysis-online-publishing">Industry Analysis: Online Publishing | Think Insights</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree that the decline of beat reporting and the hollowing-out of newsrooms predates both the open internet and AI, with one noting that the shift online masked a massive loss of sources. Others share personal experiences of running unprofitable online publications out of passion, and some criticize Salon's later editorial direction or attribute its irrelevance to declining Reddit traffic after Google's AI Overviews.

**Tags**: `#journalism`, `#media-industry`, `#online-publishing`, `#newsroom-decline`, `#community-discussion`

---

<a id="item-11"></a>
## [Motorola Signature 27 launches with official GrapheneOS support at $1,599](https://motorolanews.com/motorola-signature-27-2/) ⭐️ 6.0/10

Motorola has announced the Signature 27, a flagship smartphone with a starting MSRP of $1,599 that will officially support GrapheneOS, marking the first non-Pixel device to receive such certification. This is a significant milestone for the privacy-focused mobile community because GrapheneOS has until now been officially available only on Google Pixel devices, so expanding to Motorola gives users a new hardware option and could pressure other OEMs to follow suit. The high $1,599 price limits accessibility, and trust concerns remain because Motorola modifies low-level firmware components such as the bootloader and modem, which could affect GrapheneOS's security guarantees; the device also oddly promotes Gemini alongside GrapheneOS.

hackernews · monneyboi · Nov 5, 16:01 · [Discussion](https://news.ycombinator.com/item?id=50380810)

**Background**: GrapheneOS is an open-source, privacy- and security-hardened mobile operating system built on the Android Open Source Project. Due to strict hardware security requirements, it has been officially supported only on recent Google Pixel devices, though the project announced in 2026 plans to certify selected Motorola devices. Android Verified Boot is a key mechanism that ensures the integrity of the operating system, and custom OS support requires cooperation from device makers and chip vendors.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GrapheneOS">GrapheneOS</a></li>
<li><a href="https://source.android.com/docs/security/features/verifiedboot/boot-flow">Boot flow | Security | Android Open Source Project</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters expressed skepticism about trusting Motorola, citing its Chinese ownership and firmware modifications, while others questioned the odd pairing of GrapheneOS with Gemini. Many also criticized the $1,599 price, saying they would rather stick with cheaper Pixel devices or wait for mid-range Motorola options.

**Tags**: `#GrapheneOS`, `#mobile-security`, `#privacy`, `#hardware`, `#Android`

---

<a id="item-12"></a>
## [Blog Post Urges Archiving YouTube Videos Before They Disappear](https://criminallyvulgar.dev/you-should-absolutely-download-your-favourite-youtube-videos/) ⭐️ 6.0/10

A blog post on criminallyvulgar.dev argues that users should download and archive their favorite YouTube videos before they vanish, sparking a Hacker News discussion with 278 points and 124 comments about archiving practices, legal limitations, and tools like yt-dlp. The post highlights the growing issue of digital content disappearing from platforms due to copyright takedowns, account deletions, or policy changes, affecting anyone who relies on YouTube as a cultural or educational archive. It underscores the tension between preservation and copyright law, and the practical role of tools like yt-dlp in personal archiving. The discussion mentions that playlists often show 'unavailable videos are hidden' at rates around 10% for five-year-old lists, and that yt-dlp can preserve playlist structure using commands like --embed-metadata and --parse-metadata. Legal caveats include that downloading copyrighted content without permission generally violates YouTube's Terms of Service and may infringe copyright under the DMCA, even for personal use.

hackernews · surprisetalk · Nov 5, 13:00 · [Discussion](https://news.ycombinator.com/item?id=50378571)

**Background**: YouTube hosts billions of videos, but content can be removed for various reasons, leading to link rot and lost media. yt-dlp is a community-maintained fork of youtube-dl, a command-line tool for downloading videos from YouTube and over 1,000 other sites, widely used for archiving, education, and journalism despite legal challenges. Digital archiving involves preserving content for future access, but copyright law often restricts sharing archived material, creating a 'hoarding' dilemma for archivists.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Yt-dlp">Yt-dlp</a></li>
<li><a href="https://github.com/yt-dlp/yt-dlp">GitHub - yt-dlp/yt-dlp: A feature-rich command-line audio ...</a></li>
<li><a href="https://legallyexplained.com/is-it-legal-to-download-youtube-videos/">Is It Legal to Download YouTube Videos? 2026 Guide</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree with the archiving sentiment, sharing anecdotes of lost videos and large personal archives, but some raise concerns about legal sharing and the futility of hoarding. Others debate the value of letting content disappear, while technical tips include using yt-dlp commands to maintain playlist structure and warnings to keep archiving methods quiet to avoid losing access.

**Tags**: `#YouTube`, `#digital-archiving`, `#data-preservation`, `#yt-dlp`, `#copyright`

---

<a id="item-13"></a>
## [Opinion: Tech Companies Still Fail to Understand Users Despite Data Collection](https://rakhim.exotext.com/i-wish-tech-companies-knew-more-about-me) ⭐️ 6.0/10

An opinion piece on rakhim.exotext.com argues that despite massive data collection, tech companies' personalization and targeted advertising still fail to understand users, sparking a rich Hacker News debate with 272 comments. This matters because it questions the effectiveness of the multi-billion-dollar personalization and ad-tech industry, suggesting that current algorithms may not deliver the value they promise to users or advertisers. The article is an opinion piece without technical specifics, but the community discussion highlights concrete examples such as Spotify and YouTube Music failing to notice that a user skips every electronic track with vocals, and Google's real advertising proposition of selling access to an expensive website's audience on cheaper sites.

hackernews · freetonik · Nov 5, 13:40 · [Discussion](https://news.ycombinator.com/item?id=50378942)

**Background**: Recommendation systems and targeted advertising rely on collecting user behavior data to predict preferences and serve personalized content or ads. Despite advances in machine learning, these systems often optimize for engagement or advertiser goals rather than genuine user understanding, leading to phenomena like filter bubbles and irrelevant ads.

<details><summary>References</summary>
<ul>
<li><a href="https://mljourney.com/how-recommendation-systems-work/">How Recommendation Systems Work - ML Journey</a></li>
<li><a href="https://en.wikipedia.org/wiki/Filter_bubble">Filter bubble - Wikipedia</a></li>
<li><a href="https://theconversation.com/the-ugly-truth-tech-companies-are-tracking-and-misusing-our-data-and-theres-little-we-can-do-127444">The ugly truth: tech companies are tracking and misusing our data ...</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree that targeted advertising fails to understand users, with some arguing that ads are about selling advertisers' products rather than finding what users want, and others noting that many people don't mind ads. A key insight is that Google's tracking is primarily to sell audiences across sites, not to understand user desires.

**Tags**: `#personalization`, `#targeted-advertising`, `#recommendation-systems`, `#privacy`, `#tech-industry`

---

<a id="item-14"></a>
## [Sparse Predictive Hierarchies Fail to Match Backprop on Chess Prediction Task](https://www.reddit.com/r/MachineLearning/comments/1xov58r/empirical_evaluation_of_sparse_predictive/) ⭐️ 6.0/10

A new empirical study tested Sparse Predictive Hierarchies (SPH) with local learning rules on chess policy/value prediction against an Lc0 baseline, finding that a 44.9M-parameter SPH model catastrophically underperformed a 3.8M-parameter CNN trained with standard backpropagation on the same dataset splits. This negative result provides valuable evidence that extreme sparsity (~99%) and local learning rules struggle with tasks requiring long-range global credit assignment, such as chess, highlighting a fundamental limitation for biologically inspired architectures and informing future research in neuromorphic computing and non-backprop learning. The SPH model used Fuzzy ART-based encoders, Dendritic Neural Layers with Leaky ReLU, and specialized policy/value heads matching Lc0 formats, with byte weights and stochastic rounding for SIMD throughput; the control CNN had only 32 channels and ~3.8M parameters, yet quickly learned board geometry and tactical threats while the SPH model failed to converge on policy.

reddit · r/MachineLearning · /u/Severe-Heat-518 · Nov 5, 21:40

**Background**: Sparse Predictive Hierarchies (SPH) are an online machine learning system developed by Ogma Corp that uses local learning rules and extreme sparsity, implemented in libraries like OgmaNeo2 and AOgmaNeo. Unlike standard deep learning models (e.g., ResNets, Transformers) that rely on global backpropagation, SPH aims to learn from streaming data with a low compute footprint, often applied in robotics and control. Fuzzy ART is a neural network model based on Adaptive Resonance Theory that performs stable category learning for analog patterns, used here as an encoder.

<details><summary>References</summary>
<ul>
<li><a href="https://ogma.ai/wp-content/uploads/2023/05/SPH_Whitepaper.pdf">Sparse Predictive Hierarchies - Ogma Intelligent Systems Corp</a></li>
<li><a href="https://github.com/ogmacorp/OgmaNeo2">GitHub - ogmacorp/OgmaNeo2: Sparse Predictive Hierarchies (SPH) dcc_sph — Sparse Predictive Hierarchies in Rust - GitHub Ogma's Sparse Predictive Hierarchies - Tangential Theories ... A Tutorial on Sparse Predictive Hierarchies: A Tutorial on OgmaNeo2 – Ogma Intelligent Systems Corp Sparse Predictive Hierarchies</a></li>
<li><a href="https://en.wikipedia.org/wiki/Adaptive_resonance_theory">Adaptive resonance theory - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#machine-learning`, `#non-backprop-learning`, `#sparse-networks`, `#chess`, `#negative-results`

---

<a id="item-15"></a>
## [Animated explainer shows how LLMs pick next token with real Qwen2.5-0.5B probabilities](https://www.reddit.com/r/MachineLearning/comments/1xopogt/i_animated_how_a_language_model_picks_the_next/) ⭐️ 6.0/10

A new 7-minute animated video walks through the token selection process of a language model using real probabilities from Qwen2.5-0.5B-Instruct, covering softmax, greedy vs. sampling, temperature, top-k, and top-p. The explainer follows a single example where the model is prompted to 'Write one sentence about the moon,' showing how after the token 'The', the model assigns 78.04% probability to 'moon' and 1.50% to 'lunar', and demonstrates how different sampling settings alter the outcome. This explainer provides a concrete, numbers-driven walkthrough of core decoding concepts that are often explained abstractly, making it a valuable pedagogical resource for learners. It also highlights practical nuances like the non-determinism of temperature 0 on servers due to batch-size-dependent addition order, which can affect reproducibility in real deployments. The video uses Qwen2.5-0.5B-Instruct with a vocabulary of 151,936 tokens and shows that greedy decoding always picks 'moon' while sampling can pick 'lunar' about 1 in 67 times. It also demonstrates top-k vs. top-p behavior, noting that at top-p 0.9, 8 tokens are kept at one step but only 1 at another where 'of' has 97.9% probability, and mentions that even temperature 0 can yield 80 different answers from 1,000 runs of Qwen3-235B due to batch-size-dependent addition order.

reddit · r/MachineLearning · /u/Rajucg · Nov 5, 18:05

**Background**: Language models generate text one token at a time by computing a probability distribution over their entire vocabulary using the softmax function. Decoding strategies like greedy selection (always picking the highest-probability token) and sampling (randomly picking according to probabilities) control how the next token is chosen. Temperature scales the logits before softmax to adjust randomness, while top-k and top-p (nucleus) sampling truncate the distribution to limit choices to the most likely tokens. These concepts are fundamental to understanding and tuning LLM outputs.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen2.5-0.5B-Instruct">Qwen/Qwen2.5-0.5B-Instruct · Hugging Face</a></li>
<li><a href="https://www.f22labs.com/blogs/what-are-temperature-top_p-and-top_k-in-ai/">Temperature, Top - p & Top - k : Best LLM Settings Explained</a></li>
<li><a href="https://memx.app/glossary/temperature-and-sampling/">Temperature and Sampling in LLMs Explained | MemX</a></li>

</ul>
</details>

**Tags**: `#llm`, `#sampling`, `#education`, `#softmax`, `#temperature`

---

<a id="item-16"></a>
## [ML PhD publication expectations: how many papers are 'productive' now?](https://www.reddit.com/r/MachineLearning/comments/1xo7q89/what_is_now_considered_a_reasonable_publication/) ⭐️ 5.0/10

A Reddit discussion on r/MachineLearning asks what publication rate is now considered 'productive' for ML PhD students and whether LLMs have inflated expectations. The thread also questions whether PhD applicants face higher pre-PhD research output expectations. Publication expectations directly affect PhD students' graduation timelines, mental health, and career prospects, and shifting norms can influence admissions and hiring in ML. If LLMs lower the barrier to producing papers, the community may need to rethink how productivity is evaluated. The discussion references top ML conferences such as NeurIPS, ICML, and ICLR, with one commenter suggesting that around 4 first-author papers at such venues is a standard expectation for graduating from a top ML PhD program. However, this impression is anecdotal and may be biased by social media posts.

reddit · r/MachineLearning · /u/confirm-jannati · Nov 5, 02:55

**Background**: NeurIPS, ICML, and ICLR are widely regarded as the premier conferences in machine learning, and publishing there is highly competitive. PhD programs in ML typically require a certain number of first-author papers for graduation, but expectations vary by institution and advisor. The rise of large language models (LLMs) has made it easier to generate text and code, potentially accelerating research output and raising questions about inflated publication norms.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Conference_on_Neural_Information_Processing_Systems">Conference on Neural Information Processing Systems - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/International_Conference_on_Machine_Learning">International Conference on Machine Learning - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/International_Conference_on_Learning_Representations">International Conference on Learning Representations - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The discussion reflects a community concern that publication expectations may be rising, possibly due to LLMs, but lacks consensus or concrete data. Commenters share anecdotal impressions, such as the 4 first-author papers benchmark, while questioning whether this is accurate for top programs.

**Tags**: `#academia`, `#machine-learning`, `#phd`, `#publication-metrics`, `#community-discussion`

---

<a id="item-17"></a>
## [Student asks: separate models or one global model for demand forecasting across 40 locations?](https://www.reddit.com/r/MachineLearning/comments/1xohxyv/best_approach_for_demand_forecasting_across_40/) ⭐️ 5.0/10

A final-year B.Tech CSE (AI/ML) student working on a multi-agent supply chain optimization project is asking for advice on whether to train 40 separate per-location demand forecasting models or a single global model on a synthetic dataset of about 1.1 million records across 40 retail locations. The global-versus-local model tradeoff is a classic and recurring design decision in demand forecasting, and the answer directly affects forecast accuracy at the product-location level, which downstream inventory planning and supply chain agents depend on. The student is concerned that a global model may average out regional demand patterns and produce inaccurate location-level forecasts, and also asks about hybrid approaches such as grouping similar locations, precautions for evaluating models on synthetic data, suitable forecasting architectures, and validation strategies that avoid data leakage across locations and time-dependent features.

reddit · r/MachineLearning · /u/Crafty_Rabbit2411 · Nov 5, 12:55

**Background**: Demand forecasting involves predicting future product demand from historical time-series data, and a central modeling choice is whether to fit one model per series (local) or a single model across many related series (global). Global models can share statistical strength across locations and handle sparse series better, while local models can capture location-specific dynamics but may overfit when data per location is limited. In multi-agent supply chain systems, specialized agents for forecasting, inventory, and logistics coordinate to improve overall decisions.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2411.06394v1">Local vs. Global Models for Hierarchical Forecasting</a></li>
<li><a href="https://medium.com/data-science/local-vs-global-forecasting-what-you-need-to-know-1cc29e66cae0">Local vs Global Forecasting: What You Need to Know</a></li>
<li><a href="https://www.ijert.org/research/multi-agent-supply-chain-optimization-system-IJERTV15IS030969.pdf">Multi-Agent Supply Chain Optimization System</a></li>

</ul>
</details>

**Tags**: `#demand-forecasting`, `#time-series`, `#machine-learning`, `#modeling-strategy`, `#supply-chain`

---

<a id="item-18"></a>
## [Window Sweaters: A Whimsical macOS App for Knitted Window Borders](https://github.com/saragordic/window-sweaters) ⭐️ 4.0/10

Product designer Sara Gordic released Window Sweaters, her first open-source project, a macOS menu-bar app that adds customizable knitted borders to windows. The project was shared on Hacker News, where it received mixed reactions. While the app itself is a small, whimsical utility with limited technical depth, its discussion highlights broader concerns about supply-chain trust in running new GitHub projects and skepticism toward LLM-era side projects. The app is built as a macOS menu-bar application that lets users apply configurable window borders and supports custom colorways. The installer backs up any previous local installation before replacing it, and the project is written in Swift.

hackernews · nickswalker · Nov 5, 16:50 · [Discussion](https://news.ycombinator.com/item?id=50381383)

**Background**: Window Sweaters is a personalization tool for macOS that decorates window edges with knitted patterns, similar to festive dock decorations. Supply-chain attacks, where malicious code is injected into open-source dependencies, have become a major security concern, making users cautious about running unvetted code. Meanwhile, the rise of LLMs has made it easier to generate code, leading some to question the effort behind new projects.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/saragordic/window-sweaters">GitHub - saragordic/ window - sweaters : A macOS menu-bar app that...</a></li>
<li><a href="https://blog.talosintelligence.com/protecting-supply-chain-2026/">Do not get high(jacked) off your own supply ( chain )</a></li>
<li><a href="https://www.linkedin.com/posts/loheander_code-review-of-llm-generated-code-is-a-trust-activity-7467490058208641024-iqza">Code review of LLM - generated code is a trust problem.</a></li>

</ul>
</details>

**Discussion**: Commenters expressed a mix of appreciation and concern: one praised the idea but said they no longer trust running code from unknown new GitHub repos due to supply-chain attacks; another felt such projects have lost their magic now that LLMs can generate them easily; and a third criticized the lack of real screenshots showing the app in action. The author responded, clarifying it was her first open-source project made purely for fun and acknowledging the trust concerns.

**Tags**: `#open-source`, `#side-project`, `#supply-chain-security`, `#LLM`, `#design`

---

<a id="item-19"></a>
## [Reddit Thread Invites ICLR 2027 Review Results Sharing](https://www.reddit.com/r/MachineLearning/comments/1xo6yzo/iclr_2027_reviews_discussion_d/) ⭐️ 4.0/10

A Reddit user posted a discussion thread on r/MachineLearning inviting researchers to share their ICLR 2027 review results as decisions are released, and pointed to tools like papercopilot and paperScorer for gauging acceptance odds. This thread reflects the growing community practice of using data-driven and LLM-based tools to predict peer-review outcomes, which can inform authors' expectations but also raises questions about over-reliance on such predictions. The original poster explicitly notes that these tools are 'only for amusement and should not be taken seriously,' and the thread itself contains no technical content or official information about ICLR 2027 review statistics.

reddit · r/MachineLearning · /u/Beautiful_Baker_2233 · Nov 5, 02:17

**Background**: ICLR (International Conference on Learning Representations) is a premier machine learning conference that uses OpenReview for peer review, where scores and reviews are publicly visible. Papercopilot is a project that aggregates and analyzes ICLR review data, while PaperScorer is a family of models (including a 7B vision-language model) that predicts accept/reject decisions from paper text and screenshots. These tools have gained attention as submission volumes to ML conferences have reached record highs.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/papercopilot/iclr-insights">papercopilot / iclr -insights: Insights from the ICLR Peer Review and...</a></li>
<li><a href="https://arxiv.org/abs/2610.31791">PaperScorer: How Predictable Is Paper Acceptance?</a></li>
<li><a href="https://huggingface.co/skonan/PaperScorer-7B-Vision-OpenReview-ICLR">PaperScorer-7B-Vision-OpenReview-ICLR - Hugging Face</a></li>

</ul>
</details>

**Tags**: `#ICLR`, `#peer-review`, `#academic-conferences`, `#machine-learning`, `#community-discussion`

---

<a id="item-20"></a>
## [Paul Ford: Browsers Are Powerful and Getting Cheaper](https://simonwillison.net/2026/Nov/5/paul-ford/) ⭐️ 3.0/10

Simon Willison quoted Paul Ford's observation from his essay 'The Web Is More Than Enough' that web browsers are very powerful application platforms and that the cost of accessing that power is decreasing seemingly every day. This highlights the ongoing trend of web browsers becoming more capable and accessible, which lowers barriers for developers to build and distribute applications, potentially affecting how software is created and consumed across the industry. The quote is a brief excerpt shared via Willison's link blog, pointing to Ford's original essay; it lacks technical specifics but underscores the economic and practical advantages of browser-based development.

rss · Simon Willison · Nov 5, 17:34

**Background**: Paul Ford is a technologist and essayist known for his writing on technology and culture, including the 2015 Bloomberg piece 'What Is Code?'. Web browsers have evolved from simple document viewers to platforms supporting complex applications like Progressive Web Apps (PWAs), which can behave like native apps. The declining cost of accessing browser capabilities refers to improvements in performance, standards, and tooling that make web development more efficient and affordable.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bloomberg.com/graphics/2015-paul-ford-what-is-code/">Paul Ford : What Is Code? | Bloomberg</a></li>
<li><a href="https://dragganaitool.com/the-evolution-of-web-browsers-from-simple-tools-to-smart-platforms/">The Evolution of Web Browsers : From Simple Tools to Smart Platforms</a></li>

</ul>
</details>

**Tags**: `#browsers`, `#web-development`, `#paul-ford`, `#web-platform`, `#link-blog`

---