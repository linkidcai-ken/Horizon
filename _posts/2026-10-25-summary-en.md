---
layout: default
title: "Horizon Summary: 2026-10-25 (EN)"
date: 2026-10-25
lang: en
---

> From 16 items, 11 important content pieces were selected

---

1. [10-Year-Old CNN Beats Frontier LLMs in Skin Cancer Diagnosis](#item-1) ⭐️ 8.0/10
2. [Oregon Police Charge News Outlet $2.5M for Records on One Officer](#item-2) ⭐️ 7.0/10
3. [Nanbeige releases Nanbeige4.3-33B, an Apache 2.0 teacher model for smaller agents](#item-3) ⭐️ 7.0/10
4. [memt-1.0 uses gated deltanet-2 and mixture-of-storage for agent memory](#item-4) ⭐️ 7.0/10
5. [Dolly Parton's Imagination Library: Free Books for Kids](#item-5) ⭐️ 6.0/10
6. [FOSDEM Talk on Resisting Internet Censorship Sparks Debate](#item-6) ⭐️ 6.0/10
7. [DreamHost Hit by Active Security Incident, Forces Password Resets](#item-7) ⭐️ 6.0/10
8. [Blind test compares five self-hosted AI agents on local Qwen model](#item-8) ⭐️ 6.0/10
9. [Reddit discussion: challenges in creating edge-case datasets for fine-tuning open-weight models](#item-9) ⭐️ 5.0/10
10. [Serbia's Vucic Concedes Election Defeat to Student Movement](#item-10) ⭐️ 4.0/10
11. [ICLR 2027 continues desk rejections to curb AI-generated submissions](#item-11) ⭐️ 4.0/10

---

<a id="item-1"></a>
## [10-Year-Old CNN Beats Frontier LLMs in Skin Cancer Diagnosis](https://lynchlab.net/llm-skin-cancer) ⭐️ 8.0/10

A blog post by the Lynch Lab reports that a 10-year-old Inception v3 convolutional neural network, fine-tuned on 68,011 dermoscopic and clinical images from the ISIC Archive, outperformed two frontier large language models in diagnosing skin cancer on a test set of 200 lesions. The author expressed surprise at the result, which has sparked debate about specialized models versus general-purpose LLMs. This finding challenges the assumption that ever-larger general-purpose LLMs will dominate all tasks, suggesting that small, specialized models can still be superior for narrow, high-stakes domains like medical imaging. It also raises important questions about how medical AI should be evaluated and deployed, affecting researchers, clinicians, and regulators. The CNN was pretrained on everyday photographs and fine-tuned on a single H100 GPU, with test lesions and all images of the same patient removed from training and validation to prevent data leakage. Critics argue the comparison may be unfair because the CNN was specifically trained for this task while the LLMs were not, and some call it 'benchmaxxing'.

hackernews · sungam · Oct 25, 17:15 · [Discussion](https://news.ycombinator.com/item?id=50233779)

**Background**: Convolutional neural networks (CNNs) are a class of deep learning models particularly effective for image recognition, and Inception v3 is a well-known architecture from 2015. Large language models (LLMs) like GPT-4 are general-purpose models trained on vast text and multimodal data, but they are not specifically optimized for medical image classification. The ISIC Archive is a large public collection of skin lesion images used for dermatology research.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Convolutional_neural_network">Convolutional neural network - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/convolutional-neural-networks">What are Convolutional Neural Networks ? | IBM</a></li>
<li><a href="https://www.nature.com/articles/s41591-026-04431-5">General-purpose large language models outperform specialized ...</a></li>

</ul>
</details>

**Discussion**: Commenters generally agreed that specialized models can outperform general LLMs on narrow tasks, with some comparing it to a calculator beating LLMs at arithmetic or a small KataGo network mastering Go. Others criticized the benchmark as 'benchmaxxing' and suggested fairer comparisons, such as providing the LLM with the training data in context or using TabPFN-style approaches.

**Tags**: `#machine-learning`, `#medical-ai`, `#model-specialization`, `#benchmarking`, `#cnn-vs-llm`

---

<a id="item-2"></a>
## [Oregon Police Charge News Outlet $2.5M for Records on One Officer](https://theintercept.com/2026/10/01/oregon-police-misconduct-public-records-cost-fee/) ⭐️ 7.0/10

The Eugene Police Department in Oregon has told a local news outlet that fulfilling its public records request about a single officer would require at least 44,816 staff hours and cost approximately $2,484,599.04. The fee, equivalent to about 21 years of work, has sparked widespread criticism and discussion about government transparency. This case illustrates how excessive fees can be used to effectively deny access to public records, undermining FOIA laws and press freedom. It affects journalists, civil liberties advocates, and the public's ability to hold law enforcement accountable. Oregon law allows agencies to recover actual costs including staff time, and fee waivers for public interest are discretionary. The estimated 44,816 hours is roughly 21 years of full-time work, making the request practically impossible to fulfill.

hackernews · tdeck · Oct 25, 18:04 · [Discussion](https://news.ycombinator.com/item?id=50234232)

**Background**: Public records laws, such as the federal Freedom of Information Act (FOIA) and Oregon's Public Records Law (ORS 192), grant the public the right to request government documents. Agencies may charge fees for processing, but when fees become prohibitively high, they can function as a de facto denial of access.

<details><summary>References</summary>
<ul>
<li><a href="https://www.inet-investigation.com/oregon-public-records-a-complete-research-guide/">Oregon Public Records : ORS 192, Courts, Criminal & Property...</a></li>
<li><a href="https://oregon.public.law/rules/oar_250-001-0020">OAR 250-001-0020 – Fees for Public Records - OregonLaws</a></li>
<li><a href="https://www.pogo.org/newsletters/the-bridge/the-bridge-foias-our-flashlight-in-the-dark">POGO | The Bridge: FOIA ’s Our Flashlight in the Dark</a></li>

</ul>
</details>

**Discussion**: Commenters expressed outrage at the absurdity of the fee, with some sharing experiences of agencies using slow-walking tactics instead. Others compared FOIA systems internationally, noting that Germany is debating similar restrictive fees while the UK generally responds within 30 days, and one commenter cited a 2015 DoD request estimated at 15 million hours and $660 million.

**Tags**: `#public-records`, `#FOIA`, `#government-transparency`, `#journalism`, `#civil-liberties`

---

<a id="item-3"></a>
## [Nanbeige releases Nanbeige4.3-33B, an Apache 2.0 teacher model for smaller agents](https://www.reddit.com/r/MachineLearning/comments/1xf6x35/nanbeige_releases_nanbeige4333b_an_apache_20/) ⭐️ 7.0/10

Nanbeige released Nanbeige4.3-33B, an Apache 2.0 licensed 33B parameter model with a 512K context window, positioned as a teacher model for distilling smaller agent models including an upcoming 3B version. The team reports 80.9 on Terminal-Bench 2.1 versus 73.0 for Qwen3.8-27B, but trails on SWE-Bench Pro with 60.3 versus 61.7. This release provides an openly licensed, high-context teacher model specifically tuned for agentic tasks, which could lower the barrier for teams building small, deployable agents via knowledge distillation. It also adds a competitive data point to the growing open-weight agent-model landscape, though the self-reported benchmarks require independent verification before being treated as a deployment ranking. The reported scores are the releasing team's own evaluations without independent replication, and the model does not win everywhere, losing on SWE-Bench Pro. A practical detail for reproducing agent results is that evaluations retain earlier reasoning with preserve_thinking=true, which the model card recommends for multi-turn tool use but not general chat; comparing task success and total generated tokens with that setting fixed would be more useful than headline scores.

reddit · r/MachineLearning · /u/jatingargiitk · Oct 25, 16:32

**Background**: Knowledge distillation trains a smaller student model on signals from a larger teacher model, preserving much of the teacher's behavior while reducing size and computational demands. Terminal-Bench is a benchmark that tests whether LLM agents can complete multi-step tasks in a terminal, such as writing and running code, while SWE-Bench Pro evaluates software-engineering problem solving. The preserve_thinking parameter controls whether a model's earlier reasoning traces are retained in context during multi-turn inference, which matters for agentic tool-call loops.

<details><summary>References</summary>
<ul>
<li><a href="https://www.datacamp.com/blog/distillation-llm">LLM Distillation Explained: Applications, Implementation... | DataCamp</a></li>
<li><a href="https://snorkel.ai/leaderboard/terminal-bench-2-1/">Terminal-Bench 2.1: LLM Terminal Agent Benchmark | Snorkel AI</a></li>
<li><a href="https://github.com/ggml-org/llama.cpp/issues/22615">Documentation: `preserve_thinking=true` preserves reasoning ...</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#open-weights`, `#agentic-models`, `#benchmarks`, `#model-release`

---

<a id="item-4"></a>
## [memt-1.0 uses gated deltanet-2 and mixture-of-storage for agent memory](https://www.reddit.com/r/MachineLearning/comments/1xeu0ht/memt10_architecture_breakdown_gated_deltanet2/) ⭐️ 7.0/10

memt-1.0 introduces a memory-native architecture that internalizes agent memory into model weights/states using gated deltanet-2 with a stable token-level memory update mechanism, combined with a mixture-of-storage (MoS) layer to scale capacity. At 128k context, memt-1.0-nano achieves roughly 1.86x end-to-end inference speedup and a 66x reduction in persistent storage compared to full-context KV caching. This approach could eliminate the need for append-only prompt stacking or external RAG pipelines in long-horizon agents, directly addressing KV cache memory bottlenecks that limit context length and increase costs. If validated, it would significantly improve efficiency for agentic tasks requiring persistent memory. The two-stage training pipeline (continued pre-training + post-training across 34B tokens) preserves general reasoning capabilities while outperforming existing parametric memory baselines, which typically degrade base LLM performance. The architecture continuously internalizes retrieved procedural experience into model weights/states during multi-turn tasks, avoiding context window bloat from raw execution logs.

reddit · r/MachineLearning · /u/Mrs-Grumpy23 · Oct 25, 05:31

**Background**: Traditional LLM agents rely on full-context KV caching or retrieval-augmented generation (RAG) to maintain memory, but these methods scale poorly with context length due to storage and compute overhead. Gated DeltaNet-2 is a linear attention variant that decouples erase and write operations for more flexible memory updates, while mixture-of-storage (MoS) is a technique to scale memory capacity by combining different storage mechanisms. Parametric memory refers to storing information directly in model parameters rather than in external databases or context windows.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2605.22791">[2605.22791] Gated DeltaNet-2: Decoupling Erase and Write in ...</a></li>
<li><a href="https://github.com/NVlabs/GatedDeltaNet-2/">Gated DeltaNet-2: Decoupling Erase and Write in ... - GitHub</a></li>
<li><a href="https://www.emergentmind.com/topics/memory-mechanisms-in-llms">Memory Mechanisms in LLMs</a></li>

</ul>
</details>

**Tags**: `#agent-memory`, `#architecture`, `#efficiency`, `#LLM`, `#machine-learning`

---

<a id="item-5"></a>
## [Dolly Parton's Imagination Library: Free Books for Kids](https://imaginationlibrary.com/) ⭐️ 6.0/10

A Hacker News discussion highlighted Dolly Parton's Imagination Library, a program that mails free books to children from birth to age five. Commenters shared personal stories and noted that while the central organization negotiates wholesale prices, local charities fund the books. The program has distributed millions of books worldwide, fostering early literacy and a love of reading. Its locally funded model allows communities to tailor the program but also means availability depends on local charitable support. Books cost about $2.50 wholesale, and the central organization selects titles and manages distribution. In Tennessee, hospitals sign up newborns, and children receive books until age five; however, without local partners, children may not receive books.

hackernews · jumploops · Oct 25, 18:23 · [Discussion](https://news.ycombinator.com/item?id=50234474)

**Background**: Dolly Parton's Imagination Library was launched in 1995 in her home county in East Tennessee, inspired by her father's inability to read. It has since expanded to five countries and gifts millions of free books each month to children from birth to age five, regardless of family income.

<details><summary>References</summary>
<ul>
<li><a href="https://imaginationlibrary.com/">Dolly Parton's Imagination Library | USA, UK, IE, CA, AU</a></li>
<li><a href="https://www.dollyparton.com/philanthropy">Philanthropy | Dolly Parton's Imagination Library ...</a></li>
<li><a href="https://readdork.com/news/why-dolly-parton-started-imagination-library-uk-history-f74ec22687">Why Dolly Parton started the Imagination Library and how it reached...</a></li>

</ul>
</details>

**Discussion**: Commenters praised the program's quality and impact, sharing personal anecdotes such as receiving books in Tennessee hospitals and a child's final book arriving with a letter from Dolly. Some noted the local funding model's limitations, while others emphasized the program's thoughtful and diverse book selection.

**Tags**: `#literacy`, `#non-profit`, `#community`, `#books`, `#Dolly Parton`

---

<a id="item-6"></a>
## [FOSDEM Talk on Resisting Internet Censorship Sparks Debate](https://talkweb.eu/openweb/4558/) ⭐️ 6.0/10

A blog post announces a FOSDEM talk titled 'I refuse to accept a censored Internet. Join Me at FOSDEM 27', which calls for resistance against internet censorship. The announcement sparked a Hacker News discussion with 175 comments and 353 points, where commenters debated the feasibility of an uncensored internet and shared related projects. Internet censorship is a growing global concern, and this talk at FOSDEM—a major free and open-source software conference—highlights the role of the tech community in addressing it. The discussion reflects broader debates about whether software alone can overcome censorship and the influence of corporations on internet infrastructure. The talk is scheduled for FOSDEM 27, but the announcement provides no technical details about the methods or tools to be presented. The Hacker News discussion includes perspectives from developers who have built circumvention tools, such as the creator of 'Mother of all VPNs' (moav.sh), who shared their experience with internet shutdowns in Iran.

hackernews · Tomte · Oct 25, 17:30 · [Discussion](https://news.ycombinator.com/item?id=50233929)

**Background**: FOSDEM (Free and Open source Software Developers' European Meeting) is an annual non-commercial conference held in Brussels, Belgium, typically in early February, attracting thousands of free and open-source software developers. Internet censorship circumvention refers to methods and tools used to bypass legal control or suppression of internet access, and it is a active area of research and development. Hacker News is a popular social news website run by Y Combinator, where technology-focused discussions often take place.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/FOSDEM">FOSDEM</a></li>
<li><a href="https://en.wikipedia.org/wiki/Internet_censorship_circumvention">Internet censorship circumvention - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Hacker_News">Hacker News</a></li>

</ul>
</details>

**Discussion**: Commenters expressed skepticism about the possibility of a truly uncensored internet, with some arguing that most people prefer censorship aligned with their political views and that corporate control of infrastructure makes circumvention difficult. Others shared positive experiences with FOSDEM and highlighted grassroots projects like MoaV that aim to provide uncensored access.

**Tags**: `#internet-censorship`, `#fosdem`, `#privacy`, `#networking`, `#community-discussion`

---

<a id="item-7"></a>
## [DreamHost Hit by Active Security Incident, Forces Password Resets](https://www.dreamhoststatus.com/) ⭐️ 6.0/10

DreamHost is responding to an active security incident that began with connectivity issues affecting its File Manager, and the company is forcing password resets for affected users. Community speculation suggests that a vulnerable installation of Monsta FTP, a commercial PHP file manager, may have been exploited to exfiltrate FTP credentials. This incident highlights the risks of relying on third-party web applications like Monsta FTP for critical hosting infrastructure, and it affects DreamHost customers who may have had credentials compromised. It also underscores the importance of timely patching and monitoring for vulnerabilities in widely used PHP tools. The incident was first noticed as connectivity issues with the File Manager, which runs Monsta FTP; recent vulnerabilities in Monsta FTP include CVE-2025-34299 (unrestricted file upload) and CVE-2026-60105 (SSRF in versions before 2.14.5). DreamHost has not publicly confirmed the root cause, and the credential exfiltration theory remains speculative.

hackernews · greenchair · Oct 25, 13:09 · [Discussion](https://news.ycombinator.com/item?id=50231166)

**Background**: DreamHost is a well-known web hosting provider that offers shared, VPS, and dedicated hosting services. Monsta FTP is a commercial PHP-based file manager that allows users to manage files over FTP and is often integrated into hosting control panels. FTP itself transmits credentials in plaintext, making it a common target for credential harvesting and data exfiltration. DreamHost experienced a major DDoS attack in August 2024, and this new incident adds to a series of recent security challenges for the company.

<details><summary>References</summary>
<ul>
<li><a href="https://www.runzero.com/blog/monsta-ftp/">Monsta FTP vulnerability : CVE-2025-34299</a></li>
<li><a href="https://www.sentinelone.com/vulnerability-database/cve-2026-60105/">CVE-2026-60105: Monsta FTP SSRF Vulnerability</a></li>
<li><a href="https://www.csidb.net/csidb/incidents/a73790e7-aee7-4956-a752-a09612cc48ab/">DreamHost (2024-08-24) - The Cyber Security Incident Database ...</a></li>

</ul>
</details>

**Discussion**: Commenters speculate that the File Manager, running Monsta FTP, was compromised via a recently published PHP vulnerability, leading to possible FTP credential exfiltration. Some users express validation for having migrated away from DreamHost years ago, while others question whether DreamHost is "falling apart" and note they initially thought the issue was on their end.

**Tags**: `#security`, `#hosting`, `#dreamhost`, `#incident`, `#php`

---

<a id="item-8"></a>
## [Blind test compares five self-hosted AI agents on local Qwen model](https://www.reddit.com/r/MachineLearning/comments/1xfgf1w/i_ran_a_blind_test_on_selfhosted_ai_agents_here/) ⭐️ 6.0/10

A Reddit user ran a blind test of five self-hosted AI agents (OpenCode, goose, Atomic Agent, Hermes, and OpenClaw) on the same local Qwen 3.8 27B uncensored Q4_K_M model via llama.cpp, across five everyday coding tasks on an M5 Max MacBook Pro with 64GB RAM. The agents were anonymized as A–E, and results showed all five passed contact merging, function renaming, and log error counting, while four passed bug fixing and receipt-to-spreadsheet conversion, with one agent failing due to asking for permission to install a library. This hands-on comparison provides practical insights for the local-LLM community, highlighting trade-offs between agent autonomy and safety when running on consumer hardware. It shows that even with the same underlying model, agent scaffolding and permission policies significantly affect task success and user experience. The test used auto-approve mode with a script deciding pass/fail, and one agent (C) failed the receipt task because it stopped to ask for permission to install a missing Python library, which went unanswered. Agent A completed all tasks in 10:29 total, while B took 24:07, and the author notes that in an unattended setting, asking for permission counts as a failure.

reddit · r/MachineLearning · /u/GapNew4766 · Oct 25, 22:57

**Background**: Self-hosted AI agents are tools that run locally on a user's machine, often using open-source models like Qwen, and can perform tasks such as coding or data manipulation. llama.cpp is a popular open-source library for running large language models locally, and Q4_K_M is a 4-bit quantization method that reduces model size and memory usage with minimal quality loss, making it feasible to run a 27B model on a high-end laptop.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Llama.cpp">Llama.cpp</a></li>
<li><a href="https://localmodel.run/guides/quantization">Quantization explained: Q4_K_M vs Q8_0 vs FP16 · localmodel.run</a></li>
<li><a href="https://huggingface.co/JonathanColetti/Qwen3.8-27B-Uncensored-GGUF">JonathanColetti/ Qwen 3 . 8 - 27 B - Uncensored -GGUF · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#self-hosted-ai`, `#ai-agents`, `#local-llm`, `#benchmarking`, `#llama.cpp`

---

<a id="item-9"></a>
## [Reddit discussion: challenges in creating edge-case datasets for fine-tuning open-weight models](https://www.reddit.com/r/MachineLearning/comments/1xfa17z/whats_the_hardest_part_of_creating_edge_cases_for/) ⭐️ 5.0/10

A Reddit user on r/MachineLearning posed a detailed question about the practical difficulties of building edge-case datasets for fine-tuning open-weight models, covering identification, generation, quality control, coverage, and impact measurement. The post has received limited engagement so far, with no substantive answers visible. As more teams fine-tune open-weight models for specialized tasks, the quality of edge-case data often determines real-world robustness, yet there is little shared methodology for systematically sourcing and validating such data. The questions raised reflect common pain points that could inform better tooling and best practices. The post breaks the problem into five areas: finding rare edge cases, generating examples (manual vs. synthetic vs. mined real data), quality control for incorrect or repetitive examples, knowing when coverage is sufficient, and measuring whether added edge cases actually improve or degrade model performance.

reddit · r/MachineLearning · /u/Humble-Shopping-9495 · Oct 25, 18:35

**Background**: Fine-tuning adapts a pre-trained open-weight model (e.g., Llama, Mistral) to a specific task using a smaller labeled dataset. Edge cases are rare or atypical inputs that fall outside the common distribution but are critical for robustness. Synthetic data generation uses a capable model to produce training examples, which can bootstrap datasets but risks quality issues like repetition or unrealistic patterns.

<details><summary>References</summary>
<ul>
<li><a href="https://fastino.ai/blog/how-to-fine-tune-open-weights-models-model-selection-data-curation-fine-tuning-strategies-and-evals">How to fine-tune open weights models: Model selection, data ...</a></li>
<li><a href="https://www.ertas.ai/blog/synthetic-data-generation-fine-tuning">Synthetic Data Generation for Fine - Tuning : Techniques... - Ertas AI</a></li>
<li><a href="https://keylabs.ai/blog/identifying-and-annotating-rare-edge-cases-to-improve-model-robustness/">Edge Case Curation for Robust Models | Keylabs</a></li>

</ul>
</details>

**Tags**: `#fine-tuning`, `#open-weight models`, `#edge cases`, `#dataset construction`, `#synthetic data`

---

<a id="item-10"></a>
## [Serbia's Vucic Concedes Election Defeat to Student Movement](https://www.reuters.com/world/europe/serbia-votes-students-seek-unseat-vucic-snap-election-2026-10-25/) ⭐️ 4.0/10

Serbian President Aleksandar Vucic conceded defeat in the country's early parliamentary election, losing to a student-led movement that had organized mass anti-corruption protests for nearly two years. The result marks the end of Vucic's 14-year grip on power. This is a major political shift in the Balkans, potentially reversing a decade of democratic backsliding and media suppression under Vucic. It could inspire similar youth-led movements across Europe and reshape Serbia's relations with the EU and Russia. The election was a snap parliamentary vote held after two years of student-led protests against corruption and media freedom restrictions. Vucic, who served as president from 2017 to 2026, had been accused of authoritarian rule and stifling independent journalism.

hackernews · consumer451 · Oct 25, 21:08 · [Discussion](https://news.ycombinator.com/item?id=50236081)

**Background**: Aleksandar Vucic has dominated Serbian politics since 2014, first as prime minister and then as president, consolidating power through control of media and state institutions. Serbia has been a candidate for EU membership, but Brussels has repeatedly criticized its deteriorating media freedom and rule of law. The student movement emerged in response to corruption and a crackdown on dissent, gaining widespread public support.

<details><summary>References</summary>
<ul>
<li><a href="https://www.dw.com/en/serbia-election-student-movement-seeks-to-end-aleksandar-vucics-rule/a-79753482">Serbia election: Student movement seeks to end Vucic's rule</a></li>
<li><a href="https://apnews.com/article/serbia-students-election-vucic-b063b0ad14261bb74ad415bfed141941">Serbia's parliament election is down to students vs. populist ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed relief and hope, with one calling it a 'beautiful day' after 14 years of oppression and lack of media freedom. Others discussed the broader regional context, noting political shifts in Bulgaria and Turkey, and raised concerns about foreign interference in future elections.

**Tags**: `#politics`, `#serbia`, `#elections`, `#geopolitics`, `#media-freedom`

---

<a id="item-11"></a>
## [ICLR 2027 continues desk rejections to curb AI-generated submissions](https://www.reddit.com/r/MachineLearning/comments/1xeu2z1/iclr_2027_is_still_handing_out_desk_rejects_n/) ⭐️ 4.0/10

A Reddit post on r/MachineLearning notes that ICLR 2027 is still issuing desk rejections, with commenters thanking organizers for 'protecting the community from AI slop.' The discussion highlights ongoing concerns about low-quality, AI-generated papers flooding ML conferences. Desk rejections at major ML conferences like ICLR signal a growing effort to maintain review quality amid a surge of LLM-assisted submissions, affecting researchers who must now ensure compliance with disclosure and reviewer registration rules. This trend could reshape submission norms across the academic ML community. ICLR 2027 desk-rejects papers if none of the authors is registered to review, and the author list is fixed from 18 September 2026. Additionally, papers that make extensive use of LLMs without disclosure are subject to desk rejection, and hallucinated citations have led to desk rejections at NeurIPS, ICLR, ICML, and ACL.

reddit · r/MachineLearning · /u/Temporary_Switch_339 · Oct 25, 05:35

**Background**: ICLR (International Conference on Learning Representations) is a top-tier machine learning conference. Desk rejection means a paper is rejected without full peer review, often due to policy violations. 'AI slop' refers to low-effort, high-volume content generated by AI, which has become a concern in academic publishing as LLMs make it easier to produce plausible-sounding but flawed papers.

<details><summary>References</summary>
<ul>
<li><a href="https://phdflow.ai/guides/desk-rejection-explained">Desk rejection at NeurIPS, ICLR , AAAI: co-authors, not PDFs</a></li>
<li><a href="https://blog.iclr.cc/2025/11/19/">November 19, 2025 – ICLR Blog</a></li>
<li><a href="https://strictcite.com/blog/neurips-2026-hallucinated-citations-desk-reject">NeurIPS Started Desk - Rejecting Papers Over References... — StrictCite</a></li>

</ul>
</details>

**Discussion**: Commenters largely support the desk rejections, framing them as necessary to protect the community from AI-generated low-quality submissions. The overall sentiment is appreciative of organizers' efforts to uphold quality, though the discussion is brief and lacks substantive debate.

**Tags**: `#peer-review`, `#ICLR`, `#academic-publishing`, `#AI-slop`, `#machine-learning`

---