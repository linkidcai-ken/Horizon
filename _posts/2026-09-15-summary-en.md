---
layout: default
title: "Horizon Summary: 2026-09-15 (EN)"
date: 2026-09-15
lang: en
---

> From 21 items, 19 important content pieces were selected

---

1. [TypeSafe AI launches System One Models and Jev for fast typed inference](#item-1) ⭐️ 8.0/10
2. [E-ink frame listens for birds and draws them as 1800s illustrations](#item-2) ⭐️ 8.0/10
3. [Internet Archive Adds Protections as Wayback Machine Battles Scraping Surge](#item-3) ⭐️ 8.0/10
4. [Google launches Gemini 3.8 Live and Live Extended Thinking](#item-4) ⭐️ 8.0/10
5. [Ex-Apple Engineer Builds M4 Mac Mini Linux GPU Driver in One Month Using LLMs](#item-5) ⭐️ 8.0/10
6. [AI agent finds Baseten admin GitHub token in Docker build history](#item-6) ⭐️ 8.0/10
7. [Prior Labs releases TabPFN-3.5, new SOTA tabular foundation model](#item-7) ⭐️ 8.0/10
8. [Rheinmetall publishes Battlesuite weapon protocol docs, not open source](#item-8) ⭐️ 7.0/10
9. [Capsule packs web apps and their data into a single SQLite file](#item-9) ⭐️ 7.0/10
10. [Norwegian Consumer Council Article Sparks Debate on Declining Product Quality](#item-10) ⭐️ 7.0/10
11. [GEFS Copy-on-Write Filesystem Ported to OpenBSD in Early Preview](#item-11) ⭐️ 7.0/10
12. [Suspected Sabotage Disrupts Netherlands Rail Network](#item-12) ⭐️ 7.0/10
13. [SHADOW-50M: 44M ternary LLM runs at 1,900 tok/s on CPU](#item-13) ⭐️ 7.0/10
14. [Researcher asks how to obtain preprocessed datasets when paper authors don't respond](#item-14) ⭐️ 6.0/10
15. [Author Cuts Apart Oversized Books to Make Them Readable](#item-15) ⭐️ 5.0/10
16. [NeurIPS 2026 Multi-Venue Logistics Spark Fairness Concerns](#item-16) ⭐️ 5.0/10
17. [uv 0.12.15 fixes pip install regression and speeds cold-cache resolution](#item-17) ⭐️ 4.0/10
18. [uv 0.12.14 Improves Error Diagnostics and Adds Download Resumption](#item-18) ⭐️ 4.0/10
19. [Reddit User Asks If Partial Algorithm Qualifies for ML Workshop](#item-19) ⭐️ 3.0/10

---

<a id="item-1"></a>
## [TypeSafe AI launches System One Models and Jev for fast typed inference](https://typesafe.ai/blog/introducing-system-one-models-and-jev) ⭐️ 8.0/10

TypeSafe AI has released its first System One Model, Jev, a new class of frontier models designed to make fast, structured decisions that software can consume directly, rather than generating open-ended text. Jev takes a block of state and a set of typed questions, returning choices, scores, or probabilities that application code can use for classification, routing, approval, or escalation. This approach could significantly speed up and reduce the cost of AI-driven automation by replacing general-purpose generation with type-safe, structured outputs, potentially benefiting developers building classification, routing, and decision-making systems. It also challenges the dominance of large language models for tasks that don't require open-ended generation. Jev does not generate prose, code, or open-ended strings; it only produces typed answers and probabilities, which limits its applicability to tasks that require structured decisions. The model is available in early access, and TypeSafe AI claims orders-of-magnitude speed and efficiency gains over frontier LLMs for these narrow tasks.

hackernews · albelfio · Sep 15, 19:25 · [Discussion](https://news.ycombinator.com/item?id=49717558)

**Background**: System One models are a new class of AI models built to make fast, structured decisions that software can use directly, as opposed to traditional large language models that generate free-form text. Type inference, a concept from programming languages, automatically determines the type of an expression, and here it is applied to AI outputs to ensure they are type-safe and directly consumable by code. TypeSafe AI emerged from stealth after two years to launch this model, aiming to automate tasks like classification and routing without the overhead of generative models.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.typesafe.ai/concepts/system-one">System One - TypeSafe AI</a></li>
<li><a href="https://typesafe.ai/blog/introducing-system-one-models-and-jev">Introducing System One Models and Jev - TypeSafe AI Blog</a></li>
<li><a href="https://runtimewire.com/article/typesafe-jev-system-one-ai-model-early-access">TypeSafe opens Jev early access for fast, typed AI decisions</a></li>

</ul>
</details>

**Discussion**: Community comments highlight the novelty of the approach but question the speed comparison to generative models, noting that Jev only produces structured output and may be best suited for classification tasks. Some see potential in combining it with design-by-contract patterns, while others point out that encoder models already provided fast probabilistic outputs without hallucinations, so the key innovation may lie in the typed interface and integration.

**Tags**: `#AI`, `#machine-learning`, `#type-systems`, `#inference`, `#LLM`

---

<a id="item-2"></a>
## [E-ink frame listens for birds and draws them as 1800s illustrations](https://github.com/arnegiacomo/fugleramme) ⭐️ 8.0/10

Developer Arne Munthe-Kaas released 'fugleramme' on GitHub, an e-ink frame that continuously listens for bird calls, identifies species using the BirdNET classifier, and renders each detected bird as a 19th-century-style illustration on the display. The project shows how embedded hardware, bioacoustic machine learning, and generative art can be combined into a small, delightful ambient device, and it has inspired a wave of similar DIY bird-listening projects in the maker community. BirdNET is a traditional neural network trained to recognize over 3,000 of the world's most common bird species from raw acoustic data, not an LLM, and the e-ink display only needs power when refreshing, which suits a low-power always-on listening device.

hackernews · arnemunthekaas · Sep 15, 12:31 · [Discussion](https://news.ycombinator.com/item?id=49711544)

**Background**: BirdNET is an open research project from the Cornell Lab of Ornithology and Chemnitz University of Technology that uses neural networks to identify birds by sound. E Ink is an electronic paper display technology that reflects light like paper and only consumes power when the image changes, making it ideal for battery-powered ambient displays. Generative art refers to artwork produced with the help of algorithms, here used to turn a detected species into a period-style illustration.

<details><summary>References</summary>
<ul>
<li><a href="https://birdnet.cornell.edu/">BirdNET – AI-Powered Sound ID</a></li>
<li><a href="https://en.wikipedia.org/wiki/E_Ink">E Ink - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters were enthusiastic, calling it one of the most inspiring HN projects in a while and praising its 'magical' quality; one noted that BirdNET is a traditional neural network rather than an LLM, another linked the related birdnet-go project, and others shared their own low-power e-ink builds.

**Tags**: `#e-ink`, `#bird-classification`, `#embedded`, `#generative-art`, `#hardware`

---

<a id="item-3"></a>
## [Internet Archive Adds Protections as Wayback Machine Battles Scraping Surge](https://blog.archive.org/2026/09/15/an-update-on-wayback-machine-access/) ⭐️ 8.0/10

The Internet Archive announced that the Wayback Machine has been hit by waves of high-volume automated traffic and that it has deployed new protections to keep the service running. The organization believes the traffic comes largely from scrapers trying to circumvent blocks on original sites by pulling content from archived copies instead. The Internet Archive is critical public infrastructure for digital preservation, and sustained scraping pressure degrades access for ordinary users while pushing some websites to opt out of archiving entirely. If this trend continues, it threatens the long-term sustainability of open, freely accessible web history. The protections appear to be rate-limiting measures, as some users report encountering HTTP 429 'Too Many Requests' errors from certain networks while other connections work normally. The Archive notes that some sites have already opted out in response to the scraping, and the traffic is widely attributed to AI-related data harvesting rather than human browsing.

hackernews · ChrisArchitect · Sep 15, 17:52 · [Discussion](https://news.ycombinator.com/item?id=49716176)

**Background**: The Wayback Machine is a free service run by the nonprofit Internet Archive that has preserved snapshots of web pages since 1996, now totaling over a trillion captures. Web scraping means using automated scripts to extract data from websites at scale, and when original sites block such bots, scrapers often redirect their efforts to archived copies. Digital preservation services like the Internet Archive depend on donations and limited infrastructure, making them vulnerable to sudden surges in automated traffic.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.archive.org/2026/09/15/an-update-on-wayback-machine-access/">An Update on Wayback Machine Access | Internet Archive Blogs</a></li>
<li><a href="https://www.niemanlab.org/2026/01/news-publishers-limit-internet-archive-access-due-to-ai-scraping-concerns/">News publishers limit Internet Archive access due to AI scraping concerns | Nieman Journalism Lab</a></li>
<li><a href="https://www.nnlm.gov/guides/data-glossary/web-scraping">Web Scraping | NNLM</a></li>

</ul>
</details>

**Discussion**: Commenters expressed strong support for the Internet Archive, with one calling its staff 'the heroes we need' for maintaining open access even via Tor without centralized gatekeepers. Others shared practical experiences, such as persistent 429 errors from a work network but not from a phone, and one user recounted recovering forgotten personal history from an early-2000s gaming review site preserved by the Archive. The overall sentiment was sympathetic, framing the situation as collateral damage from the AI arms race against free resources.

**Tags**: `#internet-archive`, `#web-scraping`, `#digital-preservation`, `#infrastructure`, `#open-access`

---

<a id="item-4"></a>
## [Google launches Gemini 3.8 Live and Live Extended Thinking](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-8-live-gemini-3-8-live-extended-thinking/) ⭐️ 8.0/10

Google announced Gemini 3.8 Live and Gemini 3.8 Live Extended Thinking, described as its most advanced live dialogue models yet, with major upgrades in intelligence and parallel reasoning for voice-driven collaboration and complex task execution. The release follows the earlier 3.1 Flash Live model and is accompanied by a dedicated model card for Gemini 3.8 Audio. This release strengthens Google's position in the fast-growing market for low-latency, real-time voice AI, where developers are building voice agents and conversational applications on top of the Gemini Live API. The addition of an Extended Thinking variant signals that Google is targeting both quick voice commands and multi-step reasoning workflows, potentially broadening enterprise adoption. The Live API remains in Preview, and Google positions Gemini 3.8 Live as the default model for low-latency voice agent experiences without reasoning delays, while the Extended Thinking variant is aimed at multi-step problem solving, complex planning, and multi-tool workflows. The models are described as cost-efficient and fast, optimized for high-volume, latency-sensitive tasks.

hackernews · leumon · Sep 15, 17:38 · [Discussion](https://news.ycombinator.com/item?id=49715947)

**Background**: The Gemini Live API enables real-time, bidirectional voice conversations with Gemini models, combining simultaneous speech-to-text input and text-to-speech output for natural, low-latency interaction. Google has been iterating on its Gemini 3 series of natively multimodal reasoning models, with the Live variants specifically tuned for real-time dialogue rather than batch or text-only use cases.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-8-live-gemini-3-8-live-extended-thinking/">Gemini 3.8 Live & Gemini 3.8 Live Extended Thinking - The Keyword</a></li>
<li><a href="https://ai.google.dev/gemini-api/docs/live-api">Gemini Live API overview | Gemini API | Google AI for Developers</a></li>
<li><a href="https://ai.google.dev/gemini-api/docs/live-api/thinking">Thinking in the Live API | Gemini API | Google AI for Developers</a></li>

</ul>
</details>

**Discussion**: Community reaction is largely positive, with users praising low latency, pleasant voices, and robust handling of thick accents, as well as the ability to use it on a workspace account. One user highlighted Gemini's strong support for niche languages like Afrikaans for live conversation and grammar practice, while another questioned when Google would overtake competitors like Fable and Astra despite its data, TPU, and advertising advantages.

**Tags**: `#Gemini`, `#Google`, `#LLM`, `#AI`, `#Live API`

---

<a id="item-5"></a>
## [Ex-Apple Engineer Builds M4 Mac Mini Linux GPU Driver in One Month Using LLMs](https://codyho.dev/blog/gpu-driver/) ⭐️ 8.0/10

An ex-Apple engineer named Cody Ho used large language models to reverse engineer and build a working Linux GPU driver for the M4 Mac Mini in about one month, achieving enough performance to run Minecraft at over 200fps. The driver targets Apple's AGX GPU firmware ABI and user-space components, but the author was subsequently banned from the Asahi Linux project for concealing his extensive LLM use and his former Apple employment. This demonstrates that LLM-assisted reverse engineering can dramatically accelerate the creation of open-source GPU drivers for undocumented Apple Silicon hardware, potentially expanding Linux usability on modern M-series Macs. However, the ethical and legal controversies—conflict of interest from the author's Apple background and Asahi Linux's strict no-AI policy—raise serious questions about whether such code can ever be upstreamed into the mainline Linux kernel. The driver required reverse engineering the AGX GPU's complex firmware ABI and user-space components, and it reportedly runs Minecraft at 212fps on the M4 Mac Mini. The author was banned from Asahi Linux not only for hiding LLM usage but also for concealing his former Apple engineer status and direct contacts with people involved in Apple Silicon development, creating a major conflict of interest.

hackernews · ADevWithAnIdea · Sep 15, 19:30 · [Discussion](https://news.ycombinator.com/item?id=49717638)

**Background**: Apple Silicon Macs use a custom GPU architecture called AGX, which lacks public documentation, making Linux GPU driver development extremely difficult. The Asahi Linux project has been reverse engineering these GPUs for years, but progress has stalled on M3 and newer chips, and the project maintains a strict no-AI policy for contributions. LLMs are increasingly used to assist with reverse engineering and code generation, but the provenance and legal status of AI-generated code remain unsettled, especially given ongoing litigation such as Apple's lawsuit against OpenAI over alleged stolen trade secrets.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Apple_M4">Apple M4 - Wikipedia</a></li>
<li><a href="https://codyho.dev/blog/gpu-driver/">I Came, I Prompted, I Left Part 2: Building a GPU Driver ... — Cody Ho</a></li>
<li><a href="https://www.phoronix.com/news/Asahi-Lina-Steps-Down-Linux-GPU">Asahi Lina Pausing Work On Apple GPU Linux Driver Development</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed: many are impressed by the speed and see LLM-assisted reverse engineering as a breakthrough for undocumented hardware, while others argue the work is ethically and legally tainted due to the author's concealed Apple background and Asahi Linux's no-AI policy. Some commenters expect AI-assisted forks to dominate for practical users, while purists may stick to non-AI versions, and several urge the developer to share code and documentation regardless of upstreaming prospects.

**Tags**: `#Linux`, `#GPU driver`, `#Apple Silicon`, `#LLM`, `#reverse engineering`

---

<a id="item-6"></a>
## [AI agent finds Baseten admin GitHub token in Docker build history](https://www.strix.ai/blog/baseten-harbor-github-pat-takeover) ⭐️ 8.0/10

Security firm Strix used an AI agent to discover a live admin GitHub personal access token for Baseten's 'basetenbot' account inside a public Docker image's build history, gaining access to production repositories within 25 minutes. The token had admin and push access to Baseten's main product repo, GitOps repo, Homebrew tap, and read/write access to private customer repositories. This incident highlights how AI agents can automate the discovery of exposed secrets in public artifacts, turning a common misconfiguration into a rapid, high-impact breach. It raises urgent questions about the security of CI/CD pipelines and the ethics of automated penetration testing without explicit authorization. The token was found in Docker build history after Strix pulled a Baseten image repository, and it granted access to critical infrastructure including per-customer repositories. Baseten rotated the token and made the Harbor project private after Strix reported the issue, but the incident underscores the risks of embedding secrets in image layers.

hackernews · bearsyankees · Sep 15, 18:11 · [Discussion](https://news.ycombinator.com/item?id=49716476)

**Background**: Baseten is a platform for deploying and serving machine learning models, managing containers, GPU capacity, and scaling. GitHub personal access tokens (PATs) are credentials used to authenticate to GitHub APIs and can have broad permissions if not scoped or expired. Docker build history can inadvertently retain secrets if they are passed as build arguments or copied into image layers, making them accessible to anyone who pulls the image.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.docker.com/build/building/secrets/">Build secrets | Docker Docs</a></li>
<li><a href="https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens">Managing your personal access tokens - GitHub Docs</a></li>
<li><a href="https://www.baseten.co/">Inference Platform: Deploy AI models in production | Baseten</a></li>

</ul>
</details>

**Discussion**: Commenters debated the legality and ethics of Strix's automated penetration testing without authorization, with some calling it great marketing for Strix but bad for Baseten. Others criticized Strix for naming the victim and questioned whether such actions cross legal boundaries, while acknowledging Baseten's swift response in rotating the token and making the repository private.

**Tags**: `#security`, `#ai-agents`, `#github`, `#penetration-testing`, `#devops`

---

<a id="item-7"></a>
## [Prior Labs releases TabPFN-3.5, new SOTA tabular foundation model](https://www.reddit.com/r/MachineLearning/comments/1wh4xhy/tabpfn35_is_released_as_the_next_sota_tabular/) ⭐️ 8.0/10

Prior Labs released TabPFN-3.5 today, a new tabular foundation model that tops both the TabArena and BeyondArena benchmarks and is SOTA for datasets with up to 1M rows and 20k features. It ships in three variants: TabPFN-3.5-Fast (in alpha, 6x faster than the base model), TabPFN-3.5-Thinking (trades compute for accuracy via API), and TabPFN-3.5-Plus. This release strengthens the case for foundation models in tabular machine learning, a domain long dominated by gradient-boosted trees like XGBoost and LightGBM. The large Elo gains on BeyondArena, especially on text-rich, high-cardinality, and high-dimensional data, suggest these models are becoming viable for messy real-world tables rather than just clean benchmarks. On BeyondArena, TabPFN-3.5 leads on text-rich, high-cardinality, and high-dimensional data with +250 Elo over the strongest previous baseline and +150 Elo ahead of the previous overall leader. TabPFN-3.5-Thinking adds +20 Elo over the base model on BeyondArena and +44 Elo on TabArena, while the Fast variant is still in alpha.

reddit · r/MachineLearning · /u/tuanacelik · Sep 15, 16:18

**Background**: TabPFN is a transformer-based foundation model from Prior Labs that uses in-context learning to solve tabular prediction problems in a single forward pass, rather than requiring per-dataset training. TabArena is a continuously maintained living benchmark for tabular ML that integrates new datasets and models to keep comparisons fair and reproducible, while BeyondArena is a unified benchmark covering diverse task types (IID, temporal, grouped) and feature types such as text and high-cardinality columns. Together they represent an effort to evaluate tabular foundation models on conditions that standard benchmarks often skip.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/PriorLabs/TabPFN">GitHub - PriorLabs/ TabPFN : TabPFN : Foundation Model for Tabular ...</a></li>
<li><a href="https://arxiv.org/abs/2506.16791">TabArena : A Living Benchmark for Machine Learning on Tabular Data</a></li>
<li><a href="https://www.alphaxiv.org/abs/2606.30410">Beyond IID: How General Are Tabular Foundation Models... | alphaXiv</a></li>

</ul>
</details>

**Tags**: `#tabular-data`, `#foundation-models`, `#machine-learning`, `#benchmarking`, `#SOTA`

---

<a id="item-8"></a>
## [Rheinmetall publishes Battlesuite weapon protocol docs, not open source](https://rheinmetall.github.io/onboardapi-documentation/9.10.0/index.html) ⭐️ 7.0/10

German defense contractor Rheinmetall published documentation for its Battlesuite connected weapon system protocol at rheinmetall.github.io/onboardapi-documentation/9.10.0. The release was widely described as open-sourcing, but the company's GitHub organization contains no corresponding source code. A major defense contractor publicly documenting a weapon-system interface protocol is unusual and could influence how third parties integrate with Battlesuite, but the lack of actual source code limits real interoperability and raises questions about what 'open' means in defense procurement. The protocol is built on DDS (Data Distribution Service), the OMG middleware standard, which commenters note is heavyweight for embedded systems that avoid dynamic memory allocation; the documentation is versioned 9.10.0 and hosted on GitHub Pages rather than released under an open-source license.

hackernews · summarity · Sep 15, 21:07 · [Discussion](https://news.ycombinator.com/item?id=49718928)

**Background**: Rheinmetall unveiled Battlesuite in May 2025 as a digital platform to link conventional weapons, drones, and battlefield data. DDS is a data-centric publish-subscribe middleware standard from the Object Management Group used in defense, aerospace, and IoT for low-latency, reliable data connectivity. Open source normally means publishing source code that others can use, study, modify, and redistribute, which is distinct from merely publishing documentation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.airforce-technology.com/news/rheinmetall-battlesuite-networked/">Rheinmetall unveils Battlesuite platform for networked combat</a></li>
<li><a href="https://www.dds-foundation.org/what-is-dds-3/">What is DDS ?</a></li>

</ul>
</details>

**Discussion**: Commenters on Hacker News were skeptical: throw1234567891 noted Rheinmetall's GitHub has no source code, calling it 'really weird,' while j-pb said excitement faded upon seeing DDS. Others compared it to ROS2 for missiles, and alhirzel wished for a DDS-like protocol with real-time guarantees and no dynamic memory allocation, citing MIL-STD-3071 as a similar DDS-based effort.

**Tags**: `#defense`, `#protocols`, `#DDS`, `#open-source`, `#embedded-systems`

---

<a id="item-9"></a>
## [Capsule packs web apps and their data into a single SQLite file](https://withcapsule.app/) ⭐️ 7.0/10

A developer released Capsule, a Rust/Tauri 2.0 tool that embeds an HTML app, its assets, and its user data into one SQLite file with a .capsule extension. Data can be stored as a localStorage-style key/value store or through a MongoDB-inspired collections API, and everything can be exported to CSV or JSON. It targets a real pain point for local-first tools: building an HTML page is easy, but persisting and sharing its data usually requires hosting. By making the app and its data a single portable file, Capsule offers a lightweight distribution model for small AI-generated tools, though its usefulness for multi-user or frequently updated apps remains debated. Documents are sandboxed by default with no direct file system access and require permission to reach the internet, and they can optionally use local or remote AI models. Because copies diverge when shared, each data entry carries a UUID and timestamp to support merging, and the author plans to open the file format spec at version 1.0.

hackernews · bashtian · Sep 15, 13:31 · [Discussion](https://news.ycombinator.com/item?id=49712278)

**Background**: Tauri is a Rust-based framework for building lightweight desktop and mobile apps with a web frontend, positioned as a smaller alternative to Electron. SQLite is a widely used embedded database that stores an entire database in a single cross-platform file, which makes it well suited to bundling data alongside an app. Capsule combines these ideas to serve the local-first software movement, where apps keep data on the user's device rather than in the cloud.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Tauri_(software_framework)">Tauri (software framework) - Wikipedia</a></li>
<li><a href="https://sqlite.org/onefile.html">SQLite: Single File Database</a></li>
<li><a href="https://localfirstweb.dev/">Local-First Software</a></li>

</ul>
</details>

**Discussion**: Commenters broadly liked the idea but raised practical concerns: one asked for device syncing, separation of app and data, and app updates; another noted the File System Access API already lets web pages read and write local files; and skeptics argued the model is hard to generalize, since sharing state changes means re-sending files and hosting may be simpler.

**Tags**: `#local-first`, `#sqlite`, `#tauri`, `#web-apps`, `#data-storage`

---

<a id="item-10"></a>
## [Norwegian Consumer Council Article Sparks Debate on Declining Product Quality](https://www.forbrukerradet.no/short-life/) ⭐️ 7.0/10

The Norwegian Consumer Council (Forbrukerrådet) published an article titled 'Let's make quality the norm again' examining the causes and consequences of declining product quality, which sparked a 294-comment discussion on Hacker News. Commenters debated economic incentives, consumer behavior, and regulatory impacts behind the trend. The discussion highlights a growing frustration among consumers and technologists that products are becoming less durable and reliable, with implications for sustainability, consumer trust, and market dynamics. It connects to broader concerns about inflation, globalization, and the difficulty of making informed purchasing decisions. Commenters pointed out that quality is hard to compare while prices are easy, leading to market failures; they also noted that premium 'quality brands' are incentivized to cut costs and cash in on their reputation, and that consumers shouldn't need expert knowledge to buy durable goods.

hackernews · ingve · Sep 15, 10:00 · [Discussion](https://news.ycombinator.com/item?id=49710109)

**Background**: The Norwegian Consumer Council is a government agency that advocates for consumer rights. The article argues that product quality has declined over time, and the Hacker News discussion explores why this happens, touching on economic concepts like inflation, price discovery, and regulatory costs.

**Discussion**: Commenters offered varied perspectives: some see declining quality as hidden inflation, others argue cheap goods have always outsold quality, and some blame economic incentives that push quality brands to cut corners. A common thread is that consumers are overburdened with the need to research purchases, and that price comparability versus quality opacity is a core problem.

**Tags**: `#consumerism`, `#quality`, `#economics`, `#regulation`, `#hackernews`

---

<a id="item-11"></a>
## [GEFS Copy-on-Write Filesystem Ported to OpenBSD in Early Preview](https://marc.info/?l=openbsd-tech&m=178948744271633&w=2) ⭐️ 7.0/10

An early preview of GEFS, a copy-on-write filesystem with block-level hashing originally built for Plan 9, has been ported to OpenBSD and posted to the openbsd-tech mailing list. The announcement sparked community discussion comparing it to HAMMER2 and sharing firsthand testing experiences. GEFS brings crash-safe snapshots and block-level corruption detection to OpenBSD, features that are rare among the filesystems typically available on BSD systems. If it matures, it could offer OpenBSD users a modern alternative to FFS with stronger data integrity guarantees. GEFS stores a hash of the data in each block pointer, so corruption from failing storage or filesystem bugs can be detected and reported rather than silently propagated. The project prioritizes being crash-safe, corruption-detecting, simple, and fast at snapshotting, in that order.

hackernews · sippingabonedry · Sep 15, 17:12 · [Discussion](https://news.ycombinator.com/item?id=49715590)

**Background**: GEFS (Good Enough File System) was created by Ori Bernstein for Plan 9 and its derivative 9front, where it has been used in production for some time. It is a copy-on-write filesystem, meaning it never overwrites existing blocks in place, which enables consistent snapshots. HAMMER2, developed by Matthew Dillon for DragonFly BSD, is a comparable filesystem with checksumming, snapshots, and deduplication that has long been discussed as a candidate for other BSDs.

<details><summary>References</summary>
<ul>
<li><a href="https://orib.dev/gefs.html">gefs</a></li>
<li><a href="https://fosdem.org/2026/schedule/event/F8QZJP-gefs_a_good_enough_file_system_for_plan_9/">FOSDEM 2026 - GEFS : A Good Enough File System</a></li>
<li><a href="https://en.wikipedia.org/wiki/HAMMER2">HAMMER2 - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters expressed strong interest in GEFS while also asking why HAMMER2 has not received more attention from other operating systems, with one linking a GitHub project to port HAMMER2 to OpenBSD. A EuroBSDCon talk on GEFS was shared, and one commenter noted they have been helping test GEFS on 9front, where the nightly builder has been running on it for quite a while, praising Ori Bernstein's work.

**Tags**: `#filesystems`, `#OpenBSD`, `#GEFS`, `#HAMMER2`, `#systems`

---

<a id="item-12"></a>
## [Suspected Sabotage Disrupts Netherlands Rail Network](https://www.bbc.com/news/articles/c8ly49w9g1edo) ⭐️ 7.0/10

A suspected act of sabotage caused major disruption across the Netherlands rail network, with the incident drawing 415 points and 384 comments on Hacker News. The timing coincided with Prinsjesdag, the annual Dutch budget day when the monarch delivers the Speech from the Throne, and protests were expected in several locations. The incident highlights how vulnerable large, distributed rail infrastructure is to deliberate disruption, and it feeds into a broader European pattern of suspected hybrid attacks on transport and critical infrastructure. It also raises difficult questions about whether fail-safe design, which deliberately stops trains on fault, can be abused at scale by attackers. Rail systems are engineered to fail safe, meaning a fault stops a train or isolates a malfunctioning component rather than allowing unsafe movement; this makes it very hard to cause two trains to collide but comparatively easy to halt all trains in an area. The Dutch network uses the NS'54 signalling system integrated with ATB cab signalling under infrastructure manager ProRail, and similar sabotage incidents have recently occurred in France and Latvia.

hackernews · choult · Sep 15, 10:22 · [Discussion](https://news.ycombinator.com/item?id=49710253)

**Background**: Fail-safe design is a core principle in railway engineering: any breakdown should result in a safe state, typically by stopping a train, shutting off a signal, or isolating a faulty component. The Dutch railway signalling system, known as NS'54, has been in effect since 1954 and is integrated with ATB, the cab signalling system widely used on the Dutch network. Because rail networks span huge geographic areas, they are extremely difficult to monitor continuously, which makes sabotage prevention a persistent challenge.

<details><summary>References</summary>
<ul>
<li><a href="https://www.intertechrail.com/fail-safe-rail-systems-standards">Fail-Safe Rail Systems & Standards</a></li>
<li><a href="https://en.wikipedia.org/wiki/Dutch_railway_signalling">Dutch railway signalling - Wikipedia</a></li>
<li><a href="https://www.reddit.com/r/trains/comments/v24ggh/protecting_rail_infrastructure_from_sabotage/">Protecting Rail infrastructure from sabotage? : r/trains - Reddit</a></li>

</ul>
</details>

**Discussion**: Commenters with rail engineering expertise noted that fail-safe design is easy to abuse at scale, since stopping all trains in an area is far simpler than causing a collision. Others linked the incident to a recent French rail sabotage near Renault's Cléon factory, a Russian warship firing flares at a Danish helicopter in the Baltic, and the timing with Prinsjesdag, debating whether this was a protest action or something else.

**Tags**: `#infrastructure-security`, `#rail-systems`, `#sabotage`, `#fail-safe-design`, `#geopolitics`

---

<a id="item-13"></a>
## [SHADOW-50M: 44M ternary LLM runs at 1,900 tok/s on CPU](https://www.reddit.com/r/MachineLearning/comments/1wgzpli/i_trained_a_44m_parameter_quantized_llm_from/) ⭐️ 7.0/10

A developer released SHADOW-50M, a 44M-parameter LLM trained from scratch on 45B tokens that ships as a 19.8 MB complete model with ternary {-1,0,+1} weights and runs at roughly 1,900 tok/s on a laptop CPU (about 500 tok/s in a browser via WebAssembly). It uses a 73,880-token vocabulary encoded as fixed 512-bit fingerprints instead of a trained embedding, plus a 159 KB compiled kernel and fixed circuits that handle arithmetic, dates, units, sorting and comparisons directly in the token stream. It shows that extreme quantization combined with hand-built deterministic circuits can make a useful, fully offline model that fits in under 20 MB and runs fast on commodity CPUs, a direction relevant to edge devices, browsers and privacy-preserving local inference. It also offers a candid comparison against a larger bf16 baseline, highlighting the trade-offs between raw benchmark scores and task-specific reliability. SHADOW loses to a 51.8M-parameter Llama-style bf16 model (Supra-50M-Reasoning) on standard benchmarks such as ARC-Easy (0.307 vs 0.435), PIQA (0.570 vs 0.600) and WikiText-2 perplexity (186 vs 165), but it answers arithmetic, date and record-retrieval questions correctly where the baseline fails. Its disk archive stores attention states at 1 bit (288 bytes/token) with a 22-byte/token index, and a persistent reinforcement trail raised measured top-1 retrieval from 0.571 to 0.743 without any training.

reddit · r/MachineLearning · /u/Final-Data-1410 · Sep 15, 12:59

**Background**: Ternary weight networks quantize all weights to {-1, 0, +1}, which eliminates multiplications and drastically cuts memory and compute, making them attractive for low-power inference. Quantized LLMs are typically run on CPUs using low-bit kernels, and WebAssembly allows such runtimes to execute directly in a browser tab. SHADOW-50M builds on these ideas by replacing the usual trained embedding table with fixed binary fingerprints and by routing certain computations to deterministic circuits rather than learned parameters.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/1605.04711">[1605.04711] Ternary Weight Networks</a></li>
<li><a href="https://www.emergentmind.com/topics/ternary-weight-networks-twns">Ternary Weight Networks Overview</a></li>
<li><a href="https://arxiv.org/pdf/2407.00088">T-MAC: CPU Renaissance via Table Lookup for Low-Bit LLM ...</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#quantization`, `#efficient-inference`, `#CPU`, `#ternary-weights`

---

<a id="item-14"></a>
## [Researcher asks how to obtain preprocessed datasets when paper authors don't respond](https://www.reddit.com/r/MachineLearning/comments/1wgutx6/d_how_do_you_get_preprocessed_dataset_of_a_paper_d/) ⭐️ 6.0/10

A researcher posted on r/MachineLearning describing an attempt to reproduce a paper where the dataset statistics in Table 1 do not match the public raw data, even after implementing the described preprocessing exactly; the closest result is still an order of magnitude off for one dataset. The authors, who stated "data available on request," have not replied to an email and a follow-up, prompting the researcher to ask the community about best practices for handling such mismatches and escalating to the journal. This highlights a persistent reproducibility pain point in machine learning research: even when code and raw data are public, missing preprocessed artifacts and unresponsive authors can block independent verification. It affects anyone doing replication studies, benchmarking, or building on prior work, and connects to broader concerns about a reproducibility crisis in ML and AI research. The mismatch is severe—an order of magnitude off for one dataset—and the researcher has already tried all reasonable interpretations of the paper's filtering steps. Key open questions include whether to keep the larger reproducible dataset and document the discrepancy, whether sampling to match the reported size would create a different irreproducible dataset, and when to escalate from email follow-ups to contacting the journal.

reddit · r/MachineLearning · /u/Individual-Safety906 · Sep 15, 08:50

**Background**: In machine learning research, reproducibility means independent researchers can obtain the same results using the same data, code, and procedures. Papers often release raw data and code but not the exact preprocessed datasets used in experiments, and "data available on request" is a common but unreliable sharing mechanism. When preprocessing details are ambiguous or incomplete, reported dataset statistics like those in a Table 1 may be impossible to match exactly, leaving replicators to decide between documenting the mismatch or attempting to approximate the original data.

<details><summary>References</summary>
<ul>
<li><a href="https://www.geeksforgeeks.org/machine-learning/reproducibility-in-machine-learning/">Reproducibility in Machine Learning - GeeksforGeeks</a></li>
<li><a href="https://arxiv.org/html/2406.14325v3">Reproducibility in Machine Learning-based Research: Overview ...</a></li>
<li><a href="https://onlinelibrary.wiley.com/doi/10.1002/aaai.70002">Reproducibility in machine-learning-based research: Overview ...</a></li>

</ul>
</details>

**Tags**: `#reproducibility`, `#machine-learning`, `#research-practice`, `#dataset`, `#academia`

---

<a id="item-15"></a>
## [Author Cuts Apart Oversized Books to Make Them Readable](https://attainablefelicity.mattkirkland.com/20260915/cut-up-your-books.html) ⭐️ 5.0/10

A personal essay on attainablefelicity.mattkirkland.com describes the author's method of physically cutting apart large, unwieldy books so they are easier to hold and read. The post sparked a Hacker News discussion with 104 points and roughly 100 comments debating physical books versus e-readers. The piece touches on a broader tension between the tactile, nostalgic experience of physical books and the convenience of e-readers, a recurring debate among avid readers and technologists. It also raises practical questions about book preservation, annotation, and how people adapt physical media to their reading habits. The method involves destructive modification of a book's binding or pages, which permanently alters the object and is not reversible. Commenters noted that e-readers offer syncing across devices, customizable presentation, and quick dictionary lookups, making them a compelling alternative for large volumes.

hackernews · matt_kirkland · Sep 15, 18:45 · [Discussion](https://news.ycombinator.com/item?id=49716953)

**Background**: Physical books, especially large reference volumes or omnibus editions, can be awkward to hold and read comfortably, which has led some readers to modify them. E-readers such as Kobo and Kindle have become popular alternatives because they are lightweight and offer adjustable text, search, and annotation features. The Hacker News community frequently debates the trade-offs between digital and physical reading experiences.

**Discussion**: Commenters were divided: some shared that they now annotate and embrace worn books rather than keeping them pristine, while others argued that cutting up books is too much effort and that e-readers are superior for large volumes. A few suspected the post was a troll or oblique commentary on AI companies' destructive scanning of rare books.

**Tags**: `#books`, `#reading`, `#e-readers`, `#DIY`, `#hacker-news`

---

<a id="item-16"></a>
## [NeurIPS 2026 Multi-Venue Logistics Spark Fairness Concerns](https://www.reddit.com/r/MachineLearning/comments/1wh0xaz/neurips_2026_handling_of_multiple_venue_locations/) ⭐️ 5.0/10

A Reddit discussion on r/MachineLearning highlights that NeurIPS 2026 will be held across three locations — Sydney, Atlanta, and Paris — with Sydney designated as the 'main' venue. Paper authors recently received forms to select a preferred venue, but are reportedly not guaranteed to present at their chosen location, raising concerns about fairness and logistics. This matters because NeurIPS is one of the largest and most prestigious AI conferences, and how it handles multi-site logistics directly affects thousands of researchers' ability to present their work, network, and advance their careers. If authors are arbitrarily assigned to satellite venues while the 'main' venue hosts the most prestigious events, it could create a two-tier experience that disadvantages certain regions. The discussion notes that NeurIPS passes for Sydney sold out in minutes, and while paper authors are guaranteed one pass at their designated location, the venue assignment process appears uncertain. The core question raised is whether having a 'main' venue with all the major events is appropriate, or whether the conference should be spread more evenly across locations.

reddit · r/MachineLearning · /u/CantKillTheLifeless · Sep 15, 13:48

**Background**: NeurIPS (Conference on Neural Information Processing Systems) is an annual interdisciplinary conference founded in 1987, covering machine learning, AI, statistics, and computational neuroscience. For 2026, it is expanding to a multi-site format with the main venue in Sydney, Australia, and satellite events in Atlanta, USA, and Paris, France. This is a significant change from the traditional single-location format and introduces new logistical and fairness challenges for attendees and authors.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Conference_on_Neural_Information_Processing_Systems">Conference on Neural Information Processing Systems - Wikipedia</a></li>
<li><a href="https://neurips.cc/">NeurIPS 2026</a></li>
<li><a href="https://x.com/NeurIPSConf/status/2036185904113475623?lang=en">NeurIPS Conference on X</a></li>

</ul>
</details>

**Discussion**: The Reddit thread reflects a mix of frustration and concern, with commenters questioning whether the 'main' venue designation unfairly concentrates prestige and resources in Sydney. Some argue that if multiple locations are necessary, the conference should be spread evenly to ensure a fair experience for all attendees, while others express uncertainty about how venue assignments will be decided.

**Tags**: `#NeurIPS`, `#conference`, `#logistics`, `#community`, `#fairness`

---

<a id="item-17"></a>
## [uv 0.12.15 fixes pip install regression and speeds cold-cache resolution](https://github.com/astral-sh/uv/releases/tag/0.12.15) ⭐️ 4.0/10

Astral released uv 0.12.15 on 2026-09-15, a patch release that reverts a change in 0.12.14 which had rejected valid installation commands such as `uv pip install --system` in `python:*` Docker images and `uv pip install --target .`. It also speeds up cold-cache resolution and HTTP cache revalidation by batching cache writes. Because uv is widely used in CI pipelines and Docker builds, the 0.12.14 regression could break containerized installs for many users, so this quick revert restores expected behavior. The performance improvement also matters for CI and fresh-machine scenarios where caches start empty. The fix is a revert of the change titled "Reject symlinked wheel installation destinations" (PR #21699), and the performance work batches cache writes to speed cold-cache resolution and HTTP cache revalidation (PR #21675). Prebuilt binaries are provided for macOS, Windows, and multiple Linux architectures including x86_64, aarch64, riscv64, s390x, and powerpc64le.

github · astral-releases-bot[bot] · Sep 15, 12:09

**Background**: uv is an extremely fast Python package and project manager written in Rust by Astral, designed as a drop-in replacement for pip, venv, and related tools. It supports project management with a universal lockfile, script execution with inline dependency metadata, and Python version management. A cold cache means the first run on a fresh machine or CI runner, where no package metadata or wheels are cached locally, making resolution and downloads slower than warm-cache runs.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.astral.sh/uv/">uv is an extremely fast Python package and project manager , written...</a></li>
<li><a href="https://github.com/astral-sh/uv">astral-sh/ uv : An extremely fast Python package and project manager ...</a></li>
<li><a href="https://towardsdatascience.com/why-package-installs-are-slow-and-how-to-fix-it/">Why Package Installs Are Slow (And How to Fix It) | Towards Data Science</a></li>

</ul>
</details>

**Tags**: `#python`, `#package-manager`, `#uv`, `#release-notes`, `#bug-fix`

---

<a id="item-18"></a>
## [uv 0.12.14 Improves Error Diagnostics and Adds Download Resumption](https://github.com/astral-sh/uv/releases/tag/0.12.14) ⭐️ 4.0/10

astral-sh/uv released version 0.12.14 on 2026-09-15, a minor patch that unifies package-operation error diagnostics with consistent hints and compact labeled cause chains, and changes exit codes so expected failures return 1 while recognized operational and internal failures return 2. It also adds resumption of interrupted downloads via HTTP Range requests when the server supports them, plus several resolver and cache performance improvements. These changes make uv easier to debug in CI and automation, since clearer error chains and distinct exit codes let scripts and pipelines react correctly to different failure types. Download resumption and faster resolution also reduce friction for users on flaky networks or working with large package indexes. The release includes a `batch-export` preview feature for exporting multiple dependency selections from a shared lockfile in one `uv export --batch` invocation, and fixes issues such as installing packages with paths longer than MAX_PATH on Windows, preventing `uv python install` from overwriting valid unmanaged Python symlinks on Unix, and redacting credentials from URL errors.

github · astral-releases-bot[bot] · Sep 15, 02:19

**Background**: uv is an extremely fast Python package and project manager from Astral, written in Rust, that handles dependency resolution, virtual environments, Python version installation, and tool execution. It uses a universal lockfile and aims to replace tools like pip, pip-tools, and virtualenv with a single fast binary. HTTP Range requests are a standard mechanism that lets clients fetch only part of a file, which is what enables resuming an interrupted download instead of starting over.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.astral.sh/uv/">uv is an extremely fast Python package and project manager , written...</a></li>
<li><a href="https://github.com/astral-sh/uv">astral-sh/ uv : An extremely fast Python package and project manager ...</a></li>
<li><a href="https://http.dev/range-request">HTTP Range Requests explained</a></li>

</ul>
</details>

**Tags**: `#python`, `#package-manager`, `#uv`, `#release-notes`, `#tooling`

---

<a id="item-19"></a>
## [Reddit User Asks If Partial Algorithm Qualifies for ML Workshop](https://www.reddit.com/r/MachineLearning/comments/1wgv7hi/how_much_work_in_progress_can_a_workshop/) ⭐️ 3.0/10

A Reddit user on r/MachineLearning asked whether a partially implemented algorithm—one that solves only problem A using a simplified principle, with preliminary results but no full implementation for problems A and B—is sufficient for a workshop submission. The user proposed submitting the existing algorithm, its results, and a plan plus mathematics for the full A-and-B version. This question reflects a common dilemma for early-career researchers navigating the norms of workshop submissions, which often serve as a venue for junior researchers to participate in conferences like ICLR. Clarifying what counts as acceptable work-in-progress helps students decide when to submit rather than wait for a full paper. The user notes that the simplified algorithm solving only problem A is not novel, and that only the full algorithm solving both A and B would be novel; the submission would therefore rely on a plan and mathematics for the unimplemented portion. Workshop policies vary, and some venues explicitly encourage submissions of varying lengths and scopes as an entry point for new researchers.

reddit · r/MachineLearning · /u/strammerrammer · Sep 15, 09:13

**Background**: Machine learning workshops are typically co-located with major conferences and are known for accepting work-in-progress, early-stage, or position papers that may not meet the novelty bar of main conference proceedings. They often aim to foster discussion and give junior researchers feedback, though organizers still enforce formatting, anonymity, and minimum academic standards. The question of how much implementation is required is a perennial one for students preparing their first submissions.

<details><summary>References</summary>
<ul>
<li><a href="https://iclr.cc/Conferences/2027/WorkshopGuidelines">ICLR 2027 Workshop Guidance</a></li>
<li><a href="https://representational-alignment.github.io/">Re-Align Workshop</a></li>

</ul>
</details>

**Tags**: `#machine-learning`, `#workshop`, `#research-advice`, `#academic-publishing`

---