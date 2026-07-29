---
layout: default
title: "Horizon Summary: 2026-07-29 (EN)"
date: 2026-07-29
lang: en
---

> From 24 items, 20 important content pieces were selected

---

1. [Open-source engine runs Gemma 4 26B in 2GB RAM on M-series Macs](#item-1) ⭐️ 8.0/10
2. [Mitchell Hashimoto Launches Superlogical on Ghostty](#item-2) ⭐️ 8.0/10
3. [Long Policy Docs Fail to Govern AI Agents](#item-3) ⭐️ 8.0/10
4. [AI Worm Self-Propagates via Copilot for Word](#item-4) ⭐️ 8.0/10
5. [AI's Role in Post-Quantum Cryptography Transition](#item-5) ⭐️ 8.0/10
6. [Claude Mythos Finds Cryptographic Weaknesses in HAWK and AES](#item-6) ⭐️ 8.0/10
7. [PostSlate achieves 10x speedup with vendor-agnostic Vulkan inference](#item-7) ⭐️ 8.0/10
8. [Vision Pro Used to Walk Through House Design Before Construction](#item-8) ⭐️ 7.0/10
9. [Kimi K3-256k: Half Cost, Same Quality](#item-9) ⭐️ 7.0/10
10. [KOReader: Open-Source E-Reader Enhances E-Ink Devices](#item-10) ⭐️ 7.0/10
11. [AI Companies Hire Thousands of Electricians and Carpenters](#item-11) ⭐️ 7.0/10
12. [ICLR 2027 Deadline Conflicts with NeurIPS 2026 Decisions](#item-12) ⭐️ 7.0/10
13. [Keychron Announces Open-Source Gaming Mouse Firmware](#item-13) ⭐️ 6.0/10
14. [Guide: Adding Custom MCP Servers to Claude and ChatGPT](#item-14) ⭐️ 6.0/10
15. [TanML: Open-Source Toolkit for Tabular Model Validation](#item-15) ⭐️ 6.0/10
16. [SQLite creator compares SQL to COBOL evolution](#item-16) ⭐️ 5.0/10
17. [Workshop Paper Accepted, Reviewers Request New Experiments](#item-17) ⭐️ 4.0/10
18. [NeurIPS E&D: How to respond to ethical reviews?](#item-18) ⭐️ 4.0/10
19. [Claude Experiences Elevated Errors Across All Models](#item-19) ⭐️ 3.0/10
20. [Survey Recruits Users of AI Companions for Research](#item-20) ⭐️ 3.0/10

---

<a id="item-1"></a>
## [Open-source engine runs Gemma 4 26B in 2GB RAM on M-series Macs](https://github.com/drumih/turbo-fieldfare) ⭐️ 8.0/10

TurboFieldfare, an open-source inference engine written in Swift and Metal, streams routed experts from SSD to run the 4-bit quantized Gemma 4 26B-A4B-IT model using only about 2 GB of RAM on any M-series Mac. This enables running a large 26B-parameter MoE model on memory-constrained devices like 8GB MacBooks, democratizing on-device AI and reducing reliance on cloud infrastructure. The engine achieves 5–6 tok/s on an 8GB M2 MacBook Air and 31–35 tok/s on an M5 MacBook Pro, using a small expert cache and bounded parallel pread to overlap SSD reads with GPU computation.

hackernews · gitpusher42 · Jul 29, 15:05 · [Discussion](https://news.ycombinator.com/item?id=49098510)

**Background**: Gemma 4 26B-A4B-IT is a Mixture-of-Experts (MoE) model from Google DeepMind with 25.2B total parameters but only 3.8B active per token. Traditional inference requires loading all weights into RAM, which is prohibitive for memory-limited devices. TurboFieldfare keeps only shared layers and KV cache in RAM, streaming experts on demand from SSD.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/google/gemma-4-26B-A4B-it">google/gemma-4-26B-A4B-it · Hugging Face</a></li>
<li><a href="https://openrouter.ai/google/gemma-4-26b-a4b-it">Gemma 4 26B A4B - API Pricing & Benchmarks | OpenRouter</a></li>

</ul>
</details>

**Discussion**: Commenters praised the approach, with some comparing it to mmap in llama.cpp and noting the advantage of synchronizing SSD reads with inference. Others provided compatibility tips for older macOS versions and expressed interest in running on non-Mac platforms like Debian.

**Tags**: `#on-device AI`, `#inference engine`, `#model quantization`, `#Swift`, `#Metal`

---

<a id="item-2"></a>
## [Mitchell Hashimoto Launches Superlogical on Ghostty](https://www.superlogical.com/) ⭐️ 8.0/10

Mitchell Hashimoto announced Superlogical, a new company building on the open-source libghostty terminal library, with a non-profit foundation now owning the Ghostty project. This move establishes a sustainable open-source model where a company builds proprietary products on top of a community-owned library, potentially inspiring similar structures in other projects. Superlogical will use libghostty as a public building block, consuming the same MIT-licensed components available to everyone, and will upstream shared terminal work for all consumers.

hackernews · yan · Jul 29, 15:41 · [Discussion](https://news.ycombinator.com/item?id=49098965)

**Background**: Ghostty is a fast, feature-rich, cross-platform terminal emulator using platform-native UI and GPU acceleration, created by Mitchell Hashimoto, also known for founding HashiCorp. libghostty is the C-compatible library extracted from Ghostty for embedding terminal functionality in third-party projects.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ghostty-org/ghostty">GitHub - ghostty-org/ghostty: 👻 Ghostty is a fast, feature-rich, and cross-platform terminal emulator that uses platform-native UI and GPU acceleration.</a></li>
<li><a href="https://mitchellh.com/writing/libghostty-is-coming">Libghostty Is Coming – Mitchell Hashimoto</a></li>
<li><a href="https://ghostty.org/">Ghostty</a></li>

</ul>
</details>

**Discussion**: Commenters praised the transfer of Ghostty to a non-profit and the open-source-first approach. Some drew parallels to COM/OLE, while others expressed frustration with the enigmatic title.

**Tags**: `#terminal`, `#open-source`, `#startup`, `#ghostty`, `#mitchellh`

---

<a id="item-3"></a>
## [Long Policy Docs Fail to Govern AI Agents](https://arxiv.org/abs/2607.25398) ⭐️ 8.0/10

A new study, Handbook.md, demonstrates that long policy documents are ineffective for governing AI agents due to context window limitations and model quantization issues. This finding challenges the common practice of using lengthy policy documents to control AI agents, highlighting fundamental limitations in current LLM architectures that affect safety and reliability in autonomous systems. The study shows that even with large context windows, models fail to reliably adhere to long policies, and quantization further degrades compliance. The research provides empirical evidence that shorter, more focused instructions are more effective.

hackernews · spIrr · Jul 29, 13:01 · [Discussion](https://news.ycombinator.com/item?id=49096969)

**Background**: AI agents are autonomous systems that perform tasks based on instructions. Long policy documents are often used to specify rules and constraints. However, LLMs have limited context windows and suffer from quantization errors that reduce their ability to process long texts accurately.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Context_window">Context window - Wikipedia</a></li>
<li><a href="https://atlan.com/know/llm-context-window-limitations/">LLM Context Window Limitations in 2026</a></li>

</ul>
</details>

**Discussion**: Community comments highlight that long context models often fail in practice, with users reporting that explicit instructions in CLAUDE.md files are ignored after a few minutes. Some argue that humans also struggle with long policy documents, so the problem is not unique to AI.

**Tags**: `#AI agents`, `#context window`, `#policy compliance`, `#LLM limitations`, `#research`

---

<a id="item-4"></a>
## [AI Worm Self-Propagates via Copilot for Word](https://enklypesalt.com/posts/context-collapse-part3-ai-worming-through-word/) ⭐️ 8.0/10

Researcher Håkon Måløy demonstrated a new prompt injection variant that turns Microsoft Copilot for Word into a self-replicating AI worm, where malicious instructions hidden in a document can propagate to new documents via Copilot's editing features. This vulnerability highlights a critical security flaw in AI-integrated productivity tools, as it allows AI worms to autonomously spread across documents and potentially access sensitive data, posing risks to enterprise users and the broader ecosystem. The attack works by embedding adversarial prompts in a document; when Copilot processes it, the AI follows the hidden instructions to alter content and propagate the attack to other documents. Two mitigation attempts by Microsoft, including a model upgrade, failed to close the vulnerability class.

hackernews · Canopy9560 · Jul 29, 11:44 · [Discussion](https://news.ycombinator.com/item?id=49096188)

**Background**: Prompt injection is a cybersecurity exploit where malicious inputs cause LLMs to behave unintendedly, as models cannot distinguish between developer instructions and user data. AI worms are self-replicating programs that use LLMs to autonomously spread across systems, as demonstrated in recent research with local open-weight models.

<details><summary>References</summary>
<ul>
<li><a href="https://enklypesalt.com/posts/context-collapse-part3-ai-worming-through-word/">Context Collapse, Part 3 - AI Worming through Word | En Klype Salt</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>
<li><a href="https://www.theregister.com/security/2026/07/29/word-worm-crawls-into-copilot-spreads-chaos/5280588">Word worm crawls into Copilot , spreads chaos</a></li>

</ul>
</details>

**Discussion**: Commenters expressed concern that this vulnerability class is fundamentally unfixable as long as AI cannot distinguish instructions from data. Some users have already uninstalled Copilot to protect their data, while others noted that simple obfuscation techniques like white text still work to hide malicious prompts.

**Tags**: `#AI security`, `#prompt injection`, `#Copilot`, `#cybersecurity`, `#LLM vulnerabilities`

---

<a id="item-5"></a>
## [AI's Role in Post-Quantum Cryptography Transition](https://simonwillison.net/2026/Jul/29/matthew-green/#atom-everything) ⭐️ 8.0/10

Matthew Green highlights that the current shift to post-quantum cryptography is an ideal time for AI to advance cryptanalysis, potentially strengthening confidence in new algorithms like HAWK. This insight is significant because AI-driven cryptanalysis could either undermine or validate post-quantum algorithms, directly impacting the security of future digital infrastructure. The timing aligns with NIST's standardization efforts, making it a critical moment for cryptographic research. Green references HAWK, a lattice-based post-quantum signature scheme in NIST's Round 3, and Impagliazzo's five worlds (e.g., Minicrypt) to frame the uncertainty. He notes that if AI succeeds in breaking hard problems, we might live in Minicrypt where public-key cryptography is impossible.

rss · Simon Willison · Jul 29, 18:18

**Background**: Post-quantum cryptography aims to develop algorithms resistant to quantum computers, which could break current RSA and ECC. NIST is standardizing these algorithms, with HAWK being a candidate. Impagliazzo's five worlds classify computational hardness scenarios, with Minicrypt being a world where one-way functions exist but public-key crypto does not.

<details><summary>References</summary>
<ul>
<li><a href="https://eprint.iacr.org/2026/1078">Post-Quantum HAWK Signature Acceleration with RISC-V-Based Hardware-Software Co-Design</a></li>
<li><a href="https://en.wikipedia.org/wiki/Post-Quantum_Cryptography_Standardization">Post-Quantum Cryptography Standardization</a></li>
<li><a href="https://blog.computationalcomplexity.org/2004/06/impagliazzos-five-worlds.html">Computational Complexity: Impagliazzo's Five Worlds</a></li>

</ul>
</details>

**Tags**: `#cryptography`, `#post-quantum`, `#AI`, `#cryptanalysis`, `#security`

---

<a id="item-6"></a>
## [Claude Mythos Finds Cryptographic Weaknesses in HAWK and AES](https://simonwillison.net/2026/Jul/28/discovering-cryptographic-weaknesses-with-claude/#atom-everything) ⭐️ 8.0/10

Anthropic researchers used their Claude Mythos model to discover mathematical flaws in the HAWK signature scheme and a reduced-round variant of AES, sharing the prompts that guided the model. The work ran for 60 hours at an estimated API cost of $100,000. This demonstrates that large language models can assist in cryptographic research, potentially accelerating the discovery of vulnerabilities. The shared prompts provide unique insight into how to effectively guide an AI model toward complex problem-solving. The discovered weaknesses have no practical impact on current systems: the AES attack targets a reduced-round variant, and the HAWK flaw is theoretical. The model required persistent human encouragement to not give up, as shown in the prompts.

rss · Simon Willison · Jul 28, 22:45

**Background**: Cryptographic hash functions and signature schemes like HAWK are designed to be secure against attacks. Reduced-round AES variants are simplified versions used for research. Claude Mythos is Anthropic's most powerful AI model, with restricted access due to its advanced capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ai-jarvis.eu/anthropics-mythos-found-flaws-aes-and-hawk-cryptography-100000-attack">Anthropic's Mythos Found Flaws in AES and HAWK Cryptography — at...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Mythos">Claude Mythos</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters praised the transparency of sharing prompts and the novel application of LLMs to cryptanalysis. Some questioned the cost-effectiveness, while others noted the importance of human guidance in achieving the results.

**Tags**: `#cryptography`, `#AI`, `#LLM`, `#security`, `#research`

---

<a id="item-7"></a>
## [PostSlate achieves 10x speedup with vendor-agnostic Vulkan inference](https://www.reddit.com/r/MachineLearning/comments/1v9s4mz/vendoragnostic_ml_inference_on_production_edge/) ⭐️ 8.0/10

PostSlate, a video editing tool, achieved vendor-agnostic ML inference on production edge devices using ncnn's Vulkan backend, yielding 10x speedups over ONNX CPU without requiring vendor-specific runtimes. This approach eliminates dependency on vendor-specific GPU runtimes like CUDA, enabling efficient ML inference across diverse hardware (NVIDIA, AMD, Intel, Apple Silicon) with a single backend, which is crucial for edge deployment. On an RTX 4070 with fp16, ArcFace R50 face embedding runs in 3 ms (vs. 30 ms on ONNX CPU) and SCRFD face detection in 2.5 ms (vs. 25 ms). Model size is halved from 174 MB (ONNX fp32) to 87 MB (ncnn fp16).

reddit · r/MachineLearning · /u/ppchaos · Jul 29, 10:22

**Background**: ncnn is a high-performance neural network inference framework optimized for mobile and edge devices. Its Vulkan backend leverages the cross-platform Vulkan API to run on GPUs from any vendor, avoiding the need for proprietary runtimes like CUDA or DirectML.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/upscayl/upscayl-ncnn">GitHub - upscayl/upscayl-ncnn: The Upscayl backend powered by the NCNN framework and Real-ESRGAN architecture. · GitHub</a></li>
<li><a href="https://getpostslate.com/">PostSlate - Next-Generation Video Post-Production Tooling</a></li>

</ul>
</details>

**Tags**: `#ML inference`, `#Vulkan`, `#edge computing`, `#ncnn`, `#GPU`

---

<a id="item-8"></a>
## [Vision Pro Used to Walk Through House Design Before Construction](https://christianselig.com/2026/07/vision-pro-house/) ⭐️ 7.0/10

Developer Christian Selig used an Apple Vision Pro to visualize and walk through a house design before construction, demonstrating a practical application of spatial computing in architecture. This shows how spatial computing can revolutionize architecture and design by allowing clients and architects to experience spaces at full scale before they are built, reducing costly mistakes and improving communication. The article describes using the Vision Pro to walk through a virtual model of a house, with the ability to check proportions and make adjustments in real time. The experience was validated by community members who have used similar VR tools like the HTC Vive and Quest 3 for home design.

hackernews · robbiet480 · Jul 29, 20:39 · [Discussion](https://news.ycombinator.com/item?id=49102774)

**Background**: Spatial computing refers to technology that allows computers to understand and interact with physical space, blending digital content with the real world. Apple Vision Pro is a mixed-reality headset that enables spatial computing experiences. In architecture, VR and AR tools have been used for years to visualize designs, but the Vision Pro's high-resolution passthrough and ease of use make it more accessible.

<details><summary>References</summary>
<ul>
<li><a href="https://uxatc.medium.com/embracing-the-next-frontier-unleashing-the-potential-of-spatial-ux-in-the-era-of-apple-vision-pro-e4744754d940">Embracing the Next Frontier: Unleashing the Potential of Spatial UX in...</a></li>
<li><a href="https://seeyu.hashnode.dev/spatial-computing-in-architecture-and-design">Spatial Computing in Architecture and Design</a></li>
<li><a href="https://www.prefixa.com/">XR Visualization and Spatial Computing Services | Prefixa</a></li>

</ul>
</details>

**Discussion**: Commenters shared their own experiences using VR for architecture, with one noting they used an HTC Vive to design their house ten years ago and another describing a design firm that uses Quest 3 headsets with Enscape for client walkthroughs. The overall sentiment is positive, validating the practical value of spatial computing in design.

**Tags**: `#spatial computing`, `#AR/VR`, `#architecture`, `#Apple Vision Pro`, `#design`

---

<a id="item-9"></a>
## [Kimi K3-256k: Half Cost, Same Quality](https://www.kimi.com/code/docs/en/kimi-code/models) ⭐️ 7.0/10

Kimi has released K3-256k, a variant of its K3 model with a 256k token context window that delivers the same results as the 1M version but consumes half the quota cost. This makes advanced AI more accessible and cost-effective for users who do not need the full 1M context, potentially reducing infrastructure strain and lowering barriers for broader adoption. The K3-256k model is based on the same 2.8-trillion-parameter Mixture-of-Experts architecture as the original K3, but with a reduced context window of 256k tokens, resulting in half the quota consumption.

hackernews · monneyboi · Jul 29, 19:25 · [Discussion](https://news.ycombinator.com/item?id=49101852)

**Background**: Kimi K3 is a 2.8-trillion-parameter MoE model with a 1M-token context window, built on Kimi Delta Attention and Attention Residuals. Many users find that 256k context is sufficient for most tasks, and larger contexts can degrade model performance due to the 'lost in the middle' effect.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K 3 Tech Blog: Open Frontier Intelligence</a></li>
<li><a href="https://vllm.ai/blog/2026-07-27-k3">Kimi K 3 Is Here: Efficient Day-0 Support on vLLM | vLLM Blog</a></li>

</ul>
</details>

**Discussion**: Community members welcomed the new option, noting that 256k context is often sufficient and the cost reduction is significant. Some expressed hope it would ease infrastructure pressure, while others speculated that recent model quality issues might be due to quantization.

**Tags**: `#AI`, `#LLM`, `#cost optimization`, `#context window`

---

<a id="item-10"></a>
## [KOReader: Open-Source E-Reader Enhances E-Ink Devices](https://koreader.rocks/) ⭐️ 7.0/10

KOReader, an open-source document viewer for e-ink devices, continues to gain traction with native EPUB and PDF support, customizable reading options, and cross-device sync capabilities. It is available for jailbroken Kindles, Kobos, and other e-ink devices. KOReader significantly improves the reading experience on e-ink devices by offering features absent in proprietary firmware, such as native format support and advanced customization. Its open-source nature fosters community-driven development and provides a free alternative to vendor-locked ecosystems. KOReader supports multiple file formats including EPUB, PDF, DjVu, and comic book formats, and offers features like reflow, Calibre integration, and reading progress sync. Some users report a non-intuitive UI and occasional lag, but it remains highly popular among enthusiasts.

hackernews · Cider9986 · Jul 29, 11:05 · [Discussion](https://news.ycombinator.com/item?id=49095865)

**Background**: E-ink devices like Amazon Kindle and Kobo typically run proprietary firmware that limits file format support and customization. KOReader is an open-source alternative that can be installed after jailbreaking the device, unlocking features like native EPUB reading and gesture controls. It is developed by volunteers and hosted on GitHub.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/koreader/koreader">GitHub - koreader / koreader : An ebook reader application supporting...</a></li>
<li><a href="https://grokipedia.com/page/KOReader">KOReader</a></li>

</ul>
</details>

**Discussion**: Community comments are mixed: many users praise KOReader for vastly improving their e-reader experience, with some calling it superior to proprietary software. However, others find the UI non-intuitive and gestures unreliable, and some prefer the default viewer after jailbreaking. Overall sentiment is positive, with constructive feedback on usability.

**Tags**: `#open-source`, `#e-reader`, `#software`, `#kindle`, `#kobo`

---

<a id="item-11"></a>
## [AI Companies Hire Thousands of Electricians and Carpenters](https://www.nytimes.com/2026/07/29/business/economy/data-center-electricians-training.html) ⭐️ 7.0/10

AI companies are recruiting thousands of electricians and carpenters to build data centers, with demand for skilled trades rising sharply over the past three years. This trend highlights the growing infrastructure demands of AI, but the boom-and-bust nature of data center construction poses career risks for tradespeople. Randstad reports a 30% increase in demand for construction workers, 25% for welders, and 18% for electricians. By 2030, the U.S. may need 140,000 more electricians, HVAC techs, and welders for AI infrastructure.

hackernews · thm · Jul 29, 14:43 · [Discussion](https://news.ycombinator.com/item?id=49098198)

**Background**: Data centers require extensive electrical and cooling systems, driving demand for trades like electricians and plumbers. The construction boom has seen spending on data centers soar 437% since 2021, but such booms are historically cyclical.

<details><summary>References</summary>
<ul>
<li><a href="https://wolfstreet.com/2026/03/23/construction-of-data-centers-power-plants-factories-and-office-buildings-boom-bust/">Construction of Data Centers, Power Plants, Factories, and Office Buildings: Boom & Bust | Wolf Street</a></li>
<li><a href="https://qazinform.com/news/ai-infrastructure-boom-creates-new-labor-demand-90d45b">AI infrastructure boom creates new labor demand</a></li>
<li><a href="https://www.csis.org/analysis/genais-human-infrastructure-challenge-can-united-states-meet-skilled-trade-labor-demand">GenAI’s Human Infrastructure Challenge—Can the United States Meet Skilled Trade Labor Demand Through 2030? | CSIS</a></li>

</ul>
</details>

**Discussion**: Commenters warn about the boom-and-bust cycle, noting that electricians could earn $300k one year and $30k the next. Others highlight the growing need for plumbers due to liquid cooling trends in data centers.

**Tags**: `#AI`, `#data centers`, `#labor market`, `#trades`, `#infrastructure`

---

<a id="item-12"></a>
## [ICLR 2027 Deadline Conflicts with NeurIPS 2026 Decisions](https://www.reddit.com/r/MachineLearning/comments/1v9v4e7/iclr_2027_deadline_is_before_neurips_2026/) ⭐️ 7.0/10

ICLR 2027 has set its full paper deadline for September 16, 2026, which is eight days before NeurIPS 2026 releases its acceptance decisions. This scheduling conflict may disadvantage papers that could improve after a NeurIPS rejection, forcing researchers to submit to ICLR without knowing their NeurIPS outcome. The ICLR 2027 deadline is September 16, 2026 (Anywhere on Earth), while NeurIPS 2026 decisions are expected around September 24, 2026. The overlap creates a tight window for resubmission.

reddit · r/MachineLearning · /u/1414vo · Jul 29, 12:43

**Background**: ICLR (International Conference on Learning Representations) and NeurIPS (Conference on Neural Information Processing Systems) are two of the top-tier machine learning conferences. Researchers often submit papers to multiple conferences, and the timing of deadlines and decisions can affect their ability to revise and resubmit work.

<details><summary>References</summary>
<ul>
<li><a href="https://iclr.cc/Conferences/2027/Dates">2027 Dates and Deadlines</a></li>
<li><a href="https://neurips.cc/Conferences/2026/Dates">2026 Dates and Deadlines</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion highlights frustration with the scheduling conflict, with one commenter noting that it will hurt papers that have improved since NeurIPS submission or were unfairly rejected. Another comment thread discusses broader issues of reviewer ghosting and suggests penalizing non-responsive reviewers.

**Tags**: `#conference scheduling`, `#machine learning`, `#research community`, `#ICLR`, `#NeurIPS`

---

<a id="item-13"></a>
## [Keychron Announces Open-Source Gaming Mouse Firmware](https://www.digitalfoundry.net/news/2026/07/keychron-announces-first-open-source-firmware-for-gaming-mice) ⭐️ 6.0/10

Keychron announced ZGM, an open-source gaming mouse firmware built on Zephyr RTOS, with a planned release in Q1 2027 for the G6 HE mouse. This could bring the same open-source customization culture from keyboards to gaming mice, but the 6-9 month wait and existing QMK-based mice raise questions about its novelty. The firmware is built on Zephyr RTOS, not QMK, and will initially support only the Keychron G6 HE mouse. The GitHub repository currently contains no source code.

hackernews · JLO64 · Jul 29, 16:36 · [Discussion](https://news.ycombinator.com/item?id=49099715)

**Background**: QMK (Quantum Mechanical Keyboard) is a popular open-source firmware for keyboards, but its support for mice is limited. Zephyr RTOS is a real-time operating system designed for resource-constrained devices, offering modular hardware support. Keychron is known for open-source keyboards and is now extending that philosophy to mice.

<details><summary>References</summary>
<ul>
<li><a href="https://zgm.gg/">ZGM Firmware — Zephyr Gaming Mouse</a></li>
<li><a href="https://www.pcgamer.com/hardware/gaming-mice/keychrons-gaming-mouse-firmware-is-going-open-source-while-the-company-critiques-firmware-you-cant-read-cant-audit-cant-change/">Keychron's gaming mouse firmware is going open - source , while the...</a></li>
<li><a href="https://www.digitalfoundry.net/news/2026/07/keychron-announces-first-open-source-firmware-for-gaming-mice">Keychron announces first open - source firmware for gaming mice</a></li>

</ul>
</details>

**Discussion**: Community comments express skepticism: some note that QMK-based mice like Ploopy already exist, questioning ZGM's added value. Others criticize the early announcement with no source code, calling it vaporware. A few are hopeful but concerned about limited form factors.

**Tags**: `#open-source`, `#firmware`, `#gaming mice`, `#keychron`, `#qmk`

---

<a id="item-14"></a>
## [Guide: Adding Custom MCP Servers to Claude and ChatGPT](https://simonwillison.net/2026/Jul/29/mcp-in-claude-and-chatgpt/#atom-everything) ⭐️ 6.0/10

Simon Willison published a tutorial explaining how to connect custom MCP (Model Context Protocol) servers to the standard chat interfaces of Claude and ChatGPT. This enables developers to extend the capabilities of popular AI chatbots by integrating custom tools and data sources, fostering more flexible and powerful AI applications. The process involves multiple steps, including setting up an MCP server and configuring the chat interface to communicate with it. The tutorial is based on Simon Willison's TIL (Today I Learned) page.

rss · Simon Willison · Jul 29, 00:13

**Background**: The Model Context Protocol (MCP) is an open standard introduced by Anthropic in November 2024 to standardize how AI systems like LLMs integrate with external tools and data sources. It provides a unified interface for reading files, executing functions, and handling contextual prompts. Major AI providers including OpenAI and Google DeepMind have adopted MCP.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol</a></li>
<li><a href="https://modelcontextprotocol.io/">What is the Model Context Protocol (MCP)? - Model Context Protocol</a></li>
<li><a href="https://github.com/modelcontextprotocol/servers">GitHub - modelcontextprotocol/ servers : Model Context Protocol Servers</a></li>

</ul>
</details>

**Tags**: `#MCP`, `#Claude`, `#ChatGPT`, `#AI`, `#tutorial`

---

<a id="item-15"></a>
## [TanML: Open-Source Toolkit for Tabular Model Validation](https://www.reddit.com/r/MachineLearning/comments/1va7w4p/opensource_tabular_model_validation_toolkit_tanml/) ⭐️ 6.0/10

The developers of TanML have released an MIT-licensed automated validation toolkit for tabular machine learning models, which runs locally and provides an end-to-end workflow including data profiling, preprocessing, feature ranking, model development, evaluation, drift analysis, stress testing, SHAP explainability, and audit-ready Word reports. This toolkit addresses the growing need for automated model validation in regulated industries like banking and insurance, where compliance with model risk management guidelines is critical. By offering a free, open-source solution, TanML could lower the barrier for smaller firms to adopt rigorous validation practices. TanML is built with a zero-config Streamlit UI and exports audit-ready, editable Word reports (.docx). It covers data quality checks, correlation/VIF analysis, performance metrics, drift detection, and SHAP-based explainability.

reddit · r/MachineLearning · /u/AccomplishedLeg1508 · Jul 29, 20:22

**Background**: Model validation is a critical step in machine learning workflows, especially in regulated industries where models must be documented and tested for robustness, fairness, and stability. SHAP (SHapley Additive exPlanations) is a popular method for explaining model predictions by attributing each feature's contribution. Model risk management (MRM) frameworks, such as those from the FDIC and OCC, require banks to validate models used for credit risk, stress testing, and other purposes.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/tdlabs-ai/tanml">GitHub - tdlabs-ai/ tanml : Automated validation toolkit for tabular ML ...</a></li>
<li><a href="https://shap.readthedocs.io/en/latest/example_notebooks/overviews/An+introduction+to+explainable+AI+with+Shapley+values.html">An introduction to explainable AI with Shapley values — SHAP latest documentation</a></li>
<li><a href="https://www.ibm.com/think/topics/model-risk-management">What Is Model Risk Management? | IBM</a></li>

</ul>
</details>

**Tags**: `#tabular data`, `#model validation`, `#open source`, `#MLOps`, `#regulated industries`

---

<a id="item-16"></a>
## [SQLite creator compares SQL to COBOL evolution](https://simonwillison.net/2026/Jul/29/d-richard-hipp/#atom-everything) ⭐️ 5.0/10

D. Richard Hipp, creator of SQLite, drew a parallel between COBOL programmers and SQL, arguing that new tools like SQL change jobs rather than eliminate them. This insight from a respected figure in database technology offers a reassuring perspective on automation and job displacement in the software industry, emphasizing that programming roles evolve with new abstractions. Hipp noted that before SQL, querying large datasets required expensive COBOL programmers; SQL simplified the task but did not eliminate programming jobs—it changed them.

rss · Simon Willison · Jul 29, 21:15

**Background**: COBOL is a business-oriented programming language from the 1960s, still used in legacy systems. SQL (Structured Query Language) is a declarative language for managing relational databases, introduced in the 1970s. D. Richard Hipp is best known for creating SQLite, the most widely deployed database engine.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/D._Richard_Hipp">D. Richard Hipp</a></li>
<li><a href="https://en.wikipedia.org/wiki/COBOL">COBOL - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#sql`, `#careers`, `#programming-history`, `#d-richard-hipp`

---

<a id="item-17"></a>
## [Workshop Paper Accepted, Reviewers Request New Experiments](https://www.reddit.com/r/MachineLearning/comments/1v9owaf/workshop_paper_accepted_reviewers_asked_new/) ⭐️ 4.0/10

A researcher's workshop paper was accepted at a top conference, but reviewers requested additional experiments after acceptance, with no second review phase before the camera-ready deadline. This situation highlights a gap in the workshop review process where post-acceptance requests can bypass standard peer review, potentially affecting the integrity of the publication. The camera-ready version is the final, non-negotiable manuscript submitted for publication, and workshops typically do not have a second review phase after initial acceptance.

reddit · r/MachineLearning · /u/rokk07 · Jul 29, 07:21

**Background**: In academic publishing, a camera-ready paper is the final version that is published exactly as submitted, without further editing. Workshops at top conferences often have a single review cycle; after acceptance, authors submit the camera-ready version directly. Reviewer requests for additional experiments after acceptance are unusual because there is no mechanism for re-review.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aischolar.com/news/article/what-is-a-camera-ready-paper">What is a Camera-Ready Paper?</a></li>
<li><a href="https://www.iconf.org/news/801">What is a Camera-Ready Paper? Definition & Submission Checklist (IEEE/ACM)--iConf</a></li>

</ul>
</details>

**Discussion**: The Reddit community advised the author to contact the workshop chairs for clarification, as ignoring the request might risk publication, while running experiments could be unnecessary if not required for acceptance.

**Tags**: `#machine learning`, `#academic publishing`, `#workshop paper`, `#peer review`

---

<a id="item-18"></a>
## [NeurIPS E&D: How to respond to ethical reviews?](https://www.reddit.com/r/MachineLearning/comments/1v9hth4/neurips_ed_should_authors_respond_to_ethical/) ⭐️ 4.0/10

An author submitted to the NeurIPS E&D track and received ethical review comments alongside official reviews, asking whether and how to respond during the discussion period before August 3. This question highlights the growing importance of ethics review in top ML conferences and the need for clear author guidelines on responding to ethical concerns. According to NeurIPS 2025 ethics reviewer call, ethics reviews are anonymized when made visible to authors during the author response period, and authors can respond via the official comment feature.

reddit · r/MachineLearning · /u/Empty_Astronomer8376 · Jul 29, 01:32

**Background**: NeurIPS introduced an ethics review process to ensure submissions adhere to the NeurIPS Code of Ethics. The E&D (Ethics & Datasets) track specifically focuses on ethical considerations and dataset contributions. Authors are expected to engage with ethical reviews similarly to technical reviews.

<details><summary>References</summary>
<ul>
<li><a href="https://neurips.cc/Conferences/2025/CallForEthicsReviewers">NeurIPS 2025 Call for Ethics Reviewers</a></li>
<li><a href="https://blog.neurips.cc/2026/05/12/neurips-2026-call-for-ethics-reviewers/">NeurIPS 2026 Call for Ethics Reviewers – NeurIPS Blog</a></li>

</ul>
</details>

**Tags**: `#NeurIPS`, `#conference`, `#ethics`, `#review process`

---

<a id="item-19"></a>
## [Claude Experiences Elevated Errors Across All Models](https://status.claude.com/incidents/q2kg8n613kr3) ⭐️ 3.0/10

Claude experienced elevated errors across all models, causing a temporary outage that disrupted service for users. This outage highlights the reliability challenges faced by AI assistants as they become more integrated into daily workflows, affecting productivity and trust. The incident lasted several hours, with users reporting failed agent runs and API errors (e.g., HTTP 529). No root cause or resolution details were provided in the status update.

hackernews · gregsadetsky · Jul 29, 19:50 · [Discussion](https://news.ycombinator.com/item?id=49102150)

**Background**: Claude is a series of large language models developed by Anthropic, designed to be safe and helpful AI assistants. Service outages, while not uncommon for cloud-based AI services, can significantly impact users who rely on Claude for coding, writing, and other tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_(AI)">Claude ( AI ) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community comments were humorous, with users joking about forgetting how to code and rediscovering old tools like vim. Some shared technical details of the outage, such as agents failing with API errors.

**Tags**: `#outage`, `#Claude`, `#status`

---

<a id="item-20"></a>
## [Survey Recruits Users of AI Companions for Research](https://www.reddit.com/r/MachineLearning/comments/1v9maa7/exploring_humanai_relationships_honours_thesis_r/) ⭐️ 3.0/10

Julia Bain and two other honours researchers at the University of the Sunshine Coast are recruiting participants aged 18+ who have used AI for friendship or romantic purposes within the last 6 months for an anonymous survey on human-AI relationships. This research contributes to the growing field of human-AI interaction, particularly the study of artificial intimacy, which has significant implications for understanding how AI companions affect human social and emotional well-being. The survey takes about 25-30 minutes, is anonymous, and has received ethics approval (S262259) from the UniSC Human Research Ethics Committee. Participants can access the survey via Qualtrics and find more details in the project information sheet.

reddit · r/MachineLearning · /u/Ok-Suggestion2488 · Jul 29, 05:02

**Background**: AI companions are devices or applications designed to simulate companionship through social, emotional, or relational interaction, such as chatbots like Replika. Artificial intimacy refers to forming social connections or intimate relationships with AI entities, a phenomenon that has grown with advances in large language models and affective computing.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_companion">AI companion</a></li>
<li><a href="https://en.wikipedia.org/wiki/Artificial_intimacy">Artificial intimacy - Wikipedia</a></li>
<li><a href="https://www.qualtrics.com/free-account/">Free Online Survey Maker Tool - Qualtrics</a></li>

</ul>
</details>

**Tags**: `#human-AI interaction`, `#survey`, `#AI companions`

---