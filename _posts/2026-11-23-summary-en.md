---
layout: default
title: "Horizon Summary: 2026-11-23 (EN)"
date: 2026-11-23
lang: en
---

> From 9 items, 9 important content pieces were selected

---

1. [Lean formalization of disputed Riemann Hypothesis proof sparks debate](#item-1) ⭐️ 8.0/10
2. [OpenAI Links Perplexity to Model Intelligence](#item-2) ⭐️ 8.0/10
3. [Tim O'Reilly: Silicon Valley Optimizes for Shareholder Value, Not Human Flourishing](#item-3) ⭐️ 7.0/10
4. [Show HN: Game casts player as an LLM's subagent](#item-4) ⭐️ 7.0/10
5. [Beginner's Guide to Local AI with Inkling, Qwen, and Unsloth](#item-5) ⭐️ 6.0/10
6. [Miniature 3D San Francisco map with live vehicles wows Hacker News](#item-6) ⭐️ 6.0/10
7. [Open Social Web Alliance pushes email-like open social protocol](#item-7) ⭐️ 5.0/10
8. [Simon Willison's Select Styling Specimens Tool](#item-8) ⭐️ 5.0/10
9. [Audubon Magazine Catalogs Birds of GTA 6's Leonida](#item-9) ⭐️ 4.0/10

---

<a id="item-1"></a>
## [Lean formalization of disputed Riemann Hypothesis proof sparks debate](https://claude.ai/artifact/CtQyX8qfYAF822bgHJHHE3) ⭐️ 8.0/10

A progress map has been published for the Lean formalization of Alessandro Masullo's manuscript, which claims to prove the Riemann Hypothesis (or its generalized form). The effort has already surfaced hundreds of errata issues, and the announcement's credibility is under scrutiny after Ravi Vakil reportedly said he had not examined the document and Brian Conrad called for 'major revision'. If the proof holds, it would resolve the most famous open problem in mathematics and qualify for the Clay Millennium Prize; if it fails, the episode highlights the risks of premature announcement and the growing role of AI-assisted and formal-verification efforts in frontier mathematics. Contributors caution that the hundreds of errata issues range from minor to serious and that it is too early to tell whether the core idea has a fatal hole; a single gap would collapse the entire formalization, so the progress bar should not be read as evidence of correctness.

hackernews · Qision · Nov 22, 23:12 · [Discussion](https://news.ycombinator.com/item?id=50605045)

**Background**: The Riemann Hypothesis, posed by Bernhard Riemann in 1859, asserts that all non-trivial zeros of the zeta function have real part 1/2, and it remains unproven. Lean is a proof assistant and functional programming language based on dependent type theory that lets mathematicians write proofs as code checked by a computer; it is currently being used to formalize huge results such as Fermat's Last Theorem.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Lean_(proof_assistant)">Lean (proof assistant) - Wikipedia</a></li>
<li><a href="https://www.claymath.org/millennium/riemann-hypothesis/">Riemann Hypothesis - Clay Mathematics Institute</a></li>
<li><a href="https://www.nacionale.com/en/articles/what-happens-next-alessandro-masullo-riemann-proof-revision-credit-clay-prize">Vakil: problems reported in Masullo 's GRH draft</a></li>

</ul>
</details>

**Discussion**: Commenters are sharply divided: some mathematicians contributing to the repository ask for spare compute tokens and warn against overinterpreting the errata list, while others stress that the progress bar says nothing about correctness and that a major hole is likely. Several express concern about the credibility of the original announcement and unease about AI systems outpacing human mathematicians.

**Tags**: `#mathematics`, `#Riemann Hypothesis`, `#Lean`, `#formalization`, `#proof verification`

---

<a id="item-2"></a>
## [OpenAI Links Perplexity to Model Intelligence](https://openai.com/index/perplexity-and-intelligence/) ⭐️ 8.0/10

OpenAI published an article arguing that pretraining cross-entropy, measured by perplexity or log-perplexity, is a remarkably consistent indicator of language model intelligence. The piece, attributed to OpenAI researcher Jakub Pachocki, has sparked a 334-comment Hacker News discussion about evaluation metrics. This matters because perplexity offers a simple, stable benchmark for tracking AI progress, contrasting with the proliferation of increasingly complex and often opaque evaluation suites. If perplexity reliably correlates with capability, it could become a shared standard for comparing models across labs and guiding pretraining decisions. Perplexity is the inverse geometric mean of token probabilities, ranging from 1 (perfect prediction) to vocabulary size (random guessing). The article notes that log-perplexity on a held-out set has declined steadily across model generations, and Microsoft has reportedly shared MAI-2 Base's log-perplexity of 0.819 on OpenAI's evaluation set.

hackernews · acossta · Nov 22, 17:06 · [Discussion](https://news.ycombinator.com/item?id=50601525)

**Background**: Perplexity is a standard metric in natural language processing that quantifies how well a language model predicts a sequence of tokens; lower values indicate better predictive performance. Cross-entropy loss, which perplexity exponentiates, is the default training objective for most language models, including transformers like GPT and BERT. Despite the rise of reinforcement learning and reasoning-focused models, perplexity remains a core evaluation tool because it directly measures a model's ability to compress and model raw data.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/perplexity-and-intelligence/">Perplexity and Intelligence - OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Perplexity">Perplexity - Wikipedia</a></li>
<li><a href="https://community.openai.com/t/perplexity-and-intelligence/1419510">Perplexity and Intelligence - Community - OpenAI Developer ...</a></li>

</ul>
</details>

**Discussion**: Commenters broadly found the perplexity-intelligence link surprising yet intuitive, with one noting that prediction and compression rates naturally capture progress in extracting world models from raw data. Others expressed shock that cross-entropy loss remains so predictive despite the shift toward RL and reasoning models, and welcomed a simple benchmark amid increasingly convoluted evaluations. A Microsoft representative also announced that MAI models would be added to the comparison chart.

**Tags**: `#perplexity`, `#intelligence`, `#language-models`, `#evaluation-metrics`, `#AI`

---

<a id="item-3"></a>
## [Tim O'Reilly: Silicon Valley Optimizes for Shareholder Value, Not Human Flourishing](https://www.oreilly.com/radar/what-happened-to-silicon-valley/) ⭐️ 7.0/10

In a lecture at Johns Hopkins University, Tim O'Reilly argued that Silicon Valley has shifted from customer-centered innovation to extraction driven by shareholder capitalism, monopoly ambitions, and hype. He proposes mechanism design—reverse game theory—as a framework to redesign the rules of the game so that human flourishing, not corporate profit, becomes the goal. This critique from a prominent tech figure highlights growing concerns about the tech industry's incentives and their societal impact, especially as AI intensifies economic stakes. It adds momentum to debates on stakeholder capitalism and could influence how investors, founders, and policymakers think about market rules and corporate governance. O'Reilly frames mechanism design as reverse game theory: instead of analyzing the current game, ask what game we ought to be playing. He links Silicon Valley's evolution to the current AI boom, arguing that technology's value depends on the rules, incentives, and interfaces around it, and favors openness as a direction.

hackernews · greenyouse · Nov 22, 19:20 · [Discussion](https://news.ycombinator.com/item?id=50602947)

**Background**: Mechanism design is a branch of economics and game theory that studies how to construct rules—called mechanisms—that produce good outcomes according to a predefined metric, even when the designer lacks full information about participants' preferences. Often described as reverse game theory, it starts with a desired outcome and works backward to find a game that implements it. The field was recognized with the 2007 Nobel Memorial Prize in Economic Sciences awarded to Leonid Hurwicz, Eric Maskin, and Roger Myerson. O'Reilly's lecture applies this concept to critique Silicon Valley's shift from value creation to value extraction under shareholder capitalism.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mechanism_design">Mechanism design</a></li>
<li><a href="https://www.oreilly.com/radar/what-happened-to-silicon-valley/">What Happened to Silicon Valley? – O’Reilly</a></li>
<li><a href="https://news.lavx.hu/article/tim-o-reilly-traces-silicon-valley-s-shift-from-value-creation-to-extraction">Tim O'Reilly Traces Silicon Valley's Shift From Value ...</a></li>

</ul>
</details>

**Discussion**: Commenters largely agreed with O'Reilly's critique, with some emphasizing the need to hold mechanism designers accountable and to collectively decide what humanity should optimize for. Others pointed to the ZIRP era as a proximate cause that allowed companies to grow excessively and incentivized risky expansion, while some lamented the rise of self-serving 'VC influencers' and the loss of integrity in Silicon Valley.

**Tags**: `#silicon-valley`, `#tech-industry`, `#capitalism`, `#mechanism-design`, `#venture-capital`

---

<a id="item-4"></a>
## [Show HN: Game casts player as an LLM's subagent](https://github.com/gulivan/worker755) ⭐️ 7.0/10

A developer released a Show HN game called worker755 on GitHub where the player takes on the role of a subagent receiving instructions from an LLM manager. The project gained traction on Hacker News with 273 points and 65 comments, where players shared experiences and debated the near-future reality of AI middle managers. The game creatively satirizes the emerging dynamic of LLMs acting as managers over human workers, offering a thought-provoking commentary on AI-human collaboration and agentic workflows. It resonates with current trends in multi-agent systems where orchestrator LLMs delegate tasks to subagents, prompting reflection on how such hierarchies might translate to human roles. The game is available on GitHub as an open-source project, and players have noted that the LLM manager sometimes provides exact commands rather than letting them solve tasks independently. Some players have experimented with adversarial actions, such as attempting to delete all files with 'rm -rf' to see the manager's response.

hackernews · ivantgam · Nov 22, 13:56 · [Discussion](https://news.ycombinator.com/item?id=50599762)

**Background**: In agentic AI systems, an orchestrator LLM often breaks down tasks and delegates them to subagents—separate AI instances that execute specific subtasks and return results. This hierarchical pattern is increasingly used in agentic workflows, where autonomous agents plan, use tools, and coordinate to achieve goals with minimal human intervention. The game flips this paradigm by placing a human in the subagent role, exploring themes of control, delegation, and the future of work.

<details><summary>References</summary>
<ul>
<li><a href="https://kenashe.ai/blog/2026-11-22-what-a-game-about-being-an-llms-subagent-teaches-about-agent-design/">What a Game About Being an LLM's Subagent Teaches About Agent ...</a></li>
<li><a href="https://learn.microsoft.com/en-us/agents/architecture/multi-agent-orchestrator-sub-agent">Orchestrator and subagent multi-agent patterns | Microsoft Learn</a></li>
<li><a href="https://www.ibm.com/think/topics/agentic-workflows">What are agentic workflows? - IBM</a></li>

</ul>
</details>

**Discussion**: Commenters found the game fun and engaging, with some noting that the manager gave exact commands instead of allowing independent problem-solving. Others debated whether this scenario is already reality, suggesting that AI middle managers will soon emerge as a natural evolution of current assistant services. A few made humorous references to science fiction, such as 'Butlerian Jihad Now'.

**Tags**: `#LLM`, `#game`, `#AI agents`, `#human-AI collaboration`, `#Show HN`

---

<a id="item-5"></a>
## [Beginner's Guide to Local AI with Inkling, Qwen, and Unsloth](https://www.gpupartner.com/blog/beginners-guide-local-ai-inkling-qwen-unsloth) ⭐️ 6.0/10

A new beginner's guide explains how to run local AI models such as Qwen and Unsloth, and it has sparked an 89-comment Hacker News discussion where users share hands-on tips on affordable hardware and quantization. This guide and the surrounding discussion lower the barrier to entry for hobbyists who want to run LLMs on their own machines, showing that useful local AI is possible on consumer-grade GPUs and older enterprise cards rather than requiring cloud-scale infrastructure. Community members report running large models on modest hardware: a 27B Qwen model at 14 tokens/s on an Nvidia P40 (24GB, ~$300 used) and a 2-bit quantized 27B model at 40 tokens/s with 128k context on a 12GB RX 6700 XT, while one user found Inkling Small struggled with a simple coding task that Qwen completed in 17 minutes.

hackernews · Retell15 · Nov 22, 21:01 · [Discussion](https://news.ycombinator.com/item?id=50603845)

**Background**: Local AI refers to running large language models on your own hardware instead of using cloud APIs. Quantization reduces the precision of model weights (e.g., to 4-bit or 2-bit) so models fit in limited GPU memory with modest quality loss. Unsloth is an open-source library for efficiently running and fine-tuning models locally, and Inkling is an open-weights multimodal model from Thinking Machines Lab with a 975B-parameter mixture-of-experts architecture (41B active).

<details><summary>References</summary>
<ul>
<li><a href="https://unsloth.ai/">Unsloth - Run and Train Models Locally</a></li>
<li><a href="https://cast.ai/blog/demystifying-quantizations-llms/">LLM Quantization Methods: GPTQ, AWQ, GGUF - Cast AI</a></li>
<li><a href="https://arxiv.org/html/2411.02530v1">A Comprehensive Study on Quantization Techniques for Large ...</a></li>

</ul>
</details>

**Discussion**: Commenters are enthusiastic but pragmatic: some compare local AI to the early, expensive plasma TV era and expect a ~5-year path to mainstream practicality, while others share concrete hardware recipes (P40, RX 6700 XT) and note that quantized 125B Qwen Flash models can outperform 27B models on low-VRAM setups. A notable counterpoint is that Inkling Small reportedly struggled with a simple coding task that Qwen finished quickly.

**Tags**: `#local-ai`, `#llm`, `#quantization`, `#hardware`, `#tutorial`

---

<a id="item-6"></a>
## [Miniature 3D San Francisco map with live vehicles wows Hacker News](https://smallsf.com/) ⭐️ 6.0/10

A new interactive website, smallsf.com, presents a miniature 3D model of San Francisco where buses, planes, and boats move in real time. The project was shared on Hacker News and received 146 points and 63 comments, with users praising its creativity but noting rendering glitches when zooming in. This project demonstrates how web-based 3D visualization can create engaging, real-time city models that capture public imagination, potentially inspiring similar side projects and showcasing the accessibility of modern web graphics tools. It highlights the growing interest in digital twins and interactive maps for entertainment and education. The map includes live tracking of buses, planes, and boats, but users have reported issues such as missing landmarks (e.g., Patricia's Green in Hayes Valley) when zooming. The site provides an about page that may detail the tools used, though the exact tech stack is not specified in the discussion.

hackernews · dutilh · Nov 22, 20:33 · [Discussion](https://news.ycombinator.com/item?id=50603589)

**Background**: Interactive 3D city maps are web applications that render urban environments in three dimensions, often using technologies like WebGL and mapping libraries such as CesiumJS or Mapbox. These maps can integrate live data feeds to show moving vehicles, creating a 'digital twin' experience. Side projects like this are commonly shared on Hacker News, where developers showcase creative uses of web technologies.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=50487228">Show HN: Isometric SF – A pixel-art map of the SF Bay Area ...</a></li>
<li><a href="https://topostreets.com/how-to-build-interactive-web-3d-maps-with-cesiumjs/">How to Build Interactive Web 3D Maps with CesiumJS</a></li>

</ul>
</details>

**Discussion**: Community reaction was positive overall, with users calling it 'fantastic' and expressing a desire to have similar maps for their own cities. However, some criticized rendering glitches, such as missing parks when zoomed in, and others joked about playing GTA in the map.

**Tags**: `#interactive-maps`, `#3d-visualization`, `#web-development`, `#side-projects`, `#hackernews`

---

<a id="item-7"></a>
## [Open Social Web Alliance pushes email-like open social protocol](https://osw-alliance.net/en/) ⭐️ 5.0/10

The Open Social Web Alliance (OSWA) has announced an initiative to develop a standardized, email-like open social protocol, aiming to create a roadmap for interoperable and public-interest-oriented social networks. The announcement, hosted at osw-alliance.net, outlines a vision for social media that strengthens democratic discourse but provides few technical specifics. This initiative adds to the growing movement toward decentralized social media, which seeks to counter the concentrated power of centralized platforms like Facebook and X. If successful, a standardized open protocol could enable interoperability between different social platforms, giving users more control over their data and interactions. The alliance brings together researchers, civil society organizations, and digital policy experts, but the website's messaging is vague and lacks concrete technical details or timelines. The protocol is compared to email, suggesting a federated approach where users can communicate across different servers and services.

hackernews · doener · Nov 22, 15:24 · [Discussion](https://news.ycombinator.com/item?id=50600511)

**Background**: Decentralized social media protocols like ActivityPub (used by Mastodon) and AT Protocol (used by Bluesky) aim to create open, interoperable social networks where no single entity controls the conversation. These protocols are often compared to email, which allows users on different providers to communicate seamlessly. The Open Social Web Alliance appears to be advocating for a similar standardized approach, though it remains unclear how it relates to existing protocols.

<details><summary>References</summary>
<ul>
<li><a href="https://synosys.github.io/news/open_social_web_alliance/">Philipp Lorenz-Spreen contributes to new alliance for an open social ...</a></li>
<li><a href="https://www.theverge.com/2023/4/20/23689570/activitypub-protocol-standard-social-network">ActivityPub is the next big thing in social networks | The Verge</a></li>
<li><a href="https://arxiv.org/abs/2505.22962">Seeing the Politics of Decentralized Social Media Protocols</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters were skeptical, criticizing the website's fluffy prose and questioning whether social or democratic problems can be engineered away with clever tools. Some noted that monetization incentives favor discord over healthy discourse, and others expressed doubt that users will move en masse to a new platform without trust and tangible benefits.

**Tags**: `#open-social-web`, `#decentralization`, `#social-media`, `#protocols`, `#community-discussion`

---

<a id="item-8"></a>
## [Simon Willison's Select Styling Specimens Tool](https://simonwillison.net/2026/Nov/22/select-styling/) ⭐️ 5.0/10

Simon Willison built a tool called Select Styling Specimens that catalogs all the ways HTML <select> boxes can be styled across browsers, using Claude Fable 5.2 to generate the page. He also shared his preferred CSS snippet that makes select boxes render consistently in Chrome, Safari, and Firefox. This tool provides a practical reference for web developers frustrated by inconsistent default rendering of select elements across browsers, helping them achieve cross-browser consistency with minimal CSS. It also demonstrates how AI-assisted development can quickly produce niche utility tools. The recommended CSS uses appearance: none to remove native styling, then applies custom padding, border, border-radius, and an inline SVG background image for the dropdown arrow. This approach ensures a uniform look across Chrome, Safari, and Firefox, though it may affect accessibility or native mobile behavior.

rss · Simon Willison · Nov 22, 19:45

**Background**: HTML <select> elements have historically been difficult to style consistently because each browser renders them with its own native UI controls. While basic CSS properties like width, background, and border can be applied, fully customizing the dropdown arrow and option list often requires workarounds or JavaScript libraries. The appearance property allows developers to strip native styling and build custom designs, but cross-browser testing remains essential.

<details><summary>References</summary>
<ul>
<li><a href="https://stackoverflow.com/questions/1895476/how-do-i-style-a-select-dropdown-with-only-css">html - How do I style a dropdown with only CSS ... Code sample</a></li>
<li><a href="https://www.anthropic.com/claude-fable-and-mythos-5-2">Introducing Claude Fable 5.2 and Claude Mythos 5.2</a></li>

</ul>
</details>

**Tags**: `#html`, `#css`, `#web-development`, `#cross-browser`, `#ai-assisted-development`

---

<a id="item-9"></a>
## [Audubon Magazine Catalogs Birds of GTA 6's Leonida](https://www.audubon.org/magazine/birds-of-gta-6-field-guide-vice-city-wildlife) ⭐️ 4.0/10

Audubon magazine published a field guide-style article cataloging the bird species that appear in Grand Theft Auto VI's fictional state of Leonida, which includes Vice City. The piece highlights the game's detailed wildlife, sparking a Hacker News discussion with 362 points and 164 comments. This crossover between a respected conservation magazine and a blockbuster video game underscores how realistic game worlds have become, blurring the line between entertainment and naturalistic observation. It also shows the cultural reach of GTA 6, which is set to be one of the most anticipated media releases of the decade. The article is part of Audubon's tradition of creative environmental coverage, while the game's setting, Leonida, is a fictional state based on Florida, with Vice City standing in for Miami. The map is roughly twice the size of GTA V's, featuring diverse ecosystems that support varied birdlife.

hackernews · gaws · Nov 22, 19:10 · [Discussion](https://news.ycombinator.com/item?id=50602843)

**Background**: Audubon is the flagship quarterly magazine of the National Audubon Society, a nonprofit dedicated to bird conservation, known for its award-winning journalism and photography. Grand Theft Auto VI, developed by Rockstar Games, is set in the fictional state of Leonida, which includes Vice City and the Leonida Keys, and is scheduled for release in 2025. The game's unprecedented attention to detail extends to wildlife, prompting this unusual field guide.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Audubon_(magazine)">Audubon (magazine)</a></li>
<li><a href="https://rockstarspy.com/gta-6/leonida/">Leonida explained: GTA 6 's Florida stand-in, 6 regions</a></li>

</ul>
</details>

**Discussion**: Commenters largely veered away from birds, discussing wishes for co-op play (e.g., one player as Jason, another as Lucia), the game's story-focused design versus sandbox elements, and the inclusion of electric vehicles and charging stations. Some expressed a desire for a tamer mode for children, while others praised the detailed wildlife mods in Red Dead Redemption 2 and anticipated similar depth in GTA 6.

**Tags**: `#gaming`, `#GTA 6`, `#wildlife`, `#off-topic`, `#community-discussion`

---