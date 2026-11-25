---
layout: default
title: "Horizon Summary: 2026-11-25 (EN)"
date: 2026-11-25
lang: en
---

> From 9 items, 9 important content pieces were selected

---

1. [OpenAI preprint claims matrix multiplication exponent is exactly 9/4](#item-1) ⭐️ 10.0/10
2. [Ternary Bonsai 2.5 27B: Tiny Ternary Model Matches Frontier on SWE-bench](#item-2) ⭐️ 8.0/10
3. [OpenAI's GPT-6.2 designs protein minibinders by writing code](#item-3) ⭐️ 8.0/10
4. [Check Point servers breached via V8 PRNG state reconstruction](#item-4) ⭐️ 8.0/10
5. [Simon Willison Identifies Three LLM Inflection Points in Twelve Months](#item-5) ⭐️ 8.0/10
6. [GPT-6.2 Astra Solves 1808 Sketchbook Mystery in 22 Minutes](#item-6) ⭐️ 8.0/10
7. [PenGPT: A Generative Transformer for Handwriting and Sketches](#item-7) ⭐️ 7.0/10
8. [Hacker News Discusses Helsinki's Gödel Enigma Project](#item-8) ⭐️ 7.0/10
9. [uv 0.13.10 Released with Security Fix and Lockfile Validation](#item-9) ⭐️ 5.0/10

---

<a id="item-1"></a>
## [OpenAI preprint claims matrix multiplication exponent is exactly 9/4](https://github.com/openai/math/blob/main/preprints/The-matrix-multiplication-exponent-is-nine-fourths-November-24-2026/paper.pdf) ⭐️ 10.0/10

OpenAI posted a preprint on its public openai/math GitHub repository on November 24, 2026, claiming that the matrix multiplication exponent ω is exactly 9/4 (2.25) over every field, with a matching lower bound. This follows an earlier October 2026 preprint that gave an upper bound over the complex numbers. This is a major theoretical computer science result because it pins down the exact asymptotic complexity of matrix multiplication, a fundamental operation used throughout scientific computing, machine learning, and graph algorithms. If verified, it would be the biggest shift in the matrix multiplication exponent since 1979 and would refute the long-standing conjecture that ω = 2. The result has not been peer reviewed, and the preprint reportedly comes from an unreleased OpenAI model whose recipe is not disclosed. The claimed exponent 9/4 is higher than the current best known upper bound of about 2.371, so the lower bound would close the gap if the proof holds.

hackernews · E-Reverance · Nov 25, 01:19 · [Discussion](https://news.ycombinator.com/item?id=50637220)

**Background**: The matrix multiplication exponent, denoted ω, is the smallest real number such that any two n×n matrices over a field can be multiplied using O(n^{ω+o(1)}) field operations. Trivially ω ≥ 2, and the conjecture that ω = 2 has been open for decades. The best known upper bound is around 2.371, achieved through advanced algebraic techniques, while lower bounds have remained close to 2.

<details><summary>References</summary>
<ul>
<li><a href="https://letsdatascience.com/news/openai-preprint-claims-matrix-multiplication-exponent-is-exa-7997d3b1">OpenAI preprint claims matrix multiplication exponent is ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Matrix_multiplication_algorithm">Matrix multiplication algorithm - Wikipedia</a></li>
<li><a href="https://prove2.me/campaigns/matmul-omega">Matrix multiplication exponent · Prove2Me</a></li>

</ul>
</details>

**Discussion**: Commenters noted that this paper is part of a set of four OpenAI papers resolving eight problems from a Top 500 open math problems list, including strongly polynomial linear programming and parity games. Some expressed skepticism about OpenAI holding back stronger internal models and about the lack of peer review, while others debated the practical significance given that the result is a lower bound and no efficient algorithm is provided.

**Tags**: `#matrix multiplication`, `#algorithms`, `#complexity theory`, `#OpenAI`, `#mathematics`

---

<a id="item-2"></a>
## [Ternary Bonsai 2.5 27B: Tiny Ternary Model Matches Frontier on SWE-bench](https://prismml.com/news/bonsai-2-5-27b) ⭐️ 8.0/10

PrismML released Ternary Bonsai 2.5 27B, a ternary-quantized model that reportedly matches frontier models on SWE-bench Verified while running efficiently on consumer hardware. The model builds on the Qwen3.8-27B hybrid-attention architecture and ternary weight format of Bonsai 2, achieving 1.76 bits per weight and a 5.93 GB footprint versus 53.8 GB for the FP16 model. This demonstrates that extremely low-bit quantization can preserve or even enhance agentic coding capabilities, potentially enabling powerful local AI assistants on everyday devices. It also fuels the debate on whether small models are catching up to frontier models and how reliable benchmarks like SWE-bench Verified are for measuring real-world performance. The model retains the Qwen3.8-27B hybrid-attention architecture and ternary weight format, using 1.76 bits per weight for a total size of 5.93 GB, compared to 53.8 GB for the FP16 version. It targets long-horizon, tool-driven work and shows improvements in agentic execution, coding, and multi-turn tool use over its predecessor.

hackernews · b0m · Nov 24, 20:08 · [Discussion](https://news.ycombinator.com/item?id=50633922)

**Background**: Ternary quantization reduces neural network weights to three values: -1, 0, and +1, often with a scaling factor, which drastically cuts memory and compute requirements. SWE-bench Verified is a benchmark that evaluates language models on resolving real GitHub issues from Python repositories, and it is widely used to measure coding and reasoning abilities. PrismML's Bonsai series explores ternary quantization to make large models deployable on consumer hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://prismml.com/news/bonsai-2-5-27b">PrismML — Introducing Ternary Bonsai 2 . 5 27 B : Powering Agentic...</a></li>
<li><a href="https://huggingface.co/prism-ml/Ternary-Bonsai-2.5-27B-GGUF">prism-ml/ Ternary - Bonsai - 2 . 5 - 27 B -GGUF · Hugging Face</a></li>
<li><a href="https://www.swebench.com/">SWE - bench Leaderboards</a></li>

</ul>
</details>

**Discussion**: Commenters reported hands-on results: one user achieved 22-25 tokens/s on a Mac Mini M5 Pro with 24GB RAM and easily fit 128k context, finding it potentially usable for agentic coding. Others debated whether the SWE-bench score reflects genuine progress or benchmark-maxxing, and some requested comparisons with equivalently small models like Qwen3.8 quantized to Q1/Q2. A self-created long-horizon benchmark showed Bonsai 2.5 completing tasks 29% faster than Bonsai 2 with 17% fewer steps, though both passed 5 of 8 tasks.

**Tags**: `#local-llm`, `#quantization`, `#ternary-models`, `#swe-bench`, `#agentic-coding`

---

<a id="item-3"></a>
## [OpenAI's GPT-6.2 designs protein minibinders by writing code](https://openai.com/index/gpt-6-models-demonstrate-intrinsic-protein-design-capabilities/) ⭐️ 8.0/10

OpenAI reported that GPT-6.2, given the 3D structures of five target proteins and desired attachment sites, wrote code to generate 3D designs for potential minibinders without using specialized protein AI models. The designs were then converted into amino acid sequences using the specialized model SolubleMPNN and filtered with other protein models for folding and binding. This demonstrates that general-purpose LLMs can act as a flexible 'glue layer' in complex scientific workflows, potentially lowering the barrier to protein design by automating code generation and tool integration. It also sparks debate about whether LLMs possess intrinsic protein-design capabilities or merely orchestrate specialized models. GPT-6.2 only produced 3D designs; converting them to sequences required SolubleMPNN, and other specialized models were used to predict folding and binding. Community members noted that the evidence is heavy on computational exploration and light on laboratory validation, and that the 'beyond specialized models' claim may be premature.

hackernews · acossta · Nov 24, 21:02 · [Discussion](https://news.ycombinator.com/item?id=50634658)

**Background**: Protein minibinders are small engineered proteins (typically under 100 amino acids) that can bind to specific targets with high affinity, and they are studied for therapeutic applications. Designing such proteins de novo often involves specialized AI models like AlphaFold for structure prediction and ProteinMPNN for sequence design, which are trained specifically for these tasks. LLMs like GPT-6.2 are general-purpose models that can write code, and their ability to coordinate specialized tools is being explored in scientific discovery.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nature.com/articles/s41467-025-56369-w">De novo design of protein minibinder agonists of TLR3 - Nature</a></li>
<li><a href="https://en.wikipedia.org/wiki/De_novo_protein_structure_prediction">De novo protein structure prediction - Wikipedia</a></li>
<li><a href="https://alphafold.ebi.ac.uk/">AlphaFold Protein Structure Database</a></li>

</ul>
</details>

**Discussion**: Commenters debated the novelty of GPT-6.2's contribution: some argued it acts as a 'glue layer' between specialized models and can outperform them at certain tasks, while others questioned what GPT-6.2 actually designed since the sequence is the structure for proteins. Concerns were also raised about the lack of laboratory controls and the premature 'beyond specialized models' framing.

**Tags**: `#AI`, `#protein-design`, `#LLM`, `#biotechnology`, `#code-generation`

---

<a id="item-4"></a>
## [Check Point servers breached via V8 PRNG state reconstruction](https://www.greynoise.io/blog/check-point-security-management-servers-intrusion-campaign) ⭐️ 8.0/10

An active intrusion campaign is exploiting Check Point security management servers by reconstructing the internal state of the V8 JavaScript engine's pseudo-random number generator (PRNG) from Math.random() outputs. Attackers collected session cookies from repeated logins to the HFS loginSrp1 endpoint, recovered the session-cookie signing key, and forged admin session cookies to breach over 22 organizations. This incident highlights the critical risk of using non-cryptographically secure PRNGs like Math.random() for security-sensitive operations, potentially affecting countless Node.js applications. It also underscores the growing sophistication of attacks and raises concerns about future AI-enabled cyberattacks. The attack exploits the predictability of V8's PRNG, which is seeded with a limited state and can be reconstructed from a small number of outputs. The campaign likely used CVE-2026-16232 as an initial vector, and all affected organizations had their Check Point Security Management Server exposed to the internet.

hackernews · louiereederson · Nov 24, 16:32 · [Discussion](https://news.ycombinator.com/item?id=50630594)

**Background**: JavaScript's Math.random() is not cryptographically secure; it uses a deterministic PRNG that can be reverse-engineered if enough outputs are observed. Many developers mistakenly use it for generating tokens, keys, or session identifiers, leading to vulnerabilities like CWE-338. Check Point security management servers are central to managing firewall rules and security policies, making them high-value targets.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/random">Math . random () - JavaScript | MDN</a></li>
<li><a href="https://cybersecuritynews.com/check-point-security-management-servers/">Hackers Target Check Point Security Management Servers ...</a></li>
<li><a href="https://dipsylala.github.io/FlawFixingGuidance/CWE-338/javascript/">JavaScript - CWE Remediation Guidance</a></li>

</ul>
</details>

**Discussion**: Commenters expressed concern that this is just the beginning of AI-driven cyberattacks, with LLMs enabling less sophisticated criminals to launch complex attacks. Some questioned why Math.random() isn't made more secure by default, while others debated the initial access vector and whether exposing management servers to the internet is common.

**Tags**: `#security`, `#vulnerability`, `#PRNG`, `#Node.js`, `#cyberattack`

---

<a id="item-5"></a>
## [Simon Willison Identifies Three LLM Inflection Points in Twelve Months](https://simonwillison.net/2026/Nov/24/llm-inflection-points/) ⭐️ 8.0/10

Simon Willison published a blog post reflecting on his keynote at the AI Engineer Code Summit, arguing that LLM and coding-agent capabilities hit three significant inflection points in the past twelve months, anchored by the one-year anniversary of Claude Opus 4.5 on November 24, 2026. Willison is a highly respected voice in the LLM space, and his retrospective framing helps developers and AI engineers understand the rapid pace of change in coding agents and identify which model releases were truly consequential. The three inflection points are: the release of Claude Opus 4.5 and GPT-5.1 models in November 2025, which made coding agents reliably useful; the emergence of 'Fable class models' in June/July 2026, which can solve problems with brute force when given a goal and tools; and a third point not fully detailed in the excerpt.

rss · Simon Willison · Nov 24, 23:02

**Background**: Claude Opus 4.5 is a large language model released by Anthropic on November 24, 2025, and is considered a major advancement for coding and agentic tasks. Claude Code is Anthropic's terminal-based coding agent, introduced in February 2025 alongside Claude 3.7 Sonnet. The AI Engineer Code Summit is an application-only conference held in San Francisco in November 2026, bringing together leading coding-agent builders and AI engineers.

<details><summary>References</summary>
<ul>
<li><a href="https://ai.engineer/code/2026">AI Engineer Code Summit 2026: AI Engineering Conference, Nov...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Opus_4.5">Claude Opus 4.5</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#coding-agents`, `#AI-engineering`, `#Anthropic`, `#industry-analysis`

---

<a id="item-6"></a>
## [GPT-6.2 Astra Solves 1808 Sketchbook Mystery in 22 Minutes](https://simonwillison.net/2026/Nov/24/astra-historical-mystery/) ⭐️ 8.0/10

History professor Mark Humphries reported that GPT-6.2 Astra, with minimal prompting, autonomously identified the creator of an anonymous 1808 sketchbook held at Yale's Beinecke Library in just 22 minutes using public primary and secondary sources. The model discovered a little-known diary reference to a visit by the vicomte de Chabot and predicted that Chabot's travel journal, available only by order from Cleveland State University, would confirm the sketchbook was his work. This case study demonstrates that an AI model can autonomously conduct genuine historical research using primary sources, potentially transforming how historians approach archival work. It also raises questions about the role of human historians as agentic systems become capable of tasks previously requiring years of expertise. The model found a diary reference to a visit by the vicomte de Chabot dated five days before a date mentioned in the sketchbook at a nearby river, and suggested that Chabot's journal might confirm the attribution. The new source itself is considered a major find for Canadian and fur trade historians, and the sketchbook is digitized in Yale's collections.

rss · Simon Willison · Nov 24, 16:53

**Background**: Primary sources are original documents or objects from the period under study, while secondary sources interpret or analyze them. The Beinecke Rare Book and Manuscript Library at Yale holds extensive special collections, including anonymous manuscripts that often require detective work to attribute. GPT-6.2 Astra is an AI model designed for autonomous agentic tasks, and its ability to search archives and reason about historical evidence represents a new kind of research assistance.

<details><summary>References</summary>
<ul>
<li><a href="https://beinecke.library.yale.edu/">Beinecke Library | Yale Library</a></li>
<li><a href="https://history.ucla.edu/primary-secondary-sources/">Primary & Secondary Sources - UCLA Department of History</a></li>
<li><a href="https://www.techradar.com/tech/openai-just-launched-gpt-6-2-and-its-powerful-enough-to-recreate-the-whole-of-paris-as-a-virtual-world-you-can-explore-in-your-browser">OpenAI just launched GPT - 6 . 2 , and it's powerful enough... | TechRadar</a></li>

</ul>
</details>

**Discussion**: Mark Humphries suggests historians may face a milder version of the 'Deep Blue' crisis seen in chess and mathematics, because history involves constant reinterpretation and humanistic writing rather than chasing a single universal truth. He argues that humanity is a requirement for producing historical literature.

**Tags**: `#AI`, `#GPT-6.2`, `#historical research`, `#case study`, `#autonomous agents`

---

<a id="item-7"></a>
## [PenGPT: A Generative Transformer for Handwriting and Sketches](https://greydanus.github.io/2026/11/12/pengpt/) ⭐️ 7.0/10

PenGPT is a generative transformer that produces handwriting and sketches by modeling stroke tokens, and its author reports that roughly 80% of the effort went into building the largest, cleanest datasets possible rather than into clever architecture. The project is a concrete demonstration of the 'Bitter Lesson' in generative modeling, suggesting that scaling and curating data can outperform architectural novelty for tasks like handwriting synthesis and may influence how practitioners prioritize data work. The model operates on stroke tokens representing pen movements (such as delta x, delta y, and pen-lift), and community reports note that it can stop prematurely on some inputs and handles non-English languages like Spanish poorly.

hackernews · smusamashah · Nov 25, 00:54 · [Discussion](https://news.ycombinator.com/item?id=50637056)

**Background**: Handwriting and sketch generation models typically represent a drawing as a sequence of pen strokes rather than as pixels, allowing a transformer to predict the next stroke token much like a language model predicts the next word. Earlier systems such as Calligrapher.ai used recurrent neural networks for similar text-to-handwriting tasks, while recent work has explored GANs and transformers for style-consistent synthesis. The 'Bitter Lesson' refers to the observation that general methods leveraging computation and data tend to outperform approaches relying on hand-crafted domain knowledge.

<details><summary>References</summary>
<ul>
<li><a href="https://alexagreenberg.com/ml/robotics/transformers/2025/02/25/handwriting.html">alexagreenberg.com/ml/robotics/transformers/2025/02/25/ handwriting ....</a></li>
<li><a href="https://www.calligrapher.ai/?ref=upstract.com">Calligrapher.ai: Realistic computer- generated handwriting</a></li>
<li><a href="https://arxiv.org/pdf/2508.21040">FW-GAN: Frequency-Driven Handwriting Synthesis with Wave ...</a></li>

</ul>
</details>

**Discussion**: Commenters focused on the author's Bitter Lesson remark, with one noting they spend too much time trying to out-clever existing solutions when a clean application of known approaches would serve best. Others highlighted the 'stroke tokens' concept, reported premature stopping on some inputs and poor Spanish handling, and criticized the blog's writing style as needing cleanup by another model.

**Tags**: `#generative-models`, `#transformers`, `#handwriting-synthesis`, `#machine-learning`, `#dataset-quality`

---

<a id="item-8"></a>
## [Hacker News Discusses Helsinki's Gödel Enigma Project](https://www.helsinki.fi/en/researchgroups/godel-enigma/research/project-description) ⭐️ 7.0/10

A Hacker News discussion highlighted the University of Helsinki's Gödel Enigma project, which studies Kurt Gödel's largely untranscribed shorthand notebooks, with commenters sharing book recommendations and recovering a broken link via the Internet Archive. The project could unlock new insights into Gödel's philosophical and logical development, impacting scholars in mathematical logic, philosophy of mathematics, and history of science, and the discussion underscores broader interest in making archival materials accessible. The Gödel Enigma project, led by Jan von Plato and funded by the European Research Council from 2018 to 2023, focuses on transcribing Gödel's notebooks written in Gabelsberger shorthand, of which only the MaxPhil notebooks have been transcribed but not published.

hackernews · benbreen · Nov 24, 08:16 · [Discussion](https://news.ycombinator.com/item?id=50625265)

**Background**: Kurt Gödel was a 20th-century logician famous for his incompleteness theorems, which revolutionized mathematics and logic. After his major results in the 1930s, he published little, leaving behind extensive notebooks in Gabelsberger shorthand, a German shorthand system. The Gödel Enigma project aims to transcribe and study these notebooks to better understand his philosophical and scientific thought.

<details><summary>References</summary>
<ul>
<li><a href="https://www.helsinki.fi/en/researchgroups/godel-enigma/research/project-description">Project description | Gödel Enigma | University of Helsinki</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gabelsberger_shorthand">Gabelsberger shorthand - Wikipedia</a></li>
<li><a href="https://cordis.europa.eu/project/id/787758/reporting">The Gödel Enigma: Unveiling a Hidden Logical Heritage</a></li>

</ul>
</details>

**Discussion**: Commenters shared favorite Gödel books such as Gödel, Escher, Bach and Journey to the Edge of Reason, recovered a broken link to a publisher's page via the Internet Archive, and expressed fascination with the unstudied shorthand notebooks, with one wondering why they remained unread for so long.

**Tags**: `#godel`, `#mathematical-logic`, `#history-of-science`, `#philosophy-of-mathematics`, `#hackernews`

---

<a id="item-9"></a>
## [uv 0.13.10 Released with Security Fix and Lockfile Validation](https://github.com/astral-sh/uv/releases/tag/0.13.10) ⭐️ 5.0/10

Astral released uv 0.13.10 on 2026-11-24, a patch release that addresses security advisory GHSA-vjvj-3m3f-fgmm and adds three lockfile validation enhancements. It also updates managed CPython builds (3.11.18 through 3.16.0a2) and GraalPy 3.13.0 to build 25.6.5. This release matters for Python developers using uv because it patches a security vulnerability and improves the reliability of uv.lock by catching mismatches between declared requirements and locked versions. The lockfile validation enhancements help prevent subtle dependency resolution errors in CI and team workflows. The lockfile improvements validate that dependency requirements match locked versions, explain why uv.lock needs updating when --locked rejects it, and report missing package entries. Other fixes include rejecting wheels with inconsistent ZIP metadata and refreshing cached interpreter info when libc, macOS version, or pyvenv.cfg changes.

github · astral-releases-bot[bot] · Nov 24, 21:15

**Background**: uv is a fast Python package and project manager developed by Astral, written in Rust, that serves as a drop-in replacement for pip and provides project management with a universal lockfile called uv.lock. The lockfile pins exact versions of all dependencies across platforms and Python versions, ensuring reproducible environments. Security advisories like GHSA-vjvj-3m3f-fgmm are published when vulnerabilities are found, and patch releases address them promptly.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.astral.sh/uv/">uv - Astral</a></li>
<li><a href="https://docs.astral.sh/uv/concepts/projects/sync/">Locking and syncing | uv - docs.astral.sh</a></li>
<li><a href="https://github.com/oracle/graalpython">GitHub - oracle/graalpython: GraalPy – A high-performance...</a></li>

</ul>
</details>

**Tags**: `#python`, `#package-manager`, `#uv`, `#security`, `#release-notes`

---