---
layout: default
title: "Horizon Summary: 2026-07-03 (EN)"
date: 2026-07-03
lang: en
---

> From 20 items, 16 important content pieces were selected

---

1. [EU Spyware Committee Member Hacked with Pegasus](#item-1) ⭐️ 8.0/10
2. [Ubicloud advocates strict memory overcommit for PostgreSQL](#item-2) ⭐️ 8.0/10
3. [Wordgard: New Rich-Text Editor from ProseMirror Creator](#item-3) ⭐️ 8.0/10
4. [Current AI Launches Open Source AI Gap Map](#item-4) ⭐️ 8.0/10
5. [CDD recovers finetuning data from logits only](#item-5) ⭐️ 8.0/10
6. [Guide to Running SOTA LLMs Locally](#item-6) ⭐️ 7.0/10
7. [Costco's Success: Avoiding Last-Mile Delivery](#item-7) ⭐️ 7.0/10
8. [Valve Open-Sources Steam Machine E-Ink Screen Design](#item-8) ⭐️ 7.0/10
9. [Cost Hack: Convert Code to Images, Use OCR for LLMs](#item-9) ⭐️ 7.0/10
10. [Course Creator Reports 50%+ Sales Drop Due to AI](#item-10) ⭐️ 7.0/10
11. [H64LM: 249M MoE Transformer Built from Scratch in PyTorch](#item-11) ⭐️ 7.0/10
12. [Is Fine-Tuning Resistance a Meaningful Safety Goal for Open-Weight LLMs?](#item-12) ⭐️ 7.0/10
13. [Factories Are Just Rooms: Demystifying Manufacturing](#item-13) ⭐️ 6.0/10
14. [Let AI Coding Assistants Use Their Own Judgement](#item-14) ⭐️ 6.0/10
15. [Simon Willison's June 2026 Sponsors Newsletter](#item-15) ⭐️ 4.0/10
16. [Is Tom Yeh's AI by Hand Course Worth It?](#item-16) ⭐️ 3.0/10

---

<a id="item-1"></a>
## [EU Spyware Committee Member Hacked with Pegasus](https://citizenlab.ca/research/member-of-committee-investigating-spyware-hacked-with-pegasus/) ⭐️ 8.0/10

Citizen Lab confirmed that Stelios Kouloglou, a member of the European Parliament's committee investigating spyware, was infected with Pegasus spyware on multiple occasions in 2022 and 2023. This incident underscores the threat of state-sponsored surveillance targeting democratic oversight bodies, potentially compromising sensitive investigations and undermining trust in EU institutions. The infections occurred on October 21, 2022, and March 6-7, 2023, and the device also contained confidential medical and government documents, raising concerns about data separation policies.

hackernews · ledoge · Jul 3, 20:38 · [Discussion](https://news.ycombinator.com/item?id=48779683)

**Background**: Pegasus is a powerful spyware developed by Israel's NSO Group, capable of remotely compromising mobile devices via zero-click exploits. Citizen Lab is a leading research organization that investigates digital threats to human rights and has exposed numerous Pegasus abuses worldwide.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pegasus_(spyware)">Pegasus (spyware)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Citizen_Lab">Citizen Lab</a></li>

</ul>
</details>

**Discussion**: Commenters noted that using hardened devices like GrapheneOS could have prevented the attack, and criticized Apple and Google for not making lockdown features more accessible. Some pointed out that Greece and other EU states have been implicated in Pegasus abuse, suggesting internal EU surveillance rather than external attack.

**Tags**: `#cybersecurity`, `#spyware`, `#Pegasus`, `#European Parliament`, `#surveillance`

---

<a id="item-2"></a>
## [Ubicloud advocates strict memory overcommit for PostgreSQL](https://www.ubicloud.com/blog/postgresql-and-the-oom-killer-why-we-use-strict-memory-overcommit) ⭐️ 8.0/10

Ubicloud published a blog post explaining why they use strict memory overcommit (vm.overcommit_memory=2) for PostgreSQL to avoid OOM killer disruptions, and the community discussion highlights trade-offs and cautionary advice. This matters because PostgreSQL is sensitive to memory overcommit; using strict mode can significantly reduce OOM killer incidents, improving database stability for production deployments. The discussion also reveals that the default Linux heuristic overcommit can cause system instability under memory pressure. Strict overcommit (mode 2) refuses allocations that exceed CommitLimit, preventing the OOM killer from killing PostgreSQL, but it can cause fork failures if overcommit ratios are adjusted. The author from Ubicloud acknowledges the title was too strong and that strict mode may have side effects in other scenarios.

hackernews · furkansahin · Jul 3, 13:00 · [Discussion](https://news.ycombinator.com/item?id=48774509)

**Background**: Linux memory overcommit allows processes to allocate more virtual memory than physical RAM plus swap, hoping not all memory is used simultaneously. When memory runs out, the OOM killer terminates processes to free memory. PostgreSQL, which allocates large shared memory buffers, is often a victim. Strict overcommit (mode 2) enforces a hard limit on total committed memory.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ubicloud.com/blog/postgresql-and-the-oom-killer-why-we-use-strict-memory-overcommit">PostgreSQL and the OOM Killer: Why We Use Strict Memory Overcommit</a></li>
<li><a href="https://www.kernel.org/doc/Documentation/vm/overcommit-accounting">The Linux kernel supports the following overcommit handling modes</a></li>
<li><a href="https://www.postgresql.org/docs/current/kernel-resources.html">PostgreSQL: Documentation: 18: 18.4. Managing Kernel Resources</a></li>

</ul>
</details>

**Discussion**: Commenters noted that Linux defaults are problematic under memory pressure, and one user cautioned that mode 2 can prevent forks if overcommit ratios are adjusted, recommending thorough testing. The Ubicloud author agreed the title was too strong, acknowledging that strict mode may have unanticipated side effects.

**Tags**: `#PostgreSQL`, `#Linux`, `#memory management`, `#OOM killer`, `#database administration`

---

<a id="item-3"></a>
## [Wordgard: New Rich-Text Editor from ProseMirror Creator](https://wordgard.net/) ⭐️ 8.0/10

Wordgard is a new in-browser rich-text editor released by the creator of ProseMirror, sharing many concepts with its predecessor but offering no upgrade path. This release is significant because it comes from a highly respected developer in the web editing space, potentially influencing the future of rich-text editing tools and sparking community discussion about design trade-offs. Wordgard shares many concepts with ProseMirror but is not an upgrade; switching requires significant rework. The editor features a fresh design by artist Kamilastankiewicz.

hackernews · indy · Jul 3, 08:50 · [Discussion](https://news.ycombinator.com/item?id=48772573)

**Background**: ProseMirror is a battle-tested, open-source rich-text editor framework known for its lightweight core and steep learning curve. It serves as the foundation for many editors like Tiptap. WYSIWYG (What You See Is What You Get) editors allow users to edit content in a form that resembles the final output, a concept that has been challenging to standardize on the web.

<details><summary>References</summary>
<ul>
<li><a href="https://prosemirror.net/">ProseMirror</a></li>

</ul>
</details>

**Discussion**: Community comments express excitement about the new editor, with some noting the lack of an upgrade path from ProseMirror as a potential hurdle. Users also appreciate the design and technical depth, with one commenter finding validation in the similarities to their own block-based approach.

**Tags**: `#rich-text editor`, `#ProseMirror`, `#web development`, `#WYSIWYG`, `#open source`

---

<a id="item-4"></a>
## [Current AI Launches Open Source AI Gap Map](https://simonwillison.net/2026/Jul/3/open-source-ai-gap-map/#atom-everything) ⭐️ 8.0/10

Current AI, a non-profit founded at the AI Action Summit in Paris in February 2025, launched the Open Source AI Gap Map v0.1, indexing 421 open source AI products across models, tools, datasets, and hardware, along with 24,400 additional artifacts. This comprehensive mapping provides a structured overview of the open source AI ecosystem, helping researchers and practitioners identify gaps and opportunities, and promoting transparency in a rapidly evolving field. The map details 266 software tools, 85 models, 50 datasets, and 20 hardware projects from 228 organizations, organized into 14 categories across three stack layers. The underlying data is released under an MIT license on GitHub, including 1,184 YAML files and scripts.

rss · Simon Willison · Jul 3, 22:04

**Background**: Current AI is a global non-profit partnership backed by $400 million in committed capital, aiming to build a public option for AI. The Gap Map is an attempt to systematically catalog the open source AI landscape, which has grown rapidly but lacks comprehensive indexing.

<details><summary>References</summary>
<ul>
<li><a href="https://www.multiminds.eu/news/ai-action-summit-paris-global-talk-with-local-impact/">AI Action Summit Paris : global talk with local impact | MultiMinds</a></li>

</ul>
</details>

**Tags**: `#open source`, `#AI`, `#ecosystem`, `#mapping`, `#non-profit`

---

<a id="item-5"></a>
## [CDD recovers finetuning data from logits only](https://www.reddit.com/r/MachineLearning/comments/1umn2dk/contrastive_decoding_diffing_cdd_recovering/) ⭐️ 8.0/10

Researchers introduce Contrastive Decoding Diffing (CDD), a grey-box method that recovers verbatim finetuning data from LLMs using only logit access, without needing model weights or activations. CDD outperforms prior white-box methods like Activation Difference Lens (ADL) on the SDF benchmark, achieving a verbatim recovery score of 4+/5 on 19/20 organism×model pairs, while ADL never exceeds 3/5. This has significant implications for ML safety and interpretability by enabling data recovery with minimal model access. A single default configuration works across four model families (1B to 32B parameters) without per-organism calibration or layer selection. An unplanned finding revealed that a fictional persona "Dr. Elena Rodriguez" appeared across semantically unrelated finetuning domains, traced back to Claude Sonnet 3.6's bias in synthetic data generation.

reddit · r/MachineLearning · /u/CebulkaZapiekana · Jul 3, 19:01

**Background**: Model diffing aims to identify and explain differences between a base model and its finetuned version. Prior work, Activation Difference Lens (ADL), required full weight access and could only recover vague domain-level descriptions. Contrastive Decoding (CD) is a technique that amplifies differences between a strong and weak model by contrasting their logits; CDD adapts this idea for model diffing.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/model-diffing">Model Diffing : Techniques & Applications</a></li>
<li><a href="https://www.lesswrong.com/w/model-diffing">Model Diffing — LessWrong</a></li>
<li><a href="https://arxiv.org/abs/2309.09117">[2309.09117] Contrastive Decoding Improves Reasoning in Large Language Models</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#interpretability`, `#LLM safety`, `#model diffing`, `#finetuning`

---

<a id="item-6"></a>
## [Guide to Running SOTA LLMs Locally](https://github.com/jamesob/local-llm) ⭐️ 7.0/10

Jamesob published a comprehensive guide on GitHub detailing how to run state-of-the-art LLMs locally, covering hardware setups from budget to high-end, including a $40K+ build with 4x $12K GPUs. This guide helps developers and enthusiasts understand the real costs and trade-offs of local LLM deployment, which is crucial for privacy, offline access, and avoiding API costs. The community discussion highlights that local setups can be far more expensive than cloud subscriptions, tempering expectations. The high-end build uses 4 GPUs at $12K each, totaling $50-55K, and relies on quantization to fit models into VRAM. A mid-range option suggests 2x RTX 3090s for 48GB VRAM to run Qwen3.6-27B, while an alternative is a $3K M5 MacBook Pro with 48GB unified memory.

hackernews · livestyle · Jul 3, 15:03 · [Discussion](https://news.ycombinator.com/item?id=48775921)

**Background**: Running large language models locally requires significant GPU memory (VRAM) to hold the model weights. Quantization reduces model precision to fit into available memory, but may degrade quality. Cloud services like Claude Opus cost ~$200/month, making local setups economical only for heavy usage or specific privacy needs.

<details><summary>References</summary>
<ul>
<li><a href="https://mofchemicals.com/local-llm-ollama-guide">Local LLM Deployment — Ollama</a></li>
<li><a href="https://talkingtech.io/running-llms-locally-with-ollama-in-2026/">Running LLMs Locally with Ollama in 2026</a></li>

</ul>
</details>

**Discussion**: Commenters warn that the $40K build actually costs $50-55K and that local models are still lower quality and potentially dangerous if backdoored. Some suggest mid-range options like 2x RTX 3090s or an M5 MacBook Pro, while others note that cloud subscriptions are cheaper for most users.

**Tags**: `#LLM`, `#local deployment`, `#hardware`, `#open-source`, `#deep learning`

---

<a id="item-7"></a>
## [Costco's Success: Avoiding Last-Mile Delivery](https://phenomenalworld.org/analysis/the-anti-amazon/) ⭐️ 7.0/10

An analysis article argues that Costco's business model thrives by eschewing the complexity of last-mile home delivery, instead focusing on warehouse-based bulk sales where customers transport goods themselves. This contrast highlights a fundamental strategic divergence in retail: prioritizing operational simplicity and cost efficiency (Costco) versus convenience and speed (Amazon), with implications for logistics, pricing, and customer behavior. Costco's model involves freight trucks delivering pallets to warehouses, where customers buy in bulk and drive home, avoiding the costly 'last mile' of individual home delivery that Amazon relies on.

hackernews · bookofjoe · Jul 3, 15:14 · [Discussion](https://news.ycombinator.com/item?id=48776044)

**Background**: Last-mile delivery refers to the final step of the delivery process, from a distribution center to the customer's door, which is often the most expensive and complex part of logistics. Costco operates membership-only warehouse clubs where customers purchase large quantities at low prices, while Amazon focuses on e-commerce with rapid home delivery.

**Discussion**: Commenters praised Costco's wisdom in avoiding the last-mile problem, with one quoting a proverb: 'A clever person solves a problem; a wise person avoids it.' Others noted that Costco also offers delivery via Instacart, and that international perspectives (e.g., UK) show membership is originally for businesses but accessible to all.

**Tags**: `#retail`, `#logistics`, `#business strategy`, `#e-commerce`

---

<a id="item-8"></a>
## [Valve Open-Sources Steam Machine E-Ink Screen Design](https://www.gamingonlinux.com/2026/07/valve-open-source-the-steam-machine-e-ink-screen-so-you-can-make-your-own/) ⭐️ 7.0/10

Valve has released the CAD files, firmware, and STL files for the e-ink faceplate (dubbed "Inkterface") of the Steam Machine, allowing anyone to build their own. This move empowers the DIY community to create custom e-ink displays for the Steam Machine, fostering innovation and extending the lifespan of a niche product. The display is a standard Adafruit 5.83-inch e-ink panel (product 6397), and Valve plans to offer a pre-built "Inkterface" later this year.

hackernews · ahlCVA · Jul 3, 13:01 · [Discussion](https://news.ycombinator.com/item?id=48774518)

**Background**: The Steam Machine is a console-like PC from Valve, featuring interchangeable faceplates. The e-ink faceplate was a highlight at its reveal, but was not initially available for purchase. By open-sourcing the design, Valve enables enthusiasts to create their own versions.

<details><summary>References</summary>
<ul>
<li><a href="https://www.gamingonlinux.com/2026/07/valve-open-source-the-steam-machine-e-ink-screen-so-you-can-make-your-own/">Valve open source the Steam Machine e - ink screen ... | GamingOnLinux</a></li>
<li><a href="https://www.digitalfoundry.net/news/2026/07/valve-releases-steam-machine-e-ink-faceplate-cad-files-and-firmware">Valve releases Steam Machine e - ink faceplate CAD... | Digital Foundry</a></li>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2pnbUpuQkVSRWxnTUZnbDgzZEJDZ0FQAQ?hl=en-US&gl=US&ceid=US:en">Valve open-sources "Inkterface" e - ink screen for Steam Machine ...</a></li>

</ul>
</details>

**Discussion**: Community members praised Valve's openness, with one user wishing more companies would follow suit. Others discussed adapting the design for other devices like the Framework Desktop, and inquired about larger e-ink screens with HDMI or USB-C input.

**Tags**: `#open-source`, `#hardware`, `#gaming`, `#e-ink`, `#valve`

---

<a id="item-9"></a>
## [Cost Hack: Convert Code to Images, Use OCR for LLMs](https://github.com/teamchong/pxpipe) ⭐️ 7.0/10

A GitHub project called pxpipe reduces LLM costs by converting code into images and using OCR to extract text, exploiting a token accounting loophole where image tokens are cheaper than text tokens. This hack offers a novel cost optimization for heavy LLM users, potentially saving significant money on prompt processing, though it may be closed if providers adjust token pricing. The technique relies on the fact that many LLM APIs charge less per image token than per text token, even though the model internally processes both. However, it may increase completion tokens and latency, as noted by a prior attempt with OpenAI models.

hackernews · dimitropoulos · Jul 3, 15:50 · [Discussion](https://news.ycombinator.com/item?id=48776464)

**Background**: LLMs process text by breaking it into tokens, and APIs charge based on token count. Image inputs are typically tokenized differently (e.g., into patches) and often priced lower per token. This discrepancy creates a loophole: by rendering text as an image and using OCR, users can reduce billed tokens.

**Discussion**: Community comments highlight that this is likely a token accounting loophole that may be closed, similar to how Gemini processes PDFs without charging for text tokens. Some note prior art from last year with OpenAI models, which was ultimately more expensive due to increased completion tokens. Others sarcastically remark that this is rediscovering compressed binary formats.

**Tags**: `#LLM`, `#cost optimization`, `#OCR`, `#prompt engineering`, `#hack`

---

<a id="item-10"></a>
## [Course Creator Reports 50%+ Sales Drop Due to AI](https://simonwillison.net/2026/Jul/3/josh-w-comeau/#atom-everything) ⭐️ 7.0/10

Josh W. Comeau, creator of popular web development courses, reported that his new course 'Whimsical Animations' is on track to sell only one-third as many copies as typical launches, and his existing courses have seen sales drop by over 50% compared to last year. This provides concrete evidence that AI is disrupting the developer education market, both by reducing demand for learning due to job uncertainty and by offering free or low-cost personalized tutoring via LLMs, threatening the business model of paid course creators. Comeau attributes the decline to a 'double whammy': developers are reluctant to invest time and money in learning new skills due to fears that AI will eliminate developer jobs, and LLMs can now serve as personalized tutors, reducing the need for structured courses. He notes that other course creators are seeing similar trends.

rss · Simon Willison · Jul 3, 21:25

**Background**: Josh W. Comeau is a well-known educator in the web development community, particularly for his course 'CSS for JavaScript Developers'. The rise of large language models (LLMs) like GPT-4 has enabled AI-powered tutoring that can adapt to individual learners, posing a direct challenge to traditional paid online courses.

<details><summary>References</summary>
<ul>
<li><a href="https://joshcomeau.org/">Josh W Comeau</a></li>
<li><a href="https://medium.com/age-of-awareness/ai-in-education-personalized-learning-with-llms-57405e34446a">AI in Education: Personalized Learning with LLMs | Medium</a></li>
<li><a href="https://www.eritheialabs.com/blog/llms-in-education-empowering-personalized-learning-experiences">LLMs in Education: Personalized Learning Revolution | Eritheia Labs</a></li>

</ul>
</details>

**Tags**: `#AI impact`, `#developer education`, `#online courses`, `#LLMs`, `#tech industry trends`

---

<a id="item-11"></a>
## [H64LM: 249M MoE Transformer Built from Scratch in PyTorch](https://www.reddit.com/r/MachineLearning/comments/1umqfd2/h64lm_a_249mparameter_mixtureofexperts/) ⭐️ 7.0/10

A developer released H64LM, a 249M-parameter Mixture-of-Experts Transformer implemented entirely from scratch in PyTorch, featuring GQA, SwiGLU, RoPE, and a custom training loop. The project includes a checkpoint trained on WikiText-103 and is shared as an open-source educational resource. This project provides a rare, transparent, from-scratch implementation of a modern MoE Transformer, making advanced LLM architecture accessible for learning and experimentation. It helps bridge the gap between high-level frameworks and deep understanding of model internals. The model uses 8 experts with Top-2 routing, three auxiliary routing losses, sliding-window attention, mixed-precision training, and gradient accumulation. Known limitations include batch-size-1-only generation and fallback to DataParallel instead of true DDP.

reddit · r/MachineLearning · /u/Loose_Literature6090 · Jul 3, 21:18

**Background**: Mixture-of-Experts (MoE) is a neural network architecture that activates only a subset of parameters per input, enabling larger models with similar computational cost. Grouped Query Attention (GQA) groups queries to share key/value projections, improving inference efficiency. This project implements these techniques from scratch, avoiding high-level training frameworks like Hugging Face Trainer.

<details><summary>References</summary>
<ul>
<li><a href="https://verticalserve.medium.com/group-query-attention-58283b337c65">Attention Variations — MQA vs GQA vs MHA vs MLA | Medium</a></li>
<li><a href="https://www.emergentmind.com/topics/grouped-query-attention-6898a326-0eb0-4eae-a81c-5a5d5b7dce0c">Grouped - Query Attention in Transformers</a></li>
<li><a href="https://www.linkedin.com/pulse/accelerating-transformer-inference-grouped-query-attention-bhabani-n-oafcc">Accelerating Transformer Inference with Grouped Query Attention ...</a></li>

</ul>
</details>

**Tags**: `#Mixture-of-Experts`, `#Transformer`, `#PyTorch`, `#LLM`, `#Open Source`

---

<a id="item-12"></a>
## [Is Fine-Tuning Resistance a Meaningful Safety Goal for Open-Weight LLMs?](https://www.reddit.com/r/MachineLearning/comments/1um9bs7/what_does_safe_ai_look_like_d/) ⭐️ 7.0/10

A Reddit discussion questions whether fine-tuning resistance is a practical safety goal for open-weight LLMs, given that uncensored variants appear rapidly after release and safety measures can be bypassed easily. This debate highlights a fundamental tension in AI safety: if safety training can be undone in minutes, its value for open-weight models is questionable, affecting governance and release strategies. The discussion notes that automated scripts can remove safety refusals within 30 minutes, and defenses like TAR and SEAM are susceptible to non-fine-tuning attacks, as shown in recent research.

reddit · r/MachineLearning · /u/Aaron_Rock · Jul 3, 09:07

**Background**: Open-weight LLMs have publicly available model weights, allowing anyone to fine-tune them. Safety training aims to prevent harmful outputs, but fine-tuning can weaken these guardrails. Recent work shows that even dedicated fine-tuning defenses can be bypassed by simple methods.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2605.26526">Open - Weight LLM Fine - Tuning Defenses are Susceptible to Simple...</a></li>
<li><a href="https://www.libertify.com/interactive-library/open-weight-llm-risks-malicious-fine-tuning-analysis/">Open - Weight LLM Risks: Malicious Fine - Tuning Analysis —.</a></li>
<li><a href="https://groundy.com/articles/why-fine-tuning-strips-safety-alignment-from-open-weight-llms/">Why Fine - Tuning Strips Safety Alignment From Open - Weight LLMs...</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#open-weight models`, `#fine-tuning`, `#LLM security`, `#governance`

---

<a id="item-13"></a>
## [Factories Are Just Rooms: Demystifying Manufacturing](https://interconnected.org/home/2026/07/03/factories) ⭐️ 6.0/10

An essay argues that factories are fundamentally just rooms where people make things, challenging the perception of manufacturing as a mysterious or inaccessible domain. This perspective encourages a maker mindset and could inspire more individuals and small teams to start manufacturing, potentially reshaping local economies and innovation. The essay is published on interconnected.org and has generated 71 comments discussing practical examples and counterpoints, such as the efficiency of fast-food kitchens as factories.

hackernews · arbesman · Jul 3, 15:13 · [Discussion](https://news.ycombinator.com/item?id=48776035)

**Background**: Manufacturing is often seen as requiring large-scale, specialized facilities. The essay demystifies this by comparing factories to any room where production happens, from a kitchen to a workshop.

**Discussion**: Commenters share personal experiences, like running a small factory or working at a machine-builder, and debate whether the 'just a room' view overlooks the importance of specialized equipment and scale.

**Tags**: `#manufacturing`, `#maker culture`, `#essay`, `#technology`

---

<a id="item-14"></a>
## [Let AI Coding Assistants Use Their Own Judgement](https://simonwillison.net/2026/Jul/3/judgement/#atom-everything) ⭐️ 6.0/10

Simon Willison shared a tip from the Claude Code team: instead of dictating how Fable should work, let it use its own judgement for tasks like testing and model selection. He also prompted Claude Code to delegate coding tasks to lower-power subagents, which saved Fable tokens. This approach improves efficiency and reduces costs by avoiding unnecessary use of top-tier models for trivial tasks. It demonstrates a practical prompt engineering technique that can help developers get more done with limited AI allowances. The tip was shared during a Fireside Chat at AIE with Cat Wu and Thariq Shihipar from the Claude Code team. Jesse Vincent also suggested telling Fable to use other models for smaller tasks. Simon's prompt caused Claude to save a memory file that delegates coding to subagents using Sonnet or Haiku models.

rss · Simon Willison · Jul 3, 18:51

**Background**: Fable is a high-end AI coding assistant from Anthropic, based on Claude Fable 5, which excels at complex tasks like UI design and game coding. However, its tokens are expensive and limited. Prompt engineering techniques like delegating to subagents help balance performance and cost.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#AI coding assistants`, `#Claude Code`, `#Fable`, `#prompt engineering`

---

<a id="item-15"></a>
## [Simon Willison's June 2026 Sponsors Newsletter](https://simonwillison.net/2026/Jul/3/june-newsletter/#atom-everything) ⭐️ 4.0/10

Simon Willison released his June 2026 sponsors-only monthly newsletter, covering topics like Claude Fable 5, GPT-5.6, US export restrictions, GLM-5.2 as the best open weights model, Datasette Apps, and other updates. This newsletter provides early access to curated insights on AI model releases and open-source tools for sponsors, reflecting the rapid pace of AI development and the importance of community support. The newsletter is available to GitHub sponsors at $10/month, and a preview of the May newsletter is linked. Topics include tokenmaxxing, WASM projects, and tools like sqlite-utils and shot-scraper.

rss · Simon Willison · Jul 3, 14:50

**Background**: Simon Willison is the creator of Datasette, an open-source tool for exploring and publishing SQLite databases. He also maintains shot-scraper for automated screenshots and other open-source projects. His monthly newsletter aggregates updates on AI, open-source, and his own projects.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Datasette">Datasette</a></li>
<li><a href="https://github.com/simonw/shot-scraper">GitHub - simonw/ shot - scraper : A command-line utility for taking...</a></li>
<li><a href="https://simonwillison.net/2022/Mar/10/shot-scraper/">shot - scraper : automated screenshots for documentation, built on...</a></li>

</ul>
</details>

**Tags**: `#newsletter`, `#AI`, `#Datasette`, `#open source`

---

<a id="item-16"></a>
## [Is Tom Yeh's AI by Hand Course Worth It?](https://www.reddit.com/r/MachineLearning/comments/1umqf58/tom_yehs_ai_by_hand_is_it_worth_it_d/) ⭐️ 3.0/10

A Reddit user asked for opinions on Tom Yeh's 'AI by Hand' course to strengthen machine learning understanding for building tools with Hugging Face models. This reflects a common need among practitioners to find effective learning resources that bridge theory and practical AI tool building. The course is offered by Prof. Tom Yeh via Substack and includes hands-on exercises like calculating MoE models by hand; the user is considering a two-month subscription.

reddit · r/MachineLearning · /u/TheSmashingChamp · Jul 3, 21:17

**Background**: Tom Yeh's 'AI by Hand' is a Substack publication that teaches AI concepts through manual calculations and exercises. Hugging Face is a platform hosting open-source AI models, commonly used by developers to integrate AI into applications.

<details><summary>References</summary>
<ul>
<li><a href="https://www.byhand.ai/">AI by Hand | Prof. Tom Yeh | Substack</a></li>
<li><a href="https://www.byhand.ai/p/ai-by-hand-academy-5ec">AI by Hand Academy - by Prof. Tom Yeh - AI by Hand</a></li>
<li><a href="https://huggingface.co/">Hugging Face – The AI community building the future.</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#learning resources`, `#course review`

---