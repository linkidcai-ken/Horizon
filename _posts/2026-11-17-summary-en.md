---
layout: default
title: "Horizon Summary: 2026-11-17 (EN)"
date: 2026-11-17
lang: en
---

> From 17 items, 17 important content pieces were selected

---

1. [Carnegie Mellon launches CS Learn, free full-semester CS lectures on YouTube](#item-1) ⭐️ 8.0/10
2. [Optimizely CDN Compromised to Serve Malware on Zoom, GitLab](#item-2) ⭐️ 8.0/10
3. [Jiff 1.0: A new datetime library for Rust by BurntSushi](#item-3) ⭐️ 8.0/10
4. [Windows 11 Telemetry Tracks Developer Tools and Coding Agents](#item-4) ⭐️ 7.0/10
5. [Trmnl launches 31.5-inch color ePaper display Frame for $1200](#item-5) ⭐️ 7.0/10
6. [Marimba: A System One Model for Speech](#item-6) ⭐️ 7.0/10
7. [Duetto steers pretrained music transformer at sampling time for real-time jazz accompaniment](#item-7) ⭐️ 7.0/10
8. [BugMeNot, the Login-Sharing Service, Has Shut Down](#item-8) ⭐️ 6.0/10
9. [OpenCode launches browser product for AI agents, sparking security and competition debate](#item-9) ⭐️ 6.0/10
10. [Essay Argues Chemistry Is Fundamentally Geometry, Sparking Debate](#item-10) ⭐️ 6.0/10
11. [Cornell Report: Sheep Grazing Under Solar Arrays Benefits Farmers](#item-11) ⭐️ 6.0/10
12. [JPMorgan Chase technical issue causes online banking delays across US banks](#item-12) ⭐️ 6.0/10
13. [LLM 0.37.3 fixes logging break caused by SQLite 3.54.1 JSON change](#item-13) ⭐️ 4.0/10
14. [Reddit thread discusses AISTATS 2027 paper reviews going live](#item-14) ⭐️ 3.0/10
15. [Reddit user seeks serious AI/ML discussion spaces beyond Reddit](#item-15) ⭐️ 3.0/10
16. [Fresher seeks advice on AI/ML fundamentals after Infosys interview](#item-16) ⭐️ 3.0/10
17. [ICLR Author Asks If Area Chairs Are Moderating Rebuttal Discussions](#item-17) ⭐️ 3.0/10

---

<a id="item-1"></a>
## [Carnegie Mellon launches CS Learn, free full-semester CS lectures on YouTube](https://www.cs.cmu.edu/learn/) ⭐️ 8.0/10

Carnegie Mellon's Griffin School of Computer Science launched CS Learn, releasing full semesters of lectures from current CMU computer science courses for free on YouTube, with one course premiering each day this week and more courses coming in January. This is a significant open-education development from a top computer science institution, making high-quality current course content freely accessible to learners worldwide and potentially pressuring other universities to follow suit. The initiative is led by Phillip Compeau, who notes that students built tools to automate much of the production process; lectures are being released first, with courseware (projects, slides, notes) planned for later.

hackernews · pcompeau · Nov 16, 20:43 · [Discussion](https://news.ycombinator.com/item?id=50522980)

**Background**: OpenCourseWare (OCW) is a movement to make university course materials freely available online, pioneered by MIT in 2001. CMU's CS Learn follows this tradition but focuses on current, full-semester video lectures from its computer science program, delivered via YouTube for broad accessibility.

<details><summary>References</summary>
<ul>
<li><a href="https://ocw.mit.edu/">MIT OpenCourseWare | Free Online Course Materials</a></li>
<li><a href="https://www.classcentral.com/report/ocw-courses/">[2026] 8000+ OpenCourseWare Courses from Top... — Class Central</a></li>

</ul>
</details>

**Discussion**: Commenters generally welcomed the initiative, with alumni excited about specific courses like 15-259 and Tianqi Chen's ML Systems. Some emphasized the enduring value of fundamentals in the AI era, while others noted that lectures alone are insufficient without projects and feedback, and expressed hope that advanced courses will also be released.

**Tags**: `#education`, `#computer-science`, `#open-courseware`, `#youtube`, `#CMU`

---

<a id="item-2"></a>
## [Optimizely CDN Compromised to Serve Malware on Zoom, GitLab](https://blog.report-uri.com/worlds-largest-brands-infected-with-malware-via-optimizely/) ⭐️ 8.0/10

Optimizely's content delivery network was compromised to serve malicious code on high-traffic websites including Zoom and GitLab, as reported by Report-URI. The attack involved injecting malware into Optimizely's JavaScript snippets, affecting even Optimizely's own sites like www.optimizely.com and login.optimizely.com. This incident highlights the supply-chain risks of third-party scripts: a single compromised vendor can expose millions of users across many major sites. It underscores the need for stronger security controls and accountability for third-party script providers and the sites that embed them. The attacker gained write access to multiple unrelated customer projects, though it remains unclear whether this was via a compromised Optimizely system, a credential with cross-customer access, or another vector. Optimizely's CDN served exactly what it was given, so this was not a CDN cache-poisoning attack.

hackernews · kristjansson · Nov 16, 23:00 · [Discussion](https://news.ycombinator.com/item?id=50524767)

**Background**: Optimizely is a widely used platform for A/B testing and experimentation, and its JavaScript snippet is embedded on many high-traffic websites. These third-party scripts are loaded from the vendor's CDN, meaning any compromise at the vendor can directly affect all customer sites. Supply-chain attacks via third-party scripts have become a growing concern, as seen in similar incidents like the OptinMonster WordPress plugin compromise.

<details><summary>References</summary>
<ul>
<li><a href="https://ipban.com/your-cdn-just-pushed-malware-to-visitors/">Your CDN Just Pushed Malware To Visitors – IPBan Pro</a></li>
<li><a href="https://attack.mitre.org/techniques/T1189/">Drive-by Compromise , Technique T1189 - Enterprise | MITRE ATT&CK</a></li>

</ul>
</details>

**Discussion**: Commenters expressed frustration over the lack of accountability and the risks of third-party scripts, with some criticizing Google Tag Manager for enabling marketing to add bloated JavaScript without engineering oversight. Others suggested mitigations like NoScript and called for stronger security practices such as phased rollouts and automatic checks at both vendors and large sites.

**Tags**: `#security`, `#supply-chain`, `#web`, `#javascript`, `#cdn`

---

<a id="item-3"></a>
## [Jiff 1.0: A new datetime library for Rust by BurntSushi](https://burntsushi.net/jiff/) ⭐️ 8.0/10

Andrew Gallant (BurntSushi) has released version 1.0 of Jiff, a datetime library for Rust that aims to make common datetime operations difficult to misuse while maintaining reasonable performance. Jiff's 1.0 release provides a stable, well-designed alternative to existing Rust datetime libraries like chrono, potentially improving safety and ergonomics for Rust developers dealing with time zones and daylight saving time. Jiff puts time zone handling front and center, automatically handling many common daylight saving time problems, and its API is designed to guide users toward correct usage.

hackernews · burntsushi · Nov 16, 16:53 · [Discussion](https://news.ycombinator.com/item?id=50519744)

**Background**: Jiff is a datetime library for Rust that focuses on providing high-level primitives that are hard to misuse. It was created by Andrew Gallant, a well-known Rust developer also responsible for popular crates like ripgrep and rust-csv. The library aims to address shortcomings in existing datetime libraries by offering a safer and more ergonomic API.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/BurntSushi/jiff">GitHub - BurntSushi/ jiff : A datetime library for Rust that ...</a></li>
<li><a href="https://burntsushi.net/jiff/">A datetime library for Rust - Andrew Gallant's Blog</a></li>

</ul>
</details>

**Discussion**: The community discussion highlights appreciation for Jiff's design and BurntSushi's work, with a former chrono maintainer sharing candid insights on the challenges of improving datetime APIs. Some users express hope for wider adoption, while others ask about handling specialized time scales like TAI and UT1.

**Tags**: `#rust`, `#datetime`, `#library`, `#api-design`, `#time-scales`

---

<a id="item-4"></a>
## [Windows 11 Telemetry Tracks Developer Tools and Coding Agents](https://xusheng.dev/posts/windows-coding-agent-telemetry/) ⭐️ 7.0/10

A new report reveals that Windows 11's default telemetry collects data on which coding agents and developer tools users run, and this data can be sent to Microsoft when 'Optional diagnostic data' is enabled, which is the default setting. This raises privacy concerns for developers, as it means Microsoft can monitor their tool usage, potentially influencing decisions about migrating to Linux or other platforms, and highlights the need for transparency and control over telemetry in operating systems. Users can disable this telemetry by navigating to Settings → Privacy & security → Diagnostics & feedback and turning off 'Optional diagnostic data'; however, the article notes that some telemetry may still be collected for security and quality purposes.

hackernews · cwaffles · Nov 16, 22:58 · [Discussion](https://news.ycombinator.com/item?id=50524736)

**Background**: Telemetry is the automatic collection of data about how software is used, which helps vendors improve products but can raise privacy issues. Windows 11 has faced criticism for its extensive telemetry, and developers often use tools like VS Code and AI coding agents such as Claude Code, which may be identifiable in the data. Sandboxing is a technique to isolate AI agents for security, and Windows has been slow to provide native sandboxing, leading some to use WSL.

<details><summary>References</summary>
<ul>
<li><a href="https://code.visualstudio.com/docs/enterprise/telemetry">Manage telemetry in enterprise environments</a></li>
<li><a href="https://amux.io/guides/ai-agent-sandboxing/">AI Agent Sandboxing in 2026: Docker, E2B, Firecracker... — amux</a></li>
<li><a href="https://en.wikipedia.org/wiki/Windows_11">Windows 11 - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters expressed privacy concerns, with some planning to switch to Linux, noting that Linux gaming is now viable for single-player games. Others highlighted the specific setting to disable telemetry and discussed the lack of native AI agent sandboxing on Windows, while some suggested that Microsoft may need telemetry to prioritize features like sandboxing.

**Tags**: `#privacy`, `#telemetry`, `#windows`, `#developer-tools`, `#linux`

---

<a id="item-5"></a>
## [Trmnl launches 31.5-inch color ePaper display Frame for $1200](https://trmnl.com/blog/introducing-frame) ⭐️ 7.0/10

Trmnl has announced Frame, a 31.5-inch full-color ePaper display enclosed in a handmade wooden body, priced at $1200. The device features Spectra 6 color ePaper technology, rechargeable batteries lasting months, offline mode via microSD, and a discrete button panel. This product pushes the boundaries of large-format color ePaper displays, which have traditionally been expensive and niche. Its launch sparks discussion about the viability of ePaper for new use cases like AI coding agents and digital dashboards, and highlights challenges in pricing and quality assurance for hardware startups. Frame uses Spectra 6 color ePaper, which offers a limited color palette and slow refresh rates, making it unsuitable for video but ideal for static content. At $1200, it is significantly more expensive than Trmnl's previous products, and the handmade wooden frame adds a premium cost that some community members question.

hackernews · geerlingguy · Nov 16, 16:23 · [Discussion](https://news.ycombinator.com/item?id=50519354)

**Background**: ePaper displays are bistable, meaning they only consume power when the image changes, making them extremely energy-efficient and easy on the eyes. Color ePaper technology like Spectra 6 has emerged recently but remains costly and limited in color gamut and refresh speed. Trmnl is known for its open-source ePaper dashboard devices and has a community of DIY and productivity enthusiasts.

<details><summary>References</summary>
<ul>
<li><a href="https://shop.trmnl.com/products/frame">Frame - 31.5" Spectra 6 Color ePaper Display – TRMNL</a></li>
<li><a href="https://trmnl.com/blog/introducing-frame/">Introducing Frame | TRMNL</a></li>
<li><a href="https://www.datallen.com/blogs/the-color-epaper-display-guide.html">The Color E - Paper Display Guide: Technology , Cost, and the...</a></li>

</ul>
</details>

**Discussion**: Community reaction is mixed: some express excitement about the product but are deterred by the $1200 price, while others raise concerns about Trmnl's quality assurance and shipping delays, as well as the founder's politics. Some see potential in ePaper for AI coding agents due to reduced eye strain, but many feel the price is too steep and the wooden frame unnecessary.

**Tags**: `#ePaper`, `#hardware`, `#display-technology`, `#product-launch`, `#HN-discussion`

---

<a id="item-6"></a>
## [Marimba: A System One Model for Speech](https://www.reddit.com/r/MachineLearning/comments/1xxsqro/marimba_a_system_one_model_for_speech_r/) ⭐️ 7.0/10

Marimba introduces a System One speech model that answers typed yes/no, choice, or score questions about audio windows using a single frozen Qwen3-ASR-0.6B encoder pass per 8-second window, with Platt-calibrated probabilities. It matches or beats Qwen3-Omni (30B-A3B) on 6 of 9 tests on the same 1,000 public questions, though it loses on turn-end detection and does not generalize to unseen tasks. This work shows that a small frozen ASR encoder can serve multiple typed speech queries with calibrated probabilities, offering a highly efficient alternative to large omni models for tasks like keyword spotting, language identification, and speaker change detection. It could significantly reduce inference cost for real-time speech analytics and edge deployment. Term spotting is zero-shot, scored from the decoder's greedy and 4 beam hypotheses then Platt-calibrated without training on the terms; language ID uses the ASR model's own language scores; turn end uses a small readout on frozen layer 18; speaker change and count use readouts on layer 12. Caveats include the turn-end readout being trained on Smart Turn data (in-distribution only), AUROC 0.930 vs Smart Turn v3.2's 0.982 on Smart Turn's test set, and all heads at chance on CochlScene scene classification.

reddit · r/MachineLearning · /u/solanotodesch · Nov 16, 15:47

**Background**: Qwen3-ASR is an open-source speech recognition model family from Alibaba's Qwen team, combining a Whisper-style audio encoder with a Qwen3 language model decoder, supporting 52 languages. Platt calibration (or Platt scaling) is a method that fits a logistic regression to a classifier's scores to transform them into calibrated probabilities. Smart Turn is a dataset and model for detecting whether a speaker has finished their turn in a conversation, useful for voice agents. System One refers to fast, intuitive, automatic responses, as opposed to slower deliberate reasoning (System Two).

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/QwenLM/Qwen3-ASR">GitHub - QwenLM/ Qwen3-ASR : Qwen3-ASR is an open-source series ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Platt_scaling">Platt scaling - Wikipedia</a></li>
<li><a href="https://github.com/pipecat-ai/smart-turn">GitHub - pipecat-ai/ smart - turn · GitHub</a></li>

</ul>
</details>

**Tags**: `#speech-recognition`, `#machine-learning`, `#efficient-inference`, `#calibration`, `#audio-models`

---

<a id="item-7"></a>
## [Duetto steers pretrained music transformer at sampling time for real-time jazz accompaniment](https://www.reddit.com/r/MachineLearning/comments/1xxkyh3/steering_a_pretrained_music_transformer_at/) ⭐️ 7.0/10

Duetto is a real-time jazz partner that uses the pretrained Anticipatory Music Transformer without fine-tuning, controlling generation at sampling time via rule-based logit editing to accompany a MIDI keyboard player. It plays standards as a small band, comping while the player plays and taking solos when the player stops, with a demo of 'Autumn Leaves' at 160 bpm. This work demonstrates a practical alternative to fine-tuning for real-time music generation, showing that sampling-time steering can produce coherent, interactive jazz accompaniment with low latency. It could enable more flexible and responsive AI music partners without the need for task-specific retraining. The system uses a rule layer to mask disallowed notes and bias likely ones (chord tones, guide tones, quoted phrases) before each sample, and keeps about 1 second of music sampled ahead with resampling of unplayed parts to maintain low latency. Performance is about 12 ms/note (medium) and 18 ms/note (large) on a 3080 Ti, and ~90 ms/note on a Jetson Orin Nano; about 61% of solo notes in the demo come from quoted phrases or the theme.

reddit · r/MachineLearning · /u/GGAllin43 · Nov 16, 09:19

**Background**: The Anticipatory Music Transformer (Thickstun et al., 2023) is a generative model for symbolic music that can be conditioned on future events, making it suitable for accompaniment. Logit editing is a technique that modifies the raw output scores of a model before sampling to constrain or guide generation, often used as an alternative to fine-tuning. The Weimar Jazz Database is a public collection of transcribed jazz solos used for music research.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2306.08620">[2306.08620] Anticipatory Music Transformer</a></li>
<li><a href="https://jazzomat.hfm-weimar.de/dbformat/dboverview.html">Weimar Jazz Database (WJazzD) — The Jazzomat Research Project</a></li>

</ul>
</details>

**Tags**: `#music-generation`, `#transformer`, `#sampling-time-control`, `#real-time`, `#jazz`

---

<a id="item-8"></a>
## [BugMeNot, the Login-Sharing Service, Has Shut Down](https://www.bugmenot.com/) ⭐️ 6.0/10

BugMeNot, a service that let users share login credentials to bypass mandatory registration on websites, has shut down. The closure was noted on its website and discussed on Hacker News, where users shared memories and analysis of the service's history. BugMeNot was a widely used tool that symbolized early web culture's resistance to registration walls, and its shutdown marks the end of an era for a service that influenced the creation of RetailMeNot. The discussion highlights how websites have cracked down on shared logins, reflecting broader changes in web authentication and privacy practices. According to community comments, BugMeNot's founders leveraged its high PageRank to launch RetailMeNot, which became a highly profitable coupon-sharing site. In recent years, many shared logins on BugMeNot stopped working as websites implemented stricter checks, and alternatives like temporary email services now fill the gap.

hackernews · lode · Nov 16, 21:32 · [Discussion](https://news.ycombinator.com/item?id=50523601)

**Background**: BugMeNot was launched in 2004 as a way to bypass mandatory free registration on websites by providing shared usernames and passwords. It allowed users to access content without creating accounts, but raised ethical and legal concerns and faced blocking by some sites. RetailMeNot, founded by the same team, aggregates coupon codes and was eventually sold for hundreds of millions of dollars.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/BugMeNot">BugMeNot - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/RetailMeNot">RetailMeNot - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters expressed nostalgia for BugMeNot's usefulness, but also noted that shared logins have largely stopped working due to abuse and site crackdowns. Some pointed out that temporary email services are now a common alternative, though they lack the convenience of BugMeNot. Others shared historical details about how BugMeNot's founders spun it into RetailMeNot and profited from affiliate commissions.

**Tags**: `#BugMeNot`, `#web services`, `#shutdown`, `#privacy`, `#RetailMeNot`

---

<a id="item-9"></a>
## [OpenCode launches browser product for AI agents, sparking security and competition debate](https://opencode.ai/product/browse) ⭐️ 6.0/10

OpenCode has launched a new product called OpenCode Browse, a browser tool designed for AI agents, as announced on its website. The product aims to let AI agents interact with web content, but details on its features and security measures are limited. This launch intensifies competition in the crowded field of AI agent browser tools, where established players like Anthropic's Claude extension and Microsoft's Playwright MCP already offer similar capabilities. It also raises questions about security practices, as OpenCode faces criticism for being reckless with security. The product page provides minimal technical details, and it is unclear how OpenCode Browse differentiates from existing solutions like Playwright MCP or Claude's browser extension. Community members note that many browser solutions for agents exist, suggesting potential redundancy.

hackernews · mfiguiere · Nov 16, 21:20 · [Discussion](https://news.ycombinator.com/item?id=50523459)

**Background**: OpenCode is an open-source AI coding agent that connects to various AI models and is available as a terminal interface, desktop app, or IDE extension. AI agent browser tools allow AI models to control a web browser to perform tasks like web scraping, form filling, and testing. Playwright MCP is a Model Context Protocol server that provides browser automation capabilities using Playwright, while Claude's browser extension lets AI interact with web pages.

<details><summary>References</summary>
<ul>
<li><a href="https://opencode.ai/">OpenCode | The open source coding agent for any model</a></li>
<li><a href="https://github.com/microsoft/playwright-mcp">GitHub - microsoft / playwright - mcp : Playwright MCP server · GitHub</a></li>
<li><a href="https://chromewebstore.google.com/detail/browser-mcp-let-ai-use-yo/bjfgambnhccakkhmkepdoekmckoijdlc">Browser MCP - Let AI use your real browser - Chrome Web Store</a></li>

</ul>
</details>

**Discussion**: Commenters expressed concerns about OpenCode's security practices, with one calling the company reckless and noting that OpenCode V2 threw security out the window. Others compared the product to Anthropic's Claude extension (23 million users) and Playwright MCP, questioning the need for another browser solution when Chrome's CDP already exists. Some also asked about alternatives like OpenHands or Pi and expressed confusion over the crowded landscape.

**Tags**: `#AI agents`, `#browser automation`, `#OpenCode`, `#security`, `#developer tools`

---

<a id="item-10"></a>
## [Essay Argues Chemistry Is Fundamentally Geometry, Sparking Debate](https://chillphysicsenjoyer.substack.com/p/chemistry-is-actually-geometry) ⭐️ 6.0/10

A physics-oriented Substack essay titled 'Chemistry is Actually Geometry' argues that chemical phenomena can be understood through geometric principles, and it has sparked a lively Hacker News discussion with 72 comments. The essay and discussion touch on the philosophical debate about reductionism in science—whether complex fields like chemistry can be fully reduced to simpler, more fundamental descriptions like quantum electrodynamics or geometry—which affects how scientists and philosophers view the structure of scientific knowledge. Commenters noted that while molecular structure and protein folding are geometric, the essay covers only a small fraction of chemistry, and others warned against mistaking the map for the territory, emphasizing that analogies are useful but not proof of reality.

hackernews · sebg · Nov 16, 20:22 · [Discussion](https://news.ycombinator.com/item?id=50522643)

**Background**: Reductionism is the philosophical view that complex phenomena can be explained by reducing them to simpler, more fundamental entities or theories. In chemistry, molecular geometry describes the three-dimensional arrangement of atoms in molecules, which influences properties and reactivity. Quantum electrodynamics (QED) is the relativistic quantum field theory of electromagnetism, often cited as a fundamental theory to which chemistry can in principle be reduced.

<details><summary>References</summary>
<ul>
<li><a href="https://en.m.wikipedia.org/wiki/Reductionism">Reductionism - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Seesaw_molecular_geometry">Seesaw molecular geometry - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion was diverse, with some commenters agreeing that chemistry reduces cleanly to quantum electrodynamics, while others criticized the essay for overselling its coverage of chemistry and for conflating analogy with reality. A common sentiment was that while geometric analogies are powerful, they should not be mistaken for the territory itself.

**Tags**: `#chemistry`, `#physics`, `#geometry`, `#science-philosophy`, `#reductionism`

---

<a id="item-11"></a>
## [Cornell Report: Sheep Grazing Under Solar Arrays Benefits Farmers](https://news.cornell.edu/stories/2026/10/sheep-grazing-solar-fields-offers-farmers-economic-ecological-gains) ⭐️ 6.0/10

Cornell University published a report highlighting that grazing sheep beneath solar arrays can provide farmers with both economic and ecological benefits, such as diversified income and vegetation management. The story sparked a Hacker News discussion with 237 points and 233 comments on agrivoltaics, rural NIMBY pushback, and animal welfare. This practical application of agrivoltaics demonstrates how dual land use can address land competition between solar energy and agriculture, potentially increasing farmer acceptance and reducing rural opposition to solar farms. It also highlights animal welfare and shade benefits for livestock, which could influence future solar farm design and policy. The report focuses on sheep grazing specifically, as sheep are well-suited to navigate under and around panels without damaging equipment, unlike larger cattle. Community comments noted challenges such as affordable racking that withstands cattle rubbing and grid interconnection issues with local utilities.

hackernews · PaulHoule · Nov 16, 17:27 · [Discussion](https://news.ycombinator.com/item?id=50520182)

**Background**: Agrivoltaics, also known as agrisolar or dual-use solar, is the practice of using the same land for both solar energy production and agriculture. Solar panels can be installed between crops, elevated above crops, or arranged for livestock grazing; the shade from panels can benefit certain crops and provide shelter for animals, while farmers gain an additional income stream. The practice has been used at scale in arid regions to stabilize soils and curb desertification, and is gaining attention as a way to reduce land-use conflicts.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Agrivoltaics">Agrivoltaics</a></li>
<li><a href="https://www.realclearenergy.org/2021/11/10/nimby_rural_residents_push_back_on_large_solar_farms_802591.html">NIMBY : Rural Residents Push Back on Large Solar Farms</a></li>

</ul>
</details>

**Discussion**: Commenters broadly supported agrivoltaics, with some sharing personal experiences of rural NIMBY opposition to solar farms and others raising animal welfare concerns about livestock lacking shade in conventional farming. Practical challenges were also discussed, such as designing affordable racking that can withstand cattle and dealing with uncooperative local power companies for grid interconnection.

**Tags**: `#agrivoltaics`, `#solar-energy`, `#sustainability`, `#land-use`, `#renewable-energy`

---

<a id="item-12"></a>
## [JPMorgan Chase technical issue causes online banking delays across US banks](https://apnews.com/article/bank-outage-chase-wells-fargo-truist-50fee2693c22f597fa6ca51a97ef2cda) ⭐️ 6.0/10

A technical issue at JPMorgan Chase on Monday, November 16, caused delays and disruptions for customers accessing online banking services, with ripple effects reported at other major U.S. banks including Wells Fargo, Bank of America, and Truist. The outage highlights the interconnectedness and fragility of the U.S. banking infrastructure, where a single institution's technical problem can disrupt services for customers across multiple banks, affecting millions of users and drawing regulatory scrutiny. JPMorgan Chase stated that customers still have access to their funds and accounts and expected to resolve all issues by the end of the day; the exact root cause has not been disclosed, though speculation includes cloud or database outages.

hackernews · samk3nny · Nov 16, 18:31 · [Discussion](https://news.ycombinator.com/item?id=50521045)

**Background**: Major U.S. banks rely on complex, interconnected systems for online banking, often combining modern cloud services with legacy mainframe infrastructure. When a critical technical issue occurs at one large bank, it can cascade to others due to shared dependencies or network effects. Such outages raise concerns about operational resilience and the potential for systemic risk in the financial sector.

<details><summary>References</summary>
<ul>
<li><a href="https://apnews.com/article/bank-outage-chase-wells-fargo-truist-50fee2693c22f597fa6ca51a97ef2cda">Technical issue at JPMorgan Chase triggers online banking delays</a></li>
<li><a href="https://www.nytimes.com/2026/11/16/us/bank-outages-down.html">Chase Bank Transactions Disrupted by ‘ Technical Issue ’ Amid...</a></li>
<li><a href="https://www.usatoday.com/story/money/2026/11/16/bank-outage-nationwide-chase-bofa--live/92814152007/">Banking outage linked to Chase , impacted Wells Fargo and BofA</a></li>

</ul>
</details>

**Discussion**: Commenters on Hacker News speculated on root causes, citing a recent Revolut outage in Europe linked to Google Cloud, and pointed to underinvestment in QA and reliance on legacy mainframes (COBOL, CICS, DB/2). Some noted geographic patterns, suggesting an East Coast AWS issue, while others expressed broader anxiety about interconnected infrastructure failures.

**Tags**: `#outage`, `#banking`, `#infrastructure`, `#cloud`, `#reliability`

---

<a id="item-13"></a>
## [LLM 0.37.3 fixes logging break caused by SQLite 3.54.1 JSON change](https://simonwillison.net/2026/Nov/16/llm/) ⭐️ 4.0/10

LLM 0.37.3 is a bug-fix release that resolves a logging failure triggered by SQLite 3.54.1, which now returns SQL text instead of JSON for subqueries like `(select json_array(1))` inside `json_object()`. The fix wraps such subqueries with `json()` to restore the previous behavior. This release ensures that users of Simon Willison's LLM command-line tool, especially those who installed it via Homebrew with the latest SQLite, can continue to log prompts and responses without interruption. It also highlights how upstream database behavior changes can break downstream applications. The change in SQLite 3.54.1 was intentional: per D. Richard Hipp, `(SELECT json_array(...))` returns SQL text, not JSON, so the new behavior is correct and 3.54.0 was buggy. The workaround is to explicitly cast with `json((select json_array(1)))`.

rss · Simon Willison · Nov 16, 23:57

**Background**: LLM is a command-line tool by Simon Willison for running prompts against large language models, and by default it logs every prompt and response to a SQLite database. SQLite is an embedded database engine used widely in applications, and its JSON functions allow constructing and querying JSON data. Homebrew, a popular package manager for macOS and Linux, recently updated its SQLite package to version 3.54.1, which included a bug fix that changed how subqueries returning JSON text are handled inside `json_object()`.

<details><summary>References</summary>
<ul>
<li><a href="https://llm.datasette.io/en/stable/setup.html">Setup - LLM</a></li>
<li><a href="https://github.com/simonw/llm">simonw/ llm : Access large language models from the command - line ...</a></li>
<li><a href="https://www.sqlite.org/">SQLite Home Page</a></li>

</ul>
</details>

**Tags**: `#llm`, `#sqlite`, `#bug-fix`, `#release`, `#simon-willison`

---

<a id="item-14"></a>
## [Reddit thread discusses AISTATS 2027 paper reviews going live](https://www.reddit.com/r/MachineLearning/comments/1xxqa3i/aistats_2027_paper_discussion_d/) ⭐️ 3.0/10

A Reddit user created a discussion thread on r/MachineLearning noting that AISTATS 2027 paper reviews are supposed to go live today, inviting others to share their thoughts. Review release is a key milestone for authors awaiting decisions, and such threads often become hubs for sharing outcomes and comparing review experiences across the ML community. The post contains no technical content or specific review details, and as of the thread's creation, no substantive comments or outcomes had been shared.

reddit · r/MachineLearning · /u/LongjumpingAd4741 · Nov 16, 14:09

**Background**: AISTATS (International Conference on Artificial Intelligence and Statistics) is a peer-reviewed conference for research at the intersection of AI and statistics, ranked CCF C. Like most ML conferences, it uses a peer-review process where reviewers submit scores and comments before final decisions are made.

<details><summary>References</summary>
<ul>
<li><a href="https://aistats.org/aistats2025/">Home| Artificial Intelligence and Statistics Conference</a></li>
<li><a href="https://www.myhuiban.com/conference/1853">AISTATS 2027 (CCF C): International Conference on Artific...</a></li>

</ul>
</details>

**Tags**: `#aistats`, `#peer-review`, `#academia`, `#machine-learning`, `#reddit`

---

<a id="item-15"></a>
## [Reddit user seeks serious AI/ML discussion spaces beyond Reddit](https://www.reddit.com/r/MachineLearning/comments/1xxvby6/serious_spaces_d/) ⭐️ 3.0/10

A Reddit user on r/MachineLearning asked for recommendations of serious AI/ML discussion spaces outside Reddit, expressing dissatisfaction with existing Discord servers and subreddit quality. The user later edited the post to say they created their own space and invited others to message them. This reflects a common sentiment among AI/ML practitioners that mainstream platforms like Reddit and Discord often prioritize hype or self-promotion over substantive technical discourse. It highlights an unmet demand for higher-quality, community-driven spaces for research sharing and learning. The user notes that existing Discord servers, including those from frontier labs and Hugging Face, feel too focused on their own narratives. The post received a low score of 3.0/10, indicating limited engagement or perceived value for technical curation.

reddit · r/MachineLearning · /u/Substantial-Buyer365 · Nov 16, 17:23

**Background**: Reddit's r/MachineLearning is a popular forum for AI/ML news and research, but users often complain about noise, trolling, and low-quality posts. Discord servers hosted by organizations like Hugging Face and frontier AI labs offer real-time chat but may be biased toward their own products and communities. This has led some practitioners to seek alternative platforms for more focused and civil technical discussions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hugging_Face">Hugging Face - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The post received limited comments, but the user's edit indicates that many readers felt similarly, prompting them to create a new space. This suggests a shared frustration with current options and a willingness to build alternative communities.

**Tags**: `#community`, `#discussion`, `#machine-learning`, `#meta`, `#reddit`

---

<a id="item-16"></a>
## [Fresher seeks advice on AI/ML fundamentals after Infosys interview](https://www.reddit.com/r/MachineLearning/comments/1xy92xo/struggled_in_my_infosys_interview_as_a_fresher/) ⭐️ 3.0/10

A fresher who recently failed an Infosys interview for an AI/ML role has asked the r/MachineLearning community for advice on strengthening their technical fundamentals, despite having project experience with Python, machine learning, RAG, Agentic AI, and FastAPI. This reflects a common challenge for aspiring AI/ML engineers: the gap between project experience and deep conceptual understanding, which is critical for technical interviews and long-term career growth. The interview covered a wide range of topics including programming fundamentals, Python, JavaScript, OOP, FastAPI, Generative AI vs Agentic AI, RAG architecture, vector databases, and evaluation metrics like precision and recall. The fresher also holds a TCS Digital offer but has been waiting seven months for a joining letter.

reddit · r/MachineLearning · /u/EnvironmentalFact392 · Nov 17, 02:48

**Background**: RAG (Retrieval-Augmented Generation) is a technique that enhances large language models by retrieving relevant information from external knowledge bases to improve response accuracy. Agentic AI refers to AI systems that can autonomously perform tasks and make decisions, going beyond the content generation capabilities of Generative AI. Vector databases are specialized systems for storing and querying high-dimensional embeddings, enabling semantic search and efficient retrieval in AI applications.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Retrieval-augmented_generation">Retrieval - augmented generation - Wikipedia</a></li>
<li><a href="https://www.edureka.co/blog/what-is-agentic-ai/">What Is Agentic AI ? Architecture, Use Cases, Examples & Trends</a></li>
<li><a href="https://weaviate.io/blog/what-is-a-vector-database">What Is a Vector Database ? Similarity Search & Semantic... | Weaviate</a></li>

</ul>
</details>

**Tags**: `#career-advice`, `#interview-preparation`, `#machine-learning`, `#fresher`, `#reddit`

---

<a id="item-17"></a>
## [ICLR Author Asks If Area Chairs Are Moderating Rebuttal Discussions](https://www.reddit.com/r/MachineLearning/comments/1xy6t7g/is_anyones_ac_playing_the_role_of_discussion/) ⭐️ 3.0/10

A Reddit user posted on r/MachineLearning asking whether other authors' ICLR Area Chairs (ACs) are actively moderating discussions during the rebuttal period, noting that despite guidelines instructing ACs to encourage reviewers to respond to author rebuttals, their own paper has received "nothing but radio silence." This complaint highlights a perceived gap between ICLR's stated AC responsibilities and actual practice, which could undermine author trust in the fairness and responsiveness of the peer-review process at a premier machine-learning conference. The post is anecdotal and does not specify the paper, AC, or ICLR edition, but it references the official AC guide that tasks Area Chairs with encouraging reviewers to engage with author rebuttals; the user asks whether others have had better experiences.

reddit · r/MachineLearning · /u/Whatever_635 · Nov 17, 00:59

**Background**: ICLR (International Conference on Learning Representations) is a leading AI conference that uses the OpenReview platform for open peer review. In its process, authors submit papers, reviewers provide initial scores and comments, authors write rebuttals, and Area Chairs are expected to facilitate discussion and ensure reviewers respond before making final decisions. The AC Guide explicitly states that Area Chairs play a critical role in curating the technical programme and should encourage reviewer engagement during rebuttal.

<details><summary>References</summary>
<ul>
<li><a href="https://iclr.cc/Conferences/2025/ACGuide">AC Guide</a></li>
<li><a href="https://iclr.cc/Conferences/2026/AuthorGuide">ICLR 2026 Author Guide</a></li>
<li><a href="https://openreview.net/group?id=ICLR.cc">ICLR - OpenReview</a></li>

</ul>
</details>

**Tags**: `#ICLR`, `#peer-review`, `#academia`, `#machine-learning`, `#community-discussion`

---