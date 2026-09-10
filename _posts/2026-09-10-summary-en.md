---
layout: default
title: "Horizon Summary: 2026-09-10 (EN)"
date: 2026-09-10
lang: en
---

> From 19 items, 16 important content pieces were selected

---

1. [OpenAI's Navier-Stokes Release Includes a Lean 4 Formal Proof](#item-1) ⭐️ 9.0/10
2. [Microsoft Elevates Rust to Tier-1 Language Status](#item-2) ⭐️ 9.0/10
3. [Calif Research Unveils WeWorm, First Zero-Click WeChat Call Worm](#item-3) ⭐️ 9.0/10
4. [Shopify abandons React Native for native Swift and Kotlin](#item-4) ⭐️ 8.0/10
5. [Researchers question whether OpenAI can be trusted with unpublished math](#item-5) ⭐️ 8.0/10
6. [Forgejo 16.0.4 Fixes Critical RCE Vulnerability](#item-6) ⭐️ 8.0/10
7. [Fly connectome fails to learn Pong, audit reveals bugs and insights](#item-7) ⭐️ 8.0/10
8. [Cognition launches SWE-2 coding model, rivaling Fable 5.1 at lower cost](#item-8) ⭐️ 7.0/10
9. [NASA's Decorrelation Stretch Reveals Ancient Rock Art](#item-9) ⭐️ 7.0/10
10. [PlanetScale Launches Neki, a Closed-Source Sharded Postgres](#item-10) ⭐️ 7.0/10
11. [348M model trained from scratch beats GPT-3 175B on multi-digit arithmetic](#item-11) ⭐️ 7.0/10
12. [Blog defends keeping a big box of cables, sparking HN debate](#item-12) ⭐️ 6.0/10
13. [Free Online Music Theory Textbook Sparks Debate on Classical Bias](#item-13) ⭐️ 6.0/10
14. [uv 0.12.13 Adds GraalPy 3.13 Support and Metadata Hash Verification](#item-14) ⭐️ 4.0/10
15. [.blend URL Viewer: Simon Willison's Browser Tool for Blender Files](#item-15) ⭐️ 4.0/10
16. [Reddit Users Await ICDE Conference Results](#item-16) ⭐️ 3.0/10

---

<a id="item-1"></a>
## [OpenAI's Navier-Stokes Release Includes a Lean 4 Formal Proof](https://www.johndcook.com/blog/2026/09/09/formal-method-revolution/) ⭐️ 9.0/10

OpenAI's September 2026 release on the Navier-Stokes existence and smoothness problem included a Lean 4 formal proof, meaning the result was accompanied by a machine-checkable derivation rather than only a natural-language argument. The announcement claims an unbounded counterexample to the three-dimensional Navier-Stokes existence and smoothness problem, though the result has not yet been verified by external mathematicians. If the Lean 4 proof checks out, it would be a landmark demonstration that AI systems can contribute to solving one of the seven Millennium Prize Problems, and it would push formal verification from a niche tool into the mainstream of AI-driven mathematical research. The episode also raises urgent questions about training-data provenance, independent verification, and the cost of coordinating large fleets of AI agents on open research problems. Lean 4 is a formal proof assistant in which every step must be mechanically checked, so a proof either verifies or it does not, leaving no room for a lucky guess. Community commenters noted that Lean verification itself can be extremely slow, citing a Fermat's Last Theorem verification that reportedly took 15 hours with 230GB of RAM, and they estimated the agent cost of the Navier-Stokes effort at roughly $40 million versus about $132 million for an equivalent human effort.

hackernews · ibobev · Sep 10, 21:22 · [Discussion](https://news.ycombinator.com/item?id=49650326)

**Background**: The Navier-Stokes equations describe the motion of viscous fluids and are central to fields from aerodynamics to blood-flow modeling; the related existence and smoothness problem asks whether smooth solutions always exist in three-dimensional space and is one of the Clay Mathematics Institute's seven Millennium Prize Problems. Formal verification means proving a result against a rigorous mathematical specification so that a computer can check its correctness, and Lean 4 is one of the leading proof assistants used for this purpose. OpenAI's claimed counterexample builds on prior work by Levent Alpöge and Tristan Buckmaster on finite-time blowup for the 3D incompressible Euler equations with smooth forcing, and those researchers have raised concerns about whether their chats may have entered the model's training data.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Navier-Stokes_equations">Navier-Stokes equations</a></li>
<li><a href="https://en.wikipedia.org/wiki/Navier–Stokes_existence_and_smoothness">Navier–Stokes existence and smoothness - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Formal_verification">Formal verification - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters were divided between awe at the result and skepticism about the surrounding hype, with one noting it is astonishing that a generalized program can tackle a problem of this magnitude while others focused on Lean's performance and cost. Several disputed the framing of the cost comparison, arguing the human figure is closer to $132 million rather than four orders of magnitude cheaper, and one raised the deeper worry of what happens when an AI solves a problem that humans cannot independently verify.

**Tags**: `#AI`, `#formal-verification`, `#Lean`, `#mathematics`, `#Navier-Stokes`

---

<a id="item-2"></a>
## [Microsoft Elevates Rust to Tier-1 Language Status](https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/) ⭐️ 9.0/10

Microsoft has officially designated Rust as a tier-1 language, placing it alongside C++, C#, and TypeScript as one of the best-supported languages for internal development. The announcement, published as a guest post on the Rust Foundation website, confirms long-rumored MSVC backend integration for Rust. This is a major endorsement of Rust by one of the world's largest software vendors, signaling that Rust is now a mature, serious competitor to established systems languages like C++ and C#. It could accelerate Rust adoption across the industry, especially for greenfield systems programming where memory safety is critical. Microsoft's goal is reportedly to convert 1 billion lines of code to Rust by 2030 using automated tooling, aiming for '1 engineer, 1 month, 1 million lines of code.' DARPA is also funding efforts to automate C-to-Rust conversion through six different teams using various approaches.

hackernews · mmastrac · Sep 10, 13:39 · [Discussion](https://news.ycombinator.com/item?id=49643546)

**Background**: Rust is a systems programming language known for its memory safety guarantees, which prevent common bugs like buffer overflows and use-after-free errors at compile time without runtime overhead. Microsoft has previously reported that about 70% of its CVEs are memory safety issues, making Rust an attractive alternative to C and C++. Tier-1 status means Rust receives the same level of tooling, documentation, and support as Microsoft's other top languages.

<details><summary>References</summary>
<ul>
<li><a href="https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/">Guest Post: Rust Is Tier - 1 Language at Microsoft</a></li>
<li><a href="https://news.ycombinator.com/item?id=49643546">Rust Is Tier - 1 Language at Microsoft | Hacker News</a></li>

</ul>
</details>

**Discussion**: Commenters largely view this as a significant milestone, with some noting it shows Rust is no longer a fledgling language but a mature competitor to C++ and C#. Others highlight the strategic value for memory safety and the replacement of LLVM with MSVC's backend as the biggest technical news, while some ask when Visual Studio will get tier-1 debugging support for Rust.

**Tags**: `#Rust`, `#Microsoft`, `#systems-programming`, `#memory-safety`, `#language-adoption`

---

<a id="item-3"></a>
## [Calif Research Unveils WeWorm, First Zero-Click WeChat Call Worm](https://simonwillison.net/2026/Sep/10/calif-research/) ⭐️ 9.0/10

Calif Research released a demo of WeWorm, described as the first zero-click worm that spreads through WeChat calls on both iOS and Android, hijacking accounts without any victim interaction. The team found the bug and wrote the first remote code execution (RCE) exploit in about two days with AI assistance, then built the full worm in one more week. This demonstrates a paradigm shift in offensive security: an exploit and self-spreading worm that once took a larger team months was built by a small team in roughly nine days using AI. It raises major concerns for mobile security and shows how AI can dramatically accelerate large-scale exploit development against widely used messaging platforms. The vulnerability is a memory corruption issue in WeChat's VoIP stack, and the exploit succeeds even if the victim answers the call and hears nothing, or does not interact with the phone at all. Calif demonstrated the worm spreading among three test phones, and the research was published on September 8, 2026.

rss · Simon Willison · Sep 10, 00:56

**Background**: A zero-click exploit requires no action from the victim, making it far more dangerous than attacks that need a user to open a file or tap a link. A worm is malware that self-propagates by automatically infecting other devices, and remote code execution (RCE) means an attacker can run arbitrary code on a target device. WeChat is a massively popular messaging app in China and beyond, so a worm spreading through its call feature could reach an enormous user base.

<details><summary>References</summary>
<ul>
<li><a href="https://thehackernews.com/2026/09/wechat-zero-click-worm-took-over.html">WeChat Zero-Click Worm Took Over Accounts on iPhone and Android via Incoming Calls</a></li>
<li><a href="https://www.1950.ai/post/wechat-zero-click-worm-how-ai-turned-a-voip-vulnerability-into-a-self-spreading-account-hijacking-t">WeChat Zero-Click Worm: How AI Turned a VoIP Vulnerability Into...</a></li>
<li><a href="https://cyberinsider.com/zero-click-worm-spreads-on-iphones-and-android-via-wechat-calls/">Zero-click worm spreads on iPhones and Android via WeChat calls</a></li>

</ul>
</details>

**Tags**: `#security`, `#ai-security-research`, `#mobile-exploit`, `#zero-click`, `#wechat`

---

<a id="item-4"></a>
## [Shopify abandons React Native for native Swift and Kotlin](https://shopify.engineering/back-to-native) ⭐️ 8.0/10

Shopify announced it is moving its mobile app development away from React Native and back to fully native Swift (iOS) and Kotlin (Android) codebases. The engineering blog post details the rationale and migration approach, triggering a large discussion with 448 comments on cross-platform trade-offs. Shopify's reversal is a significant industry signal because the company was a prominent React Native adopter and contributor, and its move may influence other large teams weighing cross-platform efficiency against native performance and UX. It also highlights how AI-assisted coding agents are changing the economics of maintaining separate native codebases. The migration involves rewriting the app in Swift and Kotlin, and community members report that AI coding agents such as Codex can inventory React Native screens and scaffold native Android and iOS directories quickly, though polish still requires manual effort. Commenters also note that the migration work at Shopify predates widespread LLM assistance, suggesting the decision was driven by long-term maintenance and UX concerns rather than purely by AI tooling.

hackernews · fnthawar2 · Sep 10, 14:09 · [Discussion](https://news.ycombinator.com/item?id=49643982)

**Background**: React Native is a cross-platform framework created by Meta that lets developers write mobile apps in JavaScript/TypeScript and share code across iOS and Android. Native development instead uses Swift for iOS and Kotlin for Android, which typically yields better performance and platform-specific UX but requires separate codebases and teams. Shopify had previously invested heavily in React Native, making its reversal notable.

<details><summary>References</summary>
<ul>
<li><a href="https://reactnative.dev/">React Native · Learn once, write anywhere</a></li>
<li><a href="https://www.coderio.com/blog/software-development/swift-vs-kotlin-native-app-development/">Swift vs Kotlin for Native App Development: Complete 2026 Guide</a></li>
<li><a href="https://www.techrev.us/blog/swift-vs-kotlin-for-native-app-development/">Swift vs Kotlin: Native App Development Compared (2026 Guide) - TechRev-Blog</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree that moving off React Native can improve UX, but they debate whether AI/LLMs were the key enabler; one experienced migrator says most of their migration predated LLM assistance. Others share success with Kotlin Multiplatform and note that cross-platform frameworks often fail to reduce headcount costs as promised, while a few caution that native rewrites are still substantial efforts.

**Tags**: `#React Native`, `#mobile development`, `#Swift`, `#Kotlin`, `#cross-platform`

---

<a id="item-5"></a>
## [Researchers question whether OpenAI can be trusted with unpublished math](https://mathstodon.xyz/@andreasthom/117240535270608201) ⭐️ 8.0/10

A Mathstodon post by Andreas Thom, amplified by a Hacker News thread with 581 comments, raises the question of whether mathematicians can trust OpenAI with unpublished ideas after the company reportedly used researcher interactions to help solve a major open math problem without clear attribution. The discussion centers on OpenAI's admission that it 'cannot rule out' that de-identified data derived from users' product usage helped improve its models. This touches on core issues of research integrity, attribution, and data privacy, potentially deterring mathematicians from collaborating with or using commercial AI models and reshaping norms around how unpublished work is shared. It also feeds a broader debate about whether AI-driven mathematical discovery is genuinely superhuman or partly built on researchers' own fresh ideas. OpenAI reportedly generated 300 billion output tokens from a model still in training shortly after learning there was a credible chance a major math proof was in that model's training data, which some commenters describe as suspicious 'parallel construction.' OpenAI's own statement that it cannot rule out that de-identified usage data helped improve its models is cited as a key reason for researcher caution.

hackernews · pred_ · Sep 10, 06:49 · [Discussion](https://news.ycombinator.com/item?id=49639408)

**Background**: Large language models are trained on massive text corpora, and once unpublished research or writing is incorporated into training, it can resurface in future outputs without attribution. Attribution is technically hard because with millions of training examples the math becomes prohibitive, so researchers rely on approximations rather than actually removing individual examples. OpenAI has invited researchers to use its models, including free access programs, which means fresh, unpublished mathematical ideas may flow into systems whose training data policies are opaque.

<details><summary>References</summary>
<ul>
<li><a href="https://www.banandre.com/blog/openai-navier-stokes-millennium-problem-ai-proof-controversy">OpenAI Cracked a 90-Year-Old Math Problem in 88 Hours. - Banandre</a></li>
<li><a href="https://learningcommons.lib.uoguelph.ca/item/ai-and-your-unpublished-writing-risks-using-large-language-models/">AI and Your Unpublished Writing: Risks of Using Large Language Models | Digital Learning Commons</a></li>
<li><a href="https://www.computerworld.com/article/4211283/ais-attribution-problem-gets-worse-as-models-scale.html">AI’s attribution problem gets worse as models scale</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree the situation is ethically troubling, with one arguing that if OpenAI were a human collaborator, publishing work from a collaboration without attribution would be clearly unethical. Others note both things can be true: chats may improve a model's latent intuition while reinforcement learning on verifiable math also discovers genuinely novel techniques. Several express suspicion about the timing of the 300 billion token generation and question whether AI is truly solving open problems or whether researchers are being fooled.

**Tags**: `#AI ethics`, `#OpenAI`, `#research integrity`, `#mathematics`, `#data privacy`

---

<a id="item-6"></a>
## [Forgejo 16.0.4 Fixes Critical RCE Vulnerability](https://codeberg.org/forgejo/forgejo/src/branch/forgejo/release-notes-published/16.0.4.md) ⭐️ 8.0/10

Forgejo versions up to 16.0.3 contain a critical remote code execution vulnerability, which has been fixed in version 16.0.4 (and backported to 15.0.8). The flaw involves template expansion interfering with git repository initialization when generating a new repository from a template repository. This critical RCE vulnerability affects all self-hosted Forgejo instances up to 16.0.3, potentially allowing attackers to execute arbitrary code on the server. Administrators must upgrade immediately to protect their infrastructure and data. The vulnerability occurs during repository creation from a template: Forgejo clones the template, removes the .git folder, performs variable template expansion on files listed in .forgejo/template, and initializes a new git repository. The fix prevents template expansion from interfering with git repo initialization; Gitea is reportedly unaffected by this issue.

hackernews · weierstass · Sep 10, 15:57 · [Discussion](https://news.ycombinator.com/item?id=49645907)

**Background**: Forgejo is a self-hosted lightweight software forge, a web-based platform for collaborative software development that provides Git repository hosting, code review, issue tracking, and continuous integration. Remote code execution (RCE) is a class of cyberattacks that allows attackers to run malicious code on a remote server without physical access. Forgejo is a community fork of Gitea, and both are popular alternatives to GitHub for organizations that want to host their own development infrastructure.

<details><summary>References</summary>
<ul>
<li><a href="https://lwn.net/Articles/1093671/">Forgejo 16 . 0 . 4 and 15.0.8 address critical security vulnerability</a></li>
<li><a href="https://forgejo.org/">Forgejo – Beyond coding. We forge .</a></li>
<li><a href="https://en.wikipedia.org/wiki/Forge_(software)">Forge (software)</a></li>

</ul>
</details>

**Discussion**: Community members noted that the release notes were initially unreadable due to Codeberg rate limits, and shared alternative URLs. A Gitea project leader clarified that Gitea is protected against both issues and cautioned against shaming security reporters. Some users debated whether Forgejo's policy of disallowing LLM contributions puts it at a disadvantage, as attackers may use AI to find vulnerabilities.

**Tags**: `#security`, `#vulnerability`, `#forgejo`, `#git`, `#rce`

---

<a id="item-7"></a>
## [Fly connectome fails to learn Pong, audit reveals bugs and insights](https://www.reddit.com/r/MachineLearning/comments/1wc67ci/i_tried_to_make_a_real_fly_connectome_learn_to/) ⭐️ 8.0/10

A developer attempted to train a real subgraph of the MaleCNS v1.0 fly connectome to play Pong using dopamine-style plasticity, but it failed to learn. Auditing the failure uncovered a neuPrint regex bug that zeroed out two neuron populations, a missing photoreceptor-to-motion-detector pathway, and motor neurons with zero sensory synapses, ultimately producing a detailed negative-result case study. This rigorous negative result highlights that viral fly-brain game demos may not actually validate biological realism, as the Doom, Minecraft, and Beat Saber projects also admit failures or hand-injected behaviors. It provides a valuable case study for computational neuroscience and ML, emphasizing transparent auditing and the importance of connectivity in connectome-based models. The neuPrint regex bug involved full-match versus substring semantics, silently zeroing out two neuron populations. Half of the four available motor neurons had zero synapses from any sensory pathway, and learning-on versus learning-off produced bit-for-bit identical results across multiple seeds despite weights changing. The effect of learning appeared to quiet the system rather than improve skill, with punishment dominating due to more misses than hits.

reddit · r/MachineLearning · /u/oPeraza2007 · Sep 10, 02:28

**Background**: The MaleCNS v1.0 connectome is a full adult Drosophila male central nervous system reconstruction with 166k neurons, released by Janelia's FlyEM project, enabling detailed simulations. Connectomes map neural wiring, and dopamine-style plasticity adjusts synaptic weights based on reward or punishment signals, mimicking learning. Pong serves as a stringent testbed because it provides a binary hit/miss signal each frame, making it hard to fake success.

<details><summary>References</summary>
<ul>
<li><a href="https://male-cns.janelia.org/">Male CNS Connectome - MaleCNS connectome</a></li>
<li><a href="https://arxiv.org/abs/2512.07194">[2512.07194] Synchrony-Gated Plasticity with Dopamine Modulation for Spiking Neural Networks</a></li>

</ul>
</details>

**Discussion**: The Reddit post invites discussion on whether others have encountered similar issues with MaleCNS v1.0, particularly around the central complex and steering circuits, suggesting these as the next simulation target. The community likely appreciates the transparent negative result and the comparison to viral projects, adding insights into computational neuroscience challenges.

**Tags**: `#connectome`, `#computational-neuroscience`, `#machine-learning`, `#negative-results`, `#plasticity`

---

<a id="item-8"></a>
## [Cognition launches SWE-2 coding model, rivaling Fable 5.1 at lower cost](https://cognition.com/blog/swe-2) ⭐️ 7.0/10

Cognition released SWE-2, a coding model post-trained from the open-weight Kimi K3, claiming 50.0% on FrontierCode 1.1 Main and performance within one point of Fable 5.1 while being up to 64-70% cheaper. The company says it scaled reinforcement learning to the multi-trillion-parameter regime for the first time, building on its SWE-1.7 training infrastructure. The release intensifies competition among AI coding tools, showing that post-training an open-weight base model can approach frontier performance at a fraction of the cost. It also fuels the ongoing debate over closed-weight versus open-weight models, especially as users question whether proprietary providers can justify their pricing. SWE-2 is post-trained from Kimi K3, a 2.8T-parameter open-weight model with a 1M-token context window, and Cognition claims its medium variant makes its first code edit after a median of 18 steps versus 48 for SWE-1.7. However, community members note a large gap between Terminal Bench 2.1 (92.8%) and the newer Terminal Bench 4 (27.3%), raising concerns about benchmark overfitting and generalization.

hackernews · seelos · Sep 10, 15:29 · [Discussion](https://news.ycombinator.com/item?id=49645443)

**Background**: Cognition is an AI company known for its Devin coding agent, and SWE-2 is its latest coding-focused model. Kimi K3 is an open-weight 2.8T-parameter model from Moonshot AI designed for long-horizon coding and reasoning, while Fable 5.1 is Anthropic's frontier model with strong agentic coding capabilities. Benchmark scores like Terminal Bench and FrontierCode are used to compare coding models, but they can be gamed if models are trained on similar tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://cognition.com/blog/swe-2">Introducing SWE-2: Pushing the Pareto Frontier | Cognition</a></li>
<li><a href="https://huggingface.co/moonshotai/Kimi-K3">moonshotai/Kimi-K3 · Hugging Face</a></li>
<li><a href="https://www.anthropic.com/claude-fable-and-mythos-5-1">Introducing Claude Fable 5 . 1 and Claude Mythos 5 . 1 \ Anthropic</a></li>

</ul>
</details>

**Discussion**: Commenters expressed skepticism about benchmark generalization, pointing to the large delta between Terminal Bench 2.1 and 4.0 as evidence of possible overfitting, and recalled Cognition's past credibility issues with its Devin demo. Others questioned why they would use a closed-weight model over open alternatives like DeepSeek Flash 4.1, while some noted that post-training Kimi K3 to reach Fable 5-level capabilities is a positive sign.

**Tags**: `#AI`, `#coding-models`, `#benchmarks`, `#open-weights`, `#Cognition`

---

<a id="item-9"></a>
## [NASA's Decorrelation Stretch Reveals Ancient Rock Art](https://spinoff.nasa.gov/Manipulating_Satellite_Photos_Now_Reveals_Ancient_Images) ⭐️ 7.0/10

NASA's decorrelation stretch technique, originally developed by JPL in 1978 to enhance satellite and remote sensing imagery, is now being widely adapted to uncover ancient rock art and murals. The method, popularized for archaeology through Jon Harman's DStretch software, amplifies subtle color differences that are invisible to the naked eye. This cross-disciplinary application shows how space technology can be repurposed for cultural heritage preservation, helping archaeologists discover and document faded rock art that might otherwise remain hidden. It also highlights the broader value of signal processing and remote sensing techniques beyond their original aerospace domain. Decorrelation stretch works by removing inter-channel correlation in image pixels and reassigning variances, which can suffer from numerical instability and degenerate cases where color planes are linearly dependent. The technique is accessible to non-specialists, as similar results can be achieved in GIMP using LAB decomposition, auto input levels on chroma channels, and recomposition.

hackernews · gumby · Sep 10, 15:29 · [Discussion](https://news.ycombinator.com/item?id=49645437)

**Background**: Decorrelation stretch is an image enhancement technique that emphasizes color differences in multispectral datasets, originally created to extract more information from satellite imagery of Earth and Mars. It transforms an image so that its color planes become uncorrelated with assigned variances, making subtle features easier to spot. Archaeologists later adapted it for rock art studies because faded pigments often differ from surrounding rock in ways invisible to normal vision.

<details><summary>References</summary>
<ul>
<li><a href="https://spinoff.nasa.gov/Manipulating_Satellite_Photos_Now_Reveals_Ancient_Images">Technique for Manipulating Satellite Photos Now... | NASA Spinoff</a></li>
<li><a href="https://gizmodo.com/this-nasa-color-trick-was-meant-for-mars-now-its-unveiling-rock-art-on-earth-2000809844">This NASA Color Trick Was Meant for Mars. Now It's Unveiling Rock ...</a></li>
<li><a href="https://dstretch.com/AlgorithmDescription.pdf">DStretch Algorithm Description</a></li>

</ul>
</details>

**Discussion**: Commenters shared practical tips, including a GIMP workflow using LAB decomposition and auto input levels, and one asked for an ImageMagick implementation. Others reflected on how false-color composites changed their understanding of signal processing and sensors, while one noted the impressive commitment behind ancient rock art. A user also described an unsuccessful attempt to find hidden rock art at Angkor Wat using multiple bandpass filters.

**Tags**: `#image-processing`, `#archaeology`, `#remote-sensing`, `#NASA`, `#signal-processing`

---

<a id="item-10"></a>
## [PlanetScale Launches Neki, a Closed-Source Sharded Postgres](https://planetscale.com/blog/introducing-neki) ⭐️ 7.0/10

PlanetScale announced Neki, a sharded Postgres solution built by the team behind large-scale Vitess deployments, promising scaling to hundreds of millions of QPS and petabytes of data with zero-downtime resharding. The launch quickly drew a heated Hacker News debate over its closed-source nature, the CEO's tone toward competitors, and unresolved consistency trade-offs. Sharding Postgres at scale has long been one of the hardest problems in the database world, and a credible managed offering from PlanetScale could reshape how teams handle massive Postgres workloads. The controversy also highlights growing tension in the developer community over closed-source infrastructure products from companies with strong open-source reputations. Neki is being built in close collaboration with design partners who already operate Postgres at significant scale, and PlanetScale claims zero-downtime resharding as a core feature. However, the launch post was criticized for never clearly explaining what Neki actually is or who it is for, and the product remains closed-source despite the company's open-source heritage with Vitess.

hackernews · simon_weber · Sep 10, 15:43 · [Discussion](https://news.ycombinator.com/item?id=49645686)

**Background**: Sharding is a database architecture pattern that horizontally partitions data across multiple servers, with each node storing only a subset called a shard, enabling greater scalability than a single machine. Postgres has historically lacked native sharding, forcing teams to rely on extensions like Citus or application-level sharding, which introduces complexity around cross-shard transactions and consistency. PlanetScale originally built its reputation on Vitess, an open-source sharding system for MySQL used by YouTube and others, making its move into closed-source Postgres sharding notable.

<details><summary>References</summary>
<ul>
<li><a href="https://neki.dev/">Neki | Sharded Postgres by PlanetScale</a></li>
<li><a href="https://planetscale.com/docs/postgres/sharding">Horizontal sharding for Postgres - PlanetScale</a></li>
<li><a href="https://www.geeksforgeeks.org/system-design/sharding-vs-consistent-hashing/">Sharding Vs. Consistent Hashing - GeeksforGeeks</a></li>

</ul>
</details>

**Discussion**: Commenters heavily criticized the launch post for failing to explain what Neki is or who it is for, with one top comment sarcastically noting that every section describes problems or components but never the product itself. Others attacked the CEO's tone, pointing out he had publicly disparaged Supabase's open-source multigres while Neki remains closed-source, and raised serious technical concerns about whether eventual consistency makes Neki unsuitable for many workloads given CAP theorem trade-offs.

**Tags**: `#Postgres`, `#Database Sharding`, `#Distributed Systems`, `#PlanetScale`, `#Open Source`

---

<a id="item-11"></a>
## [348M model trained from scratch beats GPT-3 175B on multi-digit arithmetic](https://www.reddit.com/r/MachineLearning/comments/1wc7hmu/i_trained_a_348m_model_trained_from_scratch_on/) ⭐️ 7.0/10

An independent developer trained a 348M-parameter language model from scratch on 22.7B tokens, then fine-tuned it to solve arithmetic by showing step-by-step column work, achieving a 99.4% average across nine GPT-3 arithmetic sub-tasks and outperforming GPT-3 175B on multi-digit addition and subtraction. The model handles clean addition up to 14 digits after the developer expanded the place-value vocabulary from 6 to 19 entries, a fix that moved the clean ceiling from 8 to 14 digits. This result shows that a small, independently trained model can dramatically outperform a much larger model like GPT-3 175B on arithmetic when it is fine-tuned to show its work, reinforcing the value of chain-of-thought-style training over raw scale for certain reasoning tasks. It also highlights that vocabulary design can be a hidden bottleneck for arithmetic generalization, a practical insight for anyone building small specialized models. The model achieves 100% on 2- to 5-digit addition, 98-99% on subtraction, and 98% on 3x3 multiplication, but it fails at word problems (GSM8K 4%, ASDiv 16.5%), has no division, and requires greedy decoding because sampling corrupts the column routine. The developer notes that the arithmetic harness orders subtraction operands, so those results should be interpreted with that caveat.

reddit · r/MachineLearning · /u/nkthebass · Sep 10, 03:28

**Background**: Large language models often struggle with multi-digit arithmetic when asked to answer directly, and GPT-3 175B's accuracy drops sharply as digit counts increase. Chain-of-thought prompting, which asks models to produce intermediate reasoning steps, has been shown to substantially improve arithmetic performance. This project applies that idea at training time by fine-tuning a small model to always show column-by-column work with carries and borrows.

<details><summary>References</summary>
<ul>
<li><a href="https://proceedings.neurips.cc/paper_files/paper/2022/file/9d5609613524ecf4f15af0f7b31abca4-Paper-Conference.pdf">Chain - of - Thought Prompting Elicits Reasoning</a></li>
<li><a href="https://www.deeplearning.ai/the-batch/schooling-language-models-in-math">GOAT (Good at Arithmetic Tasks), a Method to Boost Large...</a></li>

</ul>
</details>

**Tags**: `#language-models`, `#arithmetic`, `#fine-tuning`, `#benchmarks`, `#small-models`

---

<a id="item-12"></a>
## [Blog defends keeping a big box of cables, sparking HN debate](https://blog.jim-nielsen.com/2026/hands-off-my-cables/) ⭐️ 6.0/10

A blog post by Jim Nielsen titled "Don't let anyone take away your big box of cables" defends the habit of hoarding cables, and it reached the front page of Hacker News with 262 points and 214 comments. Commenters shared practical organization tips, compatibility warnings, and e-waste concerns. The discussion highlights a common tension between digital minimalism and the practical need to keep spare cables, and it surfaces real risks like incompatible modular PSU cables that can destroy hardware. It also connects to the growing e-waste problem, with 62 million tonnes generated globally in 2022 and only 22.3% formally recycled. Commenters noted that grouping cables by type (e.g., USB-C, USB-A) helps deduplicate and reduce clutter, and one user warned that modular PSU cables are not interchangeable across brands despite fitting physically, which can fry hard drives. Another user shared a story of reusing a modified USB cable years later, illustrating the occasional value of hoarding.

hackernews · Brajeshwar · Sep 10, 15:27 · [Discussion](https://news.ycombinator.com/item?id=49645393)

**Background**: Cable hoarding is a common habit among tech enthusiasts who keep spare cables for future repairs or projects. USB cables are generally interchangeable for charging and data, but not all cables support the same power or data speeds, and modular power supply cables have brand-specific pinouts. E-waste is one of the fastest-growing waste streams, with improper disposal releasing hazardous substances like lead.

<details><summary>References</summary>
<ul>
<li><a href="https://www.who.int/news-room/fact-sheets/detail/electronic-waste-(e-waste)">Electronic waste (e-waste) - World Health Organization (WHO)</a></li>
<li><a href="https://superuser.com/questions/115435/are-usb-cables-device-specific">compatibility - Are USB cables device-specific? - Super User</a></li>

</ul>
</details>

**Discussion**: Commenters largely agreed on the value of keeping cables but emphasized grouping them to avoid duplicates. A key warning was about modular PSU cables not being intercompatible, which can cause hardware damage. Others expressed concern about e-waste and sought donation or swap initiatives, while one shared a personal anecdote of reusing a cable years later.

**Tags**: `#hardware`, `#cables`, `#e-waste`, `#organization`, `#hackernews-discussion`

---

<a id="item-13"></a>
## [Free Online Music Theory Textbook Sparks Debate on Classical Bias](https://musictheory.pugetsound.edu/mt21c/MusicTheory.html) ⭐️ 6.0/10

A free online music theory textbook, 'Music Theory for the 21st-Century Classroom,' was shared on Hacker News, where it garnered 137 points and 62 comments. The discussion focused on the textbook's heavy classical music emphasis, its lack of modern genres like jazz and pop, and its pedagogical approach. This resource provides a comprehensive, freely accessible music theory curriculum with assignments, useful for self-learners and educators. The debate highlights broader questions about inclusivity and relevance in music education, especially regarding non-Western and contemporary music. The textbook includes homework and assignments for self-study, and covers topics like serialism, as noted by a commenter. However, critics point out that it requires memorization without context, such as the pattern of whole and half steps in major scales, and largely omits non-Western music traditions.

hackernews · aanet · Sep 10, 17:14 · [Discussion](https://news.ycombinator.com/item?id=49647134)

**Background**: Music theory is the study of the practices and possibilities of music, often focusing on harmony, melody, rhythm, and form. Traditional Western music theory education has historically centered on classical repertoire, but there is growing momentum to include jazz, pop, and global musical traditions. Open textbooks like this aim to reduce costs and increase access for students.

**Discussion**: Commenters praised the resource's usefulness for self-study but criticized its '21st-Century' label as misleading due to its classical focus and lack of modern genres like jazz and pop, as well as non-Western music. Some also noted pedagogical shortcomings, such as presenting facts without context, while one commenter appreciated the inclusion of serialism.

**Tags**: `#music-theory`, `#education`, `#open-textbook`, `#hackernews`, `#pedagogy`

---

<a id="item-14"></a>
## [uv 0.12.13 Adds GraalPy 3.13 Support and Metadata Hash Verification](https://github.com/astral-sh/uv/releases/tag/0.12.13) ⭐️ 4.0/10

Astral's uv 0.12.13, released on 2026-09-10, adds support for GraalPy 3.13.0, verifies hashes when downloading PEP 658 metadata sidecars, and avoids full wheel downloads during resolution by reusing supported hashes from direct URL fragments. It also includes a preview feature that respects ty exclusions when uv check auto-selects virtual workspace members, plus bug fixes for Windows entry-point launchers and JSON index responses. This release strengthens supply-chain security by verifying PEP 658 metadata hashes and speeds up dependency resolution by skipping unnecessary wheel downloads, both meaningful for teams managing large Python environments. GraalPy 3.13 support also broadens uv's compatibility with alternative Python runtimes used in JVM-centric deployments. The hash verification applies specifically to PEP 658 metadata sidecar files, which are fetched separately from wheels; the performance improvement reuses hashes from direct URL fragments only when metadata is available separately. The Windows fix edits entry-point launcher resources in memory to support Nano Server and reduce antivirus contention, and JSON index responses now prefer core-metadata over legacy aliases.

github · astral-automations-bot[bot] · Sep 10, 19:27

**Background**: uv is an extremely fast Python package and project manager written in Rust by Astral, designed as a drop-in replacement for pip, pip-tools, and virtualenv workflows. GraalPy is the GraalVM implementation of Python, a high-performance runtime that runs Python on the JVM. PEP 658 is a Python packaging standard that lets package indexes serve distribution metadata as a separate .metadata sidecar file alongside a wheel, so tools can resolve dependencies without downloading the full wheel.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.astral.sh/uv/">uv is an extremely fast Python package and project manager , written...</a></li>
<li><a href="https://github.com/oracle/graalpython">GitHub - oracle/graalpython: GraalPy – A high-performance...</a></li>
<li><a href="https://peps.python.org/pep-0658/">PEP 658 – Serve Distribution Metadata in the Simple ...</a></li>

</ul>
</details>

**Tags**: `#python`, `#package-manager`, `#uv`, `#release-notes`, `#tooling`

---

<a id="item-15"></a>
## [.blend URL Viewer: Simon Willison's Browser Tool for Blender Files](https://simonwillison.net/2026/Sep/9/blender-viewer/) ⭐️ 4.0/10

Simon Willison released a .blend URL Viewer that loads Blender files directly in the browser from a URL, and demonstrated it with a Pluribus-themed Fabergé egg model generated by GPT-6 Astra in Codex over a 17-minute 51-second run. The image prompt was first produced with the newly launched ChatGPT Images 2.5, then converted into several .blend deliverables now viewable online. The tool lowers the barrier to sharing 3D work by letting anyone preview .blend files in a browser without installing Blender, which matters for AI-assisted 3D workflows where models are increasingly generated rather than hand-built. It also illustrates how frontier models like GPT-6 Astra and image tools like ChatGPT Images 2.5 are being chained together for end-to-end creative pipelines. The viewer reports loading Blender 05.01 and renders a model with 387 meshes, 1099 curves, 783,764 vertices, 1,446,560 triangles, and 17 materials, while noting that its preview shows only approximate materials and omits unapplied modifiers. GitHub-hosted .blend URLs are resolved through jsDelivr, and the viewer offers Fit, Wireframe, and Clear controls.

rss · Simon Willison · Sep 9, 23:58

**Background**: Blender is a free and open-source 3D graphics suite used for modeling, animation, rendering, and visual effects, and its native .blend file format stores scenes, meshes, materials, and other data. Because .blend files normally require Blender to open, browser-based viewers are useful for quick sharing. GPT-6 Astra is OpenAI's frontier model released in September 2026 with strong coding and computer-use abilities, and ChatGPT Images 2.5 is OpenAI's updated image generation and editing model.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Blend_(file_format)">Blend (file format)</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-6_Astra">GPT-6 Astra</a></li>
<li><a href="https://openai.com/index/introducing-chatgpt-images-2-5/">Introducing ChatGPT Images 2 . 5 | OpenAI</a></li>

</ul>
</details>

**Tags**: `#Blender`, `#GPT-6`, `#AI tools`, `#3D modeling`, `#Simon Willison`

---

<a id="item-16"></a>
## [Reddit Users Await ICDE Conference Results](https://www.reddit.com/r/MachineLearning/comments/1wc5zak/icde_results_d/) ⭐️ 3.0/10

A Reddit user posted on r/MachineLearning asking others to share and discuss ICDE conference results expected the next day. The post invites community members to post their acceptance or rejection outcomes in the thread. ICDE is one of the premier conferences in data engineering, so its results directly affect researchers' publication records, career progression, and travel plans. Community threads like this give applicants an informal way to gauge acceptance rates and share experiences before official announcements. The post contains no technical content, paper titles, or review details, and at the time of the summary it had only a low score of 3.0/10. The thread is relevant mainly to authors who submitted papers to ICDE and are waiting for decisions.

reddit · r/MachineLearning · /u/mythrowaway0852 · Sep 10, 02:19

**Background**: ICDE stands for the IEEE International Conference on Data Engineering, one of the premier venues for research in data and information engineering. The 2025 edition is scheduled to take place in Hong Kong from May 19-23, 2025, while the 2024 edition was held in Utrecht, the Netherlands. Authors typically await acceptance notifications before finalizing camera-ready papers and conference travel.

<details><summary>References</summary>
<ul>
<li><a href="https://ieee-icde.org/2025/">IEEE ICDE 2025</a></li>
<li><a href="https://icde2024.github.io/">ICDE 2024 , Utrecht Netherlands</a></li>

</ul>
</details>

**Tags**: `#ICDE`, `#conference`, `#academic-results`, `#machine-learning`, `#community-discussion`

---