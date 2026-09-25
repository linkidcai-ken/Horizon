---
layout: default
title: "Horizon Summary: 2026-09-25 (EN)"
date: 2026-09-25
lang: en
---

> From 25 items, 17 important content pieces were selected

---

1. [F-Droid 2.0 Launches With Major Redesign and Kotlin Rewrite](#item-1) ⭐️ 8.0/10
2. [Apple Disables Advanced Data Protection in the UK](#item-2) ⭐️ 8.0/10
3. [Whiteboard: An Open-Source IDE for Human-AI Software Architecture](#item-3) ⭐️ 7.0/10
4. [Why Is the Liver So Weirdly Regenerative?](#item-4) ⭐️ 7.0/10
5. [California's Wealth Tax Problem and the Land Value Tax Alternative](#item-5) ⭐️ 7.0/10
6. [arXiv Secures $17.2M to Launch as Independent Nonprofit](#item-6) ⭐️ 7.0/10
7. [Multirate DSP Principles Applied to LLMs via Hierarchical Semantic Vocoder](#item-7) ⭐️ 7.0/10
8. [Koi.rest: AI-Built Virtual Koi Pond for Relaxation](#item-8) ⭐️ 6.0/10
9. [NeurIPS Accepted Papers Visible Before Official Notifications](#item-9) ⭐️ 6.0/10
10. [Datasette 1.0a41 adds OpenTelemetry and Web Component modals](#item-10) ⭐️ 5.0/10
11. [Fifth-Year PhD Student Seeks Non-Elitist Publication Venues for Efficient Generative AI Research](#item-11) ⭐️ 4.0/10
12. [New Data Science Grad Seeks AI Residency and Pre-Doc Programs](#item-12) ⭐️ 4.0/10
13. [commit-rewriter 0.2 Adds Non-Default Branch Support](#item-13) ⭐️ 3.0/10
14. [NeurIPS Author Questions Missing Final Justification on Rejected Paper](#item-14) ⭐️ 3.0/10
15. [NeurIPS Author Registration Confusion as Sydney and Paris Venues Sell Out](#item-15) ⭐️ 3.0/10
16. [Reddit user asks: Sydney or Atlanta for NeurIPS 2026?](#item-16) ⭐️ 3.0/10
17. [EACL Author Asks Whether to Contact AC Over Silent Reviewers](#item-17) ⭐️ 3.0/10

---

<a id="item-1"></a>
## [F-Droid 2.0 Launches With Major Redesign and Kotlin Rewrite](https://f-droid.org/2026/09/24/f-droid-2.0-a-new-chapter-for-android-freedom.html) ⭐️ 8.0/10

F-Droid 2.0 was released on September 24, 2026, marking the largest update to the open-source Android app store in 10 years. The release is a complete redesign rewritten in Kotlin with Jetpack Compose, featuring simplified three-tab navigation (Discover, Search, My Apps), expanded categories, improved multilingual search including CJK support, and combinable filters, while phasing out the privileged extension. As one of the most widely used open-source Android app stores, F-Droid's overhaul affects a large community of privacy-conscious and free-software users who rely on it as an alternative to Google Play. The redesign and the phase-out of the privileged extension could reshape how users install and update apps, especially amid concerns about Google's upcoming Android lockdown. The update rewrites core components in Kotlin and builds the UI with Jetpack Compose, and it phases out the F-Droid Privileged Extension, which previously allowed silent background installs and updates when installed as a system app with root privileges. Community members noted UI issues in early screenshots, such as a broken line break in 'Syncthing-Fork' and a lack of visual differentiation between sections.

hackernews · daveoc64 · Sep 24, 15:26 · [Discussion](https://news.ycombinator.com/item?id=49831968)

**Background**: F-Droid is a free and open-source app repository for Android that only distributes software whose source code is available and buildable without proprietary dependencies. The F-Droid Privileged Extension is an optional system component that, when installed as a privileged app, lets F-Droid install, update, and remove apps without requiring the user to enable 'Unknown Sources' or manually confirm each install. F-Droid 2.0 is the project's first major redesign in a decade, moving to modern Android development practices with Kotlin and Jetpack Compose.

<details><summary>References</summary>
<ul>
<li><a href="https://f-droid.org/2026/09/24/f-droid-2.0-a-new-chapter-for-android-freedom.html">F-Droid 2.0: A New Chapter for Android Freedom | F-Droid - Free and Open Source Android App Repository</a></li>
<li><a href="https://daily.dev/posts/f-droid-2-0-gyxrkowac">F-Droid 2.0 | daily.dev</a></li>
<li><a href="https://f-droid.org/packages/org.fdroid.fdroid.privileged/">F - Droid Privileged Extension | F - Droid - Free and Open Source...</a></li>

</ul>
</details>

**Discussion**: The 248-comment discussion was largely critical of the new UI, with users complaining about a lack of visual differentiation between sections, unclear tappable areas, and a broken line break in a screenshot. Some praised the overhaul and the phase-out of the privileged extension, while others raised concerns about F-Droid's future once Google tightens Android restrictions next year.

**Tags**: `#F-Droid`, `#Android`, `#Open Source`, `#App Store`, `#Mobile Freedom`

---

<a id="item-2"></a>
## [Apple Disables Advanced Data Protection in the UK](https://macanorak.com/two-tier-encryption-in-the-uk/) ⭐️ 8.0/10

Apple has disabled its Advanced Data Protection (ADP) feature for iCloud users in the United Kingdom, reverting affected data categories to Standard Data Protection where Apple holds the encryption keys. This move came in response to a legal order under the UK's Investigatory Powers Act that would have required Apple to weaken its end-to-end encryption architecture. This creates a two-tier encryption system where UK users have weaker privacy protections than users elsewhere, potentially setting a precedent for other governments to demand similar access. It also raises concerns about platform trust and whether companies can resist legal coercion to undermine encryption. ADP normally increases the number of end-to-end encrypted iCloud categories from 14 to 23, but UK users without ADP lose end-to-end encryption for iCloud Backup, Photos, Notes, and iCloud Drive. Baseline categories such as iCloud Keychain and Health remain end-to-end encrypted by default.

hackernews · ReturnoftheHack · Sep 24, 10:39 · [Discussion](https://news.ycombinator.com/item?id=49828731)

**Background**: Advanced Data Protection is an optional Apple feature that extends end-to-end encryption to more iCloud data types, meaning only the user's devices hold the decryption keys. The UK's Investigatory Powers Act 2016 allows the government to issue technical capability notices compelling companies to assist with lawful interception, and in 2024 Apple contested proposed changes to the Act as an 'unprecedented overreach.'

<details><summary>References</summary>
<ul>
<li><a href="https://support.apple.com/en-us/108756">How to turn on Advanced Data Protection for iCloud - Apple Support</a></li>
<li><a href="https://en.wikipedia.org/wiki/Investigatory_Powers_Act_2016">Investigatory Powers Act 2016 - Wikipedia</a></li>
<li><a href="https://www.bbc.co.uk/news/articles/c20g288yldko">UK government demands access to Apple users' encrypted data</a></li>

</ul>
</details>

**Discussion**: Commenters are divided: some argue Apple has lost the courage it showed in 2015 when it resisted the FBI, pointing to mandatory age verification and KYC screens as signs of capitulation. Others note that withdrawing ADP was a pragmatic third option that satisfied the legal requirement without building a backdoor, while some call for Apple to exit the UK market entirely and warn that once such a precedent is set, it will be hard to reverse.

**Tags**: `#encryption`, `#privacy`, `#Apple`, `#UK policy`, `#security`

---

<a id="item-3"></a>
## [Whiteboard: An Open-Source IDE for Human-AI Software Architecture](https://github.com/devdotfast/whiteboard) ⭐️ 7.0/10

A team of four developers (Sid, Alex, Ketan, and Milan) launched Whiteboard, an MIT-licensed open-source desktop app that lets humans and AI coding agents architect software together on a shared canvas, integrating with tools like Claude Code and Codex. The app is built on top of CodeOSS and introduces a Rust-based semantic AST-aware diff viewer, clickable diagrams that jump to underlying code, and a Decision Log that links agent traces to requirements. As agentic coding becomes standard, developers increasingly merge AI-generated PRs they don't fully understand, accumulating what the team calls 'cognitive debt'; Whiteboard targets this by making architecture- and spec-level review a first-class, visual workflow. Its adoption by teams at Salesforce and Modal suggests real demand for human-in-the-loop review tools that sit above fast-moving coding agents. The semantic diff viewer summarizes large added functions as pseudocode and collapses unit tests and large documentation changes by default, all customizable via a WASM-based plugin system; however, users currently cannot edit files directly in Whiteboard, and the desktop app is macOS-only. The team plans to eventually charge for a hosted web version with trajectory storage and multiplayer reviews, while keeping everything self-hostable.

hackernews · sidharthkmenon · Sep 24, 17:21 · [Discussion](https://news.ycombinator.com/item?id=49833867)

**Background**: Whiteboard is built on CodeOSS, the open-source core of Visual Studio Code, which gives it VSCode's keybindings and Language Server Protocol (LSP) support out of the box. It connects to agentic coding tools such as Anthropic's Claude Code and OpenAI's Codex, which are terminal-based AI agents that can autonomously edit files and run commands. The project's 'semantic diff' concept refers to comparing code changes by their abstract syntax tree (AST) structure rather than line-by-line text, so reviewers see meaningful logic changes instead of formatting noise.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/microsoft/vscode">microsoft/vscode: Visual Studio Code - GitHub</a></li>
<li><a href="https://stackoverflow.com/questions/53867739/differences-between-code-oss-and-visual-studio-code">Differences between Code OSS and Visual Studio Code [closed] - Stack Overflow</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**Discussion**: Commenters were broadly positive, with one calling the streaming diagram animations a technique that will be everywhere within a year, and another praising the semantic diff viewer as something most coding harnesses handle poorly. Skepticism centered on diagram accuracy: one user flagged a sequence-diagram label ('wait for release') that didn't match the shown diff, warning about LLM development tools hallucinating, while another questioned whether an app that can't edit files still qualifies as an IDE.

**Tags**: `#open-source`, `#IDE`, `#AI-agents`, `#software-design`, `#developer-tools`

---

<a id="item-4"></a>
## [Why Is the Liver So Weirdly Regenerative?](https://dynomight.substack.com/p/liver) ⭐️ 7.0/10

A new essay on the Dynomight Substack explores why the liver is uniquely capable of regeneration, blending biology, evolutionary trade-offs, and personal narrative, and it sparked a lively Hacker News discussion featuring medical anecdotes and scientific debate. Understanding liver regeneration matters for regenerative medicine, cancer research, and transplant surgery, since the liver's ability to regrow after partial removal is both a clinical asset and a potential evolutionary trade-off linked to cirrhosis and cancer. Liver regeneration after partial hepatectomy proceeds through priming, proliferation, and termination phases, driven by cytokines and growth factors such as MET and EGFR; however, the process is compensatory hyperplasia rather than true organ regrowth, and it can go awry in chronic injury, leading to fibrosis or cancer.

hackernews · jbotz · Sep 24, 16:23 · [Discussion](https://news.ycombinator.com/item?id=49832938)

**Background**: The liver is the only internal human organ capable of significant regeneration; after surgical removal of up to two-thirds of its mass, the remaining tissue can regrow to its original size within weeks. This capacity is thought to have evolved as a survival advantage against injury and toxins, but it comes with trade-offs, as unchecked proliferation can contribute to liver cancer. The article and discussion also touch on why other organs, like the heart or kidneys, lack this ability.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Liver_regeneration">Liver regeneration - Wikipedia</a></li>
<li><a href="https://www.nature.com/articles/s41575-020-0342-4">Liver regeneration: biological and pathological mechanisms and implications | Nature Reviews Gastroenterology & Hepatology</a></li>
<li><a href="https://news.mit.edu/2021/3-questions-kristin-knouse-livers-regenerative-capabilities-1215">3 Questions: Kristin Knouse on the liver ’s regenerative capabilities</a></li>

</ul>
</details>

**Discussion**: Commenters shared personal experiences with liver transplants and wound healing, debated whether humans are optimized for skin and blood repair, and noted that regeneration is limited even in salamanders; the overall sentiment was appreciation for the article's human touch and accessible science writing.

**Tags**: `#biology`, `#regeneration`, `#evolution`, `#medicine`, `#science-communication`

---

<a id="item-5"></a>
## [California's Wealth Tax Problem and the Land Value Tax Alternative](https://blog.landeconomics.org/p/california-is-chasing-wealth-that) ⭐️ 7.0/10

A Land Economics blog post argues that California's reliance on taxing mobile wealth is fundamentally flawed because wealthy individuals can easily relocate or litigate to avoid such taxes, and proposes a land value tax (LVT) as a more stable alternative. The article sparked a high-quality Hacker News discussion with 283 comments debating the economic merits and practical implementation challenges of LVT. This debate is significant because California and other high-tax jurisdictions face growing pressure to fund public services while mobile capital and wealthy residents increasingly relocate to lower-tax regions, and the choice between wealth taxes and land value taxes could reshape tax policy design and economic competitiveness. The discussion also highlights broader questions about tax fairness, efficiency, and the feasibility of implementing theoretically sound policies in practice. Land value tax is levied solely on the unimproved value of land, excluding buildings and improvements, and economists since Adam Smith and David Ricardo have favored it for not causing economic inefficiency. However, implementation requires a robust land ownership register and accurate valuations that separate land value from improvements, which critics note is difficult—Santa Clara County's assessor, for example, sometimes simply divides total property value by two to estimate land value.

hackernews · idbnstra · Sep 24, 20:34 · [Discussion](https://news.ycombinator.com/item?id=49836419)

**Background**: A land value tax (LVT) is a levy on the value of land without regard to buildings or other improvements, and it is often associated with Henry George, who argued that land is a common inheritance and that taxing its unimproved value would discourage speculation and encourage efficient use. Wealth taxes, by contrast, target an individual's total net worth and are criticized for being difficult to enforce when assets and owners are mobile. California's tax system relies heavily on income and property taxes, and proposals for a wealth tax have raised concerns about capital flight.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Land_value_tax">Land value tax - Wikipedia</a></li>
<li><a href="https://worksinprogress.co/issue/the-failure-of-the-land-value-tax/">The failure of the land value tax - Works in Progress Magazine</a></li>
<li><a href="https://www.sciencedirect.com/science/article/abs/pii/S0264837719315704">Implementing a land value tax: Considerations on moving from theory to practice</a></li>

</ul>
</details>

**Discussion**: Commenters largely agreed that a wealth tax is a bad idea, with one noting it is a symptom of a broken tax system and that the wealthy can simply leave or fight in court. However, several raised concerns about LVT implementation, including how to accurately assess land value separately from improvements and whether the tax can truly be passed on to renters. Others argued that raising property taxes is politically unviable because homeowners strongly oppose it.

**Tags**: `#economics`, `#taxation`, `#california`, `#land-value-tax`, `#policy`

---

<a id="item-6"></a>
## [arXiv Secures $17.2M to Launch as Independent Nonprofit](https://www.reddit.com/r/MachineLearning/comments/1wox8kt/arxiv_receives_multiyear_philanthropic/) ⭐️ 7.0/10

arXiv announced it has received $17.2 million in multiyear philanthropic commitments from Simons Foundation International, XTX Markets, and Siegel Family Endowment, spanning three to five years, to support its launch as an independent nonprofit organization. This funding gives arXiv long-term financial stability as it separates from Cornell University and becomes self-governing, which matters because arXiv is the primary preprint platform for AI/ML, physics, and mathematics research, and its continuity directly affects how millions of researchers share and access findings. The commitments are multiyear, covering three to five years, and come from three distinct funders: Simons Foundation International, the UK-based algorithmic trading firm XTX Markets, and the Siegel Family Endowment; the announcement was made on the arXiv blog.

reddit · r/MachineLearning · /u/Nunki08 · Sep 24, 09:43

**Background**: arXiv is a free, open-access repository of electronic preprints in fields such as physics, mathematics, computer science, and statistics, launched in 1991 and now receiving roughly 24,000 submissions per month. It has historically been hosted and supported by Cornell University, but is transitioning to operate as an independent nonprofit. Preprints are papers posted publicly before peer review, and in many fields arXiv is the default place where research first appears.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ArXiv">ArXiv</a></li>
<li><a href="https://www.sfi.org.bm/">SFI - Simons Foundation International</a></li>
<li><a href="https://en.wikipedia.org/wiki/XTX_Markets">XTX Markets</a></li>

</ul>
</details>

**Tags**: `#arXiv`, `#open access`, `#research infrastructure`, `#philanthropy`, `#nonprofit`

---

<a id="item-7"></a>
## [Multirate DSP Principles Applied to LLMs via Hierarchical Semantic Vocoder](https://www.reddit.com/r/MachineLearning/comments/1wp4w9a/applying_multirate_dsp_principles_to_llms_a/) ⭐️ 7.0/10

A developer released a PyTorch reference architecture that applies multirate digital signal processing (DSP) principles to large language models, splitting generation into a slow-rate sentence-level Planner and a fast-rate token-level Vocoder. On TinyStories, the decoupled model reached validation loss 0.61 versus 2.37 for an equivalent-size baseline GPT, though it exhibited conditioning over-reliance and exposure bias. This cross-disciplinary experiment suggests that decoupling slow semantic planning from fast local token synthesis could improve convergence and efficiency in hierarchical text generation, offering an alternative to prefix-tuning or deep cross-attention. If the identified bottlenecks can be resolved, it may influence how future LLMs allocate compute across semantic and syntactic levels. The architecture uses a frozen SentenceTransformer for compressed semantic embeddings, a banded sliding-window causal mask for local attention, and a late-stage cross-attention adapter that adjusts logits via Logits_final = Logits_base + softplus(alpha) * Logits_delta. The author notes that true VRAM savings require swapping standard PyTorch boolean masking for FlashAttention-2 block-sparse masks, and that 15% semantic dropout did not prevent artificially high Top-1 accuracy (~85%).

reddit · r/MachineLearning · /u/valrela · Sep 24, 15:34

**Background**: Multirate DSP is a classical signal-processing technique that processes signals at different sampling rates, using upsampling and downsampling to separate slow-varying content from fast details. In text-to-speech, a similar two-stage design is standard: a model generates a slow-rate mel-spectrogram, and a high-rate vocoder such as WaveNet synthesizes discrete audio samples. This project transfers that idea to LLMs by treating BPE tokens as the fast discrete signal and sentence-level semantic embeddings as the slow continuous signal.

<details><summary>References</summary>
<ul>
<li><a href="https://www.eetimes.com/multirate-dsp-part-1-upsampling-and-downsampling/">EETimes - Multirate DSP , Part 1: Upsampling and Downsampling</a></li>
<li><a href="https://yusukehashimotolab.github.io/AI-Knowledge-Notes/knowledge/en/ML/speech-audio-introduction/chapter4-speech-synthesis.html">Chapter 4: Speech Synthesis ( TTS ) - AI Terakoya</a></li>
<li><a href="https://arxiv.org/abs/2602.23333">[2602.23333] SemanticVocoder: Bridging Audio Generation and Audio Understanding via Semantic Latents</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#DSP`, `#hierarchical-modeling`, `#PyTorch`, `#text-generation`

---

<a id="item-8"></a>
## [Koi.rest: AI-Built Virtual Koi Pond for Relaxation](https://koi.rest/) ⭐️ 6.0/10

A developer named Paul, who has ADHD and recently became unemployed, launched Koi.rest, a virtual koi pond built entirely with AI assistance despite his lack of JavaScript knowledge. The project was shared on Hacker News as a Show HN post, where it received 101 points and 24 comments. This project exemplifies the growing trend of AI-assisted development, where individuals can create functional web applications without deep programming expertise. It also highlights how personal projects can address mental health and relaxation needs, resonating with a community facing similar challenges. The virtual pond allows users to watch koi fish and listen to zen background sounds, but users reported performance issues such as low frame rates (around 3fps) and laggy interactions. The developer used AI to code the project, embracing a 'good enough' approach rather than perfection.

hackernews · hxii · Sep 24, 21:33 · [Discussion](https://news.ycombinator.com/item?id=49837006)

**Background**: AI-assisted development, sometimes called 'vibe coding,' involves using large language models to generate code from natural language descriptions, enabling non-programmers to build software. JavaScript is the core programming language of the web, essential for interactive features like animations and real-time updates. Virtual zen gardens and digital 'third places' are online spaces designed for relaxation and minimal social interaction, offering a calming escape.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vibe_coding">Vibe coding - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/JavaScript">JavaScript</a></li>

</ul>
</details>

**Discussion**: Commenters praised the concept and zen atmosphere but widely reported performance issues like lag and low frame rates. Suggestions included adding interactivity (e.g., clicking lily pads, feeding fish) and fading in other users' koi to reduce distraction. Some questioned the authenticity of the shared pond experience, noting they only saw a few koi.

**Tags**: `#Show HN`, `#virtual environment`, `#relaxation`, `#AI-assisted development`, `#web performance`

---

<a id="item-9"></a>
## [NeurIPS Accepted Papers Visible Before Official Notifications](https://www.reddit.com/r/MachineLearning/comments/1wp6oi3/neurips_accepted_papers_are_now_visible_r/) ⭐️ 6.0/10

NeurIPS accepted papers became visible on the conference site before official notification emails were sent, with one Reddit user reporting their paper marked as accepted despite scores of 5-4-4. Another user shared statistics showing 30,709 valid main track submissions, 7,900 accepted papers, 112 orals, and 292 spotlights. This early visibility gives ML researchers informal access to acceptance decisions ahead of official announcements, sparking immediate community discussion about scores, acceptance thresholds, and the overall competitiveness of this year's cycle. The reported acceptance rate of roughly 25.7% continues NeurIPS's trend of being one of the most selective and prestigious venues in machine learning. The reported scores of 5-4-4 suggest that borderline papers can still be accepted depending on reviewer discussion and area chair decisions, and the 7,900 accepted papers out of 30,709 submissions imply an acceptance rate of approximately 25.7%. The 112 oral and 292 spotlight slots represent a very small fraction of accepted papers, making these distinctions highly competitive.

reddit · r/MachineLearning · /u/levydawg · Sep 24, 16:41

**Background**: NeurIPS (Conference on Neural Information Processing Systems) is a flagship annual machine learning conference held each December, and its peer review process typically involves multiple reviewers assigning numeric scores to each submission. Papers are then categorized as poster, spotlight, or oral presentations based on reviewer scores and committee deliberation, with authors usually notified by email before results appear publicly. The conference has grown dramatically in recent years, with submission numbers exceeding 20,000 and acceptance rates hovering around 20-26%.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Conference_on_Neural_Information_Processing_Systems">Conference on Neural Information Processing Systems - Wikipedia</a></li>
<li><a href="https://github.com/lixin4ever/Conference-Acceptance-Rate">GitHub - lixin4ever/Conference-Acceptance-Rate: Acceptance rates for the major AI conferences · GitHub</a></li>
<li><a href="https://aip.riken.jp/news/neurips2025/">46 papers were accepted at NeurIPS 2025 | Center for Advanced Intelligence Project</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion centers on users sharing their acceptance experiences and scores, with surprise that a 5-4-4 paper was accepted, and others chiming in with aggregate submission and acceptance statistics. The overall sentiment is a mix of excitement for accepted authors and anxiety for those still awaiting decisions.

**Tags**: `#NeurIPS`, `#machine-learning`, `#academic-conference`, `#research-community`, `#peer-review`

---

<a id="item-10"></a>
## [Datasette 1.0a41 adds OpenTelemetry and Web Component modals](https://simonwillison.net/2026/Sep/24/datasette/) ⭐️ 5.0/10

Datasette 1.0a41 was released with OpenTelemetry support contributed by Alec Garcia, and all of Datasette's modal dialogs were refactored into a single reusable Web Component that is now documented for other plugins to use. Adding OpenTelemetry gives Datasette operators a vendor-neutral way to trace and observe queries and requests, which matters for running the tool in production, while exposing the modal Web Component lowers the barrier for plugin authors to build consistent UI. The telemetry support is documented in Datasette's internals section, and the modal Web Component is documented in the JavaScript plugins section, though this remains an alpha release (1.0a41) rather than a stable 1.0.

rss · Simon Willison · Sep 24, 19:15

**Background**: Datasette is an open-source tool by Simon Willison for exploring and publishing data, often used to browse SQLite databases through a web interface. OpenTelemetry is a CNCF observability framework providing vendor-neutral APIs and libraries for collecting traces and metrics. Web Components are a set of browser standards, including custom elements and shadow DOM, that let developers define reusable encapsulated HTML elements.

<details><summary>References</summary>
<ul>
<li><a href="https://opentelemetry.io/">OpenTelemetry</a></li>
<li><a href="https://en.wikipedia.org/wiki/Web_Components">Web Components</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Web_components">Web Components - Web APIs - MDN Web Docs - Mozilla</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#opentelemetry`, `#web-components`, `#release`, `#javascript`

---

<a id="item-11"></a>
## [Fifth-Year PhD Student Seeks Non-Elitist Publication Venues for Efficient Generative AI Research](https://www.reddit.com/r/MachineLearning/comments/1wp8ung/publication_venue_recommendations_r/) ⭐️ 4.0/10

A fifth-year PhD student with no publications posted on r/MachineLearning asking for recommendations of non-elitist journals or conferences where they can publish research on efficient Generative AI to fulfill graduation requirements, after repeated rejections from top-tier AI conferences despite good review scores. This request highlights a growing tension in machine learning academia, where acceptance rates at flagship venues like NeurIPS remain extremely low, leaving many capable students struggling to meet graduation requirements and prompting discussion about the role of alternative, less selective venues. The student explicitly asked not to be recommended 'elitist club conferences like NeurIPS,' and clarified that their research focuses on efficient Generative AI; they noted that journal or conference venue does not matter at this point, only completing the degree.

reddit · r/MachineLearning · /u/academic-targaryen · Sep 24, 18:02

**Background**: NeurIPS (Conference on Neural Information Processing Systems) is one of the most prestigious annual AI conferences, first proposed in 1986, and its high selectivity means many strong submissions are rejected. Efficient Generative AI research focuses on reducing the computational cost of training and running generative models such as image, text, and audio generators. PhD programs in machine learning typically require a certain number of peer-reviewed publications before graduation, which creates pressure when top venues reject papers with otherwise positive reviews.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Conference_on_Neural_Information_Processing_Systems">Conference on Neural Information Processing Systems - Wikipedia</a></li>
<li><a href="https://neurips.cc/">2026 Conference</a></li>

</ul>
</details>

**Tags**: `#academic publishing`, `#machine learning`, `#generative AI`, `#career advice`, `#reddit`

---

<a id="item-12"></a>
## [New Data Science Grad Seeks AI Residency and Pre-Doc Programs](https://www.reddit.com/r/MachineLearning/comments/1wp5apl/residency_predoc_programs_or_lesserknown/) ⭐️ 4.0/10

A recent data science bachelor's graduate posted on r/MachineLearning asking for advice on finding AI residency, pre-doc, and lesser-known fellowship programs to gain research experience. The poster noted that many big-company AI residency websites appear outdated and wondered whether those programs are effectively defunct. This reflects a broader uncertainty among new graduates about which research-training pipelines in AI are still active, especially as corporate residency programs quietly wind down while independent fellowships like MATS and Anthropic's safety program expand. Clearer information on these paths matters for early-career talent trying to break into AI research without a PhD. The poster specifically cites Ai2's pre-doc positions as a model, mentions competitive fellowships such as Anthropic's Safety Program and MATS, and asks whether lesser-known fellowships exist. MATS is a fully funded 12-week fellowship in Berkeley or London offering roughly $6.4k/month plus compute credits, while Ai2 offers a postdoctoral Young Investigators Program.

reddit · r/MachineLearning · /u/Jaded-Air-7216 · Sep 24, 15:49

**Background**: AI residency programs are typically short-term, paid positions that let people without a PhD work alongside researchers to build ML research experience, while pre-doc programs are one- to two-year research assistantships often used as a stepping stone to PhD applications. Fellowships like MATS focus specifically on AI alignment, interpretability, and security, and predoc.org maintains a listing of pre-doctoral opportunities across institutions.

<details><summary>References</summary>
<ul>
<li><a href="https://www.matsprogram.org/">MATS Research</a></li>
<li><a href="https://www.predoc.org/opportunities">Search a comprehensive listing of pre -doctoral opportunities</a></li>
<li><a href="https://allenai.org/careers">Careers | Ai 2</a></li>

</ul>
</details>

**Tags**: `#career-advice`, `#machine-learning`, `#residency-programs`, `#pre-doc`, `#fellowships`

---

<a id="item-13"></a>
## [commit-rewriter 0.2 Adds Non-Default Branch Support](https://simonwillison.net/2026/Sep/24/commit-rewriter/) ⭐️ 3.0/10

Simon Willison released commit-rewriter 0.2, which adds support for rewriting commits on branches other than the default branch. Users can now target another branch by running `uvx commit-rewriter --branch other`, addressing GitHub issue #3. This update removes a significant limitation for developers who work with feature branches, release branches, or other non-default branches, making the tool usable in more real-world Git workflows. It reflects the ongoing trend of small, focused CLI utilities that automate tedious version-control chores. The new behavior is opt-in via the `--branch` flag, and the tool is distributed as a Python package runnable through `uvx`, so no permanent installation is required. The release is a minor 0.2 version bump, indicating the core functionality remains otherwise unchanged.

rss · Simon Willison · Sep 24, 20:06

**Background**: Git stores commits as an immutable chain, so editing an older commit requires rewriting that commit and every commit after it, typically done with tools like `git rebase` or `git commit --amend`. commit-rewriter is a utility by Simon Willison that automates this kind of history rewriting, and `uvx` is the command from the uv Python package manager for running a tool in an ephemeral environment without installing it globally.

<details><summary>References</summary>
<ul>
<li><a href="https://git-scm.com/book/en/v2/Git-Tools-Rewriting-History">7.6 Git Tools - Rewriting History</a></li>
<li><a href="https://www.reddit.com/r/Python/comments/1guf2fh/if_you_use_uv_what_are_your_use_cases_for_uvx/">If you use uv, what are your use cases for uvx? : r/Python - Reddit</a></li>

</ul>
</details>

**Tags**: `#git`, `#tooling`, `#release`, `#version-control`, `#simon-willison`

---

<a id="item-14"></a>
## [NeurIPS Author Questions Missing Final Justification on Rejected Paper](https://www.reddit.com/r/MachineLearning/comments/1wpa4gp/neurips_reject_final_justification_r/) ⭐️ 3.0/10

A Reddit user reported that their NeurIPS submission was rejected with three ratings of 4, yet the meta-review they received was identical to the one posted in July and contained no final justification comment from the program chairs. They noted the rejection email emphasized that ACs and SACs had been asked to provide careful feedback, especially in borderline cases, but no such feedback appeared. This highlights a recurring transparency concern in large machine learning conferences, where authors in borderline cases expect substantive meta-reviews but sometimes receive only recycled or minimal feedback. Such experiences can erode trust in the peer-review process and discourage participation, even though they do not reflect a technical breakthrough. The paper received ratings of 4-4-4, which typically places it in a borderline range where additional AC/SAC discussion is most valuable. The user specifically points out that the meta-review text was unchanged from July, suggesting no post-discussion update was made.

reddit · r/MachineLearning · /u/Lonely_Ostrich6165 · Sep 24, 18:49

**Background**: NeurIPS is one of the largest and most competitive machine learning conferences, using a multi-stage review process involving reviewers, area chairs (ACs), and senior area chairs (SACs). After initial reviews and author rebuttals, ACs write meta-reviews that summarize the discussion and justify acceptance or rejection. In borderline cases, program chairs often ask ACs and SACs to provide additional final justification comments to explain the decision more thoroughly.

<details><summary>References</summary>
<ul>
<li><a href="https://neurips.cc/Conferences/2024/AC-Guidelines">2024 Area Chair (AC) Guidelines</a></li>
<li><a href="https://neurips.cc/Conferences/2025/AC-Guidelines">2025 Area Chair (AC) Guidelines</a></li>
<li><a href="https://papers.neurips.cc/paper_files/paper/2020/file/176bf6219855a6eb1f3a30903e34b6fb-MetaReview.html">Review for NeurIPS paper: Pointer Graph Networks</a></li>

</ul>
</details>

**Tags**: `#NeurIPS`, `#peer review`, `#academic publishing`, `#machine learning`, `#conference`

---

<a id="item-15"></a>
## [NeurIPS Author Registration Confusion as Sydney and Paris Venues Sell Out](https://www.reddit.com/r/MachineLearning/comments/1wpg672/registration_for_authors_of_accepted_papers_at/) ⭐️ 3.0/10

A Reddit user reported that when trying to register for NeurIPS on the official website, the Sydney and Paris venues were already sold out, despite having previously filled out location preference forms. They asked what the correct registration and venue selection procedure is for authors of accepted papers, noting it is much more confusing than last time. NeurIPS is one of the largest and most prestigious machine learning conferences, and at least one author of every accepted paper must register for the main conference. Confusion or capacity limits in the multi-site registration process can directly affect whether accepted papers are presented and whether authors can attend. According to NeurIPS's own blog and FAQ, if a site reaches capacity, top-choice locations cannot be guaranteed, and the designated presenting author receives guaranteed registration tied exclusively to their allocated poster site. A 'Virtual Only Pass' is not sufficient to satisfy the author registration requirement, though student authors only need a student registration.

reddit · r/MachineLearning · /u/general_landur · Sep 24, 22:53

**Background**: NeurIPS (Conference on Neural Information Processing Systems) is an annual machine learning and computational neuroscience conference held each December. For its 2026 edition, the conference is being held across three sites—Sydney, Atlanta, and Paris—which introduces a more complex multi-site registration and venue allocation process than previous single-location editions.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.neurips.cc/2026/08/27/navigating-neurips-2026-a-breakdown-of-the-multi-site-registration-process/">Navigating NeurIPS 2026: A Breakdown of the Multi-Site Registration Process – NeurIPS Blog</a></li>
<li><a href="https://neurips.cc/FAQ/AuthorRegistration">Author Registration</a></li>
<li><a href="https://en.wikipedia.org/wiki/Conference_on_Neural_Information_Processing_Systems">Conference on Neural Information Processing Systems - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#NeurIPS`, `#conference`, `#registration`, `#logistics`, `#machine learning`

---

<a id="item-16"></a>
## [Reddit user asks: Sydney or Atlanta for NeurIPS 2026?](https://www.reddit.com/r/MachineLearning/comments/1wpgsp0/sydney_or_atlanta_for_neurips_2026d/) ⭐️ 3.0/10

A Reddit user who had their first authored paper accepted at NeurIPS 2026 asked the r/MachineLearning community whether they should attend the Sydney or Atlanta location, and which site most other attendees are choosing. The post is a personal logistics question rather than a technical or research contribution. NeurIPS 2026 is being held across three sites — Sydney, Atlanta, and Paris — which is a notable change from the conference's traditional single-location format, so attendees must now decide which site offers the best experience. This matters to the thousands of authors, reviewers, and students planning their December travel and budgets. According to official NeurIPS information, the 2026 conference runs December 6–12, with Sydney, Atlanta, and Paris as the three host locations, and the organization has published a breakdown of the multi-site registration process. The Reddit post itself contains no technical content and received a low community score, so responses are likely to be anecdotal travel advice.

reddit · r/MachineLearning · /u/RedTea1997 · Sep 24, 23:21

**Background**: NeurIPS (Conference on Neural Information Processing Systems) is one of the largest and most prestigious annual machine learning conferences, traditionally held in December and historically hosted in a single city. For 2026, the organizers have expanded to a multi-site format spanning Sydney, Atlanta, and Paris, which raises new questions about registration, presentation logistics, and which location most attendees will choose. Having a first-authored paper accepted at NeurIPS is a significant career milestone for many researchers, making the choice of which site to attend a meaningful decision.

<details><summary>References</summary>
<ul>
<li><a href="https://neurips.cc/">2026 Conference</a></li>
<li><a href="https://en.wikipedia.org/wiki/Conference_on_Neural_Information_Processing_Systems">Conference on Neural Information Processing Systems - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#NeurIPS`, `#conference`, `#academic travel`, `#community discussion`, `#machine learning`

---

<a id="item-17"></a>
## [EACL Author Asks Whether to Contact AC Over Silent Reviewers](https://www.reddit.com/r/MachineLearning/comments/1woox4w/eacl_reviewers_no_response_d/) ⭐️ 3.0/10

A Reddit user on r/MachineLearning reports that during the ongoing EACL rebuttal period, none of their reviewers have responded to their author responses, and one reviewer gave a score of 2 with confidence 5 based on a limitation the author had explicitly disclosed in the paper. The author asks whether they should send a confidential message to the area chair (AC) if nothing changes within two days. This reflects a recurring tension in NLP and ML conference peer review: reviewers are not obligated to respond during rebuttals, yet authors have limited recourse when a review appears to violate the conference's own rules. How ACs handle such cases affects author trust in the review process and the fairness of acceptance decisions at major venues like EACL. The author notes the rebuttal is still ongoing, so scores could still change, and that the other two reviews scored 3 and 4, which the author considers acceptable. The core complaint is that a stated limitation was treated as a weakness, which the author claims the conference's own rules prohibit.

reddit · r/MachineLearning · /u/No_Sky9786 · Sep 24, 01:55

**Background**: EACL is the European Chapter of the Association for Computational Linguistics conference, with EACL 2026 scheduled for Rabat, Morocco, in March 2026. In ACL-family conferences, the rebuttal period lets authors respond to reviews before final decisions, and area chairs oversee reviewers and help resolve disagreements. Reviewers are generally not required to reply to rebuttals, and authors can sometimes send confidential notes to ACs when they believe a review is flawed or rule-violating.

<details><summary>References</summary>
<ul>
<li><a href="https://2026.eacl.org/">The 19th Conference of the European Chapter of the Association for Computational LinguisticsRabat, MoroccoMarch 24-29, 2026 -</a></li>
<li><a href="https://qipeng.me/blog/what-does-an-area-chair-do/">What does an area chair actually do, anyway? | Peng Qi</a></li>
<li><a href="https://www.sigarch.org/should-conferences-have-a-rebuttal-phase/">Should conferences have a rebuttal phase? - SIGARCH</a></li>

</ul>
</details>

**Tags**: `#academic-conferences`, `#peer-review`, `#EACL`, `#NLP`, `#community-discussion`

---