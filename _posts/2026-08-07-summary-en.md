---
layout: default
title: "Horizon Summary: 2026-08-07 (EN)"
date: 2026-08-07
lang: en
---

> From 31 items, 23 important content pieces were selected

---

1. [DeepSeek V4 Flash 0731: Faster, Cheaper, and More Capable](#item-1) ⭐️ 8.0/10
2. [OpenAI Unveils New Security Controls for Critical Cyber Capabilities](#item-2) ⭐️ 8.0/10
3. [Oracle Bans AI-Generated Code in OpenJDK Contributions](#item-3) ⭐️ 8.0/10
4. [Rust-Based pgrust Makes Postgres 300x Faster for Analytics](#item-4) ⭐️ 8.0/10
5. [Cloudflare Kitesurf: Agent-First Browser on V8 Isolates](#item-5) ⭐️ 8.0/10
6. [2027 Memory Capacity Reportedly Sold Out Amid AI Demand](#item-6) ⭐️ 8.0/10
7. [A Year of Fighting Scrapers on a 1.5 Million-Page Website](#item-7) ⭐️ 8.0/10
8. [Assembly Hall of Shame: Showcasing Slowest x86 Instructions](#item-8) ⭐️ 7.0/10
9. [Tech Worker Disillusionment: What Happens When an Entire Class Loses Faith](#item-9) ⭐️ 7.0/10
10. [SDSS Releases All-Sky Map of Half a Million Supermassive Black Holes](#item-10) ⭐️ 7.0/10
11. [App Store Rejects App for Nonexistent Tarot Feature](#item-11) ⭐️ 7.0/10
12. [Codex with GPT-5.6 Sol Ultra Outshines Claude Fable 5 in Raccoon Heist Game Test](#item-12) ⭐️ 7.0/10
13. [Tokenpocalypse: Companies Scramble to Cut AI Spending](#item-13) ⭐️ 7.0/10
14. [Optimal LLM Quantization Bit-Width Under Fixed Memory Budget](#item-14) ⭐️ 7.0/10
15. [Improved Bad Apple Compression via SIREN Batch Sampling](#item-15) ⭐️ 6.0/10
16. [Open-Source Tool Generates Slides from Papers Using Local LLMs](#item-16) ⭐️ 6.0/10
17. [uv 0.12.3 Adds CPython 3.13.15 and Workspace Optimizations](#item-17) ⭐️ 5.0/10
18. [textlog: A Quiet, Text-Only Microblogging Platform with No JavaScript](#item-18) ⭐️ 5.0/10
19. [ACM Multimedia 2026 Registration and APC Fees Draw Criticism](#item-19) ⭐️ 5.0/10
20. [MLP Trained on ImageNet-1k Entirely on Android Phone](#item-20) ⭐️ 4.0/10
21. [Seeking OCR Strategies for Doctor Handwriting](#item-21) ⭐️ 4.0/10
22. [CIKM 2026 Decisions Released, Community Shares Results](#item-22) ⭐️ 4.0/10
23. [US Researchers Weigh NeurIPS 2026: Sydney vs Atlanta](#item-23) ⭐️ 3.0/10

---

<a id="item-1"></a>
## [DeepSeek V4 Flash 0731: Faster, Cheaper, and More Capable](https://arcprize.org/results/deepseek-v4-flash-0731) ⭐️ 8.0/10

DeepSeek released the official version of DeepSeek-V4-Flash-0731 on July 31, 2026, superseding the preview version with substantially enhanced agentic capabilities. The model retains the same structure as DeepSeek-V4-Flash-DSpark, including a speculative decoding module for faster inference. This update significantly improves speed and capability while maintaining low cost, making it a strong competitor to leading closed-source models. Users report it is good enough for almost everything and cheap enough that costs are irrelevant, which could accelerate adoption of open-weight models in production. DeepSeek-V4-Flash-0731 is a sparse mixture-of-experts model with 284B total parameters and 13B active parameters, supporting a 1M-token context window. It achieves top-tier performance in coding benchmarks and significantly narrows the gap with closed-source models on reasoning and agentic tasks.

hackernews · tosh · Aug 7, 17:56 · [Discussion](https://news.ycombinator.com/item?id=49214008)

**Background**: DeepSeek is a Chinese AI company known for releasing open-weight large language models. The V4 Flash series is designed for efficiency, offering fast inference and high throughput at a fraction of the cost of premium models. The 0731 release is the official version, following an earlier preview, and includes a speculative decoding module to speed up generation.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash-0731">deepseek-ai/DeepSeek-V4-Flash-0731 · Hugging Face</a></li>
<li><a href="https://openrouter.ai/deepseek/deepseek-v4-flash-0731">DeepSeek V4 Flash 0731 - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://deepinfra.com/deepseek-ai/DeepSeek-V4-Flash">deepseek-ai/DeepSeek-V4-Flash - Demo - DeepInfra</a></li>

</ul>
</details>

**Discussion**: Users are generally positive, praising the model's speed, capability, and cost-effectiveness. One user noted running it locally on 2x RTX Pro 6000 Blackwell achieved ~8k tok/s prefill and ~250 tok/s on a single stream. However, some reported issues like infinite loops and token waste, and a side discussion emerged about account bans on Claude, unrelated to DeepSeek.

**Tags**: `#AI`, `#DeepSeek`, `#LLM`, `#Model Release`, `#Performance`

---

<a id="item-2"></a>
## [OpenAI Unveils New Security Controls for Critical Cyber Capabilities](https://openai.com/index/responding-next-frontier-critical-cyber-capabilities/) ⭐️ 8.0/10

OpenAI announced new security measures for advanced AI models that may possess critical cyber capabilities, including stricter security controls and isolated testing environments. This follows the disclosure that its upcoming Astra model may cross a critical cybersecurity threshold. This marks a significant step in AI safety as models approach capabilities that could be misused for cyberattacks. The measures aim to prevent malicious use while maintaining legitimate security research, impacting the broader AI and cybersecurity ecosystem. The announcement references the Preparedness Framework first published in December 2023. OpenAI's Daybreak program already offers controlled access to cyber-tuned models like GPT-5.5-Cyber for authorized red teaming, gated behind Trusted Access verification.

hackernews · artninja1988 · Aug 7, 16:39 · [Discussion](https://news.ycombinator.com/item?id=49213029)

**Background**: OpenAI has been developing the Preparedness Framework to guide how it identifies and responds to emerging AI capabilities in areas like cybersecurity. The framework helps the company plan actions as models approach critical thresholds. This latest move reflects ongoing efforts to balance AI advancement with safety and security.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/responding-next-frontier-critical-cyber-capabilities/">Responding to the next frontier of critical cyber capabilities</a></li>
<li><a href="https://finance.yahoo.com/technology/article/openai-says-its-upcoming-astra-model-may-have-critical-cybersecurity-capabilities-amid-rash-of-ai-model-hacks-194909085.html?fr=sycsrp_catchall">OpenAI says its upcoming Astra model may have 'critical ...</a></li>
<li><a href="https://www.unite.ai/openai-says-upcoming-astra-model-may-cross-critical-cybersecurity-threshold/">OpenAI Says Upcoming Astra Model May Cross Critical ...</a></li>

</ul>
</details>

**Discussion**: Community comments show a mix of technical insights and skepticism. Some users shared positive experiences with OpenAI's Sol model in vulnerability discovery, while others criticized the lack of transparency about past incidents and questioned the effectiveness of new security controls. There is also concern about the centralization of AI and a desire to move systems on-premises.

**Tags**: `#AI safety`, `#cybersecurity`, `#OpenAI`, `#security controls`, `#vulnerability research`

---

<a id="item-3"></a>
## [Oracle Bans AI-Generated Code in OpenJDK Contributions](https://app.dealroom.co/news/feed/oracle-bans-ai-generated-code-from-openjdk-despite-ellison-s-claim-oracle-isn-t-writing-its-own-code) ⭐️ 8.0/10

Oracle has implemented an interim policy banning AI-generated code from OpenJDK community contributions, citing legal and review burden concerns. The policy applies to submissions from the community, though core developers may be exempt. This policy could set a precedent for other open-source projects grappling with AI-generated contributions, potentially slowing innovation but protecting legal integrity. It also highlights the tension between Oracle's AI investments and its cautious stance on AI in critical codebases. The policy is an interim measure, with a final version being drafted by Oracle's lawyers. Contributors must soon check a checkbox in Skara, the automated PR review system, to confirm compliance with the AI policy.

hackernews · delduca · Aug 7, 17:36 · [Discussion](https://news.ycombinator.com/item?id=49213754)

**Background**: OpenJDK is the open-source implementation of Java, widely used in enterprise environments. Oracle, as the corporate sponsor, manages contributions to ensure code quality and legal safety. The ban reflects concerns about copyright provenance and the burden of reviewing AI-generated code, which may lack the care of human-written contributions.

<details><summary>References</summary>
<ul>
<li><a href="https://openjdk.org/legal/ai">OpenJDK Interim Policy on Generative AI</a></li>
<li><a href="https://www.infoq.com/news/2026/06/oracle-genai-policies/">Oracle's OpenJDK Bans Generative AI Contributions While... - InfoQ</a></li>

</ul>
</details>

**Discussion**: Commenters generally support the ban, noting Oracle's legal history and the practical burden on reviewers. Some point out the irony of Oracle's AI investments, while others clarify that the policy may not apply to core developers, focusing on community submissions.

**Tags**: `#OpenJDK`, `#AI-generated code`, `#Oracle`, `#policy`, `#open source`

---

<a id="item-4"></a>
## [Rust-Based pgrust Makes Postgres 300x Faster for Analytics](https://malisper.me/how-we-made-postgres-hundreds-of-times-faster-the-query-engine/) ⭐️ 8.0/10

The author of pgrust, a Rust-based query engine for Postgres, published a detailed post explaining how it achieves hundreds of times faster analytics through batching, operator fusion, and SIMD. The project also emphasizes correctness via formal verification and differential fuzz testing. This could significantly boost Postgres's analytical performance, making it more competitive with specialized OLAP databases like DuckDB and ClickHouse. It also demonstrates the viability of Rust-based query engines and adaptive planning, potentially influencing future database development. The post details techniques such as batching (processing multiple rows at once), operator fusion (combining operators to reduce overhead), and SIMD (single instruction, multiple data) for parallel data processing. The author mentions proving over 1000 user-facing functions have identical logic in pgrust and Postgres, and the project is open-source.

hackernews · poly2it · Aug 7, 11:00 · [Discussion](https://news.ycombinator.com/item?id=49208535)

**Background**: Traditional Postgres uses a row-based execution model, which is inefficient for analytical queries that scan large datasets. Modern analytical databases often use columnar storage, vectorized execution, and SIMD to achieve high performance. Operator fusion and batching are techniques to reduce per-row overhead and improve cache locality.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/pdf/1610.09166">Push vs. Pull-Based Loop Fusion in Query Engines</a></li>
<li><a href="https://www.vldb.org/cidrdb/papers/2025/p7-schmidt.pdf">Rethinking MIMD-SIMD Interplay for Analytical Query ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Formal_verification">Formal verification - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The author engaged in the comments, addressing trust concerns by highlighting formal verification and fuzz testing. Some commenters expressed skepticism about adoption due to the lack of the Postgres core team's backing, while others praised the adaptive planning feature and the potential for embedding pgrust as an alternative to SQLite.

**Tags**: `#Postgres`, `#Rust`, `#query-engine`, `#performance`, `#SIMD`

---

<a id="item-5"></a>
## [Cloudflare Kitesurf: Agent-First Browser on V8 Isolates](https://blog.cloudflare.com/kitesurf/) ⭐️ 8.0/10

Cloudflare announced Kitesurf, an agent-first browser that runs in V8 isolates, built on the open-source Blitz engine. This enables efficient browser automation at the edge. This represents a significant step in browser automation and edge computing, potentially enabling more efficient and scalable agent-based web interactions. It could impact developers and businesses relying on web scraping, testing, and automated content generation. Kitesurf is built on Blitz, a modular open-source browser engine developed by Dioxus Labs. Cloudflare intends to open source and upstream their patches to Blitz. The browser runs in V8 isolates, allowing lightweight execution contexts for high concurrency.

hackernews · m3h · Aug 7, 10:42 · [Discussion](https://news.ycombinator.com/item?id=49208393)

**Background**: V8 isolates are lightweight execution contexts inside Google's V8 engine that allow edge platforms to run thousands of tenants per process without containers or VMs. An agent-first browser is designed to enable AI agents to perform tasks in the browser, such as web scraping, testing, and content generation. Cloudflare's Browser Run service already offers headless Chrome on its global network, and Kitesurf extends this concept with a more efficient architecture.

<details><summary>References</summary>
<ul>
<li><a href="https://www.clodo.dev/blog/v8-isolates-comprehensive-guide">V8 Isolates: From Concept to Production – Building Efficient ...</a></li>
<li><a href="https://fordelstudios.com/research/how-v8-isolates-actually-work-under-the-hood">How V8 Isolates Work: Architecture, Limits, and Trade-offs ...</a></li>

</ul>
</details>

**Discussion**: Community comments show mixed reactions. Some praise the technical innovation and open-source plans, while others express concerns about potential conflicts with Cloudflare's anti-bot services. There are also questions about practical use cases for browser agents and skepticism about the company's dual role as CDN and agent provider.

**Tags**: `#browser`, `#cloudflare`, `#edge computing`, `#web scraping`, `#open source`

---

<a id="item-6"></a>
## [2027 Memory Capacity Reportedly Sold Out Amid AI Demand](https://www.ign.com/articles/ramageddon-continues-another-year-as-2027-memory-capacity-is-reportedly-sold-out) ⭐️ 8.0/10

Memory suppliers have reportedly sold out their entire production capacity for 2027, driven by surging AI demand and HBM production constraints. This marks an unprecedented level of forward selling in the memory industry. This development signals prolonged memory shortages and potential price increases for consumer electronics, servers, and AI hardware through 2027. It underscores the strategic importance of memory supply in the AI-driven economy and may accelerate investment in alternative memory technologies. HBM production consumes roughly three times the wafer supply of DDR5 for the same bit count, constraining non-HBM memory supply. TSMC's CoWoS packaging capacity is also sold out through 2026, further bottlenecking the AI chip supply chain.

hackernews · inigyou · Aug 7, 07:58 · [Discussion](https://news.ycombinator.com/item?id=49207236)

**Background**: Memory chips are essential components in computers, smartphones, and AI accelerators. HBM (High Bandwidth Memory) is a specialized type of DRAM stacked vertically to provide high bandwidth, crucial for AI workloads. The shift of wafer capacity to HBM production has created a shortage of conventional DRAM, affecting consumer products.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ign.com/articles/memory-shortage-sees-2027-production-reportedly-sold-out-as-demand-far-outstrips-supply">Memory Suppliers Reportedly Now Sold Out For Whole of 2027 ...</a></li>
<li><a href="https://www.idc.com/resource-center/blog/why-the-memory-market-is-still-tight-what-comes-next/">Memory Market Outlook: Why Tightness Lasts to 2027 - IDC</a></li>
<li><a href="https://appleinsider.com/articles/26/08/05/ram-production-worldwide-is-sold-out-through-2027">Apple's high-priced RAM nightmare confirmed to stay for 2027</a></li>

</ul>
</details>

**Discussion**: Commenters expressed concerns about rising costs and supply constraints, with some noting the impact on consumer electronics and inflation. Technical users highlighted the wafer trade-off between HBM and DDR5, while others shared personal strategies like stockpiling or reducing AI usage.

**Tags**: `#memory`, `#hardware`, `#AI`, `#supply chain`, `#HBM`

---

<a id="item-7"></a>
## [A Year of Fighting Scrapers on a 1.5 Million-Page Website](https://patronview.com/news/99-percent-of-my-website-traffic-is-bots/) ⭐️ 8.0/10

A website owner detailed a year-long battle against scrapers and bots on their 1.5 million-page site, reporting traffic spikes, a 500% cost increase in one month, and the trade-offs of using Cloudflare versus alternatives like Anubis. This highlights the growing challenge of bot mitigation for website owners, the financial impact of such attacks, and the broader debate about relying on centralized services like Cloudflare versus open-web alternatives. It offers practical insights for others facing similar issues. The site's normal monthly bill is around $90, but one spike month saw a 500% increase, partly due to D1 costs. The author acknowledges being a scraper themselves, adding nuance to the discussion. Cloudflare offers Bot Fight Mode (free) and Super Bot Fight Mode (paid) as simple toggles, while Anubis uses proof-of-work to detect real browsers.

hackernews · petercooper · Aug 7, 14:51 · [Discussion](https://news.ycombinator.com/item?id=49211386)

**Background**: Web scraping and bot traffic are common issues for websites, often consuming resources and increasing costs. Mitigation strategies range from simple rate limiting to advanced solutions like Cloudflare's bot management, which uses machine learning and behavioral analysis. Alternatives like Anubis employ proof-of-work challenges to distinguish humans from bots without relying on centralized services.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cloudflare.com/products/bot-mitigation/">Cloudflare Bot Management - Stop Bad Bots</a></li>
<li><a href="https://developers.cloudflare.com/bots/">Overview · Cloudflare bot solutions docs</a></li>

</ul>
</details>

**Discussion**: Community comments express concerns about Cloudflare's centralization, with one user noting that outsourcing decisions on who can access a site to a large company undermines the open web. Others recommend Anubis as an effective alternative, sharing success stories. Some suggest moving to static sites to reduce costs, while another user shares frustration about AI search bots like Claude fetching thousands of pages without compensation.

**Tags**: `#web scraping`, `#bot mitigation`, `#Cloudflare`, `#cost optimization`, `#site reliability`

---

<a id="item-8"></a>
## [Assembly Hall of Shame: Showcasing Slowest x86 Instructions](https://github.com/xoreaxeaxeax/asm-hall-of-shame) ⭐️ 7.0/10

A GitHub repository titled 'Assembly Hall of Shame' has been created to showcase the slowest x86 instructions, gaining significant community traction with 179 points and 38 comments. The repository includes a leaderboard of instructions that take unusually long to execute, such as a 12ms write to an ACPI IO port. This repository provides a novel and entertaining exploration of CPU performance quirks, offering valuable insights for systems programmers and hardware enthusiasts. It highlights how certain instructions can trigger unexpected behaviors like SMM traps, which has implications for performance optimization and low-level security research. The repository includes rules that state trapped, emulated, or virtualized instructions may only time the trap, not the handler. One notable entry is a 12ms write to an ACPI IO port, which is suspected to trap to System Management Mode (SMM) for handling, and the repository links to related projects like 'smiiiiiiiiiiiiiiii' that use slow instructions to break SMI.

hackernews · piotrgrabowski · Aug 7, 18:01 · [Discussion](https://news.ycombinator.com/item?id=49214098)

**Background**: x86 processors include a wide range of instructions, some of which are rarely used and can be extremely slow due to microarchitectural quirks or because they trigger special execution modes. System Management Mode (SMM) is a privileged operating mode in x86 CPUs that suspends normal execution, including the OS, to handle firmware-level tasks such as power management or thermal control. SMM is triggered by a System Management Interrupt (SMI), and code running in SMM is invisible to the OS, making it both a security concern and a source of unexpected performance hits.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/System_Management_Mode">System Management Mode - Wikipedia</a></li>
<li><a href="https://wiki.osdev.org/System_Management_Mode">System Management Mode - OSDev Wiki SoK: 20 Years of Power, Privilege, and Peril in x86 System ... System Management Mode deep dive: How SMM isolation hardens ... SMM and BIOS: x86 Internals Explained | PDF | Cpu Cache ... SMM and BIOS: Insights for x86 Systems | PDF - Scribd</a></li>
<li><a href="https://vanbulck.net/files/woot26-smm.pdf">SoK: 20 Years of Power, Privilege, and Peril in x86 System ...</a></li>

</ul>
</details>

**Discussion**: The community discussion includes references to related topics like Core War, and comments on the rules of the repository, with one user noting that the 12ms ACPI IO port write likely traps to SMM. Another user humorously suggests that 'Nop' should be #1 because it is infinitely slow for what it does, while another reflects on how computers still feel slow despite executing millions of instructions per millisecond, citing abstraction overhead.

**Tags**: `#assembly`, `#x86`, `#hardware`, `#performance`, `#systems`

---

<a id="item-9"></a>
## [Tech Worker Disillusionment: What Happens When an Entire Class Loses Faith](https://www.noemamag.com/why-is-everyone-in-tech-so-sad/) ⭐️ 7.0/10

An article on Noema Magazine explores the widespread sadness and loss of faith among tech workers, prompting a deep community discussion about the industry's current state and future. The piece resonates strongly, with 272 points and 409 comments on Hacker News. This article highlights a significant and timely issue about tech worker disillusionment, which could impact talent retention, innovation, and the broader economy. The high engagement suggests it resonates deeply with many in the industry, indicating a potential shift in workforce sentiment. The article discusses the emotional state of tech workers, including feelings of sadness and a desire for more grounded occupations. Community comments draw historical parallels, such as the decline of the printing trade, and highlight the toxicity of the online world as a contributing factor.

hackernews · RickJWagner · Aug 7, 12:42 · [Discussion](https://news.ycombinator.com/item?id=49209539)

**Background**: The tech industry has long been seen as a source of high-paying, stable jobs, but recent years have brought layoffs, burnout, and a sense of moral compromise. This article taps into a broader societal trend of questioning the value and sustainability of tech careers, especially as the industry faces economic uncertainty and ethical scrutiny.

**Discussion**: Community comments express a range of perspectives, from historical analogies (e.g., the decline of printing) to personal reflections on losing passion and even daydreaming about homelessness. Some commenters note the toxicity of the online world, while others question the feasibility of escaping to grounded occupations, given economic realities.

**Tags**: `#tech industry`, `#worker morale`, `#career disillusionment`, `#mental health`, `#societal trends`

---

<a id="item-10"></a>
## [SDSS Releases All-Sky Map of Half a Million Supermassive Black Holes](https://www.sdss.org/black-hole-mapper-release-20/) ⭐️ 7.0/10

The Sloan Digital Sky Survey (SDSS) has released Data Release 20 (DR20), which includes an all-sky map of over 500,000 supermassive black holes, marking a major milestone for the Black Hole Mapper program. This dataset provides unprecedented insights into the masses, growth, and physics of quasars and active galactic nuclei across cosmic time, significantly advancing our understanding of supermassive black holes and galaxy evolution. DR20 includes over 3.3 million optical spectra spanning 500,000 galaxies and 1.5 million stars, and features the first southern hemisphere optical observations from Las Campanas Observatory, coordinated with eROSITA X-ray data.

hackernews · MarcoDewey · Aug 7, 15:24 · [Discussion](https://news.ycombinator.com/item?id=49211921)

**Background**: Supermassive black holes are extremely dense regions at the centers of galaxies, with masses millions to billions of times that of the Sun. The SDSS-V survey uses the Black Hole Mapper program to observe these objects across the sky, providing a comprehensive view of their distribution and properties.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sdss.org/black-hole-mapper-release-20/">Mapping Monsters: SDSS-V Data Release 20 Unveils All-Sky ...</a></li>
<li><a href="https://phys.org/news/2026-08-monsters-unveils-sky-views-supermassive.html">Mapping monsters: Data release unveils all-sky views of ...</a></li>
<li><a href="https://www.openaccessgovernment.org/sdss-v-data-release-20-unveils-all-sky-views-of-supermassive-black-holes/212810/">SDSS-V data release 20 unveils all-sky views of supermassive black holes</a></li>

</ul>
</details>

**Discussion**: Community members expressed excitement about the data, with one noting the simultaneous release of the eROSITA X-ray catalogue, which nearly doubled known X-ray sources. Others asked about the gridded patterns in the map, questioning whether they are artifacts or real features, and discussed the potential for individual researchers to use SDSS data with modern AI techniques.

**Tags**: `#astronomy`, `#black holes`, `#SDSS`, `#data release`, `#cosmology`

---

<a id="item-11"></a>
## [App Store Rejects App for Nonexistent Tarot Feature](https://daringfireball.net/2026/08/app_store_rejection_of_the_week_dark_hours) ⭐️ 7.0/10

Apple's App Store rejected the game Dark Hours, claiming it included a live tarot reading feature, despite the app having no such functionality. The developer's appeals, including to the App Review Board, were upheld based on this incorrect assertion. This incident highlights the arbitrary and opaque nature of Apple's app review process, which can significantly impact developers' livelihoods and user access to apps. It underscores ongoing concerns about platform gatekeeping and the need for more transparent and consistent review standards. The developer, Godier, escalated the rejection to the App Review Board, which responded that the original rejection was valid because they 'understand that the app includes a live tarot reading feature.' The app has no tarot, horoscope, or astrology-related content, as confirmed by the developer and others.

hackernews · _da_ · Aug 7, 18:59 · [Discussion](https://news.ycombinator.com/item?id=49214863)

**Background**: The App Store review process is a gatekeeping mechanism where Apple manually reviews apps before they are published. Developers often face rejections for reasons that can be unclear or inconsistent, leading to frustration and appeals. This case is particularly egregious because the stated reason is factually incorrect.

<details><summary>References</summary>
<ul>
<li><a href="https://daringfireball.net/2026/08/app_store_rejection_of_the_week_dark_hours">Daring Fireball: App Store Rejection of the Week: Dark Hours</a></li>
<li><a href="https://developer.apple.com/forums/thread/750787">The App Review Process at Apple is… | Apple Developer Forums</a></li>
<li><a href="https://www.revenuecat.com/blog/growth/the-ultimate-guide-to-app-store-rejections">The ultimate guide to App Store rejections | RevenueCat</a></li>

</ul>
</details>

**Discussion**: Commenters expressed frustration with the arbitrary nature of App Store reviews, sharing personal experiences of inconsistent decisions. Some noted the irony that astrology apps like Co-Star have been featured by Apple, while this app was rejected for a nonexistent feature. Others pointed to broader issues of platform gatekeeping and the need for reform.

**Tags**: `#App Store`, `#Developer Experience`, `#Mobile Apps`, `#Platform Governance`, `#Tech Criticism`

---

<a id="item-12"></a>
## [Codex with GPT-5.6 Sol Ultra Outshines Claude Fable 5 in Raccoon Heist Game Test](https://simonwillison.net/2026/Aug/7/moonlight-mayhem/#atom-everything) ⭐️ 7.0/10

Simon Willison ran the exact same prompt on Codex Desktop with GPT-5.6 Sol Ultra, which produced a much better game called 'Moonlight & Mayhem' compared to his earlier Claude Fable 5 version. The new game features a museum heist with multiple raccoons, though it initially had a bug with oversized eyeballs that was fixed with a simple prompt. This comparison highlights the rapid progress in AI-assisted coding, showing that newer models like GPT-5.6 Sol Ultra can produce more complex and polished games from a single prompt. It provides practical insights for developers evaluating AI tools for software development, potentially influencing tool choices and expectations. Codex spent 52 minutes on the project, with an estimated API cost of $23.28 (700.7K input tokens plus 32.5M cached tokens, and 148K output tokens) if not using a subscription. The full transcript is available in the GitHub repository, and Simon noted that Claude Code lacks a 'copy as Markdown' feature that Codex has.

rss · Simon Willison · Aug 7, 19:18

**Background**: AI-assisted coding tools like Codex and Claude Code use large language models to generate code from natural language prompts. GPT-5.6 is a family of models from OpenAI with variants Luna, Terra, and Sol, where Sol is the most capable and 'ultra' mode coordinates multiple subagents for complex tasks. Simon Willison is a well-known developer and blogger who frequently tests AI tools, and this comparison follows his earlier experiment with Claude Fable 5.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/gpt-5-6/">GPT-5.6: Frontier intelligence that scales with your ambition | OpenAI</a></li>
<li><a href="https://openai.com/index/previewing-gpt-5-6-sol/">Previewing GPT-5.6 Sol: a next-generation model | OpenAI</a></li>
<li><a href="https://openai.com/index/introducing-the-codex-app/">Introducing the Codex app | OpenAI</a></li>

</ul>
</details>

**Tags**: `#AI coding`, `#GPT-5.6`, `#Codex`, `#Claude`, `#game development`

---

<a id="item-13"></a>
## [Tokenpocalypse: Companies Scramble to Cut AI Spending](https://simonwillison.net/2026/Aug/7/pdfs-are-terrible/#atom-everything) ⭐️ 7.0/10

A 404 Media report from June 24 reveals that companies like Accenture are scrambling to reduce AI spending as token consumption skyrockets, with non-engineers and PDF-to-markdown conversions identified as major cost drivers. This highlights a growing enterprise challenge: AI token costs are becoming a significant financial burden, forcing companies to rethink usage patterns and optimize workflows. It underscores the need for cost-aware AI adoption strategies across industries. Accenture's internal data shows that non-engineers, not engineers, are driving token consumption, and converting PDFs to markdown is a major token consumer. Converting files to markdown can reduce token usage by 65-90% without content quality loss.

rss · Simon Willison · Aug 7, 16:18

**Background**: Token consumption in AI refers to the total tokens used per request, including input and output tokens, directly determining LLM costs. As AI workloads scale, enterprises are seeking ways to manage token spend, with PDF-to-markdown conversion emerging as a key optimization technique.

<details><summary>References</summary>
<ul>
<li><a href="https://www.deloitte.com/us/en/insights/topics/emerging-technologies/ai-tokens-how-to-navigate-spend-dynamics.html">AI tokens: How to navigate AI’s new spend dynamics | Deloitte Insights</a></li>
<li><a href="https://www.mindstudio.ai/blog/convert-files-markdown-reduce-ai-tokens">How to Convert Files to Markdown to Reduce AI Token Usage by Up to 90% | MindStudio</a></li>
<li><a href="https://aiproductivity.ai/news/pdf-to-markdown-llm-token-savings/">PDF to Markdown: Cut LLM Token Costs by Up to 50%</a></li>

</ul>
</details>

**Tags**: `#AI costs`, `#token consumption`, `#enterprise AI`, `#cost optimization`

---

<a id="item-14"></a>
## [Optimal LLM Quantization Bit-Width Under Fixed Memory Budget](https://www.reddit.com/r/MachineLearning/comments/1vi6im4/what_is_currently_considered_the_theoretically/) ⭐️ 7.0/10

A Reddit user asks whether current research identifies a theoretical optimal quantization bit-width for LLMs under a fixed memory budget, comparing smaller models at higher bits versus larger models at lower bits. The question references recent advances in 3-bit, 2-bit, and 1.5-bit quantization and calls for evidence from scaling laws or large empirical studies from 2025–2026. This question addresses a critical trade-off in LLM deployment: whether to prioritize model size or precision under memory constraints. The answer could guide practitioners in selecting optimal quantization levels for maximum capability, impacting efficiency and cost in real-world applications. The user specifically mentions open-source formats like GGUF and notes that 4-bit was historically considered the sweet spot, but newer methods show strong results at 3-bit, 2-bit, and even ~1.5-bit. They ask for evidence on whether a 2-bit 70B model generally beats a 4-bit 35B model, and whether quantization degradation eventually outweighs parameter gains.

reddit · r/MachineLearning · /u/takuonline · Aug 7, 17:10

**Background**: Quantization reduces the memory footprint of LLMs by representing weights with fewer bits, enabling larger models to fit into limited hardware. Recent research, such as ParetoQ, has explored extremely low-bit quantization (1-bit to 4-bit) and proposed scaling laws to compare trade-offs. The optimal bit-width depends on the balance between model size and accuracy, which is an active area of study.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2502.02631">ParetoQ: Improving Scaling Laws in Extremely Low-bit LLM ...</a></li>
<li><a href="https://arxiv.org/pdf/2502.02631v1">ParetoQ: Scaling Laws in Extremely Low-bit LLM Quantization</a></li>
<li><a href="https://dasroot.net/posts/2026/02/gguf-quantization-quality-speed-consumer-gpus/">GGUF Quantization : Quality vs Speed on Consumer GPUs</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#quantization`, `#model compression`, `#efficiency`, `#machine learning`

---

<a id="item-15"></a>
## [Improved Bad Apple Compression via SIREN Batch Sampling](https://www.reddit.com/r/MachineLearning/comments/1vhvfws/improved_compression_of_bad_apple_into_a_neural/) ⭐️ 6.0/10

The author improved the compression of the Bad Apple video into a SIREN neural network by using a different batch sampler that feeds pixels from across the entire video, achieving better fidelity with the same model architecture (4 x 512 sine layers, 792,257 parameters). This demonstrates that simple training data sampling strategies can significantly impact the quality of implicit neural representations for video compression, offering a practical improvement without changing the model. It also highlights the potential and limitations of using SIRENs for video compression, which could inform future research in neural compression. The model does not actually learn motion; intermediate frames are nonsensical. The author also tried a full-frame-rate version, but image reconstruction suffered compared to the low-rate version, and adding a separate autoencoder degraded quality while reducing model size.

reddit · r/MachineLearning · /u/cpldcpu · Aug 7, 09:06

**Background**: SIREN (Sinusoidal Representation Networks) is a neural network architecture that uses periodic sine activation functions to represent complex natural signals, such as images, audio, and video, as implicit neural representations. In this context, the network is trained to map coordinates (e.g., pixel locations and time) to pixel values, effectively compressing the video into the network's weights. The batch sampler determines which training samples are fed to the network during training, and the author found that sampling pixels from the entire video rather than a limited set of frames improves fidelity.

<details><summary>References</summary>
<ul>
<li><a href="https://www.vincentsitzmann.com/siren/">Implicit Neural Representations with Periodic Activation ...</a></li>
<li><a href="https://arxiv.org/abs/2006.09661">[2006.09661] Implicit Neural Representations with Periodic ...</a></li>
<li><a href="https://github.com/vsitzmann/siren">GitHub - vsitzmann/siren: Official implementation of ... [2006.09661] Implicit Neural Representations with Periodic ... SIRENs — Implicit Neural Representations with Periodic ... Improving Accuracy and Efficiency of Implicit Neural ... SIREN Architecture | vsitzmann/siren | DeepWiki GitHub - dalmia/siren: PyTorch implementation of Sinusodial ...</a></li>

</ul>
</details>

**Tags**: `#neural compression`, `#SIREN`, `#video`, `#machine learning`, `#experiment`

---

<a id="item-16"></a>
## [Open-Source Tool Generates Slides from Papers Using Local LLMs](https://www.reddit.com/r/MachineLearning/comments/1vi0c4k/built_a_tool_to_generate_slides_from_research/) ⭐️ 6.0/10

A developer released academi_slide, an open-source tool that automatically generates slide decks and briefs from research papers using local LLMs (Ollama, llama.cpp) or cloud models. It extracts sections, tables, charts, metrics, and citations, and supports multilingual input/output. This tool addresses a common pain point for researchers and students by automating slide creation while prioritizing privacy through local processing. It fits the growing trend of local-first AI tools, offering an alternative to cloud-based services for sensitive or unpublished research. The tool uses prompt optimization and deck planning to produce a solid first draft, and can build both the slide deck and a brief in minutes. It is early-stage and open source, with the repository available on GitHub.

reddit · r/MachineLearning · /u/nickemlop · Aug 7, 13:14

**Background**: Creating presentation slides from research papers is often tedious and time-consuming. Many existing AI tools rely on cloud services, which raises privacy concerns for unpublished or sensitive data. Local LLMs, such as those run via Ollama or llama.cpp, allow processing on the user's own hardware, ensuring data privacy. Similar tools exist, but academi_slide differentiates itself by focusing on academic documents and multilingual support.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/CyberTimon/Powerpointer-For-Local-LLMs">GitHub - CyberTimon/Powerpointer-For-Local-LLMs: Local Powerpointer - A beautiful powerpoint generator which uses the power of local running large language models to generate the powerpoint slides. · GitHub</a></li>
<li><a href="https://medium.com/@gaddam.rahul.kumar/building-an-llm-powered-slide-deck-generator-with-langgraph-973aeaac0a06">Building an LLM-Powered Slide Deck Generator with LangGraph | by Rahul Kumar | Medium</a></li>
<li><a href="https://www.academicslides.com/">AcademicSlides - Present Your Research. Perfectly.</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#Research Tools`, `#Open Source`, `#Privacy`, `#Presentation`

---

<a id="item-17"></a>
## [uv 0.12.3 Adds CPython 3.13.15 and Workspace Optimizations](https://github.com/astral-sh/uv/releases/tag/0.12.3) ⭐️ 5.0/10

uv 0.12.3 was released on 2026-08-07, adding support for CPython 3.13.15 and introducing preview features for output format selection in `uv cache size` and JSON streaming for `uv workspace metadata`. It also includes several performance optimizations for workspace handling and Linux startup latency. This patch release improves the developer experience for Python package management by adding support for the latest CPython patch version and reducing memory usage for large workspaces. The performance optimizations, especially in conflict-heavy resolutions and Linux startup, help maintain uv's reputation as a fast and efficient tool. The preview features include `--output-format` for `uv cache size` with options for automatic, human-readable, or raw-byte output, and `uv workspace metadata --quiet` now preserves JSON output while suppressing diagnostics. Performance improvements include streaming JSON output for workspace metadata, reusing compiled workspace exclusion patterns, and avoiding slow procfs reads during Python interpreter discovery on Linux.

github · astral-automations-bot[bot] · Aug 7, 16:34

**Background**: uv is a fast Python package and project manager written in Rust, known for its speed and low overhead. Workspaces in uv allow managing multiple related packages in a single project, and `uv workspace metadata` exports workspace information as JSON for other tools to consume. The release also includes documentation updates, such as adding PEP 740 attestations to the GitHub Actions publishing example.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.astral.sh/uv/reference/internals/metadata/">Workspace Metadata | uv</a></li>
<li><a href="https://github.com/astral-sh/uv-dev/blob/main/docs/reference/internals/metadata.md">uv-dev/docs/reference/internals/metadata.md at main · astral ...</a></li>
<li><a href="https://docs.astral.sh/uv/concepts/projects/workspaces/">Using workspaces | uv - Astral</a></li>

</ul>
</details>

**Tags**: `#uv`, `#python`, `#release`, `#performance`, `#tooling`

---

<a id="item-18"></a>
## [textlog: A Quiet, Text-Only Microblogging Platform with No JavaScript](https://textlog.cc/about) ⭐️ 5.0/10

textlog, an open-source, text-only microblogging platform with no JavaScript, was showcased on Hacker News. It limits notes to 280 characters and focuses on a minimalist, quiet user experience. This project highlights a growing interest in minimal, distraction-free social platforms that prioritize text and simplicity over multimedia and engagement metrics. It offers an alternative to mainstream microblogging services, appealing to users who prefer a quieter online space. textlog is built without JavaScript, ensuring fast loading and accessibility. Notes are capped at 280 characters, similar to Twitter's original limit, and the platform supports following people and hashtags. The project is open-source, allowing community contributions and self-hosting.

hackernews · stagas · Aug 7, 10:52 · [Discussion](https://news.ycombinator.com/item?id=49208458)

**Background**: Microblogging is a form of blogging that uses short posts without titles, such as status updates. Traditional platforms like Twitter and Mastodon often include multimedia and complex features, while textlog strips these away to focus purely on text. The no-JavaScript approach aligns with a broader movement toward simpler, more performant web technologies.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Microblogging">Microblogging - Wikipedia</a></li>
<li><a href="https://textlog.cc/about">about · textlog</a></li>
<li><a href="https://en.wikipedia.org/wiki/Comparison_of_microblogging_and_similar_services">Comparison of microblogging and similar services - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The Hacker News community responded positively, with users praising its simplicity and open-source nature. Some compared it to similar projects like Bear Blog and org-social, while others questioned the need for complexity in rendering and suggested using a static site generator. One user expressed disinterest due to the 280-character limit.

**Tags**: `#microblogging`, `#open-source`, `#text-only`, `#minimalism`, `#web`

---

<a id="item-19"></a>
## [ACM Multimedia 2026 Registration and APC Fees Draw Criticism](https://www.reddit.com/r/MachineLearning/comments/1vhtrz2/on_the_acm_multimedia_2026_conference/) ⭐️ 5.0/10

A researcher reported that ACM Multimedia 2026 requires separate registrations and article processing charges (APCs) for each accepted paper, even for workshops. The total cost to present two workshop papers could reach USD 1,850, which the researcher deems unreasonable. This highlights the growing financial burden on researchers due to ACM's full transition to open access, which may discourage participation and disproportionately affect authors from low-resource institutions. It also sparks debate about the fairness of charging APCs on top of high registration fees. The registration portal does not allow the same email address to be used for multiple registrations, forcing authors to use different emails. The APC is USD 350 (or USD 250 for ACM members), while full author registration costs USD 950 (or USD 850 for members), and workshop registration costs USD 500.

reddit · r/MachineLearning · /u/rokk07 · Aug 7, 07:24

**Background**: ACM has moved to a fully open access publishing model, requiring authors to pay APCs for their papers unless covered by institutional agreements. ACM Multimedia is a premier conference in the field, and its registration fees typically cover access to sessions but not publication costs. The researcher's complaint reflects a broader trend of rising publication costs in academia.

<details><summary>References</summary>
<ul>
<li><a href="https://2026.acmmm.org/site/registration.html">ACM Multimedia 2026 Conference — Registration</a></li>
<li><a href="https://humanrobotinteraction.org/2026/acms-new-open-access-publishing-model/">ACMs New Open Access Publishing Model – HRI 2026</a></li>
<li><a href="https://libraries.acm.org/acmopen/apc-list-pricing">Article Processing Charge (APC) List Pricing</a></li>

</ul>
</details>

**Tags**: `#ACM`, `#conference`, `#registration`, `#APC`, `#open access`

---

<a id="item-20"></a>
## [MLP Trained on ImageNet-1k Entirely on Android Phone](https://www.reddit.com/r/MachineLearning/comments/1vhwwfr/imagenet1k_classifier_trained_entirely_on_an/) ⭐️ 4.0/10

A Reddit user trained a multilayer perceptron (MLP) with about 500K parameters on a downscaled 32x32 version of ImageNet-1k entirely on an Android phone using PyTorch and Termux, achieving 4.59% top-1 validation accuracy after 5 epochs. The training took around 30 minutes on a Dimensity 9300+ CPU using four Cortex-X4 cores. This experiment demonstrates the feasibility of training neural networks on mobile devices, pushing the boundaries of edge computing. While the accuracy is low, it highlights the potential for on-device machine learning and could inspire further optimization for mobile training. The model is an MLP with around 500K parameters, trained on a 32x32 downscaled ImageNet-1k for 5 epochs. The user chose MLP over CNN due to stability and faster training speed (10-30x faster per step) on the phone, and the training was CPU-only using 4 Arm Cortex-X4 cores.

reddit · r/MachineLearning · /u/Tall_Abrocoma_3533 · Aug 7, 10:30

**Background**: ImageNet-1k is a large-scale image classification dataset with 1000 classes, typically used to benchmark deep learning models. A multilayer perceptron (MLP) is a feedforward neural network with fully connected layers, which is simpler than convolutional neural networks (CNNs) and often less effective for image tasks. Termux is an Android terminal emulator that provides a Linux environment, allowing users to run Python and PyTorch on mobile devices without rooting.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Multilayer_perceptron">Multilayer perceptron - Wikipedia</a></li>
<li><a href="https://termux.dev/en/">Termux | The main termux site and help pages.</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion is limited, but likely includes comments about the low accuracy and the novelty of training on a phone. Some may question the choice of MLP over CNN, while others might appreciate the experimental effort.

**Tags**: `#MLP`, `#ImageNet`, `#Mobile Training`, `#Edge Computing`, `#Experiment`

---

<a id="item-21"></a>
## [Seeking OCR Strategies for Doctor Handwriting](https://www.reddit.com/r/MachineLearning/comments/1vi7br1/good_ocr_strategy_for_detecting_doctor/) ⭐️ 4.0/10

A Reddit user posted a request for OCR strategies to extract text from doctor handwriting, sharing an example image of a handwritten medical note. The post seeks community advice on effective approaches for this challenging task. Doctor handwriting recognition is a persistent problem in healthcare, where illegible notes can lead to errors and inefficiencies. Advances in OCR and AI, such as vision-language models, are improving accuracy and could significantly streamline medical documentation workflows. Traditional OCR methods achieve 65-78% accuracy on medical documents, while vision-language models (VLMs) reach 85-95%, according to a 2026 guide. The user's example image likely contains clinical shorthand and abbreviations, which require specialized models trained on medical handwriting.

reddit · r/MachineLearning · /u/Miserable-Love9055 · Aug 7, 17:40

**Background**: Handwriting recognition involves converting handwritten text in images into machine-readable text. It is a challenging machine learning problem due to variability in writing styles, especially in medical settings where doctors often write quickly and use shorthand. Recent advances in deep learning and vision-language models have significantly improved performance on such tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.extend.ai/resources/ocr-physician-handwriting-complete-guide">OCR for Physician Handwriting Guide April 2026 | Extend</a></li>
<li><a href="https://en.wikipedia.org/wiki/Handwriting_recognition">Handwriting recognition - Wikipedia</a></li>
<li><a href="https://nanonets.com/blog/handwritten-character-recognition/">Handwriting Recognition with ML (An In-Depth Guide)</a></li>

</ul>
</details>

**Discussion**: No community comments were provided for this post, so the sentiment and viewpoints are unknown.

**Tags**: `#OCR`, `#handwriting recognition`, `#machine learning`, `#medical`

---

<a id="item-22"></a>
## [CIKM 2026 Decisions Released, Community Shares Results](https://www.reddit.com/r/MachineLearning/comments/1vhtto1/cikm_2026_decisions_r/) ⭐️ 4.0/10

CIKM 2026 paper decisions are being announced today, with the resource track outcomes already sent out. One user reported preliminary acceptance rates of 2/6 full papers and 1/3 short papers from their batch. This announcement is significant for researchers in information and knowledge management, as CIKM is a top-tier conference in the field. The results will influence the research community's visibility and career progression for many authors. The conference is the 35th ACM International Conference on Information and Knowledge Management, scheduled for November 7-11, 2026, in Rome, Italy. The resource track focuses on datasets, benchmarks, and reusable resources, distinct from the main research track.

reddit · r/MachineLearning · /u/Happy-Hustler · Aug 7, 07:27

**Background**: CIKM is a leading international forum for research on information and knowledge management, covering topics like data mining, information retrieval, and databases. The conference typically includes multiple tracks, such as the applied research track and the resource track, each with separate review processes. Decisions are released in batches, and authors often share their outcomes on social media to gauge acceptance rates.

<details><summary>References</summary>
<ul>
<li><a href="https://cikm2026.diag.uniroma1.it/">Home - CIKM 2026</a></li>
<li><a href="http://www.cikmconference.org/">Conference on Information and Knowledge Management (CIKM)</a></li>

</ul>
</details>

**Discussion**: The Reddit thread shows a mix of anticipation and sharing, with one user reporting their acceptance numbers. The overall sentiment is neutral-positive, as researchers await or share their outcomes, though no detailed discussions or controversies have emerged yet.

**Tags**: `#CIKM`, `#conference`, `#research`, `#announcement`

---

<a id="item-23"></a>
## [US Researchers Weigh NeurIPS 2026: Sydney vs Atlanta](https://www.reddit.com/r/MachineLearning/comments/1vi5xz7/2026_neurips_where_are_you_going_d/) ⭐️ 3.0/10

A Reddit user in r/MachineLearning asked US-based researchers whether they plan to attend NeurIPS 2026 in Sydney or Atlanta, reflecting the conference's dual-location format. This question highlights the logistical and financial considerations that influence conference attendance, which can affect community engagement and networking opportunities for US researchers. The choice between an international and domestic venue may impact participation rates and the overall conference experience. NeurIPS 2026 is scheduled to be held in both Sydney, Australia, and Atlanta, USA, offering attendees a choice of location. The Reddit post has a low score (3/10) and no comments, indicating limited community engagement at the time of analysis.

reddit · r/MachineLearning · /u/rsesrsfh · Aug 7, 16:48

**Background**: NeurIPS (Conference on Neural Information Processing Systems) is a premier annual machine learning conference. In recent years, it has adopted a hybrid or multi-location format to accommodate a global audience, with 2026 featuring both Sydney and Atlanta as host cities.

**Tags**: `#NeurIPS`, `#conference`, `#community`

---