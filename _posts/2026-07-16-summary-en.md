---
layout: default
title: "Horizon Summary: 2026-07-16 (EN)"
date: 2026-07-16
lang: en
---

> From 27 items, 22 important content pieces were selected

---

1. [Thinking Machines Lab Releases Inkling, a 975B Open-Weights MoE Model](#item-1) ⭐️ 9.0/10
2. [xAI Open-Sources Grok Build After Privacy Backlash](#item-2) ⭐️ 9.0/10
3. [Moonshot AI Releases Open-Weight Kimi K3 Model](#item-3) ⭐️ 8.0/10
4. [GPT-5.6 Codex Bug Can Delete User Files](#item-4) ⭐️ 8.0/10
5. [Linus Torvalds: Linux Is Not Anti-AI, Fork If You Disagree](#item-5) ⭐️ 8.0/10
6. [ExTernD: Ternary LLM PTQ with Arbitrary Accuracy](#item-6) ⭐️ 8.0/10
7. [PnP-CoSMo: Plug-and-Play Multi-Contrast MRI Reconstruction](#item-7) ⭐️ 8.0/10
8. [Schema Harness Achieves 99% on ARC-AGI-3](#item-8) ⭐️ 8.0/10
9. [Decoy Font: Visual Illusion Fools AI Vision Models](#item-9) ⭐️ 7.0/10
10. [OnePlus Halts New Product Launches in Europe and North America](#item-10) ⭐️ 7.0/10
11. [DABSN: New Recurrent LM Architecture Seeks Collaborators](#item-11) ⭐️ 7.0/10
12. [Rethinking AI Memory: From Facts to Reasoning Patterns](#item-12) ⭐️ 7.0/10
13. [QLoRA default learning rate 2e-4 causes overfitting on small datasets](#item-13) ⭐️ 7.0/10
14. [Microsoft Comic Chat Open-Sourced After 30 Years](#item-14) ⭐️ 6.0/10
15. [Classical ML for LLM Text Detection: Feasibility Debated](#item-15) ⭐️ 6.0/10
16. [Interactive Linear Algebra Book Draws Praise and Critique](#item-16) ⭐️ 6.0/10
17. [Mermaid to Unicode Box Art via WebAssembly](#item-17) ⭐️ 6.0/10
18. [Best Python Tools for Multi-Objective Surrogate-Based Optimization](#item-18) ⭐️ 6.0/10
19. [Google Rebrands NotebookLM to Gemini Notebook](#item-19) ⭐️ 5.0/10
20. [Inaugural RTCA Workshop at NeurIPS 2026](#item-20) ⭐️ 5.0/10
21. [ECCV Registration Fees Spark Student Outrage](#item-21) ⭐️ 4.0/10
22. [Reddit User Seeks Efficient AI/ML News Curation](#item-22) ⭐️ 3.0/10

---

<a id="item-1"></a>
## [Thinking Machines Lab Releases Inkling, a 975B Open-Weights MoE Model](https://simonwillison.net/2026/Jul/16/inkling/#atom-everything) ⭐️ 9.0/10

Thinking Machines Lab, founded by Mira Murati, released Inkling, a 975B-parameter open-weights Mixture-of-Experts multimodal model under the Apache-2.0 license, with 41B active parameters and a 1M-token context window. Inkling strengthens the US open-weights ecosystem, offering a competitive alternative to Chinese open models and enabling fine-tuning via the Tinker platform, potentially accelerating AI customization and research. Inkling is not a frontier model but a strong base for fine-tuning, trained on 45 trillion tokens of text, images, audio, and video. A smaller variant, Inkling-Small (276B total, 12B active), is still being tested.

rss · Simon Willison · Jul 16, 15:35

**Background**: Mixture-of-Experts (MoE) is a neural network architecture that activates only a subset of parameters per input, enabling larger total parameter counts with lower computational cost. Open-weights models make trained parameters publicly available, allowing fine-tuning and deployment by anyone.

<details><summary>References</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/introducing-inkling/">Inkling: Our open-weights model - Thinking Machines Lab</a></li>
<li><a href="https://www.marktechpost.com/2026/07/15/thinking-machines-lab-releases-inkling-a-975b-parameter-open-weights-multimodal-moe-with-41b-active-parameters-and-controllable-thinking-effort/">Thinking Machines Lab Releases Inkling: A 975B-Parameter Open ...</a></li>
<li><a href="https://alphasignal.ai/news/mira-murati-s-thinking-machines-drops-inkling-a-975b-open-multimodal-reasoning">Mira Murati's Thinking Machines Drops Inkling, a 975B Open ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#open-weights`, `#multimodal`, `#Mixture-of-Experts`, `#Mira Murati`

---

<a id="item-2"></a>
## [xAI Open-Sources Grok Build After Privacy Backlash](https://simonwillison.net/2026/Jul/15/grok-build/#atom-everything) ⭐️ 9.0/10

xAI released the entire Grok Build codebase under the Apache 2.0 license after the grok CLI tool was found to upload entire directories to cloud storage, including sensitive user data. The company deleted all retained user data and disabled default data retention. This incident highlights critical privacy risks in AI-powered developer tools and sets a precedent for transparency through open-sourcing. The move may restore user trust and encourage other companies to adopt similar practices. The Grok Build codebase contains 844,530 lines of Rust, with only about 3% vendored code. The repository has a single initial commit, providing no commit history. The subagent system prompt includes a directive not to reveal its contents to the user.

rss · Simon Willison · Jul 15, 23:59

**Background**: The grok CLI tool is a coding agent that runs in the terminal, using xAI's Grok models. Users discovered that running the tool in a directory would upload the entire directory to xAI's Google Cloud buckets, exposing SSH keys, password databases, and other private files. This led to widespread backlash and prompted xAI to act.

<details><summary>References</summary>
<ul>
<li><a href="https://x.ai/cli">Grok Build | SpaceXAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apache_License">Apache License</a></li>

</ul>
</details>

**Discussion**: The community expressed outrage over the privacy violation, with one user reporting that their entire home directory was uploaded. The open-sourcing was seen as a positive step, but some questioned whether it was sufficient to rebuild trust. Others appreciated the transparency and the ability to run the tool locally.

**Tags**: `#AI`, `#security`, `#open source`, `#CLI`, `#privacy`

---

<a id="item-3"></a>
## [Moonshot AI Releases Open-Weight Kimi K3 Model](https://www.kimi.com/blog/kimi-k3) ⭐️ 8.0/10

Moonshot AI has released Kimi K3, an open-weight large language model with a 1M-token context window, claiming frontier-level performance second only to Claude Fable 5 and GPT-5.6 Sol in their evaluations. This release intensifies the commoditization of AI intelligence by Chinese labs, potentially pressuring US frontier models on pricing and openness, while raising data privacy concerns due to Moonshot's policy of training on API usage data. Kimi K3 is designed for long-horizon coding and end-to-end knowledge work, with full model weights to be released in the coming days along with a technical report. The model is available via the Kimi API platform.

hackernews · vincent_s · Jul 16, 14:46 · [Discussion](https://news.ycombinator.com/item?id=48935342)

**Background**: Open-weight models release the trained neural network weights but not the full training code or data, allowing others to run and fine-tune the model. Moonshot AI is a Beijing-based company founded in 2023, known as one of China's 'AI Tiger' companies focusing on large language models.

<details><summary>References</summary>
<ul>
<li><a href="https://platform.kimi.ai/docs/guide/kimi-k3-quickstart">Kimi K3 - Kimi API Platform</a></li>
<li><a href="https://en.wikipedia.org/wiki/Moonshot_AI">Moonshot AI - Wikipedia</a></li>
<li><a href="https://medium.com/lets-code-future/open-weight-ai-models-what-they-are-and-why-openais-next-move-matters-f86fe481973a">Open - Weight AI Models : What They Are, and Why... | Medium</a></li>

</ul>
</details>

**Discussion**: Commenters expressed concerns about Moonshot training on API data, with one noting the policy allows use of content to improve services. Another speculated that Chinese labs are commoditizing intelligence to drive hardware sales, while a third pointed out that the model's censorship may be client-side rather than native.

**Tags**: `#AI`, `#open-source`, `#China`, `#large language model`, `#commoditization`

---

<a id="item-4"></a>
## [GPT-5.6 Codex Bug Can Delete User Files](https://simonwillison.net/2026/Jul/16/bad-codex-bug/#atom-everything) ⭐️ 8.0/10

OpenAI's GPT-5.6 Codex has a bug where it can delete user files when full access mode is enabled without sandboxing, due to an error in overriding the $HOME environment variable. This bug highlights significant safety risks in AI coding agents, especially for developers who rely on these tools for automated code generation and execution. It underscores the need for robust sandboxing and review mechanisms in AI-assisted development environments. The bug occurs when the model attempts to override $HOME to define a temporary directory but mistakenly deletes $HOME instead. The issue is most common when full access mode is enabled and sandboxing protections like auto review are disabled.

rss · Simon Willison · Jul 16, 17:45

**Background**: GPT-5.6 Codex is an AI coding agent from OpenAI that can generate code, run terminal commands, and debug code. Sandboxing isolates agent execution from the host system to prevent unintended actions. The $HOME environment variable points to the user's home directory, and overriding it incorrectly can lead to file deletion.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.3-Codex">GPT-5.3-Codex</a></li>
<li><a href="https://www.firecrawl.dev/blog/ai-agent-sandbox">AI Agent Sandbox: How to Safely Run Autonomous Agents in 2026</a></li>

</ul>
</details>

**Tags**: `#codex`, `#coding-agents`, `#generative-ai`, `#ai-safety`, `#bug`

---

<a id="item-5"></a>
## [Linus Torvalds: Linux Is Not Anti-AI, Fork If You Disagree](https://simonwillison.net/2026/Jul/16/linus-torvalds/#atom-everything) ⭐️ 8.0/10

Linus Torvalds, the creator of Linux, stated on the Linux Media mailing list that Linux is not an anti-AI project and that AI is a clearly useful tool, inviting dissenters to fork or leave. This authoritative endorsement from the top-level maintainer signals a strong pro-AI direction for the Linux kernel project, potentially influencing the broader open-source community's stance on AI integration. Torvalds emphasized that AI is a tool like any other, and its usefulness is no longer in question, though he acknowledged other open questions about AI's economy.

rss · Simon Willison · Jul 16, 13:26

**Background**: Linus Torvalds is the creator and lead maintainer of the Linux kernel, one of the largest open-source projects. His statements carry significant weight in the open-source community. The debate over AI in open source has been contentious, with some projects adopting AI tools and others opposing them on ethical or practical grounds.

**Tags**: `#Linux`, `#AI`, `#Open Source`, `#Kernel Development`

---

<a id="item-6"></a>
## [ExTernD: Ternary LLM PTQ with Arbitrary Accuracy](https://www.reddit.com/r/MachineLearning/comments/1uy2zb3/externd_expandedrank_ternary_decomposition/) ⭐️ 8.0/10

ExTernD introduces expanded-rank ternary decomposition for post-training quantization of LLMs, decomposing each weight matrix into two ternary matrices and a diagonal scaling matrix to overcome the fixed-size limitation of ternary quantization. This approach enables ternary quantization to achieve accuracy approaching any quantization level with only a modest increase in VRAM, potentially making high-accuracy LLM deployment more efficient on resource-constrained hardware. The inner rank can be arbitrarily large, allowing accuracy to be arbitrarily fine-tuned, and the method requires only slightly more VRAM than current quantization methods while leveraging efficient ternary arithmetic.

reddit · r/MachineLearning · /u/LMTLS5 · Jul 16, 13:31

**Background**: Post-training quantization (PTQ) reduces the precision of LLM weights to lower bit-widths (e.g., 4-bit, 2-bit, or ternary) to decrease memory and computation. Ternary quantization uses values in {-1, 0, +1}, but previous methods were limited by fixed matrix size, restricting accuracy. ExTernD addresses this by decomposing the matrix into two ternary matrices and a diagonal scaling matrix, expanding the effective rank.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2607.13511">[2607.13511] ExTernD: Expanded - Rank Ternary Decomposition ...</a></li>
<li><a href="https://arxiv.org/html/2607.13511">ExTernD: Expanded - Rank Ternary Decomposition Ternary LLM...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Matrix_decomposition">Matrix decomposition - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#quantization`, `#ternary`, `#PTQ`, `#model compression`

---

<a id="item-7"></a>
## [PnP-CoSMo: Plug-and-Play Multi-Contrast MRI Reconstruction](https://www.reddit.com/r/MachineLearning/comments/1uy2h66/pnpcosmo_a_multicontrast_mri_reconstruction/) ⭐️ 8.0/10

PnP-CoSMo is a novel plug-and-play framework for multi-contrast MRI reconstruction that learns contrast-invariant content and style from image-domain data, eliminating the need for raw k-space training data. The paper was published in Medical Image Analysis. This approach removes a major data bottleneck in machine learning-based MRI reconstruction by not requiring raw k-space data, and it generalizes across different MR contrasts and forward operators. It could accelerate clinical MRI workflows and improve reconstruction quality without extensive paired training datasets. The framework consists of two stages: first, a content/style model is learned purely from image-domain data; second, the frozen model serves as a prior in iterative reconstruction. It is designed to be generalizable and provides an built-in explanatory framework.

reddit · r/MachineLearning · /u/void_gear · Jul 16, 13:10

**Background**: Multi-contrast MRI acquires images with different tissue contrasts, aiding diagnosis but requiring long scan times. Accelerating acquisition via undersampling and reconstruction is common, but many deep learning methods need raw k-space data for training, which is often unavailable. Content/style modeling separates image content (anatomy) from style (contrast), enabling contrast-invariant priors.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2509.04888">[2509.04888] INR meets Multi-Contrast MRI Reconstruction Deep unregistered multi-contrast MRI reconstruction Multi-Contrast MRI Reconstruction Based on Frequency Domain ... A plug-and-play method for guided multi-contrast MRI ... Prior-Guided Image Reconstruction for Accelerated Multi ... [2409.14113] Accelerated Multi-Contrast MRI Reconstruction ... Fast Multi-contrast MRI Reconstruction</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S0730725X21000795">Deep unregistered multi-contrast MRI reconstruction</a></li>
<li><a href="https://ieeexplore.ieee.org/document/10497580">Multi-Contrast MRI Reconstruction Based on Frequency Domain ...</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion is substantive, with the author engaging and explaining the work. Commenters appreciate the novelty of avoiding raw k-space data and the plug-and-play nature, though some ask about computational cost and comparison with existing methods.

**Tags**: `#MRI reconstruction`, `#machine learning`, `#medical imaging`, `#plug-and-play`, `#content/style modeling`

---

<a id="item-8"></a>
## [Schema Harness Achieves 99% on ARC-AGI-3](https://www.reddit.com/r/MachineLearning/comments/1uyf8oo/new_fable5opus48_harness_called_schema_claims_99/) ⭐️ 8.0/10

A new harness called Schema achieves 99% on the ARC-AGI-3 Public set using Claude Opus 4.8 and Fable 5, without modifying model weights. This near-perfect score on a challenging interactive reasoning benchmark suggests that improving the inference process around models can dramatically boost performance, potentially shifting focus from scaling models to engineering better harnesses. Schema uses a fixed fallback rule: Opus 4.8 and Sol xhigh run first; games scoring below 80 are rerun with Fable 5 and Sol max, and the higher per-game score is retained. It also achieves 95.35% using GPT-5.6 Sol.

reddit · r/MachineLearning · /u/we_are_mammals · Jul 16, 21:02

**Background**: ARC-AGI-3 is an interactive reasoning benchmark where AI agents must explore novel grid-world environments, infer rules, and achieve goals through trial and error. Unlike static puzzles, it tests an agent's ability to adapt and learn on the fly. A harness is a system that orchestrates how a model interacts with the environment, including observation processing, prediction testing, and plan execution.

<details><summary>References</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>
<li><a href="https://the-decoder.com/new-arc-agi-3-benchmark-shows-that-humans-still-outperform-llms-at-pretty-basic-thinking/">New ARC - AGI - 3 benchmark shows that humans still outperform LLMs...</a></li>
<li><a href="https://huggingface.co/blog/Svngoku/claude-fable-5-technical-harness-report">Claude Fable 5 — Technical Harness Report</a></li>

</ul>
</details>

**Discussion**: The post aims to foster technical discussion, and the president of ARC Prize acknowledged it, saying 'Looks cool - need to dig into it.' No direct community comments are provided in the content.

**Tags**: `#ARC-AGI`, `#AI benchmarking`, `#harness`, `#Claude Opus`, `#Fable 5`

---

<a id="item-9"></a>
## [Decoy Font: Visual Illusion Fools AI Vision Models](https://www.mixfont.com/experiments/decoy-font) ⭐️ 7.0/10

Decoy Font is a font that displays different text to humans and AI vision models by exploiting differences in how they process high-frequency versus low-frequency image details. This demonstrates a creative adversarial attack on computer vision systems, highlighting vulnerabilities in AI perception that could have implications for AI safety and security. The font uses high-frequency outlines for one text and low-frequency shading for another, so humans see the low-frequency text while AI models focus on high-frequency details.

hackernews · ray__ · Jul 16, 16:18 · [Discussion](https://news.ycombinator.com/item?id=48936584)

**Background**: Computer vision models often rely on high-frequency features like edges and fine details, while human vision is more sensitive to low-frequency patterns like shapes and blobs. Adversarial examples exploit such differences to cause misclassification. Decoy Font is a practical example of this principle applied to text.

**Discussion**: Community comments show mixed reactions: some find it cool but not practically useful, while others report successful tests with GPT, Gemini, and Claude. One user noted that dark background themes can reveal the decoy text, affecting the illusion.

**Tags**: `#adversarial AI`, `#font design`, `#computer vision`, `#visual illusion`, `#AI safety`

---

<a id="item-10"></a>
## [OnePlus Halts New Product Launches in Europe and North America](https://community.oneplus.com/thread/2170715118587871237) ⭐️ 7.0/10

OnePlus has decided to stop launching new products in Europe and North America, but will continue to support existing devices with software updates and security patches. This marks a significant retreat from key Western markets for OnePlus, which was once a popular 'hacker's choice' for its stock Android experience and unlocked bootloaders. The move reflects the brand's integration into OPPO and a shift in global strategy. Existing OnePlus devices in these regions will continue to receive scheduled software updates and security patches within their original support periods. The company is backed by OPPO, ensuring ongoing support.

hackernews · pilililo2 · Jul 16, 10:14 · [Discussion](https://news.ycombinator.com/item?id=48932539)

**Background**: OnePlus was founded in 2013 with a focus on high-spec, affordable smartphones with near-stock Android. It gained a loyal following among enthusiasts for offering unlocked bootloaders and factory images. Over time, the brand shifted toward mainstream consumers and integrated more closely with parent company OPPO, leading to changes in software and hardware strategy.

**Discussion**: Community comments express disappointment, with users noting OnePlus's decline from its enthusiast roots. Some clarify that the news is about halting new product launches, not full operations, and highlight that existing devices will still be supported. Former employees mention a demanding work culture and hollowed-out staffing.

**Tags**: `#OnePlus`, `#smartphone`, `#business strategy`, `#tech industry`

---

<a id="item-11"></a>
## [DABSN: New Recurrent LM Architecture Seeks Collaborators](https://www.reddit.com/r/MachineLearning/comments/1uycffg/seeking_collaborators_for_scaling_and_independent/) ⭐️ 7.0/10

The author introduces DABSN (Dynamic Adaptive Bias State Network), a novel recurrent architecture for language models, and shares a preprint with open-source code. A 24M-parameter model trained on 1B tokens shows promising results, and the author seeks collaborators for scaling and independent evaluation. This work could offer an alternative to transformer-based models, potentially improving efficiency for long-context tasks. Open collaboration may accelerate development and validation of recurrent architectures in the LLM ecosystem. The architecture is evaluated on reasoning, memory, and long-sequence benchmarks including MQAR, Copy, Key-Value retrieval, and A5/60. Implementations are provided in PyTorch, C++, and Triton for reproducibility.

reddit · r/MachineLearning · /u/BleedingXiko · Jul 16, 19:17

**Background**: Recurrent neural networks (RNNs) process sequences step by step, making them efficient for long contexts but historically harder to train than transformers. DABSN aims to improve upon traditional RNNs with adaptive bias mechanisms, potentially bridging the gap with attention-based models.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/multi-query-associative-recall-mqar">MQAR : Multi-Query Associative Recall</a></li>

</ul>
</details>

**Tags**: `#recurrent architecture`, `#language model`, `#open source`, `#research collaboration`, `#scaling`

---

<a id="item-12"></a>
## [Rethinking AI Memory: From Facts to Reasoning Patterns](https://www.reddit.com/r/MachineLearning/comments/1uy6yht/are_current_ai_memory_architectures_optimizing/) ⭐️ 7.0/10

A Reddit post questions whether current AI memory architectures should shift from storing descriptive facts to inferring higher-level reasoning patterns, such as a user's explanatory frameworks and characteristic reasoning styles. This proposal could fundamentally change how AI systems personalize interactions, moving beyond simple fact recall to modeling how users think, potentially enabling deeper, more adaptive assistance. The author contrasts current descriptive memory (e.g., 'user is interested in economics') with an inferential memory that captures patterns like 'user explains economic outcomes through incentives and institutional constraints.'

reddit · r/MachineLearning · /u/Boris_Ljevar · Jul 16, 16:00

**Background**: Current AI memory systems, such as those used in chatbots and agents, primarily store facts, preferences, and conversation summaries in a descriptive manner. These systems rely on retrieval-augmented generation (RAG) and persistent context to recall information. The post speculates whether future systems could evolve to infer and refine abstract reasoning patterns from interactions, effectively building a model of the user's cognitive style.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/IAAR-Shanghai/Awesome-AI-Memory">IAAR-Shanghai/Awesome-AI-Memory - GitHub</a></li>
<li><a href="https://zylos.ai/research/2026-04-05-ai-agent-memory-architectures-persistent-knowledge/">AI Agent Memory Architectures: From Context Windows to ...</a></li>
<li><a href="https://ajithp.com/2025/06/30/ai-native-memory-persistent-agents-second-me/">AI-Native Memory and the Rise of Context-Aware AI Agents ...</a></li>

</ul>
</details>

**Tags**: `#AI memory`, `#machine learning`, `#cognitive architectures`, `#context management`, `#reasoning`

---

<a id="item-13"></a>
## [QLoRA default learning rate 2e-4 causes overfitting on small datasets](https://www.reddit.com/r/MachineLearning/comments/1uy1z8b/the_qlora_2e4_default_is_wrong_under_10k_samples/) ⭐️ 7.0/10

A Reddit user discovered that the default QLoRA learning rate of 2e-4 leads to overfitting on datasets with fewer than 10,000 samples, and reducing it to 1e-4 significantly improves evaluation performance. This finding challenges widely adopted defaults from tutorials and the QLoRA paper, potentially saving ML practitioners weeks of debugging and improving fine-tuning outcomes for small custom datasets. The user reports that with 2e-4, the model overfits within the first epoch, while dropping to 1e-4 and increasing epochs from 3 to 5 produced the best evaluation gains. They suggest a rule: above 30k samples use 2e-4, under 10k start at 1e-4 or lower.

reddit · r/MachineLearning · /u/Pretty-Ad774 · Jul 16, 12:50

**Background**: QLoRA is a parameter-efficient fine-tuning method that quantizes the base model to 4-bit and trains low-rank adapters. The default learning rate of 2e-4 originates from the Alpaca dataset (52k samples) and is widely copied in tutorials. Small datasets (<10k) are common for custom tasks, making this a practical issue.

<details><summary>References</summary>
<ul>
<li><a href="https://www.heulistic.com/blog/learning-rate-qlora-fine-tuning">What Learning Rate to Use for QLoRA Fine-Tuning</a></li>
<li><a href="https://medium.com/@matteo28/qlora-fine-tuning-with-unsloth-a-complete-guide-8652c9c7edb3">QLoRA Fine-Tuning with Unsloth | Medium</a></li>
<li><a href="https://deepwiki.com/artidoro/qlora">artidoro/qlora | DeepWiki</a></li>

</ul>
</details>

**Discussion**: The post received strong engagement, with many commenters sharing similar experiences and validating the finding. Some debated the exact threshold and suggested also tuning rank and alpha. A few noted that the QLoRA paper itself used 2e-4 only for larger datasets.

**Tags**: `#QLoRA`, `#fine-tuning`, `#learning rate`, `#overfitting`, `#LLM`

---

<a id="item-14"></a>
## [Microsoft Comic Chat Open-Sourced After 30 Years](https://opensource.microsoft.com/blog/2026/07/16/microsoft-comic-chat-is-now-open-source/) ⭐️ 6.0/10

On July 16, 2026, Microsoft released the source code for Comic Chat (later renamed Microsoft Chat), a graphical IRC client from 1996, under an open-source license on the Microsoft Open Source Blog. This open-sourcing preserves a piece of internet history and allows developers to study, modify, and run a nostalgic chat client that pioneered comic-style avatars in online conversations. Comic Chat was developed by Microsoft researcher David Kurlander and first shipped with Internet Explorer 3.0 in 1996; it extended the IRC protocol with custom messages for character appearance and emoting, which some in the IRC community criticized.

hackernews · jervant · Jul 16, 16:06 · [Discussion](https://news.ycombinator.com/item?id=48936426)

**Background**: IRC (Internet Relay Chat) is a text-based chat protocol that became popular in the 1990s for group and private messaging. Comic Chat was a graphical IRC client that automatically rendered conversations as comic strips with characters, balloons, and actions, offering a unique visual experience compared to traditional text-based clients like mIRC.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Comic_Chat">Comic Chat</a></li>
<li><a href="https://opensource.microsoft.com/blog/2026/07/16/microsoft-comic-chat-is-now-open-source/">Microsoft Comic Chat is now open source | Microsoft Open Source Blog</a></li>
<li><a href="https://en.wikipedia.org/wiki/IRC_client">IRC client</a></li>

</ul>
</details>

**Discussion**: Commenters expressed nostalgia and shared personal stories, with one noting it inspired his startup Chogger. Another recalled that Comic Chat was somewhat reviled in the IRC community for extending the protocol with non-standard features. The original developer was credited by the person who made the open-sourcing happen.

**Tags**: `#open source`, `#microsoft`, `#irc`, `#retro computing`, `#nostalgia`

---

<a id="item-15"></a>
## [Classical ML for LLM Text Detection: Feasibility Debated](https://blog.lyc8503.net/en/post/llm-classifier/) ⭐️ 6.0/10

A blog post explores using classical machine learning (e.g., SVM, Naive Bayes) to detect LLM-generated text, presenting a small-scale experiment with Chinese text. This approach offers a lightweight alternative to deep learning detectors, but community skepticism highlights fundamental limitations in reliably distinguishing AI-generated text from human-written content. The classifier is small enough to potentially run in a browser extension, but its accuracy may degrade as LLMs evolve and adopt new phrasing patterns.

hackernews · uneven9434 · Jul 16, 16:41 · [Discussion](https://news.ycombinator.com/item?id=48936880)

**Background**: LLM-generated text detection is a binary classification task that aims to determine whether a text was produced by an AI. Methods include watermarking, statistical analysis, neural detectors, and human-assisted approaches. Classical ML techniques like SVM and Naive Bayes have long been used for text classification tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://direct.mit.edu/coli/article/51/1/275/127462/A-Survey-on-LLM-Generated-Text-Detection-Necessity">A Survey on LLM-Generated Text Detection: Necessity, Methods ...</a></li>
<li><a href="https://arxiv.org/abs/2310.14724">[2310.14724] A Survey on LLM-Generated Text Detection ... AI-generated text detection: A comprehensive review of ... A Survey on LLM-Generated Text Detection: Necessity, Methods ... The State of the Art in Detecting LLM-Generated Text in ... The Science of Detecting LLM-Generated Text NLP2CT/LLM-generated-Text-Detection - GitHub</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S1574013725000693">AI-generated text detection: A comprehensive review of ...</a></li>

</ul>
</details>

**Discussion**: Commenters are largely skeptical: one argues text lacks information density for reliable provenance detection, calling it 'tarot card reading.' Another suggests measuring effort rather than AI origin. A third proposes browser-based detection but acknowledges limitations.

**Tags**: `#LLM detection`, `#machine learning`, `#AI-generated text`, `#classification`

---

<a id="item-16"></a>
## [Interactive Linear Algebra Book Draws Praise and Critique](https://immersivemath.com/ila/) ⭐️ 6.0/10

The Immersive Linear Algebra book, published in 2015, offers interactive figures to visualize concepts, making it a unique educational resource. This approach could improve math education by making abstract concepts more accessible, but the lack of rigorous proofs limits its use for deeper learning. The book is praised for its interactive visualizations but criticized for omitting theorems and proofs, which some consider essential for true understanding.

hackernews · srean · Jul 16, 15:32 · [Discussion](https://news.ycombinator.com/item?id=48935951)

**Background**: Linear algebra is a foundational math subject involving vectors, matrices, and transformations. Traditional textbooks rely on static diagrams, while this book uses interactive figures to illustrate concepts dynamically.

**Discussion**: Comments are largely positive, with users expressing nostalgia and appreciation for the interactive approach. However, one commenter criticizes the lack of depth, noting that programmers often favor visual simplifications over rigorous proofs.

**Tags**: `#linear algebra`, `#education`, `#interactive`, `#visualization`

---

<a id="item-17"></a>
## [Mermaid to Unicode Box Art via WebAssembly](https://simonwillison.net/2026/Jul/16/grok-mermaid/#atom-everything) ⭐️ 6.0/10

Simon Willison ported a Rust-based Mermaid-to-Unicode renderer from the open-sourced Grok CLI codebase to WebAssembly, enabling terminal-style diagram rendering directly in the browser. This tool demonstrates a practical use of WebAssembly to bring a Rust library into the browser, allowing developers to render Mermaid diagrams as Unicode box art without a server or JavaScript library. The renderer is self-contained and originally part of xAI's Grok Build coding agent. Willison used Claude Code for web (Fable 5) to generate the WebAssembly integration, and the tool includes controls for max width, copy as text, and copy link.

rss · Simon Willison · Jul 16, 00:33

**Background**: Mermaid is a popular JavaScript-based diagramming tool that renders diagrams in the browser. WebAssembly (WASM) allows code written in languages like Rust to run in the browser at near-native speed. This project compiles a Rust Mermaid renderer to WASM, enabling diagram rendering without the full Mermaid JavaScript library.

<details><summary>References</summary>
<ul>
<li><a href="https://mermaid.js.org/intro/syntax-reference.html">Diagram Syntax | Mermaid</a></li>
<li><a href="https://blog.logrocket.com/implement-webassembly-webgl-viewer-using-rust/">Implement a WebAssembly WebGL viewer using Rust</a></li>
<li><a href="https://www.aimadetools.com/blog/grok-build-complete-guide/">Grok Build Complete Guide: xAI's Multi-Agent Coding CLI (2026)</a></li>

</ul>
</details>

**Tags**: `#WebAssembly`, `#Mermaid`, `#diagrams`, `#Rust`, `#tools`

---

<a id="item-18"></a>
## [Best Python Tools for Multi-Objective Surrogate-Based Optimization](https://www.reddit.com/r/MachineLearning/comments/1uxty9v/best_current_tools_for_multiobjective/) ⭐️ 6.0/10

A Reddit user asked for recommendations on the best Python/Colab-friendly tools for multi-objective surrogate-based optimization (MOSBO) on heterogeneous study data with hierarchical modeling, considering PyMC, pymoo/pysamoo, SMT, and MATLAB. This query highlights the growing need for accessible, open-source MOSBO workflows in applied domains like meta-analysis, where computational efficiency and handling of heterogeneous data are critical. The user has ~40 studies with protocol variables and baseline-dependent outcomes, aiming for continuous optimization of three objectives under physiological constraints. They prefer Colab-friendly solutions due to Chromebook limitations.

reddit · r/MachineLearning · /u/BleakReason · Jul 16, 05:43

**Background**: Multi-objective surrogate-based optimization (MOSBO) uses surrogate models (e.g., kriging, radial basis functions) to approximate expensive objective functions, reducing computational cost. Tools like pysamoo (built on pymoo) and SMT provide ready-to-use algorithms for such tasks. Hierarchical modeling separates protocol effects from baseline effects, common in meta-analysis.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/anyoptimization/pysamoo">GitHub - anyoptimization/pysamoo pysamoo · PyPI [2204.05855] pysamoo: Surrogate-Assisted Multi-Objective ... GitHub - anyoptimization/pysamoo MANY - arXiv.org (PDF) pysamoo: Surrogate-Assisted Multi-Objective ...</a></li>
<li><a href="https://smt.readthedocs.io/">SMT : Surrogate Modeling Toolbox — SMT 2.14.2.dev1+g0d3602a74...</a></li>
<li><a href="https://arxiv.org/html/2412.14854v1">Surrogate-assisted multi-objective design of complex multibody systems</a></li>

</ul>
</details>

**Tags**: `#multi-objective optimization`, `#surrogate modeling`, `#hierarchical modeling`, `#Python tools`, `#meta-analysis`

---

<a id="item-19"></a>
## [Google Rebrands NotebookLM to Gemini Notebook](https://blog.google/innovation-and-ai/products/gemini-notebook/notebooklm-gemini-notebook/) ⭐️ 5.0/10

Google has rebranded NotebookLM to Gemini Notebook, aligning the product name with its Gemini AI model family. The update also introduces the ability to run code directly within notebooks, rolling out to Pro users soon. This rebranding reflects Google's strategy to unify its AI products under the Gemini brand, potentially simplifying user perception. However, the community expresses concerns that name changes often precede feature bloat or product discontinuation at Google. The tool remains a research and note-taking assistant using retrieval-augmented generation (RAG) with Gemini models. The new code execution feature allows deeper data analysis within notebooks, and notebooks will sync across the Gemini app and Google Search.

hackernews · xnx · Jul 16, 16:08 · [Discussion](https://news.ycombinator.com/item?id=48936451)

**Background**: NotebookLM, launched by Google Labs, is an AI-powered research assistant that helps users interact with their documents. It gained popularity for features like Audio Overviews, which generate podcast-like discussions. The rebranding to Gemini Notebook aligns it with Google's broader Gemini ecosystem.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/products/gemini-notebook/notebooklm-gemini-notebook/">NotebookLM is now Gemini Notebook - The Keyword</a></li>
<li><a href="https://en.wikipedia.org/wiki/NotebookLM">NotebookLM</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gemini_Notebook">Gemini Notebook</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed: some users welcome the clearer branding, while others fear this signals eventual enshittification or product death, citing past Google product rebrandings like Hangouts to Meet. A few users also compare NotebookLM's audio features unfavorably to ChatGPT Live.

**Tags**: `#Google`, `#rebranding`, `#AI`, `#product update`

---

<a id="item-20"></a>
## [Inaugural RTCA Workshop at NeurIPS 2026](https://www.reddit.com/r/MachineLearning/comments/1uy8e0v/cfp_rtca_neurips_2026_r/) ⭐️ 5.0/10

The first Real-Time Conversational Agents (RTCA) Workshop has been announced for NeurIPS 2026 in Sydney, Australia, with a call for papers and demos on topics like streaming speech, video generation, and evaluation of live systems. This workshop addresses the critical gap in evaluating and advancing real-time multimodal conversational AI, which is essential for natural human-AI interaction and has implications for voice assistants, avatars, and embodied agents. Submissions are due by August 29, 2026, and the workshop is non-archival, allowing authors to publish elsewhere. Topics include full-duplex audio-language models, turn-taking, and on-device deployment.

reddit · r/MachineLearning · /u/Few-Ferret9700 · Jul 16, 16:51

**Background**: Real-time conversational agents require systems that can listen, speak, and generate video simultaneously with low latency, which is more challenging than offline generation. Full-duplex communication, where both parties can speak at once, is a key capability for natural interaction. NeurIPS is a top machine learning conference, and its workshops highlight emerging research areas.

<details><summary>References</summary>
<ul>
<li><a href="https://neurips.cc/Conferences/2026/WorkshopsGuidance">NeurIPS 2026 Workshops Guidance</a></li>
<li><a href="https://neurips.cc/Conferences/2026/CallForWorkshops">Call For Workshops 2026 - neurips.cc</a></li>
<li><a href="https://www.linkedin.com/posts/niki-foteinopoulou-48aa3b45_rtca-2026-real-time-conversational-agents-activity-7483207605096574977-Wunh">RTCA 2026 | Real-Time Conversational Agents | Niki Foteinopoulou</a></li>

</ul>
</details>

**Tags**: `#NeurIPS`, `#workshop`, `#conversational AI`, `#multimodal`, `#real-time`

---

<a id="item-21"></a>
## [ECCV Registration Fees Spark Student Outrage](https://www.reddit.com/r/MachineLearning/comments/1uxyd6z/why_is_eccv_so_insanely_expensive_for_students/) ⭐️ 4.0/10

A Reddit user reports that ECCV requires paper presenters to pay full registration fees ($805) instead of the student rate ($440), despite being students, and their travel grant and waiver applications were rejected. This policy places a heavy financial burden on student researchers, potentially discouraging participation in top conferences and exacerbating inequities in academic publishing. ECCV 2026 registration information confirms that main conference paper authors must register by July 17, 2026, and the full registration fee includes access to all sessions and materials; student registration is not available for presenting authors.

reddit · r/MachineLearning · /u/NotGondor · Jul 16, 09:55

**Background**: ECCV (European Conference on Computer Vision) is a premier biennial computer vision conference. Many top-tier conferences require at least one author to register at the full rate for each accepted paper, a common but controversial practice that can cost students hundreds of dollars.

<details><summary>References</summary>
<ul>
<li><a href="https://eccv.ecva.net/Conferences/2026/Registration">Registration Information - ECCV 2026</a></li>
<li><a href="https://eccv.ecva.net/Conferences/2024/Registration">Registration Information</a></li>

</ul>
</details>

**Discussion**: The Reddit thread expresses widespread frustration, with users sharing similar experiences and suggesting alternatives like seeking supervisor funding, applying for multiple grants, or presenting remotely if allowed.

**Tags**: `#conference fees`, `#ECCV`, `#student issues`, `#academia`

---

<a id="item-22"></a>
## [Reddit User Seeks Efficient AI/ML News Curation](https://www.reddit.com/r/MachineLearning/comments/1uyecez/whats_the_best_and_complete_way_to_keep_up_with/) ⭐️ 3.0/10

A Reddit user posted a question asking for the best and most complete way to keep up with AI/ML news without spending too much time, expressing that their current newsletter subscription is insufficient. This question highlights a common pain point in the fast-moving AI/ML field, where professionals and enthusiasts struggle to stay informed without being overwhelmed. The discussion could surface useful curation strategies and tools for the community. The post has a low score of 3.0/10, indicating it is a routine question without novel insights. No comments or web search results are available for this analysis.

reddit · r/MachineLearning · /u/mehmetflix_ · Jul 16, 20:28

**Background**: AI/ML news is published across many sources like arXiv, Twitter, newsletters, and blogs, making it hard to track comprehensively. Many professionals rely on curated newsletters or social media, but often feel they miss important updates.

**Tags**: `#AI/ML`, `#news`, `#community`

---