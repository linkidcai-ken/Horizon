---
layout: default
title: "Horizon Summary: 2026-07-17 (EN)"
date: 2026-07-17
lang: en
---

> From 24 items, 16 important content pieces were selected

---

1. [Firefox Compiled to WebAssembly Runs Inside Another Browser](#item-1) ⭐️ 9.0/10
2. [First Atmosphere Found on Rocky Exoplanet in Habitable Zone](#item-2) ⭐️ 8.0/10
3. [Kimi K3 and the Pelican Benchmark: Tokenizer Quirks Revealed](#item-3) ⭐️ 8.0/10
4. [Open Source AI Models Gaining on Closed Rivals](#item-4) ⭐️ 8.0/10
5. [Prism Leaks Users' Papers via Compilation Bug](#item-5) ⭐️ 8.0/10
6. [EU AI Act OpenRAG: 933 Legal Chunks with BGE-M3 Embeddings](#item-6) ⭐️ 8.0/10
7. [Zilog Z80 Microprocessor Celebrates 50th Anniversary](#item-7) ⭐️ 7.0/10
8. [Recurse Center Founder Thanks HN for 15 Years of Support](#item-8) ⭐️ 7.0/10
9. [Practical Tips for Running SQLite](#item-9) ⭐️ 7.0/10
10. [Frame: Linux X Server Written in Assembly via Claude](#item-10) ⭐️ 6.0/10
11. [Real-Time SSH Honeypot Visualization](#item-11) ⭐️ 6.0/10
12. [Three Non-Solution Responses to Problems](#item-12) ⭐️ 6.0/10
13. [LLM Cliché Highlighter Tool](#item-13) ⭐️ 6.0/10
14. [Convert golf courses to offset data center water use](#item-14) ⭐️ 4.0/10
15. [User Seeks Experiences on Short Paper Acceptance at Top NLP Conferences](#item-15) ⭐️ 3.0/10
16. [BMVC Rebuttal Deadline: Modified Review Timestamps Raise Questions](#item-16) ⭐️ 3.0/10

---

<a id="item-1"></a>
## [Firefox Compiled to WebAssembly Runs Inside Another Browser](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 9.0/10

Puter has compiled the full Firefox browser to WebAssembly, enabling it to run inside another browser such as Chrome. The project uses the Wisp protocol over WebSocket to proxy all network traffic through Puter's servers. This is a groundbreaking technical achievement that demonstrates a new paradigm for browser-in-browser execution, potentially enabling new capabilities for web platforms. It also showcases the power of AI-assisted programming, as the project used an estimated $25,000 worth of Claude Opus and Fable tokens. Firefox was chosen because Gecko has strong single-process support, which simplifies the WebAssembly compilation. The demo supports end-to-end encryption: traffic to HTTPS sites remains encrypted, while HTTP traffic is visible in cleartext. The project's servers had to be scaled up to handle traffic from Hacker News.

rss · Simon Willison · Jul 16, 23:34

**Background**: WebAssembly (Wasm) is a low-level binary instruction format that allows code written in multiple languages to run in the browser at near-native speed. Compiling a full browser like Firefox to Wasm is extremely challenging because browsers are complex, multi-process applications that typically require direct access to system resources. The Wisp protocol is a low-overhead protocol for tunneling multiple TCP and UDP sockets over a single WebSocket connection, which is necessary because browser code cannot open arbitrary network connections.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/ wisp - protocol : Wisp is a low-overhead...</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion was highly positive, with many expressing amazement at the technical feat. Some commenters raised concerns about the cost of proxying all traffic through Puter's servers, and the team confirmed they had to scale up servers to handle the load.

**Tags**: `#WebAssembly`, `#Firefox`, `#browser engineering`, `#Wasm`, `#virtualization`

---

<a id="item-2"></a>
## [First Atmosphere Found on Rocky Exoplanet in Habitable Zone](https://www.bbc.com/news/articles/cy4kdd1e0ejo) ⭐️ 8.0/10

Astronomers using the James Webb Space Telescope have detected an atmosphere on LHS 1140b, a rocky exoplanet in the habitable zone of its red dwarf star, 48 light-years away. This marks the first confirmed atmosphere on a rocky planet in a habitable zone. This discovery challenges previous assumptions that red dwarf planets cannot retain atmospheres due to intense stellar radiation, opening new possibilities for finding habitable worlds. It also demonstrates JWST's capability to characterize rocky exoplanet atmospheres, a key step toward detecting biosignatures. LHS 1140b is about 1.7 times Earth's radius and orbits its star every 24.7 days. The detected gas is helium, which requires a high escape velocity to be retained, suggesting the planet is not a mini-Neptune but a rocky world with a substantial atmosphere.

hackernews · neversaydie · Jul 17, 14:06 · [Discussion](https://news.ycombinator.com/item?id=48947560)

**Background**: Red dwarf stars are the most common stars in the galaxy, but their habitable zones are very close, exposing planets to intense stellar flares and radiation that can strip atmospheres. LHS 1140b was previously thought to be a super-Earth or water world, but JWST's emission spectroscopy ruled out a mini-Neptune scenario, confirming its rocky nature with an atmosphere.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bbc.com/news/articles/cy4kdd1e0ejo">First atmosphere found around Earth-like planet LHS 1140 b</a></li>
<li><a href="https://earthsky.org/space/water-world-mini-neptune-lhs-1140-b/">Is this nearby exoplanet a water world? Or a mini-Neptune?</a></li>
<li><a href="https://nasaspacenews.com/2024/08/can-planets-around-red-dwarfs-sustain-life/">Can Planets Around Red Dwarfs Sustain Life? - NASA Space News</a></li>

</ul>
</details>

**Discussion**: Commenters expressed surprise that a rocky planet around a red dwarf could retain an atmosphere, with one noting that JWST data ruled out a mini-Neptune interpretation. Others discussed future propulsion systems to reach the planet and the significance of helium detection for escape velocity.

**Tags**: `#exoplanets`, `#JWST`, `#astronomy`, `#atmosphere`, `#habitable zone`

---

<a id="item-3"></a>
## [Kimi K3 and the Pelican Benchmark: Tokenizer Quirks Revealed](https://simonwillison.net/2026/Jul/16/kimi-k3/) ⭐️ 8.0/10

Simon Willison analyzed Kimi K3 using the 'pelican on a bike' benchmark, finding that the prompt 'Generate an SVG of a pelican riding a bicycle' consumes 95 tokens in Kimi K3 versus 10 in OpenAI, suggesting an 85-token hidden system prompt. This benchmark highlights critical limitations in LLM evaluation, particularly the lack of agentic tool-use testing, and exposes tokenizer inconsistencies and hidden prompts that affect model behavior and cost. Kimi K3 uses a hybrid linear attention mechanism (KDA) with a 1M-token context window and is the first open-source 3-trillion-parameter model, but its tokenizer counts 'hi' as 86 tokens, indicating a hidden system prompt likely related to reasoning effort.

hackernews · droidjj · Jul 17, 14:21 · [Discussion](https://news.ycombinator.com/item?id=48947717)

**Background**: The 'pelican on a bike' benchmark is a simple test where an LLM is asked to generate an SVG of a pelican riding a bicycle. It is used to compare model quality, cost, and speed, but does not test agentic capabilities like tool calling. Tokenizers convert text into tokens for LLM processing, and token counts affect pricing and context limits.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jul/16/kimi-k3/">Kimi K3, and what we can still learn from the pelican benchmark</a></li>
<li><a href="https://github.com/simonw/pelican-bicycle">GitHub - simonw/pelican-bicycle: LLM benchmark: Generate an ...</a></li>
<li><a href="https://platform.kimi.ai/docs/guide/kimi-k3-quickstart">Kimi K3 - Kimi API Platform</a></li>

</ul>
</details>

**Discussion**: Commenters debated whether pelicans on bikes appear in training data, with one noting that Simon's own blog content likely appears in training sets. Others appreciated the benchmark for revealing hidden prompts and tokenizer quirks, and some proposed adversarial variants to test agentic robustness.

**Tags**: `#LLM`, `#benchmark`, `#tokenizer`, `#agentic`, `#AI evaluation`

---

<a id="item-4"></a>
## [Open Source AI Models Gaining on Closed Rivals](https://stateofopensource.ai/) ⭐️ 8.0/10

A new analysis from Mozilla's State of Open Source AI report shows open source AI models have overtaken closed models in token processing volume on OpenRouter, with open models now handling 63% of tokens compared to 37% for closed models, a dramatic shift from 60-40 in favor of closed models just four months ago. This trend suggests that open source models may soon dominate the AI landscape, potentially undermining the business models of companies like OpenAI and Anthropic that rely on proprietary models. The shift could democratize AI access, reduce costs, and accelerate innovation across industries. The analysis is based on OpenRouter data showing open models processed 4.19 trillion tokens on a recent day, up nearly 5x from 888 billion tokens four months earlier. However, some community members criticized the report for being AI-generated and lacking original analysis.

hackernews · rellem · Jul 17, 14:31 · [Discussion](https://news.ycombinator.com/item?id=48947825)

**Background**: Open source AI models, such as Meta's Llama and Mistral, are released with publicly available weights and often allow free use and modification, while closed models like OpenAI's GPT-4 and Anthropic's Claude are proprietary and accessed via APIs. The debate between open and closed AI has intensified as open models improve rapidly, narrowing the performance gap.

<details><summary>References</summary>
<ul>
<li><a href="https://aisally.substack.com/p/open-vs-closed-ai-models">Open vs closed AI models: key differences and why it matters</a></li>
<li><a href="https://aimultiple.com/llm-market-share">LLM Market Share: Compare Usage & Adoption</a></li>

</ul>
</details>

**Discussion**: Community comments were mixed: some users celebrated the data showing open models' growth, while others criticized the Mozilla report for being AI-generated and lacking depth. One commenter noted that the presentation felt like an LLM's idea of a CTO deck, and another argued that using AI to write about open source AI undermines the report's credibility.

**Tags**: `#open source`, `#AI`, `#machine learning`, `#market analysis`, `#LLMs`

---

<a id="item-5"></a>
## [Prism Leaks Users' Papers via Compilation Bug](https://www.reddit.com/r/MachineLearning/comments/1uz75qt/prism_accidentally_leaked_d/) ⭐️ 8.0/10

A compilation bug in the Prism AI platform caused it to return someone else's paper to users, exposing unpublished research before the site was taken down within 10 minutes of the first report. This incident highlights critical security and privacy risks for AI-powered research platforms, potentially compromising users' unpublished work and eroding trust in such tools. The bug was first flagged on Discord and Twitter, and Prism's team responded quickly by taking the site offline. Users are worried their own papers may have been exposed.

reddit · r/MachineLearning · /u/Few-Monitor5103 · Jul 17, 17:59

**Background**: Prism is an AI-native workspace for scientists to write and collaborate on research, introduced by OpenAI. It is designed to modernize scientific workflows but, like any cloud platform, must handle sensitive unpublished data securely.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/introducing-prism/">Introducing Prism | OpenAI</a></li>

</ul>
</details>

**Discussion**: The Reddit community expressed concern and frustration over the leak, with many users worried about their unpublished research being exposed. Some praised Prism's quick response, but overall sentiment was negative regarding the security lapse.

**Tags**: `#security`, `#privacy`, `#AI platform`, `#data leak`, `#machine learning`

---

<a id="item-6"></a>
## [EU AI Act OpenRAG: 933 Legal Chunks with BGE-M3 Embeddings](https://www.reddit.com/r/MachineLearning/comments/1uytlac/eu_ai_act_openrag_933_legally_structured_chunks/) ⭐️ 8.0/10

A new open dataset, EU AI Act OpenRAG, provides 933 legally-structured chunks of the EU AI Act with BGE-M3 embeddings in a single SQLite file, along with retrieval evaluation results showing improved recall over a baseline sliding-window approach. This dataset enables more accurate retrieval-augmented generation (RAG) and legal NLP research on the EU AI Act by using the regulation's own legal structure rather than arbitrary text windows, potentially improving compliance tools and legal analysis. The SQLite database contains 933 chunks, each with a normalized 1024-dimensional BGE-M3 embedding, exact EUR-Lex links, and Article 113 application-date metadata; retrieval evaluation shows structural chunking achieves recall@20 of 0.541 versus 0.449 for the baseline.

reddit · r/MachineLearning · /u/Automatic-Forever-63 · Jul 17, 08:18

**Background**: Retrieval-augmented generation (RAG) combines large language models with external knowledge bases to improve output accuracy. BGE-M3 is a multilingual embedding model supporting dense, sparse, and multi-vector retrieval. EUR-Lex is the official online database of EU law. The EU AI Act (Regulation 2024/1689) is a landmark legal framework for artificial intelligence.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/BAAI/bge-m3">BAAI/bge-m3 · Hugging Face</a></li>
<li><a href="https://en.wikipedia.org/wiki/Retrieval-augmented_generation">Retrieval-augmented generation - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/EUR-Lex">EUR-Lex</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion includes technical questions about the chunking methodology and retrieval evaluation, with the author providing clarifications on the structural approach and baseline comparisons. Overall sentiment is positive, with interest in using the dataset for legal NLP tasks.

**Tags**: `#RAG`, `#legal NLP`, `#EU AI Act`, `#embeddings`, `#open dataset`

---

<a id="item-7"></a>
## [Zilog Z80 Microprocessor Celebrates 50th Anniversary](https://goliath32.com/blog/z80.html) ⭐️ 7.0/10

The Zilog Z80 microprocessor marks its 50th anniversary, with the community sharing nostalgic stories of learning assembly and digital electronics on this iconic chip. The Z80's longevity and influence on personal computing and embedded systems make this anniversary a significant milestone in computing history, highlighting its role in educating generations of programmers and engineers. The Z80 is fully binary compatible with the Intel 8080 but differs in flag register behavior for some operations, and it repurposed undefined opcodes for new instructions.

hackernews · st_goliath · Jul 17, 19:41 · [Discussion](https://news.ycombinator.com/item?id=48951461)

**Background**: Introduced in 1976, the Z80 was an 8-bit microprocessor widely used in home computers like the TRS-80 and ZX Spectrum, as well as in embedded systems. Its instruction set was a superset of the Intel 8080, making it easy to adopt while offering additional features.

**Discussion**: Community members shared personal stories of learning assembly on Z80-based systems like the TRS-80 and ZX-81, with one user recalling using a logic probe and oscilloscope to understand digital electronics. Another noted the binary compatibility nuance regarding the flag register.

**Tags**: `#Z80`, `#microprocessor`, `#history`, `#retrocomputing`, `#assembly`

---

<a id="item-8"></a>
## [Recurse Center Founder Thanks HN for 15 Years of Support](https://news.ycombinator.com/item?id=48949551) ⭐️ 7.0/10

The founder of the Recurse Center published a thank-you post on Hacker News on the eve of the program's 15th anniversary, recounting how an initial HN launch helped the retreat grow from a failed startup idea to a community that has positively impacted over 3,000 programmers. This milestone highlights the enduring value of community-driven, self-directed programming education and the role of platforms like Hacker News in nurturing non-traditional tech initiatives. It also underscores that meaningful impact does not always require a billion-dollar business model. The Recurse Center started as a failed Y Combinator startup called 'OkCupid for jobs' before pivoting to a free, self-directed programming retreat. Paul Graham's comment on the original HN launch post noted the venture might not be a billion-dollar business but was a benevolent thing to do.

hackernews · nicholasjbs · Jul 17, 16:57

**Background**: The Recurse Center (formerly Hacker School) is a nonprofit, self-directed educational retreat for programmers in New York City, where participants work on personal projects without formal instructors or curriculum. Hacker News is a social news website run by Y Combinator, focusing on computer science and entrepreneurship, and has been a key source of applicants for the Recurse Center.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Recurse_Center">Recurse Center</a></li>
<li><a href="https://en.wikipedia.org/wiki/Hacker_News">Hacker News</a></li>

</ul>
</details>

**Discussion**: The community comments express gratitude and admiration, with alumni sharing positive experiences and others expressing interest in attending. One commenter noted that most HN alumni don't last a decade, making this milestone particularly noteworthy.

**Tags**: `#Recurse Center`, `#Hacker News`, `#programming education`, `#community`, `#milestone`

---

<a id="item-9"></a>
## [Practical Tips for Running SQLite](https://jvns.ca/blog/2026/07/17/learning-about-running-sqlite/) ⭐️ 7.0/10

A blog post by Julia Evans collects practical tips for running SQLite, including using the .expert mode for index recommendations and various backup strategies. These tips help developers optimize SQLite performance and ensure data safety, addressing common pain points like slow queries and backup complexity. The .expert mode analyzes queries and recommends indexes, while backup strategies include using .dump with compression and tools like s3-credentials for cloud backups.

hackernews · surprisetalk · Jul 17, 17:45 · [Discussion](https://news.ycombinator.com/item?id=48950122)

**Background**: SQLite is a lightweight, embedded database engine widely used in applications. The .expert command in the SQLite CLI helps users identify missing indexes by simulating query plans. Backing up SQLite databases can be tricky due to locking and file consistency requirements.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48950122">Learning a few things about running SQLite | Hacker News</a></li>
<li><a href="https://sqlite.org/cli.html">Command Line Shell For SQLite</a></li>

</ul>
</details>

**Discussion**: Community comments highlight real-world experiences: one user shares a backup script using .dump with zstd compression, another built a tool (s3-credentials) to simplify AWS credential generation for backups. There is also discussion about DELETE batching and the sqlite_stat tables for query planning.

**Tags**: `#SQLite`, `#database`, `#backup`, `#optimization`

---

<a id="item-10"></a>
## [Frame: Linux X Server Written in Assembly via Claude](https://isene.org/2026/07/Frame.html) ⭐️ 6.0/10

Developer Geir Isene announced Frame, a Linux X server written entirely in x86_64 assembly, totaling about 25,000 lines of code, which was generated using the AI assistant Claude. This project challenges the notion that X11 is too complex to reimplement, and it sparks debate about the role of AI in software development, especially for low-level systems programming. Frame is part of a larger project called CHasm, which includes a window manager, terminal, shell, and screen greeter, all written in assembly and totaling around 100,000 lines. The author claims it runs a live environment, but community members report issues with window focus.

hackernews · guybedo · Jul 17, 15:31 · [Discussion](https://news.ycombinator.com/item?id=48948597)

**Background**: The X Window System (X11) is a network-transparent display protocol widely used on Unix-like systems. An X server manages graphical displays and input devices. Writing an X server from scratch is a significant undertaking due to the protocol's complexity; most implementations are based on the reference implementation from X.Org.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theregister.com/software/2026/07/14/frame-a-new-x11-server-implemented-directly-in-assembly/5270498">Frame: A new X11 server – implemented directly in assembly</a></li>
<li><a href="https://www.phoronix.com/news/Frame-X11-Server-Assembly">Frame: A New X11 Server Implementation Written Entirely In ...</a></li>
<li><a href="https://daily.dev/posts/frame---the-first-linux-assembly-x-server-efi34gznu">Frame - the first Linux Assembly X server - daily.dev</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some admire the technical curiosity, while others express disappointment that the code was AI-generated rather than manually written. One commenter noted that using an LLM as a compiler to produce assembly is an interesting approach, while another questioned the authenticity of the project.

**Tags**: `#X11`, `#assembly`, `#AI-generated code`, `#Linux`, `#Hacker News`

---

<a id="item-11"></a>
## [Real-Time SSH Honeypot Visualization](https://honeypotlive.cc/) ⭐️ 6.0/10

A new website, honeypotlive.cc, displays real-time interactions of bots and attackers with an SSH honeypot, showing commands and patterns as they happen. This project provides a live glimpse into the constant background noise on public IPs, helping security enthusiasts and researchers understand automated attack patterns. The honeypot captures SSH login attempts and commands, but some users have abused the web interface by spamming large text, obscuring real bot activity.

hackernews · tusksm · Jul 17, 14:05 · [Discussion](https://news.ycombinator.com/item?id=48947548)

**Background**: An SSH honeypot is a decoy server that mimics a real SSH service to log malicious activity. Bots continuously scan public IPs for open SSH ports and attempt to log in with common credentials or exploit vulnerabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://cheese-hub.github.io/network-security/04-ssh-honeypot/index.html">Network Security: SSH Honeypot</a></li>
<li><a href="https://github.com/droberson/ssh-honeypot">GitHub - droberson/ ssh - honeypot : Fake sshd that logs ip addresses...</a></li>
<li><a href="https://maketecheasier.com/create-ssh-honeypot-linux-server/">How to Create an SSH Honeypot to Catch... - Make Tech Easier</a></li>

</ul>
</details>

**Discussion**: Commenters found the project fun but noted spam abuse and limited insight; some suggested improvements like using LLMs for more realistic responses.

**Tags**: `#honeypot`, `#SSH`, `#security`, `#visualization`

---

<a id="item-12"></a>
## [Three Non-Solution Responses to Problems](https://improvesomething.today/responses-to-problems/) ⭐️ 6.0/10

The article identifies three common responses to problems besides solving them: ignoring, preserving, and redefining the problem. Understanding these responses helps individuals and organizations recognize counterproductive behaviors and improve problem-solving effectiveness. The 'preserving the problem' response occurs when stakeholders benefit from the problem's existence, such as budget or power retention.

hackernews · surprisetalk · Jul 17, 14:00 · [Discussion](https://news.ycombinator.com/item?id=48947490)

**Background**: Problem-solving is often assumed to be the default response to issues, but in reality, people may avoid solving problems for various reasons. This article categorizes those alternative responses into three types, offering a framework for analysis.

**Discussion**: Commenters shared real-world examples, noting that ignoring trivial problems can be efficient, while preserving problems is common in government and organizations where solving them would reduce budgets or power.

**Tags**: `#problem-solving`, `#psychology`, `#management`, `#organizational-behavior`

---

<a id="item-13"></a>
## [LLM Cliché Highlighter Tool](https://simonwillison.net/2026/Jul/17/llm-cliche-highlighter/#atom-everything) ⭐️ 6.0/10

Simon Willison introduced a web app called LLM cliché highlighter that highlights ten common clichés found in LLM-generated writing, such as "no fluff, no filler, no jargon." This tool helps readers quickly identify AI-generated text, addressing a growing annoyance with formulaic LLM writing. It also serves as a practical utility for writers and editors to refine AI-assisted content. The app was created using "vibe coding" with Fable 5, meaning the developer described the project in a prompt and the AI generated the code. It highlights patterns like "delve into," "game-changer," and "in today's digital landscape."

rss · Simon Willison · Jul 17, 12:11

**Background**: Large language models (LLMs) like GPT-4 often produce text with distinctive clichés and repetitive phrasing. "Vibe coding" is a term coined by Andrej Karpathy in 2025, referring to AI-assisted programming where the developer describes the goal and accepts generated code without thorough review.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vibe_coding">Vibe coding</a></li>
<li><a href="https://github.com/nanxstats/llm-cliches">GitHub - nanxstats/llm-cliches: A curated collection of commonly used clichés and phrases in Large Language Models outputs · GitHub</a></li>

</ul>
</details>

**Tags**: `#llm`, `#tools`, `#ai`, `#writing`

---

<a id="item-14"></a>
## [Convert golf courses to offset data center water use](https://simonwillison.net/2026/Jul/17/spot-birds-not-golf/#atom-everything) ⭐️ 4.0/10

A blog post suggests hyperscalers like Google could offset their data center water consumption by buying and converting golf courses into public parks, promoting birdwatching as a sustainable hobby. The post calculates that Google's 2025 water use of 10.9 billion gallons could be offset by acquiring about 40 of the 120 golf courses in California's Coachella Valley. This creative proposal highlights the growing environmental pressure on hyperscale data centers, especially regarding water usage for cooling AI workloads. While not a serious policy suggestion, it sparks discussion on unconventional sustainability offsets and the scale of water consumption by tech giants. Google used 10.9 billion gallons of water in 2025, about 30 million gallons per day. The Coachella Valley has 120 golf courses, each using roughly 800 acre-feet per year (~750,000 gallons per day), so acquiring 40 courses would offset Google's usage.

rss · Simon Willison · Jul 17, 02:58

**Background**: Data centers, especially hyperscale ones, require vast amounts of water for cooling, with a single facility consuming up to 5 million gallons per day. Water usage effectiveness (WUE) is a key metric, and regulators are increasingly scrutinizing water consumption. An acre-foot is a US unit of water volume equal to about 325,851 gallons, commonly used for large-scale water measurement.

<details><summary>References</summary>
<ul>
<li><a href="https://kovastack.ai/blog/datacenter-water-usage-how-much-water-hyperscalers-use-2026">Datacenter Water Usage 2026: How Much Water Hyperscalers ...</a></li>
<li><a href="https://insights.aecom.com/insights/article/why-hyperscalers-are-putting-water-at-the-heart-of-data-center-growth-plans">Why hyperscalers are putting water at the heart of data ...</a></li>
<li><a href="https://www.coloradoriverdistrict.org/water-measurement/">Water Measurement - Basic Units of Water | Colorado River District</a></li>

</ul>
</details>

**Tags**: `#data centers`, `#water usage`, `#sustainability`, `#AI energy`

---

<a id="item-15"></a>
## [User Seeks Experiences on Short Paper Acceptance at Top NLP Conferences](https://www.reddit.com/r/MachineLearning/comments/1uz8w8q/shortpaper_at_aclemnlpeacl_r/) ⭐️ 3.0/10

A Reddit user posted a query asking for experiences and acceptance rates of short papers at ACL, EMNLP, and EACL conferences in 2025/2026, noting that short papers appear to have lower acceptance rates than long papers. This query highlights a common concern among NLP researchers about the competitiveness of short paper submissions, which may influence submission strategies and resource allocation. The user specifically asks about tracks and overall assessments, indicating a need for practical insights beyond official statistics.

reddit · r/MachineLearning · /u/No_Cardiologist7609 · Jul 17, 19:02

**Background**: ACL, EMNLP, and EACL are top-tier conferences in natural language processing. Short papers typically present preliminary results or smaller contributions, and their acceptance rates can vary significantly from long papers.

**Tags**: `#NLP`, `#conferences`, `#ACL`, `#EMNLP`, `#EACL`

---

<a id="item-16"></a>
## [BMVC Rebuttal Deadline: Modified Review Timestamps Raise Questions](https://www.reddit.com/r/MachineLearning/comments/1uz7hbu/bmvc_rebuttals_update_d/) ⭐️ 3.0/10

A Reddit user reports that some BMVC reviews show modification timestamps after the July 11 rebuttal deadline, suggesting reviewers may have updated scores after the rebuttal period ended. This raises concerns about the fairness and integrity of the BMVC review process, as late modifications could affect final decisions without authors having a chance to respond. The rebuttal access opened to reviewers on July 11 at 19:05 UTC; any review modified after that time may indicate a score update hidden from authors. The post asks how many reviews show modification timestamps past that deadline.

reddit · r/MachineLearning · /u/Forsaken_Cold6708 · Jul 17, 18:11

**Background**: BMVC (British Machine Vision Conference) is a major computer vision conference. The rebuttal phase allows authors to respond to initial reviews, after which reviewers may adjust scores. Fixed deadlines are typically enforced to ensure fairness.

<details><summary>References</summary>
<ul>
<li><a href="https://bmvc2026.bmva.org/authors/reviewing-guidelines/">Reviewing Guidelines - BMVC 2026</a></li>

</ul>
</details>

**Tags**: `#BMVC`, `#conference`, `#rebuttal`, `#review`

---