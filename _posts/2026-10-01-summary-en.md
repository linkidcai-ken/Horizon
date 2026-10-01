---
layout: default
title: "Horizon Summary: 2026-10-01 (EN)"
date: 2026-10-01
lang: en
---

> From 23 items, 20 important content pieces were selected

---

1. [Google Announces Gemini 4 Argon Frontier AI Model](#item-1) ⭐️ 9.0/10
2. [EDG open-sources its widely-used C++ front-end](#item-2) ⭐️ 8.0/10
3. [Team publicly reverses its anti-MCP stance, sparking debate](#item-3) ⭐️ 8.0/10
4. [32 Researchers Release Comprehensive Tokenization Survey for Modern NLP](#item-4) ⭐️ 8.0/10
5. [CO₂Jump: Training-Free Sampler Couples Image Understanding and Generation](#item-5) ⭐️ 8.0/10
6. [Declassified: The Top Secret URSALA, RAQUEL, and FARRAH Spy Satellites](#item-6) ⭐️ 7.0/10
7. [Singapore's Government Dating App Uses Gale-Shapley Stable Marriage Algorithm](#item-7) ⭐️ 7.0/10
8. [Magnitude launches self-optimizing inference engine for local agents](#item-8) ⭐️ 7.0/10
9. [Netlify swaps V8 isolates for Firecracker MicroVMs, claims 5x faster Edge Functions](#item-9) ⭐️ 7.0/10
10. [IEEE Spectrum Explores the Enduring Bloomberg Terminal](#item-10) ⭐️ 7.0/10
11. [Qwen-family LLMs dominate as backbone of 100+ audio models](#item-11) ⭐️ 7.0/10
12. [LessThink-Qwen3-4B cuts reasoning tokens by 44% on one GPU](#item-12) ⭐️ 7.0/10
13. [ORTUS AI open-sources RightWayUp 360° image rotation model, exposes JPEG benchmark shortcut](#item-13) ⭐️ 7.0/10
14. [Quanta Explores Spiral and Concentric Brain Waves During Memory Tasks](#item-14) ⭐️ 6.0/10
15. [Reddit Post Warns Workshop Papers Carry Little Weight in ML](#item-15) ⭐️ 6.0/10
16. [Multi-scan radar object classification boosts macro F1 on RadarScenes](#item-16) ⭐️ 6.0/10
17. [Reddit asks: what API should power general real-time LLM agents?](#item-17) ⭐️ 6.0/10
18. [Hypothetical OpenAI Lean 4 Navier-Stokes proof sparks specification gaming debate](#item-18) ⭐️ 6.0/10
19. [Isolation Forest performs best with max_samples set to 1.0 on CICIDS2017](#item-19) ⭐️ 5.0/10
20. [Author asks how to follow up on TMLR submission after reviewers go silent](#item-20) ⭐️ 4.0/10

---

<a id="item-1"></a>
## [Google Announces Gemini 4 Argon Frontier AI Model](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-argon/) ⭐️ 9.0/10

Google announced Gemini 4 Argon, a new frontier AI model positioned above the Gemini 3.8 line, targeting software engineering, enterprise knowledge work, and cyber defense. The model is rolling out soon, with early testers providing feedback as Google iterates on guardrails before making it available to developers, enterprises, and consumers. Gemini 4 Argon represents Google's latest bid to lead the frontier AI race, with major improvements in coding, cybersecurity, and complex professional work. Its release intensifies competition among frontier labs and hyperscalers, and the community sees it as evidence that AI leadership is becoming more distributed rather than winner-takes-all. According to early analyses, Gemini 4 Argon leads the Vals Index and DeepSWE v1.1 benchmarks, raises the output limit to 1 million tokens, and launches at $2/$10 per million tokens. Google describes it as built to sustain deep reasoning across complex, long-horizon workflows, and its agents are reportedly working on migrating C/C++ codebases to Rust across Google.

hackernews · bradleyg223 · Sep 30, 20:04 · [Discussion](https://news.ycombinator.com/item?id=49913571)

**Background**: A frontier model is the most advanced class of AI system available at a given time, typically a large language model trained on massive datasets at costs reaching hundreds of millions of dollars. Google's Gemini family is one of the leading commercial model lines, and each new release is closely watched for benchmark performance, pricing, and real-world coding ability.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-argon/">Introducing Gemini 4 Argon - The Keyword</a></li>
<li><a href="https://www.datacamp.com/blog/gemini-4-argon">Gemini 4 Argon: Benchmarks, Pricing, and Access | DataCamp</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/frontier-models/">What Are Frontier AI Models and How They Work - NVIDIA</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters were highly engaged, with one user describing how an earlier Gemini model reverse-engineered a GPU driver and wrote an LD_PRELOAD shim to get ROCm working on a Strix Halo. Others debated Dario Amodei's winner-takes-all thesis, argued that model and provider should be replaceable, and joked that Google still hasn't beaten the 'can't release a model' allegations.

**Tags**: `#AI`, `#Gemini`, `#Google`, `#LLM`, `#Model Release`

---

<a id="item-2"></a>
## [EDG open-sources its widely-used C++ front-end](https://edgcpp.org/#transition) ⭐️ 8.0/10

EDG (Edison Design Group) has open-sourced its C++ front-end, with the source going public on September 30, 2026, and The C++ Alliance becoming its nonprofit home. The announcement site has been criticized as low-quality AI-generated content. EDG's front-end is a respected, widely-used compiler component that powers tools like Visual C++ IntelliSense, Intel C++ Compiler, and NVIDIA CUDA NVCC, so its open-sourcing is a significant event for the C++ ecosystem. It could enable new uses such as transpiling C++ libraries to other languages and provide a professionally maintained, open alternative for compiler and tooling developers. The front-end has a long history, with earliest commits dating back to 1990, which is unusual for open-source transitions. The announcement notes that EDG the company is winding down, which is likely the reason for open-sourcing the front-end.

hackernews · iandinwoodie · Sep 30, 19:26 · [Discussion](https://news.ycombinator.com/item?id=49913192)

**Background**: A compiler front-end handles preprocessing and parsing of source code, producing an intermediate representation that back-ends turn into machine code. EDG is an American company that makes compiler front-ends for C++ (and formerly Java and Fortran), and its front-ends are widely used in commercial compilers and code analysis tools. The C++ Alliance is a nonprofit organization that supports C++ libraries and tools, and it will now maintain the EDG front-end.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Edison_Design_Group">Edison Design Group - Wikipedia</a></li>
<li><a href="https://edgcpp.org/">Open Source Transition · EDGCPP</a></li>
<li><a href="https://www.phoronix.com/news/EDG-CPP-Open-Sourced">EDG C/ C++ Front - End Open-Sourced - Phoronix</a></li>

</ul>
</details>

**Discussion**: Commenters criticized the announcement site as AI-generated 'slop' that barely makes sense, while others highlighted the significance of the open-sourcing and speculated about uses like transpiling C++ libraries to Free Pascal. One commenter noted that EDG the company is winding down, which likely explains the move, and another pointed out the unusually long commit history dating back to 1990.

**Tags**: `#C++`, `#compilers`, `#open-source`, `#EDG`, `#programming-languages`

---

<a id="item-3"></a>
## [Team publicly reverses its anti-MCP stance, sparking debate](https://earendil.com/posts/you-said-no-mcp/) ⭐️ 8.0/10

A team that had previously taken a strong public stance against the Model Context Protocol (MCP) has now publicly reversed its position, documenting the change of mind in a blog post. The reversal drew a large Hacker News discussion (610 points, 340 comments) covering MCP's practical uses, security, and industry adoption. The reversal signals that MCP is gaining acceptance even among skeptics, which matters for developers and companies deciding how to connect AI applications to external tools and data. It also highlights a broader industry trend where practical compatibility often outweighs theoretical objections to a standard. MCP was introduced by Anthropic in November 2024 as an open standard for connecting LLM applications to external data sources and tools, often described as a "USB-C port for AI." Security concerns remain a key caveat, with the NSA and OWASP both publishing guidance on MCP security risks and best practices for production deployments.

hackernews · yarapavan · Sep 30, 09:55 · [Discussion](https://news.ycombinator.com/item?id=49906637)

**Background**: The Model Context Protocol (MCP) is an open standard and open-source framework introduced by Anthropic in November 2024 to standardize how AI systems like large language models integrate and share data with external tools, systems, and data sources. Before MCP, developers often built fragmented, custom integrations for each AI application, which was fragile and time-consuming. MCP aims to replace those one-off integrations with a single, universal protocol, similar to how USB-C standardizes physical connections.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>
<li><a href="https://modelcontextprotocol.io/docs/2026-07-28/getting-started/intro">What is the Model Context Protocol (MCP)?</a></li>
<li><a href="https://cheatsheetseries.owasp.org/cheatsheets/MCP_Security_Cheat_Sheet.html">MCP Security - OWASP Cheat Sheet Series</a></li>

</ul>
</details>

**Discussion**: Commenters largely praised the team for publicly admitting a reversal rather than hiding it, with one quoting Armin Ronacher on how strong opinions often rest on outdated arguments. Others noted MCP's value beyond coding, such as configuring macOS apps via natural language, while some argued that despite its flaws MCP is "better than nothing" and will improve over time, much like USB-C or HDMI.

**Tags**: `#MCP`, `#AI`, `#developer-tools`, `#Hacker News`, `#industry-trends`

---

<a id="item-4"></a>
## [32 Researchers Release Comprehensive Tokenization Survey for Modern NLP](https://www.reddit.com/r/MachineLearning/comments/1wuccjf/tokenization_a_survey_for_modern_nlp_r/) ⭐️ 8.0/10

A team of 32 tokenizer researchers has released the most comprehensive survey of tokenization in modern NLP to date, covering algorithms, evaluations, multilinguality, encodings, and theory. The survey also addresses adjacent topics such as constrained generation, token healing, tokenizer security, and potential replacements like latent or visual tokenization. Tokenization is a foundational yet understudied component of language modeling that affects all of NLP, so this broad, deep resource is highly valuable for both researchers and practitioners. It consolidates fragmented knowledge and could guide future research and practical improvements in model performance, especially for multilingual and multimodal applications. The survey was compiled over roughly eight months by 32 researchers and spans every aspect of tokenization, including algorithms, evaluations, multilinguality, encodings, and theory. It also explores alternatives to tokenizers such as latent and visual tokenization, and covers security concerns and token healing.

reddit · r/MachineLearning · /u/mcmcmcmcmcmcmcmcmc_ · Sep 30, 18:13

**Background**: Tokenization is the process of splitting text into smaller units (tokens) that machine learning models can process, and it is a critical first step in most NLP pipelines. Despite its importance, tokenization has often been treated as an afterthought compared to model architecture, leading to calls for more systematic study. Latent tokenization uses non-interpretable dummy tokens to steer model decoding, while visual tokenization converts image or video pixels into token sequences for multimodal models.

<details><summary>References</summary>
<ul>
<li><a href="https://www.geeksforgeeks.org/nlp/tokenization-in-natural-language-processing-nlp/">What is Tokenization in Natural Language Processing ( NLP )?</a></li>
<li><a href="https://www.emergentmind.com/topics/latent-tokens">Latent Tokens in Generative Models - emergentmind.com</a></li>
<li><a href="https://portpowered.github.io/ai-model-reference/docs/concepts/visual-tokenization">Visual tokenization</a></li>

</ul>
</details>

**Tags**: `#tokenization`, `#NLP`, `#survey`, `#language modeling`, `#machine learning`

---

<a id="item-5"></a>
## [CO₂Jump: Training-Free Sampler Couples Image Understanding and Generation](https://www.reddit.com/r/MachineLearning/comments/1wtyl5m/concurrent_image_understanding_and_generation/) ⭐️ 8.0/10

A NeurIPS 2026 paper from Google, Google DeepMind, and Stony Brook University introduces CO₂Jump, a training-free sampler that uses text confidence and cross-modal attention to guide image updates during joint text-image generation. It allows low-confidence tokens to be masked and regenerated, enabling self-correction, and introduces three datasets: JEdit-1M, JMaze-200K, and JNono-200K. This addresses a real consistency mismatch in multimodal models where a model can describe a correct solution but draw a different one, which is critical for applications like image editing and puzzle solving. The training-free nature means it can be applied to existing fine-tuned models without additional training, potentially improving joint accuracy across many tasks. CO₂Jump uses one model forward pass per denoising step and was the only sampler compared that improved monotonically on both editing quality and grounding across 8–512 sampling steps. Evaluation covers image editing, maze solving, and nonograms, where joint accuracy requires both the textual answer and generated image to be correct.

reddit · r/MachineLearning · /u/Upstairs_Theme2785 · Sep 30, 07:28

**Background**: Diffusion models generate images by iteratively denoising random noise, and recent multimodal systems can generate text and images jointly. However, these outputs can be inconsistent—for example, a model might describe the correct path through a maze while drawing a different one. CO₂Jump is based on Markov jump processes, a type of stochastic process with discrete jumps, and uses cross-modal attention to let text and image generation inform each other during sampling.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Jump_process">Jump process - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Crossmodal_attention">Crossmodal attention</a></li>
<li><a href="https://arxiv.org/abs/2310.03337">[2310.03337] Denoising Diffusion Step-aware Models - arXiv.org Denoising Diffusion Step-aware Models - arXiv.org Denoising Diffusion Step-aware Models - proceedings.iclr.cc Denoising Diffusion Step-aware Models - OpenReview InDepth Guide to Denoising Diffusion Probabilistic Models DDPM Denoising Diffusion Probabilistic Models - GeeksforGeeks GitHub - EnVision-Research/DDSM: Denoising Diffusion Step ...</a></li>

</ul>
</details>

**Tags**: `#multimodal generation`, `#diffusion models`, `#NeurIPS 2026`, `#image understanding`, `#sampling methods`

---

<a id="item-6"></a>
## [Declassified: The Top Secret URSALA, RAQUEL, and FARRAH Spy Satellites](https://www.thespacereview.com/article/4951/1) ⭐️ 7.0/10

The Space Review published an in-depth article detailing the once top-secret URSALA, RAQUEL, and FARRAH signals-intelligence satellites, which operated from the 1970s into the 21st century. The piece traces a covert 'hitchhiker' program that began in 1963 and lasted more than 40 years under various names and designations. The article reveals that the United States fielded signals-intelligence satellites decades ahead of any competitor, a capability that shaped Cold War espionage and modern space-based surveillance. It also highlights the enduring secrecy of national reconnaissance programs, with many details still classified and slated for release only decades from now. The satellites were roughly the size of a large suitcase, festooned with antennas, and spun rapidly in orbit to sweep their antennas over the ground while gathering radar and other signals. The later FARRAH satellites weighed more than 1,360 kilograms, compared with 340 kilograms for FARRAH I and II, and both FARRAH I and II suffered development delays due to high packing density.

hackernews · Bluestein · Sep 30, 22:03 · [Discussion](https://news.ycombinator.com/item?id=49915082)

**Background**: These satellites were part of the National Reconnaissance Office's signals-intelligence (SIGINT) efforts, designed to intercept radar and communications from orbit. The 'hitchhiker' concept involved attaching small secondary payloads to the side of larger primary satellites, allowing covert launches under the cover of civilian or other missions. The program's existence only became public through declassified documents and historical research, and a half-scale model of FARRAH now hangs in the Smithsonian's National Air and Space Museum.

<details><summary>References</summary>
<ul>
<li><a href="https://space.skyrocket.de/doc_sdat/farrah.htm">Farrah 1, 2 (P-11 4433, 4434) - Gunter's Space Page</a></li>
<li><a href="https://thespacereview.com/article/5268/1">The Space Review: Superstar in the Smithsonian: the FARRAH satellite</a></li>

</ul>
</details>

**Discussion**: Commenters marveled at how the US deployed Hubble-class telescopes for spying decades before NASA could use similar technology for astronomy, and one noted the NRO gifted decommissioned satellites to NASA in 2012. Others expressed curiosity about what classified satellite information will be released in 2066, shared related stories about a Cold War spy satellite named after Farrah Fawcett, and joked about modern surveillance concerns like Facebook's 'Spyglasses.'

**Tags**: `#spy satellites`, `#space technology`, `#cold war`, `#surveillance`, `#national reconnaissance office`

---

<a id="item-7"></a>
## [Singapore's Government Dating App Uses Gale-Shapley Stable Marriage Algorithm](https://twitter.com/tuakdotsol/status/2105105417760391258) ⭐️ 7.0/10

Singapore has launched a government-built dating app pilot called FirstDate for public servants, which uses the Gale-Shapley stable marriage algorithm to match users. The app verifies identities through Singpass and targets single public officers, sparking debate on Hacker News about whether algorithmic matching can address declining marriage and birth rates. This is a notable real-world application of a classic game-theory algorithm to a high-stakes social problem, as Singapore attempts to reverse its falling birth rate and aging population. It raises important questions about whether dating market failures are matching problems or clearing problems, and whether government intervention in matchmaking is appropriate. The Gale-Shapley algorithm guarantees a stable matching where no two participants would prefer each other over their assigned partners, but it produces either a male-optimal or female-optimal outcome depending on which side proposes. The pilot specifically targets government workers aged 21 to 35, which critics note overlaps with the age threshold for advanced maternal age and public housing eligibility for singles.

hackernews · rzk · Sep 30, 09:27 · [Discussion](https://news.ycombinator.com/item?id=49906432)

**Background**: The Gale-Shapley algorithm, also known as the deferred acceptance algorithm, was developed in 1962 by David Gale and Lloyd Shapley to solve the stable matching problem, and Lloyd Shapley later won the Nobel Prize in Economics for this work. It is widely used in real-world matching systems such as medical residency placements and school admissions. Singapore has one of the world's lowest fertility rates and fastest-aging populations, prompting various government efforts to encourage marriage and childbearing.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gale–Shapley_algorithm">Gale–Shapley algorithm - Wikipedia</a></li>
<li><a href="https://www.ft.com/content/a2140178-c1b8-4679-8d89-1f34772c0702?syn-25a6b1a6=1">Singapore taps Nobel-winning formula for government dating app</a></li>
<li><a href="https://mustsharenews.com/government-dating-app/">'We got S'pore government dating app before GTA 6': Netizens in.....</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters were largely skeptical, with one arguing that dating market problems are clearing problems rather than matching problems and cannot be solved by clever algorithms. Others questioned whether people know their own preferences or whether preferences remain stable over time, and some drew parallels to Singapore's historical eugenics policies given the pilot's targeting of young government workers.

**Tags**: `#algorithms`, `#dating-apps`, `#public-policy`, `#game-theory`, `#social-computing`

---

<a id="item-8"></a>
## [Magnitude launches self-optimizing inference engine for local agents](https://github.com/magnitudedev/magnitude) ⭐️ 7.0/10

Magnitude, a YC S25 startup founded by Anders and Tom, launched an open-source (Apache 2.0) inference engine written in Rust that self-tunes kernels on the user's device and claims up to 2x faster decode than llama.cpp. Benchmarks on Qwen 3.6 35B A3B (4-bit, 64k context) show 92% faster decode on Mac M4 Pro (30 to 57 tok/s) and 19% faster decode on DGX Spark (49 to 58 tok/s), with 27-28% less per-agent memory usage. Most existing inference engines are optimized either for datacenter batched serving (vLLM, SGLang) or for broad compatibility (llama.cpp, Ollama), leaving a gap for local agent workloads that involve long, concurrent sessions. If Magnitude's on-device autotuning claims hold up, it could make running capable local models alongside other desktop work more practical for developers. Magnitude uses on-device kernel compilation and tuning, dynamic memory allocation that only reserves space for model weights up front, and hybrid paged attention that shares prefix caches across concurrent sessions while preserving single-session performance. It ships as a desktop app that connects to existing agents like Pi, OpenCode, Hermes, and Codex, and future plans include expert streaming, a custom kernel compiler, and multi-device utilization.

hackernews · anerli · Sep 30, 17:37 · [Discussion](https://news.ycombinator.com/item?id=49911995)

**Background**: Inference engines are the software that actually runs large language models, handling how weights are loaded, how attention is computed, and how memory is managed. llama.cpp, created by Georgi Gerganov in March 2023, popularized running quantized models on consumer hardware via the GGUF format, while vLLM and SGLang target high-throughput batched serving on datacenter GPUs. Autotuning, as used by Magnitude, means searching over kernel configurations on the actual target device to find the fastest settings rather than shipping one fixed implementation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.local-llm.net/tools/llama-cpp/">llama . cpp — Inference Engine | local-llm.net</a></li>
<li><a href="https://particula.tech/blog/sglang-vs-vllm-inference-engine-comparison">SGLang vs vLLM in 2026: Benchmarks and When to Use Each</a></li>
<li><a href="https://ar5iv.labs.arxiv.org/html/2008.03602">[2008.03602] Spatial Sharing of GPU for Autotuning DNN models</a></li>

</ul>
</details>

**Discussion**: Commenters were largely impressed by the autotuner's kernel-level search and caching, but questioned the accuracy of the UI's speed estimates, with one user noting Qwen 3.8 Q8 numbers looked about 2x slower than their real mtplx sessions. Others argued that beating llama.cpp is a low bar on Mac, since engines like ds4, omlx, and mtplx are often faster, and raised concerns that fit scores appear to be predictions from constants measured on a single M4 Max rather than per-device measurements.

**Tags**: `#inference-engine`, `#local-llm`, `#performance-optimization`, `#agents`, `#llama.cpp`

---

<a id="item-9"></a>
## [Netlify swaps V8 isolates for Firecracker MicroVMs, claims 5x faster Edge Functions](https://www.netlify.com/blog/edge-functions-firecracker-microvms/) ⭐️ 7.0/10

Netlify published a technical deep-dive explaining that it migrated its Edge Functions from V8 isolates to Firecracker MicroVMs running inside its own edge network, reporting roughly 5x faster median performance. Previously, requests were dispatched to a hosted execution service; now they execute on MicroVMs within Netlify's own infrastructure. This is a notable case study in the serverless/edge runtime trade-off between V8 isolates (fast cold starts, weaker isolation) and microVMs (stronger hardware-level isolation, historically slower to boot), and it affects how developers think about latency, security, and multi-tenancy on edge platforms. It also highlights Unikraft's role in optimizing the microVM boot path, which could influence how other edge providers design their runtimes. The reported 5x speedup is a median figure, and community members noted that the comparison may conflate the runtime change with the removal of a network hop to a hosted execution service, so the true source of the gain is disputed. Netlify's Edge Functions run JavaScript/TypeScript and are free on all plans, and the microVM portion of the story involves Unikraft's unikernel-based optimization work.

hackernews · jbott · Sep 30, 18:17 · [Discussion](https://news.ycombinator.com/item?id=49912444)

**Background**: V8 isolates are lightweight JavaScript execution contexts used by platforms like Cloudflare Workers and Vercel Edge Functions; they start almost instantly but share a process and rely on software-level isolation. Firecracker MicroVMs, originally open-sourced by AWS, are lightweight virtual machines that combine hardware virtualization's security and isolation with container-like speed and resource efficiency, making them popular for multi-tenant serverless platforms. Netlify Edge Functions let developers run JavaScript and TypeScript code at the network edge to modify requests, localize content, authenticate users, and run A/B tests with low latency.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/firecracker-microvm/firecracker">GitHub - firecracker-microvm/firecracker: Secure and fast ...</a></li>
<li><a href="https://firecracker-microvm.github.io/">GitHub Pages - Firecracker</a></li>
<li><a href="https://www.netlify.com/blog/edge-functions-explained.md">netlify .com/blog/ edge - functions -explained.md</a></li>

</ul>
</details>

**Discussion**: Commenters were divided: a Unikraft engineer (nderjung) offered to answer questions and linked technical write-ups, while others were skeptical of the 5x claim. nchmy noted Cloudflare Workers are also V8 isolates yet run far faster than the 25-40ms Netlify reported, and yencabulator argued the comparison is misleading because Netlify may have simply eliminated a network hop rather than making execution itself faster. Others praised Firecracker as one of the best microVM technologies, with one user recommending SlicerVM for local edge-style workloads.

**Tags**: `#edge-computing`, `#firecracker`, `#microvms`, `#v8-isolates`, `#serverless`

---

<a id="item-10"></a>
## [IEEE Spectrum Explores the Enduring Bloomberg Terminal](https://spectrum.ieee.org/bloomberg-terminal) ⭐️ 7.0/10

IEEE Spectrum published a historical deep-dive on the Bloomberg Terminal, examining its design, longevity, and impact on financial technology. The piece, which scored 7.0/10 and drew 221 points and 87 comments on Hacker News, sparked community discussion about the terminal's Chromium-based architecture and extreme backwards compatibility. The Bloomberg Terminal remains one of the most influential and durable pieces of financial technology, with roughly 325,000 subscribers worldwide as of 2022 and an annual cost of about $24,000 per user. Its design choices—dense information displays, proprietary networking, and decades of backwards compatibility—offer lessons for anyone building long-lived professional software. The modern Terminal is built on a private fork of Chromium that mimics the look and feel of a VT100 terminal while integrating Bloomberg's private networking and security technologies. Bloomberg maintains such extreme backwards compatibility that a second-generation Terminal from around 1985 can still display current news in its museum.

hackernews · rbanffy · Sep 30, 14:34 · [Discussion](https://news.ycombinator.com/item?id=49909583)

**Background**: The Bloomberg Terminal is a proprietary software platform from Bloomberg L.P. that lets financial professionals monitor and analyze real-time market data, read news, send messages, and place trades. First released in December 1982, it predates HTTP and is leased in two-year cycles, typically with two to six displays per setup. Its black interface and custom keyboard have become recognizable hallmarks of the service.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bloomberg_Terminal">Bloomberg Terminal</a></li>
<li><a href="https://uxmag.com/articles/the-impossible-bloomberg-makeover">As a matter of pride, some users prefer a UI to be obtuse an ugly.</a></li>

</ul>
</details>

**Discussion**: Commenters praised the terminal's terse, information-dense displays, comparing them to modern avionics cockpits that layer only the information needed at a given moment. Others highlighted its private Chromium fork, its museum-worthy backwards compatibility, and shared links to the history of the competing Reuters terminal and a talk on Bloomberg's home-grown server-side scripting.

**Tags**: `#bloomberg-terminal`, `#financial-technology`, `#history`, `#user-interface`, `#backwards-compatibility`

---

<a id="item-11"></a>
## [Qwen-family LLMs dominate as backbone of 100+ audio models](https://www.reddit.com/r/MachineLearning/comments/1wuctrt/qwenfamily_llms_are_quietly_becoming_the_backbone/) ⭐️ 7.0/10

A data-driven analysis of the audio.cpp model collection found that 32 audio model families use a Qwen-family architecture, with 20 specifically built on Qwen3 as the language backbone. These Qwen-based models now span text-to-speech, ASR/audio understanding, music generation, speech-to-speech, and even audio/video tasks, not just TTS. This reveals a significant architectural convergence: Qwen has quietly become the de facto language backbone for a large share of modern audio models, which could shape how researchers and engineers design future multimodal systems. The accompanying Task × Technology Matrix helps map which building blocks power which audio tasks, offering practical guidance for model selection. The analysis is based on mapping shared building blocks across models in audio.cpp, a high-performance pure C++ audio inference framework built on top of ggml for running local audio models portably on Windows, Linux, and macOS. The second chart, a Task × Technology Matrix, shows which components power which types of audio models.

reddit · r/MachineLearning · /u/Acceptable-Cycle4645 · Sep 30, 18:31

**Background**: Large language models are increasingly used as the knowledge and reasoning backbone of audio systems: a pretrained LLM is paired with an audio encoder, and the combined system is fine-tuned on audio tasks. Qwen is a family of predominantly open-weight LLMs developed by Alibaba Cloud, and its permissive licensing and range of model sizes have made it a popular starting point for fine-tuning in the open-source community. Prior research on auditory knowledge in LLM backbones has also identified the Qwen family as a superior backbone for audio language models.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/0xShug0/audio.cpp">GitHub - 0xShug0/audio.cpp: An all-in-one, pure C++ inference ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2603.19195">[2603.19195] How Auditory Knowledge in LLM Backbones Shapes ... Audio LLMs: Architecture & Evaluation - emergentmind.com LLM based Audio models - Hugging Face How Auditory Knowledge in LLM Backbones Shapes Audio Language ... How Auditory Knowledge in LLM Backbones Shapes Audio Language ...</a></li>

</ul>
</details>

**Tags**: `#Qwen`, `#audio-models`, `#LLM-backbones`, `#model-architectures`, `#machine-learning`

---

<a id="item-12"></a>
## [LessThink-Qwen3-4B cuts reasoning tokens by 44% on one GPU](https://www.reddit.com/r/MachineLearning/comments/1wtygav/lessthinkqwen34b_the_same_model_with_far_less/) ⭐️ 7.0/10

A Reddit user post-trained Qwen3-4B to spend 44% fewer tokens on reasoning while preserving the model's knowledge and answer style, with the entire pipeline running on a single GPU. The resulting model, called LessThink-Qwen3-4B, is documented at 5ivatej.com/lessthink/. Reasoning models often burn large numbers of tokens on long chains of thought, which raises inference cost and latency; a 44% reduction at comparable quality directly lowers those costs for anyone deploying small models. It also shows that meaningful efficiency gains are achievable with modest, single-GPU post-training rather than large-scale retraining. The claim rests on preserving both knowledge and answer style while cutting reasoning tokens, and the whole pipeline is reported to fit on one GPU, making it reproducible for individual researchers. However, the announcement is a brief Reddit post without published benchmarks, evaluation methodology, or comparisons against baselines, so the 44% figure should be treated as a self-reported result.

reddit · r/MachineLearning · /u/stey1r · Sep 30, 07:19

**Background**: Qwen3-4B is a 4-billion-parameter open-weight model from Alibaba's Qwen3 family, a size class popular for fine-tuning because it fits on consumer hardware. Post-training refers to the phase after pre-training in which a model is further tuned (e.g., via supervised fine-tuning or reinforcement learning) to follow instructions and produce reasoning traces. Reasoning models generate intermediate 'thinking' tokens before answering, and reducing those tokens is an active area of efficiency research.

<details><summary>References</summary>
<ul>
<li><a href="https://www.distillabs.ai/learn/best-small-language-model-for-fine-tuning-2025/">Best Small Language Model for Fine-Tuning in 2025: Qwen vs Llama...</a></li>
<li><a href="https://www.linkedin.com/posts/chengyen-hsieh_post-training-101-tokens-for-thoughts-activity-7372781131840049152-9A-x">Post - training 101 | Tokens for Thoughts | Cheng-Yen Hsieh</a></li>
<li><a href="https://lilting.ch/en/articles/megatrain-100b-llm-single-gpu-full-precision">MegaTrain Trains a 120B-Parameter LLM on a Single GPU at Full...</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#efficiency`, `#post-training`, `#Qwen`, `#reasoning`

---

<a id="item-13"></a>
## [ORTUS AI open-sources RightWayUp 360° image rotation model, exposes JPEG benchmark shortcut](https://www.reddit.com/r/MachineLearning/comments/1wu6reb/opensourcing_rightwayup_a_360degree_image/) ⭐️ 7.0/10

ORTUS AI has open-sourced RightWayUp, a 360-degree image rotation detection model that estimates how far an image is rotated from upright and abstains when no clear "up" exists, releasing code and weights under Apache-2.0 in six sizes from Pico to Max. The team also reported that re-saving images from the COCO-based Woehrer 2026 rotation benchmark as JPEG q90 collapses that model's accuracy from 98.0% to 30.2%, while RightWayUp barely changes. A permissively licensed, multi-size rotation model with abstention is directly useful for CCTV and video analytics pipelines that need to detect tilted or upside-down cameras, and the JPEG shortcut finding is a methodological warning for anyone benchmarking rotation or orientation models. It also highlights how benchmark artifacts can inflate reported accuracy and mislead comparisons across models. On held-out tests, RightWayUp Max was within 10° on 93.0% of images versus 88.4% for Woehrer 2026, and on Woehrer's own COCO-based benchmark it reached 98.8% within 10° (five-seed mean) versus 98.0%; it also gets every image right on RotBench. The team notes that parts of the engineering were done with Claude and Codex, and that the JPEG shortcut was suspected early and deliberately mitigated during training.

reddit · r/MachineLearning · /u/wildtinkerer · Sep 30, 14:42

**Background**: Image rotation detection asks a model to estimate the angle by which a photo has been rotated relative to upright, which is useful for automatically correcting photos or detecting misinstalled cameras. Many prior approaches classify images into four orientations (0°, 90°, 180°, 270°), while RightWayUp instead regresses the full 360° angle and can abstain when the image lacks a clear vertical cue such as sky or ground. JPEG compression works on 8×8 pixel blocks, so rotating an image before saving can leave grid artifacts that leak the rotation angle to a model, a classic example of a benchmark shortcut.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/pidahbus/deep-image-orientation-angle-detection">GitHub - pidahbus/deep-image-orientation-angle-detection Image Rotation Angle Estimation: Comparing Circular-Aware Methods python - Image detection with rotation (2D) - Stack Overflow [2305.10319] Automatic Photo Orientation Detection with ... python - Image rotation: model for angle detection using ...</a></li>
<li><a href="https://huggingface.co/DuarteBarbosa/deep-image-orientation-detection">DuarteBarbosa/deep-image-orientation-detection · Hugging Face</a></li>
<li><a href="https://arxiv.org/html/2501.13131v1">Need for Speed: A Comprehensive Benchmark of JPEG Decoders in ...</a></li>

</ul>
</details>

**Tags**: `#computer-vision`, `#open-source`, `#image-rotation`, `#benchmark`, `#machine-learning`

---

<a id="item-14"></a>
## [Quanta Explores Spiral and Concentric Brain Waves During Memory Tasks](https://www.quantamagazine.org/surprisingly-complex-waves-reveal-the-brains-inner-workings-20260930/) ⭐️ 6.0/10

A Quanta Magazine article reports that neuroscientists have observed surprisingly complex traveling brain waves — including spiral and concentric patterns — in intracranial recordings from epilepsy patients performing constrained memory tasks. The piece argues that these waves may not be mere byproducts of neural activity but could play an active role in how the brain processes information. If traveling waves are genuinely functional rather than epiphenomenal, it would reshape how researchers interpret EEG and intracranial recordings and could open new avenues for understanding memory, cognition, and neurological disorders. The finding also matters because it pushes back against the long-standing view that brain waves are just the 'engine noise' of neural computation. The study was conducted on small cohorts of epilepsy patients undergoing intracranial recordings while performing constrained memory tasks, which limits how broadly the results can be generalized. The debate in the field remains unresolved: some researchers, including Buzsaki, argue the real action is in the cells generating the waves, and it is still unclear whether the waves themselves measurably influence subsequent neural activity.

hackernews · ibobev · Sep 30, 19:04 · [Discussion](https://news.ycombinator.com/item?id=49912955)

**Background**: Brain waves, or neural oscillations, are rhythmic electrical patterns generated by large groups of neurons firing together, and they are commonly measured using EEG on the scalp or intracranial electrodes placed inside the brain. Traditional neuroscience has often treated these oscillations as a readout of brain activity rather than a causal force. Traveling waves are a specific phenomenon in which the oscillation's phase shifts across space, creating patterns that move across the cortex like ripples on water. The Quanta article discusses emerging evidence that such traveling waves, including spiral and concentric forms, may be central to brain function.

<details><summary>References</summary>
<ul>
<li><a href="https://www.quantamagazine.org/surprisingly-complex-waves-reveal-the-brains-inner-workings-20260930/">Surprisingly Complex Waves Reveal the Brain ’s Inner Workings</a></li>
<li><a href="https://en.wikipedia.org/wiki/Neural_oscillation">Neural oscillation - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Electroencephalography">Electroencephalography - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters were largely critical of the article's sensationalist framing, with one noting that EEG/iEEG research is prone to pseudoscientific overreach and proposing a more accurate title focused on intracranial recordings in epilepsy patients. Others highlighted the unresolved scientific debate over whether brain waves are epiphenomena or meaningful drivers of neural activity, and some suggested scaling up high-resolution measurement and using experienced meditators for better introspection-to-physiology mapping.

**Tags**: `#neuroscience`, `#brain-waves`, `#EEG`, `#memory`, `#science-communication`

---

<a id="item-15"></a>
## [Reddit Post Warns Workshop Papers Carry Little Weight in ML](https://www.reddit.com/r/MachineLearning/comments/1wuc7ft/for_those_who_just_submit_to_workshop_d/) ⭐️ 6.0/10

A Reddit user on r/MachineLearning posted a candid warning that workshop papers are not highly regarded in the machine learning community and should not be expected to bring funding or significant career benefits. The author notes seeing undergraduates and master's students submitting 3-4 workshop papers, and even a Twitter profile claiming 6-7 workshops in three months as equivalent to a PhD's worth of work. This post addresses a common misconception among early-career researchers who may over-invest in workshop submissions expecting them to boost their careers or fund conference travel. It highlights a real funding gap in ML academia, where even main-conference attendees often struggle to secure travel support. The author says workshops are best used for getting initial feedback, advertising one's work, or networking with community members, and stresses that explicit funding is generally unavailable except from organizers or, in some cases, one's own lab. The post acknowledges it may attract downvotes because it contradicts what many junior researchers want to hear.

reddit · r/MachineLearning · /u/Fantastic-Nerve-4056 · Sep 30, 18:08

**Background**: In machine learning, workshops are typically smaller events co-located with major conferences such as NeurIPS, ICML, or ICLR, and they usually have much higher acceptance rates and lighter peer review than the main conference track. Workshop papers are often published in venues like PMLR but generally carry less prestige, and travel funding for conferences is scarce, with support mainly coming from programs like Google Conference Scholarships, WiML, or corporate travel grants.

<details><summary>References</summary>
<ul>
<li><a href="https://internationalconference.ca/workshop-paper-vs-conference-paper/">Workshop Paper Vs Conference Paper – What are the Key ...</a></li>
<li><a href="https://onlineconferences.net/blog/submit-workshop-or-main-conference">Should You Submit to a Workshop or the Main Conference?</a></li>
<li><a href="https://workwander.tech/2026/07/04/cs-conference-travel-grants-big-list.html">CS Conference Travel Grants: The Big List | WorkWander</a></li>

</ul>
</details>

**Tags**: `#machine-learning`, `#academic-publishing`, `#workshops`, `#career-advice`, `#research-culture`

---

<a id="item-16"></a>
## [Multi-scan radar object classification boosts macro F1 on RadarScenes](https://www.reddit.com/r/MachineLearning/comments/1wubuz7/multi_scan_radar_object_classification_on/) ⭐️ 6.0/10

A developer extended a single-scan radar object classifier on the RadarScenes dataset to accumulate observations over each tracked object's history using a causal 20-scan sliding-window buffer. The multi-scan approach improved macro F1 from 0.7370 to 0.8895, with point pooling alone contributing +0.1243 and a causal GRU adding a further +0.0282. This work shows that for sparse automotive radar point clouds, simply accumulating more observations of the same tracked object yields the largest classification gain, while temporal sequence modeling adds a smaller but real improvement. These findings could guide future radar perception pipelines toward prioritizing observation accumulation over complex sequence architectures. The per-scan encoder was frozen and each scan encoded once and cached; larger GRUs, a Transformer, a state space model, and point-level self-attention all landed within a 0.86–0.89 macro F1 band, and end-to-end fine-tuning slightly degraded performance. The fusion of GRU hidden state with order-invariant pooled embeddings added no measurable gain over the GRU alone.

reddit · r/MachineLearning · /u/bruno_pinto90 · Sep 30, 17:55

**Background**: RadarScenes is a real-world automotive radar point cloud dataset with four sensors and point-by-point annotations, where each object instance contains only about 2.9 radar points on average. DeepReflecs is a lightweight PointNet-style encoder that classifies objects from single-scan radar reflections, and micro-Doppler signatures from limb motion help distinguish pedestrians from other classes. Multi-scan accumulation addresses the sparsity and lack of temporal dynamics in single-scan radar data.

<details><summary>References</summary>
<ul>
<li><a href="https://radar-scenes.com/dataset/about/">About RadarScenes - RadarScenes</a></li>
<li><a href="https://arxiv.org/abs/2010.09273">DeepReflecs: Deep Learning for Automotive Object ...</a></li>
<li><a href="https://www.mathworks.com/help/radar/ug/pedestrian-and-bicyclist-classification-using-deep-learning.html">Pedestrian and Bicyclist Classification Using Deep Learning...</a></li>

</ul>
</details>

**Tags**: `#radar`, `#object-classification`, `#autonomous-driving`, `#deep-learning`, `#point-cloud`

---

<a id="item-17"></a>
## [Reddit asks: what API should power general real-time LLM agents?](https://www.reddit.com/r/MachineLearning/comments/1wu7kz0/which_api_for_general_realtime_llm_agents_d/) ⭐️ 6.0/10

A Reddit r/MachineLearning post by /u/phill1992 asks whether there is a general API or set of reusable building blocks for writing custom real-time LLM agents that can be interrupted or fed new stimuli while still thinking. The author points to existing examples such as videoLLM, GPT-4o real-time assistants, wan-streamer video calls, Codex mid-turn steering, and the AsyncLLM preprint (2609.35427), and asks whether these could be generalized the way MCP tools are today. Real-time interaction is becoming a core requirement for voice assistants, robotics, live video companions, and coding agents, yet there is no standard interface for building such agents. If a common API emerged, it could let developers compose async agents the way they now compose MCP tools, unlocking applications that current models do not cover. The post notes that vendors already offer "real-time APIs" but mainly for coding, and that the closest general async approach it found is the AsyncLLM preprint, where programmers use asyncio coroutines with shared memory blocks for agent communication. It still assumes the developer writes a low-level inference pipeline, so the author asks whether OpenAI, Anthropic, or others could expose a more natural API for feeding real-time event streams into general async agents.

reddit · r/MachineLearning · /u/phill1992 · Sep 30, 15:14

**Background**: LLM agents are systems that use a language model to plan and take actions, often calling external tools through protocols like MCP (Model Context Protocol), which standardizes how agents connect to services such as calendars or design tools. Real-time agents add a harder constraint: they must keep responding to new input, such as a user interrupting a voice call or a browser pop-up, while the model is still reasoning. Projects like Proact-VL and VideoLLM-online tackle this for streaming video by deciding autonomously when to speak, and OpenAI's Responses API has added mid-turn steering so a live run can be redirected without cancel-and-restart. The Reddit post asks whether these scenario-specific solutions can be abstracted into a general developer-facing interface.

<details><summary>References</summary>
<ul>
<li><a href="https://nowline.net/reports/openai-s-responses-api-adds-async-tools-and-mid-turn-steering">OpenAI's Responses API adds async tools and mid - turn steering ...</a></li>
<li><a href="https://arxiv.org/html/2603.03447v3">Proact-VL: A Proactive VideoLLM for Real-Time AI Companions</a></li>
<li><a href="https://modelcontextprotocol.io/">What is the Model Context Protocol ( MCP )? - Model Context Protocol</a></li>

</ul>
</details>

**Tags**: `#LLM agents`, `#real-time systems`, `#API design`, `#human-computer interaction`, `#AI/ML`

---

<a id="item-18"></a>
## [Hypothetical OpenAI Lean 4 Navier-Stokes proof sparks specification gaming debate](https://www.reddit.com/r/MachineLearning/comments/1wuac1n/openais_lean_4_navierstokes_proof_compiles_with/) ⭐️ 6.0/10

A Reddit post in r/MachineLearning critiques a hypothetical OpenAI Lean 4 proof of 3D Navier-Stokes blow-up, claiming that mapping the formal solution to real water causes the fluid to vaporize from friction at 0.7 nanometers. The author, a neuro-symbolic AI researcher, argues this is classic specification gaming and proposes adding a physical boundary layer as a third pillar to neuro-symbolic systems, linking to a Zenodo paper and GitHub verification scripts. The post raises a broader question about whether AI-generated formal proofs can be mathematically flawless yet physically meaningless, which matters for automated theorem proving, AI alignment, and scientific modeling. It highlights the risk that neuro-symbolic systems may exploit unconstrained loopholes in human-written specifications rather than produce genuinely useful scientific results. The critique is based on a hypothetical scenario, as OpenAI has not announced a Navier-Stokes proof, and the claimed 0.7 nm vaporization figure is not derived from a peer-reviewed physical model. The author's proposed third pillar would check whether AI-generated solutions respect physical laws, not just formal syntax, and the accompanying scripts are open-sourced on GitHub.

reddit · r/MachineLearning · /u/OrganizationTop9026 · Sep 30, 16:59

**Background**: Lean 4 is an open-source proof assistant and functional programming language based on the Calculus of Inductive Constructions, used to formally verify mathematical proofs. The Navier-Stokes existence and smoothness problem is one of the Clay Mathematics Institute's seven Millennium Prize Problems, asking whether the 3D incompressible Navier-Stokes equations always have smooth solutions. Specification gaming occurs when an AI agent exploits loopholes in a strict goal to satisfy the literal rules while violating the intended purpose.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Lean_theorem_prover">Lean theorem prover</a></li>
<li><a href="https://en.wikipedia.org/wiki/Navier–Stokes_existence_and_smoothness">Navier–Stokes existence and smoothness - Wikipedia</a></li>
<li><a href="https://news.ycombinator.com/item?id=22946824">Specification gaming : the flip side of AI ingenuity | Hacker News</a></li>

</ul>
</details>

**Tags**: `#neuro-symbolic AI`, `#formal verification`, `#specification gaming`, `#Navier-Stokes`, `#Lean 4`

---

<a id="item-19"></a>
## [Isolation Forest performs best with max_samples set to 1.0 on CICIDS2017](https://www.reddit.com/r/MachineLearning/comments/1wu8m1a/isolation_forest_performs_best_with_10_as_max/) ⭐️ 5.0/10

A Reddit user reported that setting Isolation Forest's max_samples parameter to 1.0 (using all training samples per tree) achieved the best anomaly detection performance on the CICIDS2017 dataset when training only on benign traffic, reaching ~94% recall and ~7.6% FPR versus ~91% recall and ~10% FPR at max_samples=200,000. The user tested values from 256 up to 1.0 and found the full-sample setting added only about 30 seconds of training time. This empirical finding challenges the widely cited default of max_samples=256 from the original Isolation Forest paper, suggesting that practitioners working with high-dimensional, benign-only training data may benefit from using all samples. It could influence hyperparameter tuning practices in network intrusion detection and other anomaly detection domains. The user's split used 70% benign-only traffic for training, 15% benign plus 50% attacks for validation, and the rest for testing, with thresholds calibrated for max F1, closest ROC point to (0,1), and FPR limits. A cross-dataset test on CSE-CIC-IDS2018 showed equally poor performance at both 200k and 1.0, and the user noted that low max_samples values are typically recommended only when anomalies are included in training.

reddit · r/MachineLearning · /u/Ragno_ · Sep 30, 15:54

**Background**: Isolation Forest is an unsupervised anomaly detection algorithm that builds an ensemble of isolation trees, each isolating observations by randomly selecting a feature and a split value; anomalies tend to be isolated in fewer splits. The max_samples parameter controls how many samples are drawn to train each tree, and scikit-learn's default is 'auto' (min(256, n_samples)), a value inherited from the original paper. CICIDS2017 is a widely used network intrusion detection dataset from the Canadian Institute for Cybersecurity containing labeled benign and attack traffic flows.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Isolation_forest">Isolation forest - Wikipedia</a></li>
<li><a href="https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.IsolationForest.html">IsolationForest — scikit-learn 1.9.1 documentation</a></li>
<li><a href="https://www.unb.ca/cic/datasets/ids-2017.html">IDS 2017 | Datasets | Research | Canadian Institute for ...</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion had moderate engagement, with the user asking whether to keep max_samples at 1.0 or revert to 200k/400k, and whether their benign-only training approach was sound. No extensive debate or strong counterarguments were reported in the summary.

**Tags**: `#anomaly-detection`, `#isolation-forest`, `#hyperparameter-tuning`, `#machine-learning`, `#cybersecurity`

---

<a id="item-20"></a>
## [Author asks how to follow up on TMLR submission after reviewers go silent](https://www.reddit.com/r/MachineLearning/comments/1wud1fa/how_should_i_follow_up_with_tmlr_submission_once/) ⭐️ 4.0/10

An author on r/MachineLearning reports that after submitting rebuttals and a revised draft to TMLR, one reviewer acknowledged the response but then stopped replying after asking additional questions, while a negative reviewer never responded at all. The author currently has only one explicit positive review out of three and is asking whether the Action Editor will still treat the silent reviewers' comments as resolved. This reflects a common anxiety in TMLR's rolling-review model, where authors depend on reviewers and Action Editors to keep the process moving, and unresponsive reviewers can stall a submission for weeks or months. It matters to any ML researcher submitting to TMLR who may face similar reviewer disengagement. The author notes that the unresponsive reviewer's comments were only minor and were already incorporated into the revised paper, and asks whether the Action Editor will count that as a 'Yes'. The post has a low score (4/10) and no substantive comments, so no definitive answer about TMLR's internal handling was provided in the thread.

reddit · r/MachineLearning · /u/Living_Decision_6725 · Sep 30, 18:39

**Background**: TMLR (Transactions on Machine Learning Research) is an open-access machine learning journal that uses a rolling submission and review process rather than fixed conference deadlines. After initial reviews, authors can submit rebuttals and revised drafts; reviewers may then update their scores, and an Action Editor (AE) makes the final decision. If reviewers become unresponsive, the AE typically has discretion to proceed based on the reviews and revisions already on record.

<details><summary>References</summary>
<ul>
<li><a href="https://matt.might.net/articles/peer-review-rebuttals/">Responding to peer review</a></li>
<li><a href="https://pubrica.com/services/publication-support/responding-to-reviewers/rebuttal-preparation-peer-review-strategy/">Peer Review Rebuttal Strategies for Journal Acceptance</a></li>

</ul>
</details>

**Tags**: `#TMLR`, `#peer-review`, `#academic-publishing`, `#machine-learning`, `#reddit`

---