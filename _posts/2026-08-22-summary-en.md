---
layout: default
title: "Horizon Summary: 2026-08-22 (EN)"
date: 2026-08-22
lang: en
---

> From 16 items, 15 important content pieces were selected

---

1. [Linus Torvalds Credits AI in Kernel Debug Session](#item-1) ⭐️ 8.0/10
2. [Developer Builds 60MB Quantized LLM from Scratch with Disk-Based Long Context](#item-2) ⭐️ 8.0/10
3. [DelveRL: Open-Source Roguelike for Training Game-Playing Agents](#item-3) ⭐️ 8.0/10
4. [Apple Deprecates hdiutil in macOS 27, Shifting to diskutil](#item-4) ⭐️ 7.0/10
5. [Munder Difflin: A Local Harness to Run an Office of AI Clones](#item-5) ⭐️ 7.0/10
6. [Coding Agents: Instruct and Verify, Not Just Review](#item-6) ⭐️ 7.0/10
7. [Evaluation Resolution Alters Brain-Like Learning Rule Rankings at V1](#item-7) ⭐️ 7.0/10
8. [Moxie's Scrap Metal Tweet Sparks Debate on Poverty and Theft](#item-8) ⭐️ 6.0/10
9. [Racket Intro Criticized as Speedrun, Not Friendly](#item-9) ⭐️ 6.0/10
10. [Z80 Microprocessor: 1970s Chip Still Thrives in Retrocomputing](#item-10) ⭐️ 6.0/10
11. [llm 0.33 Release: OpenAI 3.x Upgrade and Embedding Key Support](#item-11) ⭐️ 5.0/10
12. [LightGBM vs CatBoost: Why CatBoost Fits Interaction Toy Example Better](#item-12) ⭐️ 5.0/10
13. [AI Startup Naming Trend Spoofed in 'ElevenLabs, TwelveLabs, ThirteenLabs'](#item-13) ⭐️ 4.0/10
14. [Researcher Seeks Help After ACL ARR Desk Rejection Over Phantom Prior Review](#item-14) ⭐️ 4.0/10
15. [Canada to Match US Tariffs 'Dollar for Dollar' as Talks Collapse](#item-15) ⭐️ 3.0/10

---

<a id="item-1"></a>
## [Linus Torvalds Credits AI in Kernel Debug Session](https://simonwillison.net/2026/Aug/22/linus-torvalds/) ⭐️ 8.0/10

Linus Torvalds publicly praised an AI for assisting in a difficult kernel debug session, noting that the AI helped with grunt work and even wrote the commit message. The quote appears in a commit fixing a bug in the Intel Xe graphics driver. This marks a notable endorsement of AI's practical value in software engineering from one of the most influential figures in the field. It could encourage broader adoption of AI-assisted debugging and spark discussions about AI's role in development workflows. The debug session involved a one-line bug in the Intel Xe driver, requiring 24 debug patches and 18 kernel boots to resolve. The AI reportedly expressed pessimism, stating the problem was unsolvable, but Torvalds persisted and the fix will be included in the upcoming Linux 7.3 release.

rss · Simon Willison · Aug 22, 21:04

**Background**: The Linux kernel is the core of many operating systems, and debugging it can be extremely complex. AI-assisted programming tools, such as large language models, are increasingly used to help with code analysis and debugging, though their reliability can vary. Torvalds' comment highlights both the potential and limitations of such tools in high-stakes development.

<details><summary>References</summary>
<ul>
<li><a href="https://azat.tv/en/linus-torvalds-ai-assisted-kernel-bug-fix/">Linus Torvalds Credits AI Assistance in Rare Kernel Debugging ...</a></li>
<li><a href="https://news.ycombinator.com/item?id=49396366">Linus: And this was a debug session from hell... | Hacker News</a></li>
<li><a href="https://docs.kernel.org/next/gpu/driver-uapi.html">DRM Driver uAPI — The Linux Kernel documentation</a></li>

</ul>
</details>

**Discussion**: Hacker News discussion highlights the significance of Torvalds' endorsement, with some users noting the irony of AI's pessimism and others debating the extent of AI's contribution. Some commenters express skepticism about AI's role in kernel development, while others see it as a positive sign for future tooling.

**Tags**: `#AI`, `#Linux kernel`, `#debugging`, `#Linus Torvalds`

---

<a id="item-2"></a>
## [Developer Builds 60MB Quantized LLM from Scratch with Disk-Based Long Context](https://www.reddit.com/r/MachineLearning/comments/1vv2nkh/i_developed_my_own_quantized_llm_from_scratch/) ⭐️ 8.0/10

A developer trained a 250M parameter LLM from scratch on 30B tokens, quantized it to under 2 bits, and achieved a 60MB deployment that runs at 400 tok/s on CPU. The model also introduces a novel disk-based long-context mechanism, compressing older tokens to 1 bit and storing them on disk for retrieval. This demonstrates that highly compressed LLMs can be deployed on resource-constrained devices without GPUs, potentially enabling on-device AI applications. The disk-based long-context approach offers a scalable way to handle extremely long histories, which is a significant challenge in current LLM systems. The model uses a fixed 512-bit code for each token instead of a learned embedding table, with zero trained parameters for embeddings. It achieves a cross-entropy of 3.15 nats per token (perplexity 23.3) on held-out English web text, and scores 0.619 Spearman correlation on WordSim-353, demonstrating the effectiveness of the fixed codes.

reddit · r/MachineLearning · /u/Final-Data-1410 · Aug 22, 04:39

**Background**: Quantization reduces the precision of model weights to lower memory usage, but going below 2 bits typically degrades quality significantly. Traditional KV caches store all context in memory, limiting context length; this project instead compresses older tokens to 1 bit and stores them on disk, allowing up to 100M tokens of history. The model was trained to retrieve from this disk cache but not to reason over it, due to budget constraints.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2307.13304">[2307.13304] QuIP: 2-Bit Quantization of Large Language Models With Guarantees</a></li>
<li><a href="https://arxiv.org/html/2606.26105v1">Context Recycling for Long-Horizon LLM Inference A Hierarchical Memory Architecture for Managing Fixed Context Budgets Across Unbounded Sessions</a></li>

</ul>
</details>

**Discussion**: The Reddit community responded positively, with the author noting they expected to be roasted but received curious and helpful comments. The discussion likely included technical questions about the quantization method and disk-based retrieval, as well as validation of the results.

**Tags**: `#LLM`, `#quantization`, `#model compression`, `#efficient inference`, `#long context`

---

<a id="item-3"></a>
## [DelveRL: Open-Source Roguelike for Training Game-Playing Agents](https://www.reddit.com/r/MachineLearning/comments/1vvii1j/i_built_an_opensource_roguelike_specifically_for/) ⭐️ 8.0/10

The author released DelveRL, an open-source roguelike environment designed specifically for training game-playing agents, featuring a structured API, deterministic simulation, procedural levels, and partial observability. The included baseline reaches a median floor of 18 and extended runs reaching floor 33. DelveRL addresses a gap in reinforcement learning research by providing a purpose-built, open-source environment that is easy to integrate with agent harnesses, unlike many existing games. This could accelerate research in areas like exploration, risk management, and partial observability, benefiting the RL community. The environment runs locally, including batched renderer-free environments and a recurrent PPO trainer. The game, training code, checkpoint, bridge documentation, and raw benchmarks are all open source, allowing the community to reproduce and improve upon the baseline.

reddit · r/MachineLearning · /u/SnyderConsulting · Aug 22, 17:32

**Background**: Roguelikes are a genre of games characterized by procedural level generation, turn-based gameplay, and permadeath, making them challenging for AI agents. Reinforcement learning (RL) agents learn by interacting with an environment, and having a well-designed environment with a clean API is crucial for efficient training. PPO (Proximal Policy Optimization) is a popular RL algorithm, and its recurrent variant uses LSTM or GRU to handle partial observability.

<details><summary>References</summary>
<ul>
<li><a href="https://agoodpointpoorlymade.itch.io/delverl">DelveRL by aGoodPointPoorlyMade</a></li>
<li><a href="https://sb3-contrib.readthedocs.io/en/master/modules/ppo_recurrent.html">Recurrent PPO — Stable Baselines3 - Contrib 2.9.0 documentation</a></li>
<li><a href="https://github.com/MarcoMeter/recurrent-ppo-truncated-bptt/blob/main/trainer.py">recurrent - ppo -truncated-bptt/ trainer .py at main...</a></li>

</ul>
</details>

**Tags**: `#reinforcement learning`, `#open-source`, `#game environment`, `#AI training`, `#roguelike`

---

<a id="item-4"></a>
## [Apple Deprecates hdiutil in macOS 27, Shifting to diskutil](https://lapcatsoftware.com/articles/2026/8/7.html) ⭐️ 7.0/10

In macOS 27 Golden Gate, Apple has deprecated the hdiutil command-line tool, directing users to use diskutil image for all disk image operations. The deprecation was announced in a blog post by Lapcat Software on August 7, 2026. This change breaks longstanding workflows and scripts that rely on hdiutil, affecting many developers and system administrators. It also raises concerns about Apple's deprecation practices and backward compatibility, as the functionality is being moved rather than removed, yet the transition may cause unnecessary disruption. The deprecation is noted in macOS 27.0, with diskutil image providing subcommands for attach, create, resize, info, and chpass. Historically, hdiutil has been the primary tool for creating and managing disk images, including RAM disks, and its deprecation may also affect those capabilities.

hackernews · zdw · Aug 22, 19:04 · [Discussion](https://news.ycombinator.com/item?id=49402741)

**Background**: hdiutil is a command-line utility in macOS used for creating, mounting, and manipulating disk image files (e.g., .dmg). diskutil is another command-line tool that manages disks and volumes, and now it is being expanded to cover disk image operations. Apple has a history of deprecating tools and eventually removing them, as seen with xip, which remains in use for Xcode distribution despite being deprecated.

<details><summary>References</summary>
<ul>
<li><a href="https://lapcatsoftware.com/articles/2026/8/7.html">hdiutil is deprecated in macOS 27 Golden Gate</a></li>
<li><a href="https://github.com/argv-minus-one/dmg-license/issues/11">Help needed: `hdiutil udifrez` is deprecated by Apple but is needed by dmg-license · Issue #11 · argv-minus-one/dmg-license</a></li>
<li><a href="https://en.wikipedia.org/wiki/Disk_Utility">Disk Utility - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community members expressed skepticism about Apple's deprecation practices, with one commenter noting that Apple often ignores bug reports and that backward compatibility is purely incidental. Another pointed out that xip has been deprecated for years but is still used for Xcode distribution, suggesting hdiutil may not disappear soon. Some users also worried about the impact on RAM disk creation, as hdiutil was the only way to create them.

**Tags**: `#macOS`, `#deprecation`, `#developer tools`, `#Apple`, `#command-line`

---

<a id="item-5"></a>
## [Munder Difflin: A Local Harness to Run an Office of AI Clones](https://munderdiffl.in/) ⭐️ 7.0/10

Munder Difflin is a new local multi-agent harness that wraps around existing coding agents like Claude Code and Codex, enabling deterministic coordination of multiple AI clones without consuming tokens. It has gained over 20,000 users within a week of release. This project addresses the growing challenge of multi-agent coordination in AI coding, offering a deterministic and token-efficient alternative to current approaches. It could significantly reduce costs and improve reliability for developers using multiple AI agents, potentially influencing how future agent orchestration tools are designed. The harness supports almost all major coding agents and ensures deterministic simulations that do not consume tokens, reportedly reducing token consumption for most users. It is themed around 'The Office', with roles and pipelines rather than traditional agent definitions, as noted in community feedback.

hackernews · simonpure · Aug 22, 09:49 · [Discussion](https://news.ycombinator.com/item?id=49398152)

**Background**: Multi-agent harnesses partition task workflows into finite agent roles, each with specific responsibilities and tool access. Deterministic orchestration is crucial because non-deterministic agents can compound errors and increase token costs as they pass context. Coding agents like Claude Code and Codex are engineered systems that include model, reasoning, and tooling, and local harnesses aim to coordinate them efficiently.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/multi-agent-harness">Multi - Agent Harness Design</a></li>
<li><a href="https://www.elementum.ai/blog/are-ai-agents-deterministic">Are AI Agents Deterministic? | Elementum</a></li>
<li><a href="https://magazine.sebastianraschka.com/p/components-of-a-coding-agent">Components of A Coding Agent - by Sebastian Raschka, PhD</a></li>

</ul>
</details>

**Discussion**: Community sentiment is largely positive, with users praising the novel theme and practical value. One user noted the accuracy of the 'dysfunctional office' metaphor for agent swarms, while another provided detailed feedback on preferring pipelines and roles over fixed agents. The author actively engaged, answering questions and highlighting the token savings.

**Tags**: `#multi-agent`, `#AI`, `#coding agents`, `#harness`, `#LLM`

---

<a id="item-6"></a>
## [Coding Agents: Instruct and Verify, Not Just Review](https://simonwillison.net/2026/Aug/22/more-than-just-code-review/) ⭐️ 7.0/10

Simon Willison argues that the key skill for using coding agents is confidently instructing them on changes and verifying the results, which may not always require reviewing every line of code. This insight challenges the conventional emphasis on line-by-line code review in AI-assisted development, potentially reshaping how developers approach quality assurance with coding agents. It highlights a practical skill that could improve productivity and trust in AI-generated code. Willison suggests alternative verification methods beyond line-by-line review, such as running tests or checking specific behaviors. The post is tagged with 'agentic-engineering' and 'code-review', indicating its relevance to the emerging discipline of orchestrating autonomous AI agents.

rss · Simon Willison · Aug 22, 15:56

**Background**: Coding agents are AI systems that can autonomously write, modify, and test code based on high-level instructions. Agentic engineering is an emerging discipline that focuses on directing these agents effectively, requiring skills in instruction, oversight, and validation. Traditional code review involves manually inspecting every line for errors, but with AI-generated code, this may be inefficient, prompting new verification strategies.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/Agentic_Engineering">Agentic Engineering</a></li>
<li><a href="https://openai.com/codex/">Codex in ChatGPT | AI Coding Agents for Software... | OpenAI</a></li>

</ul>
</details>

**Tags**: `#coding-agents`, `#code-review`, `#AI`, `#LLMs`, `#agentic-engineering`

---

<a id="item-7"></a>
## [Evaluation Resolution Alters Brain-Like Learning Rule Rankings at V1](https://www.reddit.com/r/MachineLearning/comments/1vvdxwt/the_evaluation_resolution_has_been_shown_to_have/) ⭐️ 7.0/10

A new preprint demonstrates that the evaluation resolution significantly impacts which learning rule appears most brain-like at the early visual cortex (V1), showing that untrained CNNs matching trained ones is an artifact of low resolution. The study used a small CNN trained at 32px and evaluated at six resolutions from 32px to 224px. This finding is critical for model-brain comparisons, as it shows that conclusions about learning rules can be reversed by simply changing evaluation resolution. It highlights the need for standardized evaluation protocols in computational neuroscience and machine learning. The gap between trained and untrained backpropagation (BP) at V1 narrowed from -0.001±0.007 at 32px to +0.044±0.006 at 224px, a non-monotonic trend. The study ruled out several potential confounds, including train/eval resolution matching and Gabor/pixel low-level structure, and found that the backprop > untrained effect at LOC survived across all resolutions.

reddit · r/MachineLearning · /u/ConfusionSpiritual19 · Aug 22, 14:30

**Background**: Model-brain comparisons often use representational similarity analysis (RSA) to compare activations of artificial neural networks to brain responses. Learning rules like backpropagation, feedback alignment, predictive coding, and STDP are biologically plausible alternatives to standard training. The study uses THINGS-fMRI stimuli and includes human fMRI and macaque ephys data.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Spike-timing-dependent_plasticity">Spike -timing-dependent plasticity - Wikipedia</a></li>
<li><a href="https://www.emergentmind.com/topics/feedback-alignment-fa">Feedback Alignment in Neural Networks</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion is not provided, but the author invites feedback, especially on the framing of receptive-field matching. The community likely appreciates the rigorous control and the correction of batch-norm bugs in earlier preprints.

**Tags**: `#neuroscience`, `#machine learning`, `#CNN`, `#evaluation resolution`, `#brain-like models`

---

<a id="item-8"></a>
## [Moxie's Scrap Metal Tweet Sparks Debate on Poverty and Theft](https://twitter.com/moxie/status/2091218652133732491) ⭐️ 6.0/10

Moxie Marlinspike tweeted about scrap metal collection, which triggered a discussion on poverty, theft, and economic incentives. The tweet and its comments highlight the persistence of informal scrap collection and the economic pressures driving it. This discussion sheds light on the economic realities that drive informal recycling and theft, which have implications for urban infrastructure and public safety. It also reflects broader societal attitudes toward poverty and work, relevant to policymakers and community planners. The tweet is from Moxie Marlinspike, and comments reference specific scrap prices: copper at ~$5/lb and steel at $0.04/lb. One commenter notes that the post was written in 2006 but only published recently, indicating a time lag.

hackernews · tosh · Aug 22, 18:08 · [Discussion](https://news.ycombinator.com/item?id=49402189)

**Background**: Scrap metal collection is a common informal economic activity, especially in urban areas, where individuals gather discarded metals to sell for recycling. The value of metals like copper and steel fluctuates with market demand, and theft of metal from infrastructure (e.g., electrical equipment) has been a recurring problem. The discussion also touches on the stereotype that poor people are 'lazy,' countering it with examples of hard work in informal sectors.

**Discussion**: Commenters shared personal anecdotes about scrap collection, such as items disappearing quickly in Pittsburgh, and discussed the economic incentives behind metal theft. Some lamented the loss of personal blogging culture, while others noted the post's age. Overall, the sentiment was thoughtful and reflective, with a mix of nostalgia and social commentary.

**Tags**: `#economics`, `#social commentary`, `#scrap metal`, `#poverty`, `#community discussion`

---

<a id="item-9"></a>
## [Racket Intro Criticized as Speedrun, Not Friendly](https://geometridae.bearblog.dev/a-friendly-introduction-to-racket/) ⭐️ 6.0/10

A blog post titled 'A Friendly Introduction to Racket' was published, aiming to introduce Racket but assuming prior knowledge, leading to community criticism that it is more of a speedrun than a friendly tutorial. This discussion highlights the challenge of creating accessible programming language tutorials, especially for Lisp dialects like Racket, and reflects broader concerns about Racket's real-world adoption and deployment. The article covers Racket's syntax and features but assumes familiarity with concepts like lambda. Community members noted the lack of beginner-friendly explanations and pointed to deployment issues as a barrier to adoption.

hackernews · signa11 · Aug 22, 14:08 · [Discussion](https://news.ycombinator.com/item?id=49399898)

**Background**: Racket is a modern dialect of Lisp, descended from Scheme, designed for programming language design and implementation. It features a powerful macro system and is used in education and research, but its deployment options are often cited as a weakness compared to more mainstream languages.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Racket_(programming_language)">Racket (programming language)</a></li>
<li><a href="https://racket-lang.org/">Racket</a></li>
<li><a href="https://beautifulracket.com/appendix/why-racket-why-lisp.html">Beautiful Racket : Why Racket ? Why Lisp ?</a></li>

</ul>
</details>

**Discussion**: Comments criticized the tutorial for assuming prior knowledge, with one user calling it a 'speedrun'. Others shared resources like Racket Stories, and a user lamented that Racket is rarely used in production due to deployment challenges.

**Tags**: `#Racket`, `#Lisp`, `#Programming Languages`, `#Tutorial`

---

<a id="item-10"></a>
## [Z80 Microprocessor: 1970s Chip Still Thrives in Retrocomputing](https://www.computer.org/csdl/magazine/mi/2021/06/09623402/1yJTvlRLmhi) ⭐️ 6.0/10

An article from IEEE Computer Society highlights the enduring relevance of the Z80 microprocessor, a 1970s chip, and community members share nostalgic and technical perspectives on its continued use. The Z80's longevity demonstrates the lasting impact of simple, efficient processor designs, influencing retrocomputing enthusiasts and embedded systems. It also highlights a niche but passionate community that values low-level programming and historical technology. The Z80 is known for its simplicity and ease of programming, making it a favorite for assembly language hobbyists. It was used in systems like the ZX Spectrum and TRS-80, and its architecture has been studied in classic textbooks.

hackernews · asdefghyk · Aug 22, 09:49 · [Discussion](https://news.ycombinator.com/item?id=49398158)

**Background**: The Z80 is an 8-bit microprocessor introduced by Zilog in 1976, widely used in home computers and embedded systems. Its architecture is based on the Intel 8080 but with enhancements, and it remains popular for retrocomputing projects and education.

<details><summary>References</summary>
<ul>
<li><a href="https://archive.org/details/Z80_Microprocessor_1988_Macmillan_Publishing">The Z - 80 microprocessor : architecture , interfacing... : Internet Archive</a></li>
<li><a href="https://archive.org/download/Z-80_Assembly_Language_Programming">Z - 80 _ Assembly _ Language _ Programming directory listing</a></li>
<li><a href="https://epdf.pub/z-80-and-8080-assembly-language-programming.html">Z - 80 and 8080 assembly language programming - PDF Free...</a></li>

</ul>
</details>

**Discussion**: Community comments reflect nostalgia and technical appreciation, with mentions of Tom Jennings' modern Z80 computer, the fun of assembly programming on a ZX Spectrum emulator, and a question about mainframes based on the Z80. Overall sentiment is positive and enthusiastic.

**Tags**: `#retrocomputing`, `#Z80`, `#microprocessors`, `#assembly`, `#history`

---

<a id="item-11"></a>
## [llm 0.33 Release: OpenAI 3.x Upgrade and Embedding Key Support](https://simonwillison.net/2026/Aug/22/llm/) ⭐️ 5.0/10

llm 0.33 has been released, upgrading to the OpenAI Python library 3.x and switching the HTTP client dependency from httpx to httpx2. It also adds --key support for embedding commands and methods, and allows repeating -t/--template to combine templates. This release enhances the llm CLI tool's compatibility with the latest OpenAI library and improves flexibility for embedding workflows and template composition. It matters for developers who rely on llm for interacting with large language models, as it ensures smoother integration and more powerful command-line usage. The upgrade to OpenAI Python library 3.x and httpx2 addresses compatibility issues, with a quick 0.32.1 fix released earlier. Embedding models now support per-call keys via --key, with a compatibility fallback for existing plugins. The new reasoning_summary option for Responses API models supports auto, concise, and detailed values.

rss · Simon Willison · Aug 22, 17:01

**Background**: llm is a CLI utility and Python library for interacting with large language models, allowing users to run prompts or start chats against OpenAI-compatible endpoints. The OpenAI Python library provides convenient access to the OpenAI REST API, and httpx2 is a continuation of the HTTPX HTTP client library. These updates ensure llm stays current with the evolving ecosystem.

<details><summary>References</summary>
<ul>
<li><a href="https://llm.datasette.io/en/stable/">LLM : A CLI utility and Python library for interacting with Large...</a></li>
<li><a href="https://github.com/simonw/llm">GitHub - simonw/ llm : Access large language models from the...</a></li>
<li><a href="https://developers.openai.com/api/reference/python">OpenAI Python API library | OpenAI API Reference</a></li>
<li><a href="https://pypi.org/project/httpx2/">httpx 2 · PyPI</a></li>

</ul>
</details>

**Tags**: `#llm`, `#release`, `#CLI`, `#OpenAI`, `#embeddings`

---

<a id="item-12"></a>
## [LightGBM vs CatBoost: Why CatBoost Fits Interaction Toy Example Better](https://www.reddit.com/r/MachineLearning/comments/1vv7wx3/why_does_lightgbm_not_fit_my_toy_example_but/) ⭐️ 5.0/10

A Reddit user reported that LightGBM failed to fit a toy regression dataset with second-order interactions, even when the interaction variable was provided, while CatBoost fit the data perfectly using only the main effects. The user's experiments showed LightGBM predicting constant values or partial fits, contrary to expectations. This highlights practical differences in how gradient boosting libraries handle feature interactions, which can affect model performance on datasets with interaction effects. Understanding these differences helps practitioners choose the right tool and set appropriate hyperparameters for their data. The user used a dataset with two binary features (A, B) and a target y, where the mean of y is the same for each level of A and B, but the interaction AB determines y. LightGBM with min_child_samples=1 failed to fit the interaction even when AB was provided as a numeric or categorical feature, while CatBoost with min_data_in_leaf=1 fit perfectly using only A and B.

reddit · r/MachineLearning · /u/Phunfactory · Aug 22, 09:37

**Background**: Gradient boosting machines (GBMs) like LightGBM and CatBoost build an ensemble of decision trees, where each tree learns to correct the errors of previous trees. Feature interactions are captured when trees split on multiple features, but the ability to model interactions depends on the tree growth strategy and hyperparameters. LightGBM uses leaf-wise growth, which can be efficient but may miss interactions if the tree depth is limited, while CatBoost uses symmetric trees and has a different splitting strategy that may capture interactions more readily.

<details><summary>References</summary>
<ul>
<li><a href="https://codesignal.com/learn/courses/evaluating-and-finalizing-your-feature-driven-model-1/lessons/lightgbm-feature-engineering">LightGBM Feature Engineering | CodeSignal Learn</a></li>
<li><a href="https://coderzcolumn.com/tutorials/machine-learning/lightgbm-an-in-depth-guide-python">LightGBM - An In-Depth Guide [Python API]</a></li>
<li><a href="https://nustat.github.io/STAT303-3-class-notes/Lec11_More+boosting+models.html">13 LightGBM and CatBoost – Data Science III with python (Class notes)</a></li>

</ul>
</details>

**Tags**: `#LightGBM`, `#CatBoost`, `#gradient boosting`, `#feature interactions`, `#machine learning`

---

<a id="item-13"></a>
## [AI Startup Naming Trend Spoofed in 'ElevenLabs, TwelveLabs, ThirteenLabs'](https://quantumi.sh/public/labs.html) ⭐️ 4.0/10

A humorous Hacker News post titled 'ElevenLabs, TwelveLabs, ThirteenLabs' went viral, poking fun at the trend of AI startups adopting numeric-suffixed names. The post, hosted at quantumi.sh, lists fictional labs and sparked community jokes and links to real companies like Twelve Labs and 41Labs. This post highlights a notable naming pattern in the AI industry, reflecting how startups seek to appear innovative and scalable. The viral engagement underscores community interest in branding trends, which can influence how new companies position themselves. The post includes links to real companies such as Twelve Labs (twelvelabs.io) and 41Labs (41labs.ai), and mentions a co-hosted '23Labs Hackathon' by Twelve Labs and ElevenLabs. The author, quantumish, expressed surprise at the traffic, noting the server wasn't built for it.

hackernews · jemoka · Aug 22, 14:54 · [Discussion](https://news.ycombinator.com/item?id=49400408)

**Background**: AI startups often adopt names that sound futuristic and scalable, with numeric suffixes like 'ElevenLabs' or 'TwelveLabs' becoming common. This naming trend is part of a broader branding strategy to stand out in a crowded market, but it also invites parody and criticism for being formulaic.

**Discussion**: Community comments were largely humorous, with users sharing similar lab names like 1337labs.org and joking about registering names like 'sixsevenlabs'. Some pointed out that 41labs.ai looks like an AI-designed website, adding to the satire.

**Tags**: `#AI`, `#startups`, `#naming`, `#humor`

---

<a id="item-14"></a>
## [Researcher Seeks Help After ACL ARR Desk Rejection Over Phantom Prior Review](https://www.reddit.com/r/MachineLearning/comments/1vvd9ub/acl_arr_august_2026_desk_rejected_d/) ⭐️ 4.0/10

A researcher reported that two of their papers were desk rejected by ACL ARR because the program chairs claimed the papers had been previously reviewed in ARR, but the authors insist they were never submitted. The rejection occurred in the August 2026 cycle, and the researcher is seeking advice on how to appeal or resolve the issue. This incident highlights potential procedural errors in the ACL ARR system that can unfairly penalize authors, which is concerning for the NLP research community. It underscores the need for transparent and accurate record-keeping in academic publishing, as false claims of prior review can lead to unjust desk rejections and wasted effort. The desk rejection was based on the claim that the papers had been previously reviewed in ARR, but the authors state they never submitted them. The researcher is asking for advice on possible actions, such as contacting the program chairs or appealing the decision. The ACL ARR guidelines reserve the right to desk reject submissions that violate requirements, but this case appears to be a mistaken identity or record-keeping error.

reddit · r/MachineLearning · /u/malakulmout347 · Aug 22, 14:02

**Background**: ACL Rolling Review (ARR) is a peer-review platform used by ACL conferences, where papers are reviewed once and then committed to a specific conference. Desk rejection is a quick rejection without full review, often due to violations of submission requirements. In this case, the program chairs may have mistakenly matched the papers to previous submissions, possibly due to similar titles or author names, leading to an erroneous desk rejection.

<details><summary>References</summary>
<ul>
<li><a href="https://aclrollingreview.org/authorchecklist">Authors Beware: Common Submission Problems – ACL Rolling...</a></li>
<li><a href="https://2026.emnlp.org/concerning-late-desk-rejections/">Concerning late ACL 2026 desk rejections - EMNLP 2026</a></li>
<li><a href="https://2026.aclweb.org/calls/main_conference_papers/">Main Conference - ACL 2026</a></li>

</ul>
</details>

**Discussion**: The Reddit thread likely contains comments from other researchers who have experienced similar desk rejections or offer advice on how to appeal. Common suggestions may include contacting the ARR editors or program chairs directly, providing evidence of non-submission, and checking for any accidental duplicate submissions. Some may express frustration with the ARR process and call for better error handling.

**Tags**: `#ACL ARR`, `#desk rejection`, `#academic publishing`, `#NLP`, `#research process`

---

<a id="item-15"></a>
## [Canada to Match US Tariffs 'Dollar for Dollar' as Talks Collapse](https://www.bbc.com/news/articles/cvgvyy4x2mvo) ⭐️ 3.0/10

Canada announced it will retaliate against US tariffs with matching 'dollar for dollar' measures after trade negotiations broke down. The announcement was made in a statement by Prime Minister Carney on August 21, 2026. This escalation could significantly impact cross-border trade and supply chains, affecting industries in both countries. It also signals a broader trend of trade tensions that may influence global economic stability and tech-related manufacturing. The retaliatory tariffs will be applied 'dollar for dollar' to match US tariffs, though specific products and rates have not yet been detailed. The move follows the breakdown of trade talks and reflects Canada's firm stance against US trade policies.

hackernews · tartoran · Aug 22, 06:16 · [Discussion](https://news.ycombinator.com/item?id=49397074)

**Background**: Trade tariffs are taxes imposed on imported goods, often used to protect domestic industries or as leverage in negotiations. The US and Canada have a long-standing trade relationship, and recent US tariff policies have strained this relationship, leading to retaliatory measures.

**Discussion**: Comments on Hacker News show mixed reactions. Some support Canada's move as necessary to counter US aggression, while others criticize the US administration's policies as disastrous. There is also discussion about the potential for Canada to pivot closer to China and the missed opportunity for collective global action.

**Tags**: `#trade`, `#tariffs`, `#politics`, `#economy`

---