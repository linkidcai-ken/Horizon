---
layout: default
title: "Horizon Summary: 2026-08-24 (EN)"
date: 2026-08-24
lang: en
---

> From 22 items, 18 important content pieces were selected

---

1. [MS Paint and Photos Embed Invisible GUID Watermarks in AI-Edited Images](#item-1) ⭐️ 8.0/10
2. [IPFS Shipyard Maintainer Team Sunsets, Project Continues](#item-2) ⭐️ 8.0/10
3. [SQLite Database as Executable: A Clever Linux Hack](#item-3) ⭐️ 8.0/10
4. [LLMs as Spatial Software Generators for Programmable 3D Objects](#item-4) ⭐️ 8.0/10
5. [Xiaomi Xring O3 CPU Matches Apple Single-Core, Beats Multi-Core](#item-5) ⭐️ 7.0/10
6. [San Francisco Recreated as Playable Web Game](#item-6) ⭐️ 7.0/10
7. [EU Regulations Threaten Makers and Micro-Entrepreneurs](#item-7) ⭐️ 7.0/10
8. [Oceans Hit Record High Temperatures, Signaling Accelerating Climate Change](#item-8) ⭐️ 7.0/10
9. [XMPP Turns 25: A Look Back at Digital Independence](#item-9) ⭐️ 7.0/10
10. [OpenAI Cuts GPT-5.6 Sol Prices Temporarily](#item-10) ⭐️ 7.0/10
11. [Unbounded Labs Unveils Bart, a Vintage LLM Trained on Pre-1931 English](#item-11) ⭐️ 7.0/10
12. [Delay-Corrected Bellman Operator for Constrained RL Under Stochastic Delay](#item-12) ⭐️ 7.0/10
13. [AAAI 2027 Acknowledges Collusion in Reviewer Assignments](#item-13) ⭐️ 6.0/10
14. [Hyperparameter Unification in MARL Comparative Studies](#item-14) ⭐️ 6.0/10
15. [llm-anthropic 0.27 Adds Compatibility with Anthropic SDK v1.0.0](#item-15) ⭐️ 5.0/10
16. [EMNLP Author Questions Missing Meta-Review After Rejection](#item-16) ⭐️ 4.0/10
17. [BMVC 2026 IJCV Recommendation Process Questioned](#item-17) ⭐️ 3.0/10
18. [Does Abstract Registration Count as Double Submission?](#item-18) ⭐️ 3.0/10

---

<a id="item-1"></a>
## [MS Paint and Photos Embed Invisible GUID Watermarks in AI-Edited Images](https://xusheng.dev/posts/reversing/mspaint_invisible_watermark/main/) ⭐️ 8.0/10

Microsoft Paint and Photos now silently embed an invisible GUID watermark into images that have been AI-manipulated, even when the AI processing is performed locally on Copilot+ PCs. This watermark is embedded without user notification and cannot be disabled. This raises significant privacy and anonymity concerns, as the invisible watermark can be used to trace an image back to the user's Microsoft account, potentially exposing personal information. It also highlights a broader trend of invisible watermarking in AI-generated content, which could impact user trust and content authenticity. The watermark is a GUID issued by Microsoft servers, embedded into the image data even when generation is local. It is unclear if the watermark applies to all AI manipulations, such as background removal, but it is invisible and cannot be turned off.

hackernews · ComputerGuru · Aug 24, 15:28 · [Discussion](https://news.ycombinator.com/item?id=49421158)

**Background**: Invisible watermarking is a technique that embeds imperceptible data into digital media to verify origin or authenticity. Microsoft's implementation uses a GUID, which is a unique identifier that can be linked to a user's account, raising concerns about tracking and anonymity.

<details><summary>References</summary>
<ul>
<li><a href="https://xusheng.dev/posts/reversing/mspaint_invisible_watermark/main/">Microsoft Paint and Photos Embed Server-Issued GUIDs ... :: Xusheng Li</a></li>
<li><a href="https://www.imatag.com/digital-watermarking">Invisible Digital Watermarking | The smart way to protect ... The Hidden Mark: How Invisible Watermarking is Quietly ... AIWatermark℠ — Invisible and Visible Watermarking, Verified How Good Are Invisible Watermarks Now? - Medium Ultimate Guide to Invisible Watermarking Algorithms How Invisible Watermarking Works | ScoreDetect Blog Anthropic's new invisible watermark marks content generated ...</a></li>
<li><a href="https://www.techmagazines.net/the-hidden-mark-how-invisible-watermarking-is-quietly-securing-the-digital-world/">The Hidden Mark: How Invisible Watermarking is Quietly ...</a></li>

</ul>
</details>

**Discussion**: Community comments express shock and concern, with some noting that the AI aspect is a red herring and the real issue is the secret embedding of unique identifiers. Others point out potential misuse, such as copyright subpoenas, and recall past incidents where Microsoft incorrectly applied watermarks, suggesting caution in using such apps.

**Tags**: `#privacy`, `#watermarking`, `#Microsoft`, `#AI`, `#security`

---

<a id="item-2"></a>
## [IPFS Shipyard Maintainer Team Sunsets, Project Continues](https://ipshipyard.com/blog/2026-the-end-of-ipfs-at-shipyard/) ⭐️ 8.0/10

IPFS Shipyard, a major maintainer team for IPFS implementations, announced it is winding down operations, with projects like Kubo, Helia, and IPFS Desktop losing dedicated maintainers. The IPFS project itself is not shutting down but will transition to individual maintainer grants. This marks a significant shift in IPFS governance and maintenance, potentially slowing development and support for key implementations. It highlights the challenges of sustaining open-source infrastructure and may push users toward alternative p2p solutions. Affected projects include Kubo, Helia, Boxo, Rainbow, IPFS Desktop, IPFS Companion, Someguy, Service Worker Gateway, and IPFS Check. The IPFS Implementations Grants program, established in 2022, will provide individual maintainer grants to continue development.

hackernews · iand · Aug 24, 15:48 · [Discussion](https://news.ycombinator.com/item?id=49421489)

**Background**: IPFS (InterPlanetary File System) is a decentralized peer-to-peer protocol for storing and sharing files. Shipyard was a team within Protocol Labs that maintained several IPFS implementations. The transition to individual grants reflects a broader trend in open-source funding, moving away from centralized team support.

<details><summary>References</summary>
<ul>
<li><a href="https://ipshipyard.com/blog/2026-the-end-of-ipfs-at-shipyard/">The end of IPFS at Shipyard</a></li>
<li><a href="https://ipfsgrants.io/utility-grants/">IPFS Implementation Fund</a></li>
<li><a href="https://news.ycombinator.com/item?id=49421489">IPFS Maintainers Winding Down | Hacker News</a></li>

</ul>
</details>

**Discussion**: Community members clarified that only Shipyard is sunsetting, not the entire IPFS project, and expressed mixed feelings. Some suggested alternatives like Iroh, while others criticized the project's direction and the irony of using Google Forms for feedback.

**Tags**: `#IPFS`, `#decentralization`, `#open source`, `#maintenance`, `#p2p`

---

<a id="item-3"></a>
## [SQLite Database as Executable: A Clever Linux Hack](https://simonwillison.net/2026/Aug/24/your-executable-is-a-sqlite-database/) ⭐️ 8.0/10

Farid Zakaria has developed a technique that allows a SQLite database file to be executed directly as a Linux binary. This is achieved by setting the SQLite application ID to 'SELF' and storing ELF components in SQLite tables, with a custom interpreter 'self-exec' to run them. This innovation could simplify executable packaging and data embedding, allowing a single file to serve both as a database and a runnable program. It opens up new possibilities for self-contained applications and could influence how developers think about file formats and executable distribution. The technique uses the SQLite file format's 4-byte application ID at offset 68, setting it to 'SELF' (Structured Executable & Linkable Format). The ELF components are arranged into SQLite tables according to a schema, and the 'self-exec' interpreter extracts and executes them. Additionally, the Linux kernel's binfmt_misc mechanism can be configured to automatically invoke the interpreter for files matching the pattern.

rss · Simon Willison · Aug 24, 11:38

**Background**: SQLite is a widely-used embedded database that stores data in a single file, with a header that includes an application ID field. ELF (Executable and Linkable Format) is the standard binary format for executables on Linux and Unix-like systems, consisting of headers, sections, and segments. binfmt_misc is a Linux kernel feature that allows custom binary formats to be executed by associating them with user-space interpreters.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Executable_and_Linkable_Format">Executable and Linkable Format - Wikipedia</a></li>
<li><a href="https://sqlite.org/forum/info/6a768e7dca11a7b2">SQLite User Forum: Usage of application_id and magic.txt</a></li>
<li><a href="https://docs.kernel.org/admin-guide/binfmt-misc.html">Kernel Support for miscellaneous Binary Formats (binfmt_misc)</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion likely praised the cleverness of the hack and its potential applications, with some users possibly discussing the trade-offs in terms of performance and complexity. There might be debates about the practicality of using SQLite as an executable format versus traditional approaches.

**Tags**: `#SQLite`, `#ELF`, `#Linux`, `#executable`, `#binfmt_misc`

---

<a id="item-4"></a>
## [LLMs as Spatial Software Generators for Programmable 3D Objects](https://www.reddit.com/r/MachineLearning/comments/1vxcc1h/r_using_ai_as_a_spatial_software_generator_to/) ⭐️ 8.0/10

A new paper proposes using large language models (LLMs) as spatial software generators to create 3D objects that are inherently programmable, with visual demos and code available at nova3d.xyz. This approach could revolutionize 3D content creation by making objects animation-ready and adaptable from inception, potentially disrupting industries like game development, industrial design, and AR/VR/XR. The generated 3D objects are composed of logical parts with hierarchical structure and hinge/socket articulation, allowing them to adapt to different compute environments. However, the method currently lags behind traditional AI 3D generators for complex organic shapes.

reddit · r/MachineLearning · /u/mhb_11 · Aug 24, 19:10

**Background**: Traditional AI 3D generators typically produce monolithic mesh blobs that are difficult to animate or modify. Spatial programming involves describing 3D objects as code, enabling procedural generation and logical structure. LLMs are increasingly capable of generating such code, making this approach feasible.

<details><summary>References</summary>
<ul>
<li><a href="https://pyspatial.github.io/">pySpatial: Generating 3D Visual Programs for Zero-Shot ...</a></li>
<li><a href="https://arxiv.org/html/2603.00905">pySpatial: Generating 3D Visual Programs for Zero-Shot ...</a></li>

</ul>
</details>

**Tags**: `#3D generation`, `#LLM`, `#spatial programming`, `#AI research`, `#procedural generation`

---

<a id="item-5"></a>
## [Xiaomi Xring O3 CPU Matches Apple Single-Core, Beats Multi-Core](https://twitter.com/lemire/status/2091894299289874926) ⭐️ 7.0/10

Xiaomi's new Xring O3 chip reportedly matches Apple's single-core performance and surpasses it in multi-core benchmarks, based on Geekbench scores. The chip uses a 10-core all-big-core design on a 3nm process. This marks a significant milestone for Xiaomi, potentially disrupting the mobile chip market dominated by Qualcomm and MediaTek. It could pressure competitors and offer consumers more high-performance options, though power efficiency remains a critical factor. The Xring O3 achieves a Geekbench single-core score of 3,945 and multi-core score of 15,221, compared to Apple's M5 iPad scores of 3,556 and 15,285 respectively. However, power consumption metrics were not disclosed, and the comparison is against Apple's previous-generation chips.

hackernews · tosh · Aug 24, 15:08 · [Discussion](https://news.ycombinator.com/item?id=49420873)

**Background**: Mobile chip performance is typically measured by benchmarks like Geekbench, which test single-core and multi-core capabilities. Power efficiency is crucial for smartphones due to thermal and battery constraints. Xiaomi's entry into chip design could reduce its reliance on third-party suppliers.

<details><summary>References</summary>
<ul>
<li><a href="https://wazzuptechph.com/xiaomi-xring-o3-o100-d100-announced-first-devices-launch-september-2026/">Xiaomi Xring O3, O100, D100 Announced, First Devices Launch...</a></li>
<li><a href="https://mynexttablet.com/xiaomi-15-review/">Xiaomi 15 Review: 3 Weeks Against iPhone 16 Pro & S25 Ultra...</a></li>
<li><a href="https://wccftech.com/xiaomi-mi5s-specs-leaked/">Xiaomi Mi5s Specifications Apparently Leaked: Powerful SoC and...</a></li>

</ul>
</details>

**Discussion**: Commenters noted that power efficiency is the missing metric, as high performance without efficiency is impractical in phones. Some pointed out that the comparison is against Apple's older chips and that the multi-core advantage comes from having 10 cores vs 6. Others saw it as a positive step for Xiaomi, potentially threatening MediaTek and Qualcomm.

**Tags**: `#CPU`, `#Xiaomi`, `#Apple`, `#mobile chips`, `#performance`

---

<a id="item-6"></a>
## [San Francisco Recreated as Playable Web Game](https://sf.thijs.gg/) ⭐️ 7.0/10

A web-based project at sf.thijs.gg recreates the entire city of San Francisco as a playable 3D video game, built on GIS data. The project was shared on Twitter and quickly gained traction in the community. This project demonstrates the growing accessibility of GIS-based game development, allowing individuals to create immersive, real-world environments. It highlights the potential for personal and emotional connections to virtual recreations of familiar places, and could inspire similar projects for other cities. The game is accessible via a web browser and uses GIS data to model the city's terrain, buildings, and streets. The project is still in an early stage, with the creator noting that it is a work in progress and may lack some features like realistic physics.

hackernews · centrosphere · Aug 24, 17:05 · [Discussion](https://news.ycombinator.com/item?id=49422784)

**Background**: GIS (Geographic Information System) data is increasingly used in game development to create realistic virtual environments. Tools like ArcGIS provide SDKs for game engines such as Unity and Unreal, enabling developers to integrate real-world geospatial data into their projects. This project leverages similar techniques but runs entirely in the browser, making it easily accessible.

<details><summary>References</summary>
<ul>
<li><a href="https://doc.arcgis.com/en/3d/workflows/immersive-experiences/access-3d-layers-in-game-engines.htm">Use GIS data in game engines—3D Workflows | Documentation</a></li>
<li><a href="https://www.esri.com/about/newsroom/arcuser/building-video-games-with-arcgis-technology">Building Video Games with ArcGIS Technology</a></li>
<li><a href="https://github.com/lo-th/3d.city">GitHub - lo-th/3d.city: 3d city builder game · GitHub</a></li>

</ul>
</details>

**Discussion**: Community comments show a mix of emotional reactions and technical interest. One user who lived in SF for 20 years found it emotional to explore familiar places, while others discussed the potential for building similar pipelines using GIS data and streetview imagery. Some also noted the lack of realistic physics and questioned the inclusion of Apple copyright notices.

**Tags**: `#GIS`, `#game development`, `#San Francisco`, `#web`, `#3D rendering`

---

<a id="item-7"></a>
## [EU Regulations Threaten Makers and Micro-Entrepreneurs](https://lectronz.com/u/lectronz/articles/how-europe-is-killing-makers-and-micro-entrepreneurs) ⭐️ 7.0/10

An article argues that recent EU regulations, such as packaging and labeling requirements, are disproportionately harming small-scale makers and micro-entrepreneurs, potentially forcing many out of business. The piece has sparked a large discussion on Hacker News, with many commenters offering counterpoints and clarifications. This matters because the EU's regulatory framework, while aiming to protect consumers and the environment, may inadvertently stifle innovation and small business growth. The outcome could affect the livelihoods of countless micro-entrepreneurs and the diversity of products available in the EU market. The article appears to focus on the EU's Packaging and Packaging Waste Regulation (PPWR) and related rules, which impose new labeling and reporting obligations. Commenters note that micro-enterprises are often exempt or that the rules are not yet enforced, and that the author may have misrepresented the scope.

hackernews · l-one-lone · Aug 24, 13:05 · [Discussion](https://news.ycombinator.com/item?id=49419237)

**Background**: The EU has been updating regulations on packaging, waste, and product safety to promote sustainability and circular economy. These rules often apply to all businesses selling into the EU, but they can be particularly burdensome for small-scale producers who lack resources for compliance. The discussion highlights the complexity of EU law, which is implemented differently across member states.

**Discussion**: The community discussion is largely critical of the article's claims. Some commenters point out that micro-enterprises are exempt from many rules, while others note that the EU is advising member states not to enforce certain provisions until corrections are made. There is also debate about the role of member states versus the EU in creating bureaucratic hurdles.

**Tags**: `#EU regulation`, `#makers`, `#micro-entrepreneurs`, `#e-commerce`, `#policy`

---

<a id="item-8"></a>
## [Oceans Hit Record High Temperatures, Signaling Accelerating Climate Change](https://www.bbc.com/news/articles/c62m4gpnp78o) ⭐️ 7.0/10

Oceans have reached their highest recorded temperature, according to a recent report, highlighting the accelerating impact of climate change on marine environments. This milestone underscores the urgency of climate action, as warmer oceans intensify extreme weather, threaten marine ecosystems, and contribute to sea-level rise, affecting billions of people worldwide. The record was set in early 2025, with average sea surface temperatures surpassing previous highs. Scientists note that El Niño conditions and reduced ice cover are contributing factors, and further warming is expected as the year progresses.

hackernews · tcp_handshaker · Aug 24, 19:19 · [Discussion](https://news.ycombinator.com/item?id=49424606)

**Background**: Ocean temperatures are a critical indicator of global warming because oceans absorb over 90% of the excess heat from greenhouse gas emissions. Warmer oceans can lead to coral bleaching, stronger hurricanes, and altered marine food chains. The record highlights the ongoing trend of rising ocean heat content, which has been observed for decades.

**Discussion**: Commenters expressed concern about government inaction and the worsening climate crisis, with some sharing educational resources and personal reflections on the severity of a few degrees of warming. One commenter noted that reduced ice cover allows more incident energy to heat the ocean, while another pointed out that the record may be broken again as El Niño peaks.

**Tags**: `#climate change`, `#ocean temperature`, `#environment`, `#science`, `#policy`

---

<a id="item-9"></a>
## [XMPP Turns 25: A Look Back at Digital Independence](https://gultsch.de/posts/25-years-of-digital-independence/) ⭐️ 7.0/10

The article marks the 25th anniversary of XMPP (Jabber), reflecting on its legacy and role in digital independence, while sparking a renewed debate comparing it with Matrix. This milestone highlights XMPP's enduring relevance in the decentralized messaging landscape, offering a mature, open alternative to proprietary platforms. The ongoing comparison with Matrix underscores key architectural and philosophical differences that influence developer and community choices. XMPP is an XML-based protocol originally named Jabber, standardized by the IETF and maintained by the XMPP Standards Foundation (XSF). The article and community discussion note that while Matrix offers native end-to-end encryption and bridges many protocols, XMPP excels in server efficiency and EU DMA compliance.

hackernews · inputmice · Aug 24, 15:51 · [Discussion](https://news.ycombinator.com/item?id=49421536)

**Background**: XMPP (Extensible Messaging and Presence Protocol) is an open communication protocol for instant messaging, presence, and contact list maintenance, based on XML. It was created by Jeremie Miller in 1999 and has been used by major services like Google Talk and Facebook, with over 500 million users at its peak. Matrix is a newer decentralized protocol that focuses on seamless federation and end-to-end encryption, but it has been criticized for higher resource usage and potential vendor lock-in.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/XMPP">XMPP - Wikipedia</a></li>
<li><a href="https://www.process-one.net/blog/xmpp-matrix/">Understanding messaging protocols: XMPP and Matrix - ProcessOne Matrix vs XMPP: Pick the Right Messaging Standard IRC vs. Matrix vs. XMPP | Johannes Findeisen - hanez.org Matrix vs. XMPP - What's the Difference? | This vs. That Matrix vs. XMPP | Luke Smith Matrix vs XMPP: Self-Hosted Chat 2026 - Vucense XMPP vs Matrix vs MQTT: which instant messaging protocol is ...</a></li>
<li><a href="https://snapmessages.com/matrix-protocol-vs-xmpp-open-messaging-standard-comparison/">Matrix vs XMPP: Pick the Right Messaging Standard</a></li>

</ul>
</details>

**Discussion**: Community comments express nostalgia for XMPP's past integration with major platforms and hope for its future with projects like Movim and Fluux. Some users praise XMPP's simplicity and efficiency, while others note the lack of a client that matches Telegram's polish, and question whether large communities still use it.

**Tags**: `#XMPP`, `#Jabber`, `#Matrix`, `#decentralization`, `#messaging`

---

<a id="item-10"></a>
## [OpenAI Cuts GPT-5.6 Sol Prices Temporarily](https://developers.openai.com/api/docs/pricing) ⭐️ 7.0/10

OpenAI has announced temporary price reductions for its GPT-5.6 model family, including a 20% cut for input and a 33% cut for output on the Sol tier, effective until at least November 21, 2026. The new pricing for Sol is $4.00 per million input tokens and $20.00 per million output tokens. This price cut intensifies competition in the AI model market, making GPT-5.6 Sol more attractive compared to offerings from Anthropic and other providers. It reflects a broader trend of AI commoditization, where raw model performance becomes less of a differentiator and price becomes a key competitive factor. The revised pricing schedule shows Sol at $4.00 input, $0.40 cached input, $5.00 cache writes, and $20.00 output per million tokens. Terra and Luna also received price cuts, with Luna now 80% cheaper than before, and Sol remains 20x more expensive than Luna.

hackernews · tosh · Aug 24, 15:22 · [Discussion](https://news.ycombinator.com/item?id=49421074)

**Background**: GPT-5.6 is OpenAI's latest model family, launched in July 2026, with three tiers: Sol (flagship), Terra (balanced), and Luna (fastest and most affordable). OpenAI has been adjusting prices to stay competitive as open-source models and rivals like Anthropic challenge its market position. The concept of AI commoditization refers to the trend where frontier models from different providers achieve similar capabilities, making price and efficiency more important.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/advancing-the-price-performance-frontier-with-gpt-5-6/">Advancing the price-performance frontier with GPT-5.6 | OpenAI</a></li>
<li><a href="https://openai.com/index/gpt-5-6/">GPT-5.6: Frontier intelligence that scales with your ambition | OpenAI</a></li>
<li><a href="https://www.eesel.ai/blog/gpt-5-6-pricing">GPT-5.6 pricing (2026): Sol, Terra and Luna rates explained | eesel AI</a></li>

</ul>
</details>

**Discussion**: Community members generally welcome the price war, with one user praising the affordability and another noting that open-source models benefit from this competition. Some users point out that the discount is still not enough compared to other providers, and there are requests for tools to visualize live pricing. A few express skepticism about AI alignment and the long-term implications of commoditization.

**Tags**: `#OpenAI`, `#pricing`, `#AI models`, `#GPT-5.6`, `#competition`

---

<a id="item-11"></a>
## [Unbounded Labs Unveils Bart, a Vintage LLM Trained on Pre-1931 English](https://www.reddit.com/r/MachineLearning/comments/1vx94er/bart_a_vintage_llm_r/) ⭐️ 7.0/10

Unbounded Labs has introduced Bart, a 2.82B parameter LLM trained from scratch on 20.1B tokens of English text written before 1931. The project includes a demo, a detailed article, and an open-sourced HuggingFace model, along with new benchmarks and datasets. This project directly tests Demis Hassabis's hypothesis that LLMs could rediscover historical scientific insights, potentially advancing AI research on creativity and original thinking. It also introduces new benchmarks and datasets for vintage LLMs, which could benefit the broader research community. Bart was trained on a cleaned subset of Harvard's Institutional Books, reducing the corpus from 242B to 23B tokens, and achieved state-of-the-art results on the new Vintage CORE benchmark suite. The team also released a 416k-pair SFT dataset and ran 100 autonomous experiments on a single H100, achieving 60% MFU during final training.

reddit · r/MachineLearning · /u/soggydoggy8 · Aug 24, 17:20

**Background**: Demis Hassabis, CEO of Google DeepMind, proposed that an LLM trained on data up to 1911 could independently discover general relativity, as a test for AGI. This project builds on that idea by training a model on pre-1931 English text to see if it can generate original ideas similar to historical scientists. The team also created new benchmarks because existing ones were not suitable for vintage LLMs.

<details><summary>References</summary>
<ul>
<li><a href="https://officechai.com/ai/someone-built-an-llm-to-test-out-demis-hassabis-agi-definition-of-pre-1900-science-discovering-relativity/">Someone Built An LLM To Test Out Demis Hassabis' AGI Definition Of Pre-1900 Science Discovering Relativity</a></li>
<li><a href="https://arxiv.org/html/2606.02991v1">Pretraining Language Models on Historical Text - arXiv.org</a></li>
<li><a href="https://medium.com/@gabi.preda/benchmarking-historical-reasoning-in-large-language-models-5cb9be996c3c">Benchmarking Historical Reasoning in Large Language Models | by Gabriel Preda | Medium</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#training from scratch`, `#historical text`, `#AI research`, `#benchmarks`

---

<a id="item-12"></a>
## [Delay-Corrected Bellman Operator for Constrained RL Under Stochastic Delay](https://www.reddit.com/r/MachineLearning/comments/1vx11hz/delaycorrected_bellman_operator_causal/) ⭐️ 7.0/10

The post introduces a delay-corrected Bellman operator that uses an adaptive effective discount learned from the consequence-delay distribution, with a contraction proof that holds under unknown stochastic delay. It also proposes an Interventional Consequence Net (ICN) for causal attribution, pretrained on structural causal model labels. This work addresses a critical limitation in constrained RL where delayed and stochastic consequences are misattributed to temporally proximate actions, which is common in real-world settings. By providing a theoretical contraction guarantee and a causal attribution method, it could improve the reliability and applicability of safe RL in domains like robotics, finance, and healthcare. The ICN currently requires access to the environment's structural causal model to generate pretraining labels, which limits its applicability outside benchmark settings where the SCM is known or can be specified. The approach separates reward and constraint Q-functions to avoid altering TD targets when multipliers change.

reddit · r/MachineLearning · /u/No_Cauliflower7923 · Aug 24, 12:11

**Background**: In reinforcement learning, the Bellman operator is a fundamental tool for iteratively updating value functions to find optimal policies. Standard constrained RL assumes consequences are immediate and attributable to the current action, but in many real-world scenarios, violations are delayed and stochastic, making attribution difficult. Structural causal models (SCMs) provide a framework for understanding causal relationships, which can be used to attribute consequences to actions more accurately. The delay-corrected Bellman operator and ICN aim to address these challenges.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bellman_equation">Bellman equation - Wikipedia</a></li>
<li><a href="https://www.baeldung.com/cs/bellman-operator-reinforcement-learning">What Is the Bellman Operator in Reinforcement Learning? | Baeldung on Computer Science</a></li>
<li><a href="https://medium.com/causality-in-data-science/structural-causal-models-a-quick-introduction-1ab49259e921">Structural Causal Models — A Quick Introduction - Medium Stanford Causal AI Lab Deep learning of causal structures in high dimensions under ... CausalMLBook | Applied Causal Inference Powered by ML and AI Causal Machine Learning: A Survey and Open Problems SLEM: Machine Learning for Path Modeling and Causal Inference ...</a></li>

</ul>
</details>

**Tags**: `#reinforcement learning`, `#constrained RL`, `#causal inference`, `#delayed feedback`, `#Bellman operator`

---

<a id="item-13"></a>
## [AAAI 2027 Acknowledges Collusion in Reviewer Assignments](https://www.reddit.com/r/MachineLearning/comments/1vwujcy/aaai_2027_reviewer_bidding_and_assignment/) ⭐️ 6.0/10

AAAI 2027 organizers sent an email acknowledging collusion in the review process, specifically mentioning 2-cycles where authors of two papers review each other's work. This marks a rare official admission by a major AI conference that such integrity issues exist. This acknowledgment highlights ongoing integrity challenges in AI conference peer review, which could undermine trust in published research. It may prompt other conferences to address collusion more transparently and encourage the community to demand better safeguards. The post notes that most submissions come from a single country, increasing the likelihood of natural 2-cycles among authors from that country, and suggests that most colluding authors may be from that country. The author also questions whether AAAI will release submission statistics as it did previously, and criticizes the lack of code availability for many accepted papers at top conferences.

reddit · r/MachineLearning · /u/Fragrant_Fan_6751 · Aug 24, 06:11

**Background**: Peer review is a cornerstone of academic publishing, where experts evaluate submissions for quality and validity. In computer science conferences like AAAI, papers are assigned to reviewers, but collusion—such as reciprocal reviewing—can compromise the process. The 2-cycle issue arises when two authors review each other's papers, potentially leading to biased or favorable reviews. Conferences use assignment algorithms to minimize such conflicts, but they are not always effective, especially when submissions are concentrated geographically.

<details><summary>References</summary>
<ul>
<li><a href="https://aaai.org/conference/aaai/aaai-27/">AAAI -27 - AAAI</a></li>
<li><a href="https://arxiv.org/html/2608.08486">Detecting Collusion in Peer Review : Drawing Inspiration from VCG...</a></li>
<li><a href="https://cacm.acm.org/opinion/collusion-rings-threaten-the-integrity-of-computer-science-research/">Collusion Rings Threaten the Integrity of Computer Science Research...</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion is not provided, but the post itself expresses concerns about the integrity of the review process and the lack of code availability for accepted papers. The author's tone suggests frustration and a desire for more transparency, which likely resonates with other researchers who have experienced similar issues.

**Tags**: `#AAAI`, `#peer review`, `#collusion`, `#conference integrity`, `#machine learning`

---

<a id="item-14"></a>
## [Hyperparameter Unification in MARL Comparative Studies](https://www.reddit.com/r/MachineLearning/comments/1vxfmms/hyperparameters_fine_tuning_for_marl_comparative/) ⭐️ 6.0/10

A researcher training PPO variants on VMAS tasks asks whether hyperparameters should be unified across architectures for fair comparison, noting that unified settings sometimes cause non-convergence. This question highlights a common methodological challenge in MARL benchmarking: balancing fairness with optimal performance. The answer affects how comparative studies are designed and interpreted, impacting the validity of conclusions about architecture effectiveness. The researcher uses Independent PPO and Graph PPO (e.g., HetGPPO) on VMAS scenarios, and observes that optimal hyperparameters (learning rate, entropy coefficient, KL coefficient, batch size) vary per architecture and scenario. They also plan to test robustness under adversarial attacks at test time.

reddit · r/MachineLearning · /u/ham_bam0 · Aug 24, 21:10

**Background**: In multi-agent reinforcement learning (MARL), comparative studies often compare different algorithms or architectures. Hyperparameters like learning rate and entropy coefficient can significantly affect performance, and there is an ongoing debate about whether to tune them per model or use a unified set for fairness. VMAS is a vectorized multi-agent simulator for benchmarking, and HetGPPO is a heterogeneous MARL framework using graph neural networks.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/proroklab/HetGPPO">GitHub - proroklab/HetGPPO: Heterogeneous Multi-Robot ...</a></li>
<li><a href="https://github.com/proroklab/VectorizedMultiAgentSimulator">GitHub - proroklab/VectorizedMultiAgentSimulator: VMAS is a ...</a></li>
<li><a href="https://arxiv.org/abs/2207.03530">[2207.03530] VMAS: A Vectorized Multi-Agent Simulator for ... VectorizedMultiAgentSimulator (VMAS) - SourceForge.net VMAS: A Vectorized Multi-Agent Simulator for Collective Robot ... VMAS: A Vectorized Multi-Agent Simulator for Collective Robot ... VMAS — VMAS documentation</a></li>

</ul>
</details>

**Tags**: `#MARL`, `#hyperparameter tuning`, `#comparative study`, `#PPO`, `#VMAS`

---

<a id="item-15"></a>
## [llm-anthropic 0.27 Adds Compatibility with Anthropic SDK v1.0.0](https://simonwillison.net/2026/Aug/24/llm-anthropic/) ⭐️ 5.0/10

llm-anthropic 0.27 has been released, updating the Anthropic plugin for LLM to be compatible with the anthropic v1.0.0 Python library, which switched from httpx to httpx2. The update was largely automated using Claude Code with Fable 5, resulting in a pull request that gets tests passing. This release ensures that users of the LLM tool can continue to use Anthropic models without disruption after the SDK's breaking change. It also demonstrates a practical use of AI-assisted migration, as the author used Claude Code to perform the upgrade, which may inspire similar workflows in the community. The anthropic v1.0.0 library switched from httpx to httpx2, a new HTTP client library. OpenAI made a similar change in their v3.0.0 release two weeks prior. The migration was guided by Anthropic's official migration guide, and the author used a prompt with Claude Code to automate the upgrade.

rss · Simon Willison · Aug 24, 16:27

**Background**: LLM is a command-line tool by Simon Willison that provides access to various language models through plugins. The anthropic plugin allows LLM to use Anthropic's Claude models. The anthropic-sdk-python library is the official Python SDK for Anthropic's API, and its v1.0.0 release introduced breaking changes, including the switch from httpx to httpx2, which requires plugin updates.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Aug/24/llm-anthropic/">Release: llm- anthropic 0.27 | Simon Willison’s Weblog</a></li>
<li><a href="https://archlinux.org/packages/extra/any/python-httpx2/">Arch Linux - python - httpx 2 2.3.0-1 (any)</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#Anthropic`, `#Python`, `#SDK`, `#Release`

---

<a id="item-16"></a>
## [EMNLP Author Questions Missing Meta-Review After Rejection](https://www.reddit.com/r/MachineLearning/comments/1vxc1nw/is_emnlp_not_going_to_provide_a_metareview_d/) ⭐️ 4.0/10

A researcher on Reddit reported that EMNLP did not provide a meta-review for their rejected paper, unlike ACL, and expressed frustration over the decision despite the Area Chair recommending findings. This highlights potential inconsistencies in the review process across NLP conferences, which could affect author trust and decisions on resubmission. It also sparks discussion about transparency and the role of meta-reviews in ARR-based reviewing. The author mentioned that reviewers 'tanked' the paper intentionally, which they flagged, and the AC acknowledged this. They are unsure whether to resubmit through an ARR cycle to 'cleanse' the review history.

reddit · r/MachineLearning · /u/Massive-Bobcat-5363 · Aug 24, 19:01

**Background**: EMNLP uses the ACL Rolling Review (ARR) system, where papers are reviewed in cycles and authors receive reviews and a meta-review from an Area Chair. However, meta-reviews may not always be provided, depending on the venue. The ACL 2026 call states that Senior Area Chairs and Program Chairs make acceptance decisions from ARR reviews and meta-reviews, indicating the importance of meta-reviews in the process.

<details><summary>References</summary>
<ul>
<li><a href="https://aclrollingreview.org/">ACL Rolling Review – A peer review platform for the ...</a></li>
<li><a href="https://2026.aclweb.org/calls/main_conference_papers/">Main Conference - ACL 2026</a></li>

</ul>
</details>

**Discussion**: The Reddit post has no comments provided, so no community discussion is available.

**Tags**: `#EMNLP`, `#conference review`, `#NLP`, `#meta-review`

---

<a id="item-17"></a>
## [BMVC 2026 IJCV Recommendation Process Questioned](https://www.reddit.com/r/MachineLearning/comments/1vwtzix/bmvc_2026_ijcv_recommendation_d/) ⭐️ 3.0/10

A PhD student posted a question on Reddit asking how the BMVC 2026 IJCV special issue recommendation works, specifically whether it is based on review scores or a separate decision by ACs/program chairs. The post also asks if authors can know early if their paper is recommended or if they only find out later via email. This question highlights the importance of understanding journal recommendation processes for researchers aiming to publish in top venues like IJCV. Clarity on this process can help authors manage expectations and plan their publication strategies. The BMVC 2025 website states that top papers from BMVC will be invited to submit extended versions to an IJCV special issue, with papers needing 30-40% new material and rigorous journal review. The exact criteria for recommendation are not publicly detailed, and the notification process appears to be via separate email.

reddit · r/MachineLearning · /u/Secondhanded_PhD · Aug 24, 05:39

**Background**: BMVC (British Machine Vision Conference) is a major computer vision conference, and IJCV (International Journal of Computer Vision) is a top journal in the field. Many conferences invite top papers to submit extended versions to journal special issues, which undergo additional review. The recommendation is typically made by program chairs or area chairs based on review scores and paper quality.

<details><summary>References</summary>
<ul>
<li><a href="https://bmvc2025.bmva.org/">The 36th British Machine Vision Conference 2025: Home</a></li>
<li><a href="https://link.springer.com/collections/hjaaiaffcj">British Machine Vision Conference special issues (BMVC)</a></li>

</ul>
</details>

**Tags**: `#BMVC`, `#IJCV`, `#academic publishing`, `#conference`

---

<a id="item-18"></a>
## [Does Abstract Registration Count as Double Submission?](https://www.reddit.com/r/MachineLearning/comments/1vx3why/does_registering_an_abstract_not_the_full/) ⭐️ 3.0/10

A Reddit user asked whether registering an abstract without submitting the full paper counts as a double submission. The question highlights ambiguity in conference submission policies. This matters because researchers often face unclear rules about what constitutes double submission, and misunderstanding can lead to ethical violations or paper rejection. Clarifying such policies helps maintain research integrity. Double submission generally refers to submitting the same or substantially similar paper to multiple venues concurrently. However, abstract registration alone may not be considered a full submission, but policies vary by conference.

reddit · r/MachineLearning · /u/obliviousphoenix2003 · Aug 24, 14:09

**Background**: In academic publishing, double submission is considered misconduct, often leading to automatic withdrawal from conferences. Conferences typically require authors to submit original work not under review elsewhere. The distinction between abstract registration and full paper submission is not always clear, so authors should consult specific conference guidelines or supervisors.

<details><summary>References</summary>
<ul>
<li><a href="http://ccr.sigcomm.org/online/files/p40-v39n3c5-schulzrinneA.pdf">Double Submissions – Publishing Misconduct or ... - SIGCOMM</a></li>
<li><a href="https://www.editage.com/insights/duplicate-publications-and-simultaneous-submissions">Duplicate publication, Simultaneous submission: Definition ... Multiple, duplicate, concurrent publication | Editors | Elsevier Can You Submit Two Papers to the Same Conference? A Guide to ... Handling concurrent and duplicate submissions | COPE ... Double Submission, Double Publication - PMC Can you submit the same abstract to multiple conferences ...</a></li>
<li><a href="https://www.iconf.org/news/711">Can You Submit Two Papers to the Same Conference? A Guide to ...</a></li>

</ul>
</details>

**Tags**: `#academic publishing`, `#conference submission`, `#research ethics`

---