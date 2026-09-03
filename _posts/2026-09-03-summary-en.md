---
layout: default
title: "Horizon Summary: 2026-09-03 (EN)"
date: 2026-09-03
lang: en
---

> From 14 items, 12 important content pieces were selected

---

1. [OpenAI Unveils GPT-6 Astra with Near-Perfect ARC-AGI-3 Score](#item-1) ⭐️ 10.0/10
2. [Porting 1993 Amiga Assembly Game to Godot with LLM](#item-2) ⭐️ 8.0/10
3. [Go Grandmaster Shin Defeats AI KataGo with Two-Stone Handicap](#item-3) ⭐️ 8.0/10
4. [Qwen 3.8 27B on Cerebras Hits 1500 tok/s, but Rate Limits and Cost Raise Concerns](#item-4) ⭐️ 7.0/10
5. [Verisign Proposes Terminating .name Third-Level Domains](#item-5) ⭐️ 7.0/10
6. [K2 Horizon: Six Open Models, Yet Benchmarks Lag Qwen](#item-6) ⭐️ 7.0/10
7. [Artificial Beaver Dams Boost Coho Salmon Survival from 8% to 60%](#item-7) ⭐️ 7.0/10
8. [Grounding LLMs with JEPA World Models Trained in Simulation](#item-8) ⭐️ 7.0/10
9. [Mol-JEPA: A Multimodal Molecular Foundation Model Using JEPA](#item-9) ⭐️ 7.0/10
10. [AAAI-27 Desk Rejection for Minor Abstract Edits Sparks Debate](#item-10) ⭐️ 6.0/10
11. [Random Life Story Generator Draws Skepticism Over Data Accuracy](#item-11) ⭐️ 5.0/10
12. [NeurIPS Sydney Tickets Sell Out in Minutes](#item-12) ⭐️ 4.0/10

---

<a id="item-1"></a>
## [OpenAI Unveils GPT-6 Astra with Near-Perfect ARC-AGI-3 Score](https://openai.com/index/gpt-6-astra/) ⭐️ 10.0/10

OpenAI announced GPT-6 Astra, a new frontier model that achieves a 99.9% score on the ARC-AGI-3 benchmark and shows major gains in the Artificial Analysis Coding Agent Index. The model is being rolled out, with a system card available for safety details. GPT-6 Astra represents a significant milestone in AI development, potentially signaling progress toward more general intelligence. Its near-perfect ARC-AGI-3 performance could reshape expectations for frontier models and intensify competition among AI labs. The ARC-AGI-3 scorecard notes that with the Responses API harness, GPT-5.6 Sol would score around 30%, but the leaderboard shows 7.8% for Sol, indicating a methodology discrepancy. GPT-6 Astra also shows major gains in the Artificial Analysis Coding Agent Index, which is a composite of DeepSWE, Terminal-Bench v2.1, and SWE-Atlas-QnA.

hackernews · kibae · Sep 3, 18:41 · [Discussion](https://news.ycombinator.com/item?id=49554643)

**Background**: ARC-AGI-3 is an interactive reasoning benchmark that evaluates an AI agent's ability to learn unfamiliar task mechanics through action and feedback in novel environments. It is a successor to ARC-AGI-1 and ARC-AGI-2, focusing on fluid adaptive efficiency. The Artificial Analysis Coding Agent Index measures coding agent performance on end-to-end software engineering tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>
<li><a href="https://arxiv.org/abs/2603.24621">ARC-AGI-3: A New Challenge for Frontier Agentic Intelligence ARC Prize - Leaderboard ARC-AGI-3: A New Challenge for Frontier Agentic Intelligence ARC-AGI-3: The New Interactive Reasoning Benchmark GitHub - arcprize/arc-agi-3-benchmarking</a></li>
<li><a href="https://artificialanalysis.ai/agents/coding-agents">AI Coding Agent Benchmarks & Leaderboard | Artificial Analysis</a></li>

</ul>
</details>

**Discussion**: Community comments express skepticism about the ARC-AGI-3 scorecard's methodology, noting that GPT-5.6 Sol's score would be higher with the same harness used for GPT-6 Astra. Some commenters see the gains as modest compared to point updates, questioning whether this truly represents AGI. Others draw parallels to François Chollet's work on intelligence measurement, suggesting progress is still about skill acquisition rather than general intelligence.

**Tags**: `#OpenAI`, `#GPT-6`, `#AI model`, `#ARC-AGI`, `#benchmarks`

---

<a id="item-2"></a>
## [Porting 1993 Amiga Assembly Game to Godot with LLM](https://babyloniantwins.com/blog/porting-a-1993-amiga-game-to-godot/) ⭐️ 8.0/10

A developer successfully ported his 1993 Amiga game, originally written in MC68000 assembly, to the Godot engine using an LLM (Claude Fable 5). The initial port took just one evening, with additional weekends spent refining the feel and shipping it. This demonstrates a novel, practical application of LLMs for translating and preserving legacy code, potentially lowering the barrier for retro game preservation and modernization. It highlights AI's ability to understand and convert low-level assembly into modern high-level code, which could benefit developers working with legacy systems. The developer used vasm to assemble the code on a Mac, iterating until the binary was byte-identical to the original, except for a 108-byte mismatch. This discrepancy arose because the original game was assembled with AsmOne, which assembles into memory, and the shipped files were snapshots of the running game rather than clean assembler output. The developer also released the original game for free.

hackernews · rabahs · Sep 3, 14:28 · [Discussion](https://news.ycombinator.com/item?id=49550375)

**Background**: The Amiga was a personal computer popular in the late 1980s and early 1990s, known for its advanced graphics and sound. Games were often written in MC68000 assembly for performance, using tools like AsmOne, an integrated assembler environment. Godot is a modern open-source game engine that supports 2D and 3D game development, making it a suitable target for porting retro games. LLMs (Large Language Models) like Claude are AI systems capable of understanding and generating code, enabling tasks like translating assembly to higher-level languages.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Motorola_68000">Motorola 68000 - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Godot_(game_engine)">Godot (game engine)</a></li>
<li><a href="https://aminet.net/package/dev/asm/ASM-One">Aminet - dev/asm/ASM-One.lha Asm One 1.02 Manual : Rune Gram-Madsen : Free Download ... ASM-One Macro Assembler - HandWiki Commodore Software - ASM-One v1.02 Manual ASM-One Page - theflamearrows.info ASM-One Macro Assembler - EverybodyWiki Bios & Wiki Asm One 1.02 Manual : Free Download, Borrow, and Streaming ...</a></li>

</ul>
</details>

**Discussion**: Community members expressed admiration for the original assembly programming feat and enthusiasm for using LLMs to port retro games. One user shared a similar success converting a ZX81 memory dump to Go, while another asked about debugging stories from the original development. A user also noted the game's resemblance to 'Gods: Into the Wonderful' and inquired about inspiration.

**Tags**: `#LLM`, `#retrocomputing`, `#Godot`, `#game development`, `#code porting`

---

<a id="item-3"></a>
## [Go Grandmaster Shin Defeats AI KataGo with Two-Stone Handicap](https://www.kedglobal.com/artificial-intelligence/newsView/ked202607210007) ⭐️ 8.0/10

Go grandmaster Shin Jinseo defeated the AI program KataGo in a game with a two-stone handicap, a rare human victory over a top-level Go AI. The match highlights Shin's exceptional skill and strategic adaptability against artificial intelligence. This event is significant as it demonstrates that a human can still overcome a leading AI in a complex game when given a handicap, offering insights into human-AI interaction and the limits of AI in strategic domains. It also underscores the evolving relationship between human expertise and AI in competitive settings. The two-stone handicap is considered a substantial advantage in Go, typically given to weaker players. Shin Jinseo is widely regarded as the strongest human Go player in history, with a rating over 3800, far surpassing his closest rivals. The match involved a complex joseki variation, showcasing Shin's deep understanding of the game.

hackernews · gmays · Sep 3, 01:11 · [Discussion](https://news.ycombinator.com/item?id=49544762)

**Background**: KataGo is a free, open-source computer Go program developed by David Wu, first released in 2019. It uses neural networks and self-play training to achieve superhuman performance, capable of defeating top human players. In Go, handicaps are stones placed on the board to balance skill differences, with two stones being a common handicap for weaker players.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/KataGo">KataGo - Wikipedia</a></li>
<li><a href="https://github.com/lightvector/KataGo">GitHub - lightvector/KataGo: GTP engine and self-play ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Handicapping_in_Go">Handicapping in Go - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community comments highlight Shin Jinseo's extraordinary strength, noting his rating is over 120 points higher than the next strongest player, and that he replicates AI moves more closely than anyone else. Some commenters clarify that the two-stone handicap means Shin was the weaker player, but his victory is still remarkable given the AI's dominance in even games. Others discuss the strategic depth of the match, including the use of complex joseki variations, and debate the value of studying AI moves for human players.

**Tags**: `#AI`, `#Go`, `#KataGo`, `#human-AI competition`, `#game theory`

---

<a id="item-4"></a>
## [Qwen 3.8 27B on Cerebras Hits 1500 tok/s, but Rate Limits and Cost Raise Concerns](https://inference-docs.cerebras.ai/models/overview) ⭐️ 7.0/10

Qwen 3.8 27B is now available on Cerebras inference, delivering up to 1500 tokens per second. However, users report that rate limits and billing issues may hinder practical use. This marks a significant speed milestone for open-weight models, potentially enabling real-time coding assistance and other latency-sensitive applications. Yet, the practical limitations highlighted by the community could affect adoption and competitiveness against other providers. The public endpoint has a token-per-minute limit of 150,000, and cached tokens count toward this limit, causing one user to exhaust 450,000 tokens in about 90 seconds and incur $1.10 in costs. Additionally, some enterprise accounts face billing access restrictions, preventing self-serve billing.

hackernews · altertable · Sep 3, 18:32 · [Discussion](https://news.ycombinator.com/item?id=49554520)

**Background**: Cerebras Inference is a wafer-scale AI inference platform known for its high token throughput, often exceeding 2,000 tokens per second for smaller models. Qwen 3.8 27B is a compact, deployment-friendly dense vision-language model built on the Qwen 3.5 architecture, designed for coding, professional work, and agentic tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cerebras.ai/blog/introducing-cerebras-inference-ai-at-instant-speed">Introducing Cerebras Inference: AI at Instant Speed - Cerebras</a></li>
<li><a href="https://www.cerebras.ai/inference">Inference - Cerebras</a></li>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-27B">Qwen / Qwen 3 . 8 - 27 B · Hugging Face</a></li>

</ul>
</details>

**Discussion**: Community feedback is mixed: some users praise the output speed but criticize the rate limits and cost, noting that cached tokens count against the limit and that tasks can become expensive quickly. Others suggest that local inference on high-end GPUs like the RTX 5090 can achieve comparable speeds, and express interest in seeing Cerebras offer the model via OpenRouter for better flexibility.

**Tags**: `#AI`, `#LLM`, `#Cerebras`, `#Qwen`, `#Inference`

---

<a id="item-5"></a>
## [Verisign Proposes Terminating .name Third-Level Domains](https://neil.fraser.name/news/2026/09/03/) ⭐️ 7.0/10

Verisign has proposed terminating all third-level .name domains (x.y.name) and releasing the corresponding second-level domains (y.name). This proposal, dated September 3, 2026, would affect existing registrations and is currently under discussion. This policy change could disrupt existing websites and email services that rely on third-level .name domains, raising concerns about stability and domain squatting. It also challenges ICANN's mission to ensure stable and secure operation of the Internet's unique identifier systems. The proposal does not mention any grace period or reservation of second-level domains to prevent squatting. Existing second-level .name domains (e.g., dvt.name) are not affected, only third-level registrations under them.

hackernews · pavel_lishin · Sep 3, 14:54 · [Discussion](https://news.ycombinator.com/item?id=49550772)

**Background**: Domain names are structured in levels: top-level (TLD), second-level (SLD), and third-level (subdomain). The .name TLD was originally designed to allow individuals to register personal domains at the third level (e.g., john.doe.name). Verisign operates the .name registry, and ICANN oversees domain policy. Termination of existing registrations is unusual and raises legal and operational questions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Domain_name">Domain name - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Second-level_domain">Second-level domain - Wikipedia</a></li>
<li><a href="https://www.icann.org/en/blogs/details/icann-clears-the-way-for-two-character-second-level-domain-names-12-11-2014-en">ICANN Clears the Way for Two-character Second-level Domain Names</a></li>

</ul>
</details>

**Discussion**: Commenters express concern over the abrupt termination, suggesting that Verisign should at least discontinue new registrations while honoring existing ones and reserving second-level domains to prevent squatting. Some note that this contradicts ICANN's mission of stability and security, while others clarify that only third-level domains are affected, not second-level ones.

**Tags**: `#ICANN`, `#domain names`, `#policy`, `#internet governance`

---

<a id="item-6"></a>
## [K2 Horizon: Six Open Models, Yet Benchmarks Lag Qwen](https://ifm.ai/blog/k2/) ⭐️ 7.0/10

IFM released K2 Horizon, a fleet of six fully open AI models including weights, code, training data, and methodologies. However, benchmarks show the models underperform compared to Qwen's offerings of similar sizes. This release is significant for the open-source AI community as it provides full transparency, but the performance gap with Qwen may limit adoption. It highlights the competitive pressure on open models to match or exceed existing alternatives. The fleet includes models ranging from a small edge-device model to a 375B-A23B model. Notably, the dense 32B model significantly trails Qwen3.8 27B in benchmarks, and the 3.7B model was found unreliable for coding tasks.

hackernews · karimf · Sep 3, 15:36 · [Discussion](https://news.ycombinator.com/item?id=49551760)

**Background**: Fully open models release all components, including training data and code, unlike open-weight models that only share weights. Qwen is a prominent open-weight model family known for strong performance, making it a key comparison point for new open releases.

<details><summary>References</summary>
<ul>
<li><a href="https://ifm.ai/blog/k2">Introducing K2 Horizon: Frontier Performance, Radically Open</a></li>
<li><a href="https://huggingface.co/collections/IFM/k2-horizon">K2 Horizon - a IFM Collection - Hugging Face</a></li>
<li><a href="https://www.prnewswire.com/news-releases/institute-of-foundation-models-launches-the-industrys-largest-fully-open-source-fleet-of-ai-models-complete-with-weights-code-training-data-and-methodologies-302868628.html">Institute of Foundation Models Launches the Industry's ...</a></li>

</ul>
</details>

**Discussion**: Commenters praised the fully open approach but criticized the performance gap, noting the 32B and 36B models are inferior to Qwen3.8 27B. Some expressed model fatigue due to the rapid pace of releases, and one user reported the 3.7B model failed basic coding tests.

**Tags**: `#open-source`, `#AI`, `#LLM`, `#model release`, `#benchmarks`

---

<a id="item-7"></a>
## [Artificial Beaver Dams Boost Coho Salmon Survival from 8% to 60%](https://www.discoverwildlife.com/animal-facts/artificial-beaver-dams-california) ⭐️ 7.0/10

In California, the installation of artificial beaver dams has dramatically increased juvenile coho salmon survival rates from 8% to 60%. This ecological engineering intervention mimics natural beaver activity to restore stream habitats. This significant improvement offers a promising, cost-effective tool for salmon conservation, especially in regions where beaver populations are low or absent. It highlights the potential of process-based restoration to address declining salmon populations and could inform broader habitat restoration strategies. The artificial dams were designed to mimic natural beaver dams, slowing water flow and increasing groundwater infiltration. Interestingly, water temperatures decreased after damming, contrary to expectations, likely due to enhanced hyporheic exchange with cooler subsurface water.

hackernews · speckx · Sep 3, 16:21 · [Discussion](https://news.ycombinator.com/item?id=49552572)

**Background**: Coho salmon (Oncorhynchus kisutch) are a threatened species in California, and their juvenile survival is critical for population recovery. Beaver dams create complex habitats with pools and cooler water, which benefit salmon, but beaver populations have declined due to trapping and habitat loss. Artificial dams aim to replicate these benefits without reintroducing beavers, which may not be feasible in all areas.

**Discussion**: Commenters expressed curiosity about the mechanisms behind the survival increase, particularly the counterintuitive drop in water temperature, and called for more research. One commenter noted a historical parallel from a 1930s homesteader who restored dynamited beaver dams, while another questioned why beavers weren't simply reintroduced, and another wondered about potential ecological chain reactions.

**Tags**: `#ecology`, `#conservation`, `#salmon`, `#beaver dams`, `#environmental engineering`

---

<a id="item-8"></a>
## [Grounding LLMs with JEPA World Models Trained in Simulation](https://www.reddit.com/r/MachineLearning/comments/1w69gvd/grounding_llms_with_jepabased_world_models/) ⭐️ 7.0/10

A Reddit user proposes training a JEPA-style world model in a physics simulation (e.g., MuJoCo) to predict future state representations, then attaching these grounded representations to an LLM as a conditioning signal to give it physical intuition. The idea combines JEPA prediction, simulation-based grounding, and LLM attachment, which the author claims has not been done cleanly before. This addresses a fundamental limitation of LLMs: they lack grounded understanding of physical reality, akin to the 'Mary's Room' thought experiment. If successful, it could make LLMs more robust for robotics, embodied AI, and tasks requiring physical reasoning, potentially accelerating downstream learning by providing computational primitives rather than propositional facts. The proposal suggests predicting representations in an abstract embedding space rather than pixels or tokens, with an unforgiving loss that enforces physical correctness. The author questions the interface between JEPA representations and LLMs (e.g., concatenation vs. cross-attention) and whether sim-to-real transfer would survive, citing V-JEPA and DreamerV3 as adjacent work.

reddit · r/MachineLearning · /u/Full_Promotion4522 · Sep 3, 14:45

**Background**: JEPA (Joint Embedding Predictive Architecture) is a world model approach proposed by Yann LeCun, which learns to predict representations of future states in a latent space rather than raw pixels. V-JEPA is Meta's video-based world model that predicts future frame representations, and DreamerV3 is an RL agent that uses a latent world model for efficient learning. The 'Mary's Room' thought experiment illustrates the difference between knowing facts about something and having direct experiential knowledge, which is often used to critique LLMs' lack of grounding.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/World_model_(artificial_intelligence)">World model (artificial intelligence) - Wikipedia</a></li>
<li><a href="https://ai.meta.com/blog/v-jepa-2-world-model-benchmarks/">Introducing the V-JEPA 2 world model and new benchmarks for physical reasoning</a></li>
<li><a href="https://uchicagotechreview.com/articles/the-large-language-model-trapped-in-mary’s-room">The Large Language Model Trapped in Mary ’ s Room ...</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#JEPA`, `#world models`, `#grounding`, `#AI research`

---

<a id="item-9"></a>
## [Mol-JEPA: A Multimodal Molecular Foundation Model Using JEPA](https://www.reddit.com/r/MachineLearning/comments/1w6i8pr/moljepa_multimodal_molecular_foundation_model_r/) ⭐️ 7.0/10

The author introduced Mol-JEPA, a multimodal molecular foundation model based on the Joint Embedding Predictive Architecture (JEPA), along with a summary website showcasing key results. The model is presented as a research paper announcement, and the author is open to community feedback and ideas for improvement. Mol-JEPA represents a novel application of JEPA to molecular machine learning, potentially enabling more efficient learning from multimodal molecular data. This could advance drug discovery and materials science by providing a foundation model that captures complex molecular representations without relying solely on generative approaches. The model is multimodal, meaning it integrates multiple types of molecular data, and it leverages JEPA, which learns by comparing abstract representations rather than raw data. The author notes that further work is needed to improve performance, and the summary website provides key results for community review.

reddit · r/MachineLearning · /u/TerribleAntelope9348 · Sep 3, 19:56

**Background**: JEPA, or Joint Embedding Predictive Architecture, is a concept championed by Yann LeCun that learns by predicting missing parts of input in an abstract representation space, contrasting with generative models that predict in pixel or data space. Multimodal molecular foundation models aim to integrate diverse molecular data (e.g., graphs, text, omics) to enable broad downstream tasks. This work builds on recent trends in applying self-supervised learning to molecular data.

<details><summary>References</summary>
<ul>
<li><a href="https://ai.meta.com/blog/yann-lecun-ai-model-i-jepa/">I-JEPA: The first AI model based on Yann LeCun’s vision for ...</a></li>
<li><a href="https://rohitbandaru.github.io/blog/JEPA-Deep-Dive/">Deep Dive into Yann LeCun’s JEPA | Rohit Bandaru</a></li>
<li><a href="https://www.nature.com/articles/s41586-025-08710-y">Towards multimodal foundation models in molecular cell biology | Nature</a></li>

</ul>
</details>

**Tags**: `#molecular machine learning`, `#JEPA`, `#foundation model`, `#multimodal learning`, `#research paper`

---

<a id="item-10"></a>
## [AAAI-27 Desk Rejection for Minor Abstract Edits Sparks Debate](https://www.reddit.com/r/MachineLearning/comments/1w6kcp6/aaai27_desk_rejection_over_incredibly_minor/) ⭐️ 6.0/10

A researcher reported receiving a desk rejection from AAAI-27 due to minor modifications made to the title or abstract between the abstract-registration and full-paper deadlines, despite the modifications being deemed 'incredibly minor' and the rejection notice stating the decision is final with no appeals. This incident highlights potential inconsistencies in how AAAI-27's modification policy is applied, which could affect many researchers who make minor updates to their abstracts. It raises concerns about fairness and transparency in the conference's desk rejection process, potentially impacting the community's trust in AAAI. The AAAI-27 modification guidelines state that titles and abstracts can be edited after abstract registration, but warn against substantive changes that describe qualitatively different research. The rejection notice explicitly says the decision is final and appeals will not be considered, leaving the author with no recourse.

reddit · r/MachineLearning · /u/Dansilly · Sep 3, 21:12

**Background**: AAAI (Association for the Advancement of Artificial Intelligence) conference is a top venue for AI research. Desk rejection is a process where papers are rejected without full review, often for policy violations. The AAAI-27 submission instructions outline various policies, including multiple-submission and anonymity rules, which can lead to summary rejection if violated. The modification policy aims to prevent authors from changing their research direction after initial submission, but its application to minor edits is unclear.

<details><summary>References</summary>
<ul>
<li><a href="https://aaai.org/conference/aaai/aaai-27/submission-instructions/">AAAI-27 Submission Instructions - AAAI</a></li>
<li><a href="https://aaai.org/conference/aaai/aaai-27/review-process/">Review Process - AAAI</a></li>

</ul>
</details>

**Tags**: `#AAAI`, `#conference policy`, `#desk rejection`, `#academic publishing`, `#machine learning`

---

<a id="item-11"></a>
## [Random Life Story Generator Draws Skepticism Over Data Accuracy](https://anyhumanever.com/) ⭐️ 5.0/10

A new website, Any Human Ever, generates a life story for a randomly selected historical person, using AI to craft a narrative from statistical data. The project has gained attention on Hacker News, but users have raised concerns about the accuracy and internal consistency of the statistics presented. This project highlights the growing use of AI to make historical data accessible and engaging, but it also underscores the risks of presenting potentially misleading statistics as factual. The community's critical response reflects a broader concern about the reliability of AI-generated content in educational and historical contexts. The site samples a birth year and location, then uses life tables and population data to estimate lifespan and life events. However, users have pointed out that some cited statistics are internally inconsistent, such as claiming high marriage rates while also noting high child mortality, and that the cited sources may not support the claims.

hackernews · thinkingemote · Sep 3, 14:51 · [Discussion](https://news.ycombinator.com/item?id=49550698)

**Background**: The project is part of a trend of using AI and data visualization to explore history, similar to other tools like Random Lives and Emplotment. These tools aim to represent the lives of ordinary people, but they face challenges in balancing historical accuracy with narrative appeal, especially when data for past eras is sparse or uncertain.

<details><summary>References</summary>
<ul>
<li><a href="https://random-lives.github.io/random-lives/about/">About | Random Lives</a></li>
<li><a href="https://emplotment.com/">Emplotment | Historical Narrative Visualization</a></li>

</ul>
</details>

**Discussion**: Community comments are mixed: some find the project creative and useful for role-playing games, while others criticize it as misleading 'AI slop.' A key concern is the statistical methodology, with users noting that the random year selection may not follow the correct probability distribution and that cited statistics are sometimes contradictory.

**Tags**: `#AI`, `#data visualization`, `#history`, `#statistics`, `#web app`

---

<a id="item-12"></a>
## [NeurIPS Sydney Tickets Sell Out in Minutes](https://www.reddit.com/r/MachineLearning/comments/1w6gwni/neurips_sydney_sold_out_in_minutes_n/) ⭐️ 4.0/10

A Reddit post reports that NeurIPS Sydney tickets sold out within minutes, even before paper decisions were released. The post speculates about the proportion of attendees from industry and VC-funded AI labs. The rapid sellout highlights the surging demand for AI conferences, driven by industry and investment interest. This trend may affect the conference's culture, shifting focus toward recruitment and networking over academic exchange. The post notes that tickets sold out three weeks before paper decisions, indicating high anticipation. The author wonders about the percentage of industry and VC-funded AI lab attendees, suggesting a possible imbalance in the attendee mix.

reddit · r/MachineLearning · /u/alrojo · Sep 3, 19:09

**Background**: NeurIPS is a premier annual conference on neural information processing systems, attracting researchers and practitioners. In recent years, AI conferences have seen growing corporate and investor presence, leading to concerns about commercialization and reduced academic focus.

**Tags**: `#NeurIPS`, `#conference`, `#machine learning`, `#community`

---