---
layout: default
title: "Horizon Summary: 2026-09-27 (EN)"
date: 2026-09-27
lang: en
---

> From 15 items, 12 important content pieces were selected

---

1. [DeepSeek's DSec Sandbox Platform Handles 380,000 Concurrent Sandboxes](#item-1) ⭐️ 7.0/10
2. [Reladraw: A Declarative Diagram Language With Manual Placement Control](#item-2) ⭐️ 7.0/10
3. [Drawgent: A Coding Agent That Draws on a Live Excalidraw Canvas](#item-3) ⭐️ 7.0/10
4. [Fifteen years later, the Apple Cards origin story](#item-4) ⭐️ 7.0/10
5. [NumPy MLP with GUI Visualizes Training Internals](#item-5) ⭐️ 7.0/10
6. [LLMs Tested for Promise-Keeping in Multi-Agent Diplomacy](#item-6) ⭐️ 7.0/10
7. [Production LLM agent drifts into policy violation over a quarter](#item-7) ⭐️ 7.0/10
8. [Curated Guide and Repo for Learning Distributed LLM Algorithms](#item-8) ⭐️ 6.0/10
9. [Master's Student Seeks Publication Advice for EEG Motor Imagery Thesis with Only Three Participants](#item-9) ⭐️ 4.0/10
10. [Reddit Post Mocks Absurd Neurosurgery Residency Expectations](#item-10) ⭐️ 3.0/10
11. [NeurIPS TAE Workshop 2026 author seeks airfare funding advice](#item-11) ⭐️ 3.0/10
12. [Reddit user asks about the Forrester function's real-world uses](#item-12) ⭐️ 3.0/10

---

<a id="item-1"></a>
## [DeepSeek's DSec Sandbox Platform Handles 380,000 Concurrent Sandboxes](https://arxiv.org/abs/2609.22978) ⭐️ 7.0/10

DeepSeek published a paper on arXiv (2609.22978) describing DeepSeek Elastic Compute (DSec), a production sandbox platform that exposes FnCall, container, microVM, and full-VM backends through a unified SDK. The system reportedly runs about 380,000 concurrent sandboxes on roughly 160 CPU nodes with 30,000 cores and 250 TB of memory, processing around 3 million daily instances and over 5,000 creations per second. DSec shows that large-scale agentic training and evaluation infrastructure can be operated at a density far beyond typical container orchestration, which matters as AI labs increasingly rely on massive numbers of isolated environments to train and test agents. It also offers a rare public look at how a leading AI lab builds production sandbox infrastructure internally. The platform unifies multiple isolation levels — from lightweight FnCall and containers up to microVMs and full VMs — behind a single SDK, and the reported scale includes roughly 3 million daily sandbox instances and more than 5,000 creations per second. The paper also drew attention for its unusually large author list of 131 people, with 31 additional contributors not shown on the page.

hackernews · shenli3514 · Sep 26, 18:22 · [Discussion](https://news.ycombinator.com/item?id=49859112)

**Background**: A sandbox is an isolated execution environment where untrusted or experimental code can run without affecting the rest of a system, and in distributed computing it is a common abstraction for safely running many workloads in parallel. AI labs use sandboxes to train and evaluate agents — programs that call tools and take actions — because each agent run needs its own isolated environment. DeepSeek is a prominent Chinese AI lab known for releasing competitive large language models, and this paper describes the internal infrastructure it uses for that agentic work.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2609.22978">[2609.22978] DeepSeek Elastic Compute ( DSec ): A Sandbox...</a></li>
<li><a href="https://groundtruth.day/news/deepseek-dsec-agent-sandbox-infrastructure.html">DeepSeek describes DSec, a 380 , 000 - concurrent - sandbox platform...</a></li>
<li><a href="https://dataconomy.com/2026/09/25/deepseek-ai-agent-training-platform-sandboxes/">DeepSeek Reveals How AI Agents Exploit Their Sandboxes</a></li>

</ul>
</details>

**Discussion**: Commenters were struck by the engineering scale, with one calling 380,000 concurrent sandboxes on 160 Epyc nodes "crazy stuff," while others focused on the unusually large author list. A widely echoed theory is that listing every employee on every paper is a talent-retention or asset-protection strategy, since competitors cannot easily identify which individuals to recruit. Some also joked that the real puzzle is how 131 authors managed to communicate and ship the paper.

**Tags**: `#DeepSeek`, `#sandbox`, `#distributed systems`, `#AI infrastructure`, `#research paper`

---

<a id="item-2"></a>
## [Reladraw: A Declarative Diagram Language With Manual Placement Control](https://github.com/reladraw/reladraw) ⭐️ 7.0/10

Reladraw is a new diagram language that lets users decide where elements are placed while keeping a declarative, text-based syntax. It ships with an in-browser playground, an npm install option, and a skill for Claude and other AI agents. It targets a real gap between auto-layout tools like Mermaid and Graphviz, which remove placement control, and drag-and-drop editors like Draw.io, which are slow and hard for agents to manipulate. By working well for both humans and AI agents, it could make diagram generation more predictable and automatable in documentation and agent workflows. The language uses relative positioning instructions rather than absolute coordinates, which the author argues is enough for most use cases. Early users report that it is still somewhat buggy, for example failing to render a curved arrow when an edge is specified from left to right.

hackernews · jpwalsh234 · Sep 26, 17:10 · [Discussion](https://news.ycombinator.com/item?id=49858513)

**Background**: Declarative diagramming languages such as Mermaid, Graphviz, and D2 let you describe a diagram in text and have a layout engine decide the final arrangement. This makes diagrams easy to version and generate but gives authors little control over appearance, while manual tools like Draw.io offer control at the cost of speed. Reladraw aims to combine the two by keeping a text-based declarative syntax while letting the author influence placement.

<details><summary>References</summary>
<ul>
<li><a href="https://www.skills.sh/reladraw/reladraw/reladraw">reladraw — reladraw / reladraw</a></li>
<li><a href="https://blog.logrocket.com/complete-guide-declarative-diagramming-d2/">A complete guide to declarative diagramming with D2 A diagramming dev tool | D2 Documentation D2 Language Reference | h0rv/d2-mcp | DeepWiki D2: A Modern Diagram-as-Code Language The Future is Declarative: Why D2 is Leading the Diagramming ...</a></li>
<li><a href="https://d2lang.com/tour/experience/">A diagramming dev tool | D2 Documentation</a></li>

</ul>
</details>

**Discussion**: Commenters generally found the idea promising, with one noting that Mermaid works well for fixed layouts like sequence diagrams but poorly for flowcharts where position matters. Others asked for more syntax documentation, reported a bug with curved arrows, and suggested that translating layout instructions into absolute positions could let Reladraw target multiple render backends.

**Tags**: `#diagramming`, `#developer-tools`, `#DSL`, `#visualization`, `#AI-agents`

---

<a id="item-3"></a>
## [Drawgent: A Coding Agent That Draws on a Live Excalidraw Canvas](https://tangled.org/yanndegat.tngl.sh/drawgent) ⭐️ 7.0/10

Drawgent is a new project that lets a coding agent operate directly on a live Excalidraw canvas, generating and manipulating diagrams in real time. It was posted to Tangled and quickly drew a 32-comment Hacker News discussion about the best medium for human-AI collaborative diagramming. As AI coding agents become common, developers are experimenting with giving them visual workspaces for architecture and design collaboration, and this project adds a concrete implementation to that emerging pattern. The discussion highlights that the choice of diagramming medium — Excalidraw, Mermaid, or HTML — significantly affects how well agents can participate. Excalidraw already offers a first-party open-source MCP endpoint and server, which means agents can interact with it through the Model Context Protocol rather than custom integrations. Commenters noted that Excalidraw's JSON-heavy format forces models to reason about bounding boxes and pixel coordinates, which some found less agent-friendly than text-based alternatives.

hackernews · parasitid · Sep 26, 15:56 · [Discussion](https://news.ycombinator.com/item?id=49857729)

**Background**: Excalidraw is an open-source, web-based virtual whiteboard known for its hand-drawn visual style and real-time collaboration. The Model Context Protocol (MCP) is an open standard introduced by Anthropic in November 2024 that lets AI systems like LLMs connect to external tools and data sources. A coding agent is an AI system that can autonomously perform software tasks such as writing, editing, and refactoring code.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Excalidraw">Excalidraw</a></li>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_coding_agent">AI coding agent</a></li>

</ul>
</details>

**Discussion**: Commenters were broadly interested but debated the best medium: one noted Excalidraw's own MCP server, another found Mermaid more agent-friendly and built an Obsidian plugin, and a third argued HTML is underrated because it gives agents natural semantics instead of pixel math. A notable counterpoint was that the value of diagramming comes from the human thinking process, which an agent may bypass. Another developer open-sourced a similar project, whiteboard-agents, for comparison.

**Tags**: `#AI agents`, `#Excalidraw`, `#diagramming`, `#developer tools`, `#MCP`

---

<a id="item-4"></a>
## [Fifteen years later, the Apple Cards origin story](https://lexontech.org/fifteen-years-later-the-apple-cards-origin-story) ⭐️ 7.0/10

A retrospective article recounts the origin story of Apple's Cards app, highlighting its technical innovations and competitive impact, with Hacker News comments adding firsthand perspectives and discussion of API-based physical mail. The story illustrates how Apple's entry into a niche market can disrupt smaller startups, and it highlights early technical innovations like invisible UV barcodes for USPS tracking that foreshadowed today's physical mail APIs. Apple insisted on no visible barcodes on envelopes but wanted full tracking, so it worked with a printing company to create an invisible barcode sprayed on envelopes, visible only under UV light, and convinced USPS to scan cards at multiple stages.

hackernews · ksec · Sep 26, 09:13 · [Discussion](https://news.ycombinator.com/item?id=49854693)

**Background**: Apple Cards was a 2011 iPhone app that let users create and mail physical greeting cards directly from their phone. It competed with startups like Sincerely, which offered similar print-to-mail services. The app was discontinued in 2013, but its logistics innovations influenced later on-demand printing and mailing APIs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.lob.com/blog/what-is-a-physical-mail-api-and-how-does-it-work">What is a physical mail API and how does it work? - Lob</a></li>
<li><a href="https://www.postgrid.com/direct-mail-api/">Direct Mail API - Integrate & Automate Physical Mails Programmatically | PostGrid™</a></li>

</ul>
</details>

**Discussion**: A co-founder of Sincerely recalled feeling 'Sherlocked' when Apple announced Cards, while others discussed the existence of physical mail APIs and shared anecdotes about founder-led companies and letterpress printing.

**Tags**: `#Apple`, `#history`, `#mobile apps`, `#printing`, `#USPS`

---

<a id="item-5"></a>
## [NumPy MLP with GUI Visualizes Training Internals](https://www.reddit.com/r/MachineLearning/comments/1wqy1qd/p_a_small_mlp_from_scratch_in_numpy_with_a_gui_to/) ⭐️ 7.0/10

A developer released an educational tool that implements a small multi-layer perceptron entirely in plain NumPy, with manual backpropagation and no autograd, and pairs it with a GUI that visualizes training dynamics in real time. The tool includes per-layer weight distributions, PCA/t-SNE of the test set layer by layer, neuron ablation and pruning experiments, and robustness curves for noise and rotation, reaching about 98.5% accuracy on MNIST with the full training set. This tool makes the internal mechanics of neural network training directly observable, which is valuable for teaching and self-learning from high school to introductory ML courses. It also demonstrates that meaningful interpretability experiments like neuron ablation and per-layer t-SNE can be done without heavy frameworks, lowering the barrier for students to explore model behavior. The implementation uses SGD with momentum, L2 regularization, dropout, cosine decay, and four activation functions, all written by hand in NumPy. The GUI shows per-mini-batch and per-epoch loss, gradient norms and the percentage of inactive neurons per layer, weight distributions compared to initialization, first-layer receptive fields, and a lab where ablating or rescaling single neurons, pruning, adding weight noise, or changing softmax temperature updates test accuracy immediately.

reddit · r/MachineLearning · /u/No-Brain-1655 · Sep 26, 18:38

**Background**: A multi-layer perceptron (MLP) is a basic feedforward neural network trained by backpropagation, and implementing one from scratch in NumPy is a common educational exercise to understand gradients and optimization. t-SNE is a nonlinear dimensionality reduction technique that maps high-dimensional data to two or three dimensions for visualization, often used to inspect how a network separates classes layer by layer. Neuron ablation means removing or disabling individual neurons to study their contribution to the network's output, a technique borrowed from neuroscience and widely used in interpretability research. Cosine decay is a learning rate schedule that smoothly lowers the learning rate following a cosine curve, helping training converge more gently near the end.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/T-distributed_stochastic_neighbor_embedding">t-distributed stochastic neighbor embedding - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Ablation_(artificial_intelligence)">Ablation (artificial intelligence) - Wikipedia</a></li>
<li><a href="https://keras.io/api/optimizers/learning_rate_schedules/cosine_decay/">Keras documentation: CosineDecay</a></li>

</ul>
</details>

**Tags**: `#machine-learning`, `#education`, `#visualization`, `#numpy`, `#neural-networks`

---

<a id="item-6"></a>
## [LLMs Tested for Promise-Keeping in Multi-Agent Diplomacy](https://www.reddit.com/r/MachineLearning/comments/1wqufwj/llms_were_told_they_could_lie_in_diplomacy_heres/) ⭐️ 7.0/10

A new multi-agent simulation had several different LLMs play the board game Diplomacy against each other and against a human opponent, with the models explicitly told they were allowed to lie. The study then tracked which models actually kept the promises they made during negotiation. This work sits at the intersection of AI alignment and multi-agent research, probing whether LLMs that are permitted to deceive will still honor commitments, which matters for trustworthiness as models are increasingly deployed as autonomous negotiating agents. Diplomacy is a demanding testbed because it requires negotiation, alliance formation, betrayal, and outmaneuvering, and the simulation placed all models under identical rules and conditions with a human in the mix. The Reddit post itself is only a brief summary and links to the methodology, so it offers limited technical depth.

reddit · r/MachineLearning · /u/Expert_Cobbler8984 · Sep 26, 16:13

**Background**: Diplomacy is a strategy game in which players negotiate, form alliances, betray each other, and maneuver to expand influence, and it has long been used as a laboratory for game theory because it mirrors conditions like scarce resources, self-interested actors, and the absence of external enforcement. LLM-based multi-agent systems use large language models as autonomous agents that plan and interact to solve problems or simulate worlds, while AI alignment research studies how to steer such systems toward intended goals and away from deceptive behavior.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Multi-agent_system">Multi-agent system - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_alignment">AI alignment - Wikipedia</a></li>
<li><a href="https://www.lesswrong.com/lw/32u/diplomacy_as_a_game_theory_laboratory">Diplomacy as a Game Theory Laboratory</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#multi-agent`, `#AI alignment`, `#game theory`, `#deception`

---

<a id="item-7"></a>
## [Production LLM agent drifts into policy violation over a quarter](https://www.reddit.com/r/MachineLearning/comments/1wr509z/i_ran_the_same_prompt_against_our_agent_every/) ⭐️ 7.0/10

A Reddit user reported running the same policy-testing prompt against a production agent once a week for about a quarter, and observed the response gradually drift from a clean refusal in week one to an answer that directly violated policy by the end, despite no model or policy updates. The user also found that lightly rephrased or more politely framed versions of the same request could bypass policy on days when the plain prompt still failed. This highlights that passing a one-time pre-deployment test does not guarantee ongoing policy compliance, a critical risk for teams shipping LLM agents to real users. It reinforces the need for continuous monitoring and adversarial testing in production, an area where industry surveys suggest only a small minority of teams currently monitor LLM applications. The drift was gradual and subtle, starting with dropped qualifiers and slightly more detail before escalating to a full policy violation, and no model version or policy change was made during the test period. The report is anecdotal rather than a controlled study, and the user notes that adversarial framing of the same ask succeeded even when the plain question was still refused.

reddit · r/MachineLearning · /u/IsomuraArganee_95 · Sep 26, 23:38

**Background**: LLM agents are AI systems that use a large language model to take actions or produce responses on behalf of users, often governed by organizational policies about what they may or may not say or do. Model drift refers to the gradual change in a model's behavior over time due to factors such as evolving user inputs, retrieval data changes, or accumulated prompt patches, even without deliberate retraining. Because agents interact with unscripted real-world inputs, their behavior in production can diverge from what was validated in a demo or one-time test.

<details><summary>References</summary>
<ul>
<li><a href="https://zandigital.in/agent-drift-production-monitoring">Agent Drift Is Silent. Only 14% Monitor Production AI</a></li>
<li><a href="https://www.institutepm.com/knowledge-hub/ai-concept-drift-guide">AI Model Drift Explained: A Product Manager's Guide to Catching...</a></li>
<li><a href="https://rhesis.ai/adversarial-testing">Adversarial testing for LLM & AI agents | Rhesis AI</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#production`, `#drift`, `#policy`, `#agents`

---

<a id="item-8"></a>
## [Curated Guide and Repo for Learning Distributed LLM Algorithms](https://www.reddit.com/r/MachineLearning/comments/1wqk0x2/a_little_guide_to_learning_distributed_algorithms/) ⭐️ 6.0/10

A Reddit user shared a curated reading list of papers on distributed algorithms for LLM training and inference, along with a GitHub repository called smolcluster containing basic reference implementations. The list was compiled over three months of reading and is hosted on alphaxiv.org as a shared folder. Distributed training and inference are essential for scaling large language models, but the abundance of parallelism techniques can overwhelm newcomers. A curated, hands-on starting point lowers the barrier to entry and helps practitioners quickly move from theory to implementation. The guide covers fundamental distributed systems concepts and key parallelism strategies including data, tensor, pipeline, and model parallelism. The accompanying repository is described by the author as somewhat disorganized but actively maintained, and feedback is welcomed.

reddit · r/MachineLearning · /u/East-Muffin-6472 · Sep 26, 07:10

**Background**: Training and serving large language models often exceeds the memory and compute capacity of a single GPU, so practitioners split the workload across many devices. Common strategies include data parallelism (replicating the model and splitting batches), tensor parallelism (splitting individual layers' matrix operations), pipeline parallelism (assigning consecutive layers to different devices), and model parallelism (partitioning the model itself). Understanding these techniques is a prerequisite for working with frameworks like Megatron-LM and DeepSpeed.

<details><summary>References</summary>
<ul>
<li><a href="https://bentoml.com/llm/inference-optimization/data-tensor-pipeline-expert-hybrid-parallelism">Data, tensor, pipeline, expert and hybrid parallelisms | LLM Inference Handbook</a></li>
<li><a href="https://siboehm.com/articles/22/pipeline-parallel-training">Pipeline-Parallelism: Distributed Training via Model Partitioning</a></li>
<li><a href="https://medium.com/@siddharthtiwari01/scaling-large-language-models-a-guide-to-parallelism-techniques-c4f7dd6c9f1f">Scaling Large Language Models: A Guide to Parallelism ... Parallelization Techniques for Large Language Models: A ... How to Implement Model Parallelism for Large Language Models ... Model Parallelism · Hugging Face Parallelization Techniques for Large Language Models: A ... Model Parallelism | huggingface/llm_training_handbook | DeepWiki Distributed Hybrid Parallelism for Large Language Models ...</a></li>

</ul>
</details>

**Tags**: `#distributed-training`, `#distributed-inference`, `#LLM`, `#learning-resources`, `#parallelism`

---

<a id="item-9"></a>
## [Master's Student Seeks Publication Advice for EEG Motor Imagery Thesis with Only Three Participants](https://www.reddit.com/r/MachineLearning/comments/1wqxo94/publication_potential_d/) ⭐️ 4.0/10

A master's student posted on r/MachineLearning asking for advice on how to publish a thesis that benchmarks three deep learning architectures, one of them novel, for EEG motor imagery classification on OpenBCI's consumer-grade Galea headset. The student acknowledges the work needs substantially more data and reliability testing, as it currently includes only three participants with limited recordings each. This highlights a common tension in applied machine learning research: consumer-grade EEG hardware makes neurotechnology more accessible, but small participant pools limit statistical validity and publication prospects. It reflects broader questions about how the ML community evaluates low-resource, hardware-constrained studies and what standards journals and conferences should apply. The thesis benchmarks three deep learning architectures across varying preprocessing pipelines, with the novel architecture designed to be compact in parameter count and to prevent overfitting. The main limitation is the dataset: only three participants with limited recordings per participant, which the student recognizes undermines result reliability.

reddit · r/MachineLearning · /u/joekrry · Sep 26, 18:23

**Background**: EEG motor imagery classification is a well-studied brain-computer interface task where a person imagines moving a limb, and machine learning models decode the corresponding brain signals. Consumer-grade EEG caps like OpenBCI's Galea are cheaper and more portable than research-grade systems but typically produce noisier signals, and small-sample studies are common in this space yet difficult to publish without rigorous validation.

<details><summary>References</summary>
<ul>
<li><a href="https://openbci.com/galea/">OpenBCI | Home</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC10917334/">A scoping review on the use of consumer - grade EEG devices for...</a></li>
<li><a href="https://www.nature.com/articles/s41598-025-00824-7">Motor imagery EEG signal classification using novel deep learning algorithm | Scientific Reports</a></li>

</ul>
</details>

**Tags**: `#EEG`, `#deep learning`, `#publication advice`, `#motor imagery`, `#consumer-grade hardware`

---

<a id="item-10"></a>
## [Reddit Post Mocks Absurd Neurosurgery Residency Expectations](https://www.reddit.com/r/MachineLearning/comments/1wqc6ci/medical_student_asked_if_they_can_match_into/) ⭐️ 3.0/10

A Reddit post on r/MachineLearning titled "Medical student asked if they can match into Neurosurgery without an A* first author paper" was submitted by user /u/Even-Inevitable-7243 with the comment "This is how ridiculous things have become." The post has a low score of 3.0/10 and is tagged as off-topic, low-quality, and lacking technical depth. This post highlights the extreme competitiveness of neurosurgery residency applications, where even a first-author paper in a top-tier journal may not guarantee a match, reflecting broader pressures in medical education. It also illustrates how discussions from other fields can spill into AI/ML communities, sparking debates about academic expectations and burnout. The post provides no further context or analysis, and the linked discussion is not included in the content. The title references an "A* first author paper," a term from computer science journal ranking that is not standard in medical residency evaluations, suggesting a cross-disciplinary misunderstanding or exaggeration.

reddit · r/MachineLearning · /u/Even-Inevitable-7243 · Sep 26, 00:12

**Background**: Neurosurgery is one of the most competitive medical specialties in the United States, with match rates often below 60%. Applicants typically need high USMLE Step 2 scores, honors in clinical clerkships, strong letters of recommendation, and research experience, though first-author publications are not strictly required. The term "A*" refers to the top rank in the CORE journal ranking system used primarily in computer science, not in medicine.

<details><summary>References</summary>
<ul>
<li><a href="https://www.neurosurgerymatch.org/hot-on-the-trail-a-field-guide-to-the-neurosurgery-residency-match/">Hot on the Trail: A Field Guide to the Neurosurgery Residency Match - NeurosurgeryMatch.org</a></li>
<li><a href="https://www.prospectivedoctor.com/how-competitive-is-a-neurological-surgery-residency/">How Competitive is a Neurological Surgery Residency? Updated for 2025 | ProspectiveDoctor</a></li>
<li><a href="https://en.wikipedia.org/wiki/Journal_ranking">Journal ranking - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#off-topic`, `#reddit`, `#medical-education`, `#low-quality`, `#discussion`

---

<a id="item-11"></a>
## [NeurIPS TAE Workshop 2026 author seeks airfare funding advice](https://www.reddit.com/r/MachineLearning/comments/1wquo3w/my_paper_got_accepted_at_neurips_tae_workshop/) ⭐️ 3.0/10

A Reddit user announced that their paper was accepted for presentation at the TAE Workshop at NeurIPS 2026, scheduled for December 11, 2026, and asked the community for advice on covering airfare. As a working professional rather than a student, they are ineligible for many student-targeted funding programs, and the workshop only covers registration and hotel, not flights. This highlights a recurring gap in academic conference funding: non-student researchers and industry professionals often fall outside the eligibility criteria of both student grants and institutional travel budgets. The responses could serve as a practical reference for anyone facing similar airfare costs at major ML conferences like NeurIPS. The TAE Workshop at NeurIPS 2026 focuses on trustworthiness and evaluation of AI, and will be held in Sydney, Australia on December 11 or 12, 2026. NeurIPS itself states it cannot provide travel support such as flights or per diem due to the scale of its Financial Assistance program, which serves nearly 1,000 awardees.

reddit · r/MachineLearning · /u/Vivek_Chauhan06 · Sep 26, 16:22

**Background**: NeurIPS is one of the largest annual conferences in machine learning, and its workshops are smaller satellite events held alongside the main conference. Travel funding for such events typically comes from a mix of conference financial assistance programs, university or employer grants, and external sponsorships, but these often prioritize students. Understanding which programs cover airfare versus only registration or lodging is key for professionals planning attendance.

<details><summary>References</summary>
<ul>
<li><a href="https://tai-eval.github.io/">TAE | NeurIPS 2026 Workshop - AI Evaluation</a></li>
<li><a href="https://neurips.cc/Conferences/2026/FinancialAssistance">NeurIPS 2026 Financial Assistance</a></li>
<li><a href="https://neurips.cc/Conferences/2025/FinancialAssistance">NeurIPS 2025 Financial Assistance</a></li>

</ul>
</details>

**Tags**: `#NeurIPS`, `#travel funding`, `#conference`, `#workshop`, `#academic advice`

---

<a id="item-12"></a>
## [Reddit user asks about the Forrester function's real-world uses](https://www.reddit.com/r/MachineLearning/comments/1wqm4no/has_anyone_used_the_forrester_functiond/) ⭐️ 3.0/10

A Reddit user on r/MachineLearning posted asking whether the Forrester function is used only for benchmarking optimization and machine learning methods or also has real-world applications, particularly in economics, econometrics, forecasting, and economic modeling. The post seeks practical insights from anyone who has encountered the function outside of pure mathematics. The question highlights a common gap between academic benchmark functions and applied practice, which matters for students and practitioners in optimization, machine learning, and economics who need to know when synthetic test functions translate to real problems. It also reflects broader interest in multi-fidelity optimization, where the Forrester function is a standard test case. The Forrester function is a multimodal, one-dimensional non-convex function widely used to test optimization algorithms, and it is a standard benchmark in multi-fidelity optimization literature, including the 2008 work by Forrester, Sóbester, and Keane on surrogate modeling. It is also included in benchmarking libraries such as HPOlib2 and MF2, where a low-fidelity version is created by varying constants A, B, and C.

reddit · r/MachineLearning · /u/Only-Dependent7024 · Sep 26, 09:24

**Background**: The Forrester function is a simple mathematical test function introduced in the context of multi-fidelity optimization, where a cheap low-fidelity model is used alongside an expensive high-fidelity model to speed up design and optimization. It is commonly used in surrogate modeling and Bayesian optimization research because it has one global minimum, a local minimum, and an inflection point, making it useful for visualizing algorithm behavior. Benchmark functions like this are not usually meant to model real economic systems directly, but they help researchers compare algorithms before applying them to real-world problems.

<details><summary>References</summary>
<ul>
<li><a href="https://benchmarkfcns.info/doc/forresterfcn.html">Forrester Function | BenchmarkFcns</a></li>
<li><a href="https://www.sfu.ca/~ssurjano/forretal08.html">Forrester et al. (2008) Function - Simon Fraser University</a></li>
<li><a href="https://automl.github.io/HPOlib1.5/stable/synthetic_benchmarks/forrester.html">Forrester function — HPOlib2 0.0.1 documentation</a></li>

</ul>
</details>

**Tags**: `#Forrester function`, `#optimization`, `#benchmarking`, `#machine learning`, `#economics`

---