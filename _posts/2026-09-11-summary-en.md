---
layout: default
title: "Horizon Summary: 2026-09-11 (EN)"
date: 2026-09-11
lang: en
---

> From 21 items, 19 important content pieces were selected

---

1. [Terry Tao and 25 Fields Medalists Warn of AI Misalignment in Mathematics](#item-1) ⭐️ 9.0/10
2. [trynix.dev runs any Nix package in the browser via qemu-wasm](#item-2) ⭐️ 8.0/10
3. [Training a 210M text-to-image DiT from scratch on one GPU](#item-3) ⭐️ 8.0/10
4. [ACL Proposes Sustainable Reviewing Policy with Submission Caps](#item-4) ⭐️ 8.0/10
5. [Developer finds 60% of Google app ad installs were bots](#item-5) ⭐️ 7.0/10
6. [Rune, a hackable Go-based terminal editor, goes open source](#item-6) ⭐️ 7.0/10
7. [EPA Plans to Scrap Public Review Rules for Data Center Pollution](#item-7) ⭐️ 7.0/10
8. [OpenRouter's automatic provider routing can cause inconsistent model behavior](#item-8) ⭐️ 7.0/10
9. [Simon Willison on Coming to Terms with AI Coding Agents](#item-9) ⭐️ 7.0/10
10. [Datasette 1.0a39 and 0.65.4 security releases fix AI-audited bugs](#item-10) ⭐️ 7.0/10
11. [GrapheneOS releases rewritten Messages app](#item-11) ⭐️ 6.0/10
12. [Anthropic's Boris Cherny: AI-Written Code Needs a Higher Bar](#item-12) ⭐️ 6.0/10
13. [Hugging Face security.txt Redirects AI Agents to CyberGym Benchmark](#item-13) ⭐️ 6.0/10
14. [Python 3.15 Soft-Deprecates re.match() with New re.prefixmatch() Alias](#item-14) ⭐️ 6.0/10
15. [Simon Willison Urges Developers Not to Sleep on Wrapture](#item-15) ⭐️ 6.0/10
16. [PhD student reports TMLR review delays after positive feedback](#item-16) ⭐️ 5.0/10
17. [Reddit user asks how to handle confounding range variable in radar point cloud classification](#item-17) ⭐️ 5.0/10
18. [Reddit user seeks tools to convert codebases into fine-tuning datasets](#item-18) ⭐️ 5.0/10
19. [Graduate Seeks EMNLP Registration Help After Grant Rejections](#item-19) ⭐️ 3.0/10

---

<a id="item-1"></a>
## [Terry Tao and 25 Fields Medalists Warn of AI Misalignment in Mathematics](https://mathandai.org/) ⭐️ 9.0/10

On September 11, 2026, Terence Tao published a declaration titled "A Severe Misalignment of AI in Mathematics" on his blog, signed by 25 Fields Medal winners, arguing that the goals of AI companies and the mathematical community are fundamentally misaligned. The statement followed OpenAI's announcement that its AI had solved one of six open "million-dollar" problems, and OpenAI subsequently withdrew sponsorship of a Caltech math event after criticism from researchers. This is a major intervention by the world's most prominent mathematicians, signaling that the tension between commercial AI labs and scientific communities is escalating beyond mathematics into broader questions of research credit, understanding, and scientific integrity. It could shape how AI companies engage with academia and how mathematical contributions are recognized in an era of AI-generated proofs. The declaration frames the conflict as part of broader alignment issues affecting other scientific and creative professions, noting that AI companies solve math problems primarily to benchmark model strength, which the signatories say is "detrimental to the science of mathematics." The statement was published on Tao's blog and covered by The Economist, which reported that top mathematicians are outraged by OpenAI's methods.

hackernews · meredydd · Sep 11, 17:45 · [Discussion](https://news.ycombinator.com/item?id=49662371)

**Background**: Mathematics has traditionally advanced through rigorous, slow peer review and communal verification, with credit assigned for solving open problems. Recent AI models have begun solving or claiming to solve famous open problems, raising questions about whether AI-generated proofs produce genuine mathematical understanding or merely benchmark results. Terence Tao is a Fields Medalist and one of the most influential living mathematicians, and his blog is widely read across the mathematical community.

<details><summary>References</summary>
<ul>
<li><a href="https://terrytao.wordpress.com/2026/09/11/a-severe-misalignment-of-ai-in-mathematics/">A Severe Misalignment of AI in Mathematics | What's new</a></li>
<li><a href="https://officechai.com/ai/25-fields-medal-winners-including-terence-tao-sign-declaration-saying-rapid-ai-proofs-are-harming-math-in-severe-misalignment/">25 Fields Medal Winners Including Terence Tao Sign ...</a></li>
<li><a href="https://www.economist.com/science-and-technology/2026/09/11/top-mathematicians-are-outraged-by-openais-methods">Top mathematicians are outraged by OpenAI’s methods</a></li>

</ul>
</details>

**Discussion**: Commenters offered diverse perspectives: some compared the situation to Mochizuki's isolated abc conjecture proof, suggesting AI-generated incomprehensible proofs could still spur community activity; others argued AI has destroyed the yardstick of solving open problems for measuring contribution, though the capability genie is out of the bottle. Several drew analogies to 19th-century critiques of photography and 1990s fears that computers would ruin chess, noting chess ultimately grew more popular and stronger.

**Tags**: `#AI`, `#mathematics`, `#misalignment`, `#research`, `#ethics`

---

<a id="item-2"></a>
## [trynix.dev runs any Nix package in the browser via qemu-wasm](https://simonwillison.net/2026/Sep/10/trynix/) ⭐️ 8.0/10

Farid Zakaria launched trynix.dev, which uses a qemu-wasm powered x86_64 Linux virtual machine to boot any Nix package from the past 13 years entirely in the browser. Packages are URL-addressable, so visiting a link like https://trynix.dev/?pkg=python3%403.6.2 and clicking "Load" opens an interactive shell running Python 3.6.2 from 2017. This makes historical and reproducible software environments instantly accessible without servers or local installation, which could change how developers review code, reproduce bugs, and teach software history. It also demonstrates how far WebAssembly-based emulation has come, turning the browser into a portable, zero-setup execution environment. The system relies on ktock/qemu-wasm, which translates QEMU translation blocks into WebAssembly modules and uses browser APIs like WebAssembly.Module and WebAssembly.Instance to execute them. Farid has also built trynix-preview, a GitHub Action that comments a link on a pull request so reviewers can boot the PR's build in the browser with no servers involved.

rss · Simon Willison · Sep 10, 23:44

**Background**: Nix is a purely functional package manager developed in 2003 by Eelco Dolstra that installs each package into a unique, immutable location, giving builds deterministic references to all dependencies and making reproducible builds possible. QEMU is a general-purpose machine emulator, and qemu-wasm is a project that ports it to run inside a browser using WebAssembly, a binary instruction format for safe, sandboxed execution on the web. Together they let a full x86_64 Linux VM and its Nix-provided software run client-side without any backend infrastructure.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ktock/qemu-wasm">GitHub - ktock/qemu-wasm: QEMU on browser · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Nix_(package_manager)">Nix (package manager) - Wikipedia</a></li>
<li><a href="https://reproducible.nixos.org/">NixOS Reproducible Builds</a></li>

</ul>
</details>

**Tags**: `#Nix`, `#WebAssembly`, `#QEMU`, `#Reproducibility`, `#Browser`

---

<a id="item-3"></a>
## [Training a 210M text-to-image DiT from scratch on one GPU](https://www.reddit.com/r/MachineLearning/comments/1wdfmvq/training_a_210m_texttoimage_dit_from_scratch_on/) ⭐️ 8.0/10

A practitioner trained a 210M-parameter text-to-image diffusion transformer from scratch on a single RTX PRO 6000 in 3.5 days using 4.2M images at 256² resolution, and reported three empirical findings: learned null attention slots absorb ~90% of cross-attention mass, flow-matching loss acts as a health rather than quality signal, and a training-time timestep shift outperforms doubling sampling steps. The results offer rare, concrete measurements of diffusion transformer training dynamics that are usually undocumented, giving practitioners on limited hardware a reproducible recipe and diagnostic signals for building text-to-image models without large-scale compute. The model uses a cross-attention DiT (896 width, 16 blocks) with 2D RoPE, QK-norm, SwiGLU, adaLN-single, rectified flow with logit-normal timesteps, and a shift of 2.8 derived from the SD3/RAE rule; training used batch 256, 400k steps, EMA 0.9999, and torch.compile for a 2.4× speedup, with held-out FID improving from 33.7 to 27.0.

reddit · r/MachineLearning · /u/IvanMikhnenkov · Sep 11, 13:00

**Background**: Diffusion transformers (DiTs) replace the U-Net backbone of diffusion models with a transformer, and have powered text-to-image systems like Stable Diffusion 3 and text-to-video models such as Sora. Attention sinks are a known phenomenon where uninformative tokens attract a disproportionate share of attention, while register tokens are learnable tokens added to vision transformers to absorb such storage and improve performance.

<details><summary>References</summary>
<ul>
<li><a href="https://towardsdatascience.com/diffusion-transformer-explained-e603c4770f7e/">Diffusion Transformer Explained | Towards Data Science</a></li>
<li><a href="https://www.emergentmind.com/topics/attention-sinks">Attention Sinks in Transformer Models - emergentmind.com</a></li>
<li><a href="https://huggingface.co/papers/2309.16588">Paper page - Vision Transformers Need Registers</a></li>

</ul>
</details>

**Discussion**: The author asks the community which reward to start with for a next-phase Flow-GRPO run — PickScore/HPSv2, a detector-based object reward, or something verifiable like counting — inviting technical discussion on reinforcement learning fine-tuning of the base model.

**Tags**: `#diffusion-models`, `#text-to-image`, `#training-dynamics`, `#attention-mechanisms`, `#single-gpu`

---

<a id="item-4"></a>
## [ACL Proposes Sustainable Reviewing Policy with Submission Caps](https://www.reddit.com/r/MachineLearning/comments/1wd7b83/acl_sustainable_reviewing_policy_d/) ⭐️ 8.0/10

ACL announced a new "Sustainable Reviewing Policy" for its ARR (ACL Rolling Review) system, capping total submissions at 20 per author and first-author submissions at 5 per cycle, while requiring each submission to "pay" for itself by providing a qualified reviewer or chair. Submissions without a qualified service contributor will enter a lottery for remaining review capacity, and a mentorship system will be built for those not yet qualified. This is a significant policy shift for ACL, one of the top NLP conferences, as it directly addresses the unsustainable growth in paper submissions that has strained the peer-review system. If successful, it could reshape academic publishing norms by tying submission privileges to reviewing contributions, potentially influencing other conferences and fields. The policy allows non-author designated contributors to be nominated, but they must vouch for the work in an arXiv-endorsement style, and measures against system abuse (e.g., accounts systematically submitting or endorsing low-quality work) will be implemented, with penalties including bans. The caps of 20 total and 5 first-author submissions per cycle are considered generous by some community members.

reddit · r/MachineLearning · /u/S4M22 · Sep 11, 05:38

**Background**: ACL Rolling Review (ARR) is a peer-review platform for the Association for Computational Linguistics that runs in two-month cycles, where authors submit papers and receive reviews before choosing a publication venue. In recent years, submission numbers to ACL conferences have grown rapidly, overwhelming the volunteer reviewer pool and prompting discussions about sustainability. Starting in April 2024, ARR already required at least one author per submission to volunteer as a reviewer, but this new proposal goes further by capping submissions and enforcing a stricter service requirement.

<details><summary>References</summary>
<ul>
<li><a href="https://aclrollingreview.org/incentives2025">Changes to reviewer volunteering requirement and incentives in May 2025 cycle (EMNLP 2025) – ACL Rolling Review – A peer review platform for the Association for Computational Linguistics</a></li>
<li><a href="https://aclrollingreview.org/dates">Dates and Venues – ACL Rolling Review – A peer review platform for the Association for Computational Linguistics</a></li>
<li><a href="https://aclrollingreview.org/">ACL Rolling Review – A peer review platform for the ...</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion generally supports the policy, with the original poster calling it "highly required" despite being a form of gatekeeping, and noting that the caps are still generous. Some commenters likely raise concerns about fairness and potential exclusion of researchers from less-resourced institutions, but the overall sentiment leans toward seeing it as a necessary step to sustain the review process.

**Tags**: `#ACL`, `#peer-review`, `#academic-publishing`, `#NLP`, `#conference-policy`

---

<a id="item-5"></a>
## [Developer finds 60% of Google app ad installs were bots](https://dayzlegame.com/blog/google-ads-bot-farm/) ⭐️ 7.0/10

A developer spent $220 on Google app ads and found that roughly 60% of the resulting installs came from bots, according to a detailed blog post that sparked a 223-point Hacker News discussion with 116 comments. The experiment provides concrete, data-backed evidence of ad fraud on Google's mobile advertising platform. Ad fraud directly drains marketing budgets and distorts campaign analytics for app developers, who often have limited resources to detect and fight it. The case adds to growing scrutiny of Google's ad platform, especially after Google and Integral Ad Science shut down large Android ad fraud operations in 2025 and 2026. The developer's $220 spend and 60% bot-install rate are the core figures, and commenters noted that bot networks typically run from data centers rather than residential IPs, making them blockable via Google Ads' IP Exclusions setting. One commenter reported maintaining an exclusion list of over 4,000 networks in the US alone after years of running Google Ads.

hackernews · nickabe · Sep 11, 18:24 · [Discussion](https://news.ycombinator.com/item?id=49662990)

**Background**: Ad fraud refers to invalid traffic generated by automated programs that fake impressions, clicks, installs, or conversions to siphon ad revenue. Mobile ad fraud techniques include bot farms, device emulators, click injection, and install hijacking, and detection often relies on metrics like click-to-install time (CTIT) and anomaly detection. Google Play prohibits ad fraud as a form of invalid traffic, and Google Ads offers tools such as IP exclusions to help advertisers filter suspicious traffic.

<details><summary>References</summary>
<ul>
<li><a href="https://www.adweek.com/media/google-pulled-200-apps-android-ad-fraud/">Google Has Pulled Nearly 200 Apps Due to Extensive Android Ad ... EXCLUSIVE: Google Pulls 115 Android Apps Tied to Ad Fraud ... Google Ads Bot Traffic: Detect and Block Fake Clicks Ad Fraud - Play Console Help Google Ads Bots & Spam: How to Stop It & Why It Happens Bot Advertising: How Bots Hijack Ad Spend - anura.io Invalid activity - Google Ad Traffic Quality</a></li>
<li><a href="https://www.appsflyer.com/blog/measurement-analytics/mobile-ad-fraud-for-marketers/">Mobile ad fraud: The marketer’s field guide | AppsFlyer</a></li>
<li><a href="https://www.humansecurity.com/learn/topics/what-is-mobile-ad-fraud/">What is Mobile Ad Fraud? Here’s How To Stop Mobile Ad Fraud</a></li>

</ul>
</details>

**Discussion**: Commenters were largely skeptical of Google's commitment to fighting fraud, with one calling Google Ads and Meta ads 'a con' and another arguing Google is very capable of detecting fraud but turns a blind eye. A widely shared cautionary tale described a developer whose AdMob account was banned for invalid traffic after buying Google Ads to promote an app with AdMob integration. Others offered practical mitigation advice, such as excluding data center IP ranges via Google Ads' IP Exclusions, and one commenter praised the app's clean interface after installing it.

**Tags**: `#ad-fraud`, `#google-ads`, `#mobile-apps`, `#bot-detection`, `#advertising`

---

<a id="item-6"></a>
## [Rune, a hackable Go-based terminal editor, goes open source](https://rune.build/blog/rune-is-now-open-source) ⭐️ 7.0/10

Rune, a hackable cross-platform terminal editor written in Go, has been open-sourced, as announced on its official blog. The release has sparked discussion on Hacker News about its architecture, contributor incentives, and networking model. Open-sourcing a hackable Go-based editor gives developers a new, extensible tool for terminal-based workflows across Windows, macOS, and Linux. It also tests a novel revenue-sharing contributor model that could influence how future open-source projects attract and reward contributors. Rune is built in Go and targets cross-platform terminal use, with a networking model that relies on a coordination server and encryption for multi-machine workflows. The project offers participating contributors a contractual right to share in revenue generated by Rune, directly or indirectly.

hackernews · ernestrc · Sep 11, 15:31 · [Discussion](https://news.ycombinator.com/item?id=49660149)

**Background**: Terminal editors are text editors that run inside a command-line interface, often favored by developers for speed and remote work over SSH. Go is a statically typed, compiled language known for producing single static binaries that run across operating systems, making it a popular choice for cross-platform CLI tools. Rune aims to be 'hackable,' meaning users can modify and extend its behavior, similar to editors like Vim or Emacs.

**Discussion**: Commenters praised the ease of building cross-platform terminal apps and the smooth onboarding from Vim, though one user hit a conflict with fish shell's vim bindings. A major debate centered on the revenue-sharing contributor model, with one commenter calling it a 'terrible idea' that could incentivize low-quality PR spam, while another expressed concern about trusting Rune's coordination server and suggested running over Tailscale instead.

**Tags**: `#open-source`, `#developer-tools`, `#terminal`, `#go`, `#editors`

---

<a id="item-7"></a>
## [EPA Plans to Scrap Public Review Rules for Data Center Pollution](https://capitalbnews.org/data-centers-permit-rules-epa/) ⭐️ 7.0/10

The EPA plans to eliminate a federal requirement that states notify the public and allow public comment before approving air-pollution permits for industrial facilities, including the data centers being built across the country and the power plants that supply them. This proposal is part of a broader effort to streamline the New Source Review (NSR) permitting process for minor sources by removing minimum federal public participation requirements. This rollback could significantly weaken public oversight of pollution from data centers and their power plants, which are rapidly expanding due to AI and cloud computing demand. It may lead to increased emissions and public health risks in surrounding communities, while also reducing the ability of local residents to challenge permits. The rule specifically targets minor sources under the New Source Review program, eliminating the minimum federal regulatory requirements for public participation. It would affect air permits for data centers and the power plants built to feed their electricity demand, though states could still choose to maintain their own public review processes.

hackernews · doener · Sep 11, 18:05 · [Discussion](https://news.ycombinator.com/item?id=49662672)

**Background**: The EPA's New Source Review program requires industrial facilities to obtain permits before construction or major modification, and historically included public notice and comment periods. Data centers consume enormous amounts of electricity and often rely on fossil-fuel power plants, making their air pollution permits a key environmental concern. The proposed change aligns with a broader deregulatory agenda that critics say undermines the EPA's mission to protect human health and the environment.

<details><summary>References</summary>
<ul>
<li><a href="https://www.epa.gov/newsreleases/epa-proposes-streamline-state-and-local-permitting-process-minor-sources">EPA Proposes to Streamline State and Local Permitting Process ...</a></li>
<li><a href="https://truthout.org/articles/the-epa-is-planning-to-scrap-public-review-rules-for-data-center-pollution/">The EPA Is Planning to Scrap Public Review Rules for Data ...</a></li>
<li><a href="https://www.epa.gov/stationary-sources-air-pollution/clean-air-act-resources-data-centers">Clean Air Act Resources for Data Centers - US EPA</a></li>

</ul>
</details>

**Discussion**: Commenters largely condemned the move, viewing it as part of a broader gutting of the EPA and a sign that communities opposing data centers were justified. Some noted that such deregulatory changes may only last as long as the current administration, making long-term business planning uncertain.

**Tags**: `#EPA`, `#data centers`, `#environmental policy`, `#regulation`, `#public health`

---

<a id="item-8"></a>
## [OpenRouter's automatic provider routing can cause inconsistent model behavior](https://simonwillison.net/2026/Sep/11/so-you-want-to-use-openrouter/) ⭐️ 7.0/10

Mohamed Moustafa, highlighted by Simon Willison, warns that OpenRouter's automatic provider routing can make the same model endpoint behave inconsistently, because different backend providers run different serving software, optimizations, and settings. He notes that some providers even lack vision capability for vision models, and that the reasoning effort option may be processed differently, with the workaround being to pin a provider via the provider.only option. This matters because developers who rely on OpenRouter for a single unified API may unknowingly get different quality, latency, or even missing capabilities depending on which backend serves each request, undermining reproducibility and production reliability. It highlights a broader trade-off in multi-provider LLM gateways between convenience and consistent behavior. The concrete mitigation is to use the provider.only routing option to restrict requests to specific providers, and the /endpoints method returns the list of available providers for a given model ID. OpenRouter's own documentation notes that it makes a best effort to route to providers supporting tool use or a requested max_tokens, but these are best-effort rather than guarantees.

rss · Simon Willison · Sep 11, 22:49

**Background**: OpenRouter is a gateway service that lets developers call many different LLMs through a single API endpoint, automatically handling fallbacks and picking cost-effective backends across 70+ providers. Because each provider may run its own inference stack with different quantization, serving software, and feature support, the same nominal model can behave differently depending on where it is hosted. The provider.only and /endpoints features exist to give developers explicit control over this routing.

<details><summary>References</summary>
<ul>
<li><a href="https://openrouter.ai/docs/guides/routing/provider-selection">Provider Routing - Smart Multi-Provider Request ... - OpenRouter</a></li>
<li><a href="https://openrouter.ai/blog/insights/model-routing/">How OpenRouter Model Routing Works: Providers, Fallbacks ...</a></li>
<li><a href="https://simonwillison.net/2026/Sep/11/so-you-want-to-use-openrouter/">So you want to use OpenRouter? - simonwillison.net</a></li>

</ul>
</details>

**Tags**: `#OpenRouter`, `#LLM APIs`, `#provider routing`, `#AI infrastructure`, `#developer tooling`

---

<a id="item-9"></a>
## [Simon Willison on Coming to Terms with AI Coding Agents](https://simonwillison.net/2026/Sep/11/feeling-sad-about-ai/) ⭐️ 7.0/10

Simon Willison published a blog post reflecting on his Hacker News comment about the existential crisis software engineers feel when AI coding agents complete in an hour work that used to take a week. He argues that once engineers accept that translating an exact specification into decent code is no longer a unique skill, they can focus on larger problems where their experience gives them an edge over newcomers relying purely on agents. This perspective matters because AI coding agents are rapidly changing what software engineering work looks like, and many developers are grappling with anxiety about their professional relevance. Willison's argument that experienced engineers can leverage their depth to master new tools and deliver greater value offers a constructive counterpoint to the fear of automation. Willison notes that the initial reaction to an agent doing a week's work in an hour is disheartenment, but that coming to terms with this shift opens up larger opportunities. He also points out that software engineering has never had stable tools and languages beyond roughly a five-year horizon, so frequent radical change is nothing new for those who chose it as a passion.

rss · Simon Willison · Sep 11, 17:28

**Background**: AI coding agents are tools that use large language models to autonomously write, modify, debug, and refactor code, handling multi-file context and multi-step tasks rather than just completing single lines. Simon Willison is a British programmer known for co-creating the Django web framework and for his widely read blog on AI and software development. His post responds to a Hacker News discussion titled 'Feeling sad about AI,' where developers shared their anxieties about automation.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_coding_agent">AI coding agent</a></li>
<li><a href="https://en.wikipedia.org/wiki/Simon_Willison">Simon Willison</a></li>

</ul>
</details>

**Discussion**: The linked Hacker News discussion likely contains diverse viewpoints on the emotional and professional impact of AI coding agents, with some developers agreeing that adaptation is possible and others expressing concern about the pace of change. Willison's comment frames the conversation around acceptance and opportunity rather than resistance.

**Tags**: `#AI`, `#software engineering`, `#career`, `#existential crisis`, `#Hacker News`

---

<a id="item-10"></a>
## [Datasette 1.0a39 and 0.65.4 security releases fix AI-audited bugs](https://simonwillison.net/2026/Sep/11/datasette-security/) ⭐️ 7.0/10

Datasette released two security patch versions, 1.0a39 for the alpha series and 0.65.4 for the stable 0.65.x family, fixing subtle bugs found during an extensive audit conducted with Claude Fable 5.1, GPT-5.6, and GPT-6 Astra. The audit followed issues reported by Sevban Dönmez, and Simon Willison and Alex Garcia spent nearly a week collaborating on and reviewing the fixes. Anyone running a public Datasette instance, especially one that mixes public and private tables, should apply these patches promptly because the bugs could expose data that was meant to stay private. The release also signals that AI-assisted security audits by frontier models are becoming a standard part of open-source maintenance workflows. The fixes address very subtle bugs that were surfaced by multiple frontier models rather than a single tool, and the maintainers deliberately split the work so that one person wrote automated tests reproducing each issue while the other implemented the fix, ensuring two humans reviewed every change. Willison stated that security audits by frontier models will be incorporated into all future Datasette development work.

rss · Simon Willison · Sep 11, 03:27

**Background**: Datasette is an open-source tool for exploring, browsing, and publishing data, commonly used to expose SQLite databases as browsable and queryable web interfaces. Because a single instance can contain both public and private tables, access-control bugs are especially dangerous: a flaw in permission checks could let anonymous visitors read data that was intended to be restricted. Claude Fable 5.1 is a general-use model from Anthropic's Mythos-class family, released in September 2026 with safeguards that route flagged cybersecurity requests to a less capable model.

<details><summary>References</summary>
<ul>
<li><a href="https://selfhostedworld.com/software/datasette">Datasette - Self-hosted software</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Fable_5">Claude Fable 5</a></li>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#security`, `#open-source`, `#ai-assisted-audit`, `#release`

---

<a id="item-11"></a>
## [GrapheneOS releases rewritten Messages app](https://github.com/GrapheneOS/Messaging/releases/tag/13) ⭐️ 6.0/10

GrapheneOS has released a rewritten version of its Messages app, tagged as release 13 on its GitHub repository. The release has sparked community discussion about its features, installation process, and its place within the broader GrapheneOS ecosystem. For privacy-focused GrapheneOS users, the default messaging app is a core part of daily communication, so a rewritten version signals continued investment in the platform's first-party app suite. It also reflects GrapheneOS's broader push to offer hardened, privacy-respecting alternatives to standard Android apps. The release is published as tag 13 on the GrapheneOS/Messaging GitHub repository, though the provided content does not detail specific new features. Community members have asked for screenshots and clarification on whether it can be installed immediately or will arrive in the next OS release.

hackernews · microtonal · Sep 11, 18:50 · [Discussion](https://news.ycombinator.com/item?id=49663373)

**Background**: GrapheneOS is an open-source, privacy- and security-focused mobile operating system built on the Android Open Source Project (AOSP), first released in 2016 and officially supported on Google Pixel devices. It hardens low-level system components and improves app sandboxing and permission controls, and as of April 2026 had roughly 400,000 active users. The project also announced a partnership with Motorola in 2026 to certify selected Motorola devices.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GrapheneOS">GrapheneOS - Wikipedia</a></li>
<li><a href="https://grapheneos.org/">GrapheneOS: the private and secure mobile OS</a></li>

</ul>
</details>

**Discussion**: Commenters expressed a mix of interest and frustration: some asked for screenshots and installation details, one wished the call app had been prioritized over Messages due to poor UI/UX, and another lamented the lack of an official Fairphone-GrapheneOS partnership. A user in a region where SMS is mainly used for two-factor authentication said a bare-bones AOSP messaging app was never a problem for them but planned to try the new GrapheneOS app anyway.

**Tags**: `#GrapheneOS`, `#privacy`, `#Android`, `#messaging`, `#open-source`

---

<a id="item-12"></a>
## [Anthropic's Boris Cherny: AI-Written Code Needs a Higher Bar](https://simonwillison.net/2026/Sep/11/boris-cherny/) ⭐️ 6.0/10

Boris Cherny, an engineer at Anthropic, argued in a post on X that production code written by Claude should be held to a higher standard than human-written code. He described the extensive guardrails Anthropic uses to enforce this, including numerous lint rules, extensive tests, Claude-driven end-to-end tests, Claude-powered fuzzers running daily, automated code and security reviews, and automated refactoring. As AI coding agents like Claude become more widely used in production environments, this perspective highlights a key practice for teams adopting AI-assisted development: compensating for the unpredictability of generated code with stronger automated verification. It signals that rigorous engineering discipline, rather than blind trust, is what makes AI-generated code safe to ship. Cherny specifically mentions Claude-driven end-to-end tests, Claude-powered fuzzers running daily, and automated code and security reviews as part of Anthropic's guardrails. He warns that without such measures, teams can end up with a codebase that is a mess and hard to maintain down the line.

rss · Simon Willison · Sep 11, 17:47

**Background**: Fuzzing is an automated testing technique that feeds invalid, unexpected, or random inputs into a program to uncover crashes and security vulnerabilities. Lint rules are static-analysis checks that flag style issues, potential bugs, and risky patterns before code runs. Automated code review tools, increasingly AI-powered, inspect code for defects and security problems within CI/CD pipelines. Cherny's argument is that these layers of automated verification matter even more for AI-generated code, since it can be produced far faster than humans can manually review it.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Fuzzing">Fuzzing - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Automated_code_review">Automated code review</a></li>
<li><a href="https://github.com/resources/articles/what-is-fuzz-testing">What is fuzzing and fuzz testing? - GitHub</a></li>

</ul>
</details>

**Tags**: `#AI`, `#software engineering`, `#code quality`, `#Claude`, `#coding agents`

---

<a id="item-13"></a>
## [Hugging Face security.txt Redirects AI Agents to CyberGym Benchmark](https://simonwillison.net/2026/Sep/11/hugging-face-security/) ⭐️ 6.0/10

Hugging Face's security.txt file now includes a humorous note telling AI agents instructed to find vulnerabilities to instead try the publicly available CyberGym benchmark on GitHub, and to upload their model weights to Hugging Face afterward. This reflects an emerging trend where AI agents are increasingly used for automated security research, and it shows how organizations are adapting standard security disclosure channels to communicate with autonomous agents rather than just human researchers. The note is written as comments in the security.txt file, which is a machine-readable standard located at /.well-known/security.txt for defining vulnerability disclosure policies; the CyberGym benchmark, built by Berkeley RDI and collaborators, evaluates AI agents on real-world vulnerability discovery, reproduction, and exploit or patch development.

rss · Simon Willison · Sep 11, 16:04

**Background**: security.txt is a proposed standard, similar to robots.txt but for security issues, that lets websites define how security researchers should report vulnerabilities. CyberGym is a benchmark that measures how well AI agents handle real-world cybersecurity tasks in a controlled environment. Hugging Face is a major platform for hosting and sharing AI models and their weights.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Security.txt">security.txt - Wikipedia</a></li>
<li><a href="https://securitytxt.org/">security.txt: Proposed standard for defining security policies</a></li>
<li><a href="https://www.cybergym.io/">Frontier AI Cybersecurity Observatory</a></li>

</ul>
</details>

**Discussion**: The item received moderate discussion on Hacker News, with commenters appreciating the clever and humorous approach to handling AI agents probing for vulnerabilities, though it was not treated as a major technical breakthrough.

**Tags**: `#ai-security`, `#security.txt`, `#hugging-face`, `#ai-agents`, `#cybersecurity`

---

<a id="item-14"></a>
## [Python 3.15 Soft-Deprecates re.match() with New re.prefixmatch() Alias](https://simonwillison.net/2026/Sep/11/soft-deprecating-re-match/) ⭐️ 6.0/10

Python 3.15, due in October 2026, soft-deprecates the long-standing re.match() function and introduces re.prefixmatch() as an exact synonym, as described by release manager Hugo van Kemenade. The new name makes clear that the function anchors only at the start of a string, not the end. re.match() is one of the most commonly misused functions in Python's standard library, so giving it a self-explanatory alias reduces a frequent source of bugs for both beginners and experienced developers. Because it is only a soft deprecation, existing code keeps working, making the change low-risk while nudging new code toward clearer alternatives. re.prefixmatch() and re.Pattern.prefixmatch() are exact synonyms for re.match() and re.Pattern.match(), with identical behavior, and the old names remain documented and tested with no scheduled removal. For most use cases the documentation recommends re.search() to match anywhere in a string or re.fullmatch() to match the entire string.

rss · Simon Willison · Sep 11, 14:47

**Background**: Python's PEP 387 defines "soft deprecation" as marking an API as no longer recommended for new code without any promise or threat to remove it, so the API stays documented and tested but receives no further development. re.match() has long confused users because it anchors at the beginning of the string but not the end, unlike re.fullmatch(), which requires the whole string to match. Python 3.15 is expected in October 2026, and the change was proposed and explained by release manager Hugo van Kemenade.

<details><summary>References</summary>
<ul>
<li><a href="https://peps.python.org/pep-0387/">PEP 387 – Backwards Compatibility Policy | peps.python.org</a></li>
<li><a href="https://adamj.eu/tech/2026/08/16/python-prefer-prefixmatch-to-match/">Python: use re.prefixmatch () instead of re.match () from ...</a></li>
<li><a href="https://stackoverflow.com/questions/58774029/differences-between-re-match-re-search-re-fullmatch">python - Differences between re . match , re . search , re . fullmatch</a></li>

</ul>
</details>

**Discussion**: The item was surfaced via Lobste.rs, where the discussion added community validation for the change, though the overall reaction treated it as a modest, sensible clarity improvement rather than a major shift.

**Tags**: `#python`, `#regex`, `#api-design`, `#deprecation`, `#standard-library`

---

<a id="item-15"></a>
## [Simon Willison Urges Developers Not to Sleep on Wrapture](https://simonwillison.net/2026/Sep/11/wrapture/) ⭐️ 6.0/10

Simon Willison published a blog post on September 11, 2026, highlighting wrapture, a new Python monkey patching library by Graham Dumpleton that was initially released on August 31, 2026. Dumpleton has since published nearly daily tutorials covering unit testing, call recording, phased behavior, live tracing, zero-code TOML-based tracing, Flask instrumentation, slow-code detection, and OpenTelemetry export. Wrapture unifies testing and observability use cases that Python developers typically handle with separate tools like unittest.mock and New Relic-style tracing agents, potentially reducing the need for multiple dependencies. Its zero-code TOML configuration and broad instrumentation package covering frameworks such as Django, FastAPI, Flask, SQLAlchemy, and httpx could make it a versatile Swiss Army Knife for debugging and monitoring production systems. Wrapture is still alpha software (version 1.0.0a11 in the documentation) but is already usable, and it can be tried without modifying any Python code by configuring tracing in a separate TOML file. A companion package, wrapture-instrumentation, provides instrumentation for aiohttp, Django, FastAPI, Flask, gRPC, httpx, Jinja2, requests, SQLAlchemy, sqlite3, Starlette, urllib3, Uvicorn, and more, while interactive JupyterLab workshops are also available.

rss · Simon Willison · Sep 11, 13:51

**Background**: Monkey patching is a technique in dynamic languages like Python where a class, module, or function's behavior is modified at runtime without altering the original source code, commonly used in testing to replace real implementations with mocks. Graham Dumpleton is a well-known Python developer, best known as the creator of mod_wsgi, and wrapture is his new library that applies monkey patching to both testing and observability. Observability tools typically trace how a live application executes, similar to commercial products like New Relic, and wrapture aims to bring that capability into the same patching framework used for tests.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/sep/11/wrapture/">Don't sleep on wrapture | Simon Willison’s Weblog</a></li>
<li><a href="https://wrapture.readthedocs.io/en/latest/getting-started.html">Getting started — wrapture 1.0.0a11 documentation</a></li>
<li><a href="https://github.com/GrahamDumpleton/wrapture">GitHub - GrahamDumpleton/wrapture: Monkey patch, test, and ...</a></li>

</ul>
</details>

**Tags**: `#Python`, `#monkey-patching`, `#testing`, `#observability`, `#developer-tools`

---

<a id="item-16"></a>
## [PhD student reports TMLR review delays after positive feedback](https://www.reddit.com/r/MachineLearning/comments/1wd5mki/why_is_tmlr_so_slow_in_recent_times_d/) ⭐️ 5.0/10

A final-year PhD student posted on Reddit that their solo-authored TMLR submission received timely and positive reviews with minor revisions, but after submitting the revised version, the reviewers went silent for over two months. Despite reminders to the Action Editor and Editor-in-Chief, the status remains unchanged, causing frustration as postdoc application deadlines approach. This highlights a growing concern about the reliability of TMLR's review timeline, which is a key reason authors choose it over conferences. Delays can directly impact early-career researchers' job applications and career progression, potentially undermining trust in the journal. The student submitted a solo-authored paper, received positive reviews with minor revisions, and after resubmission, only one reviewer acknowledged that concerns were addressed. Over two months passed with no further updates, and reminders to the Action Editor and Editor-in-Chief did not change the status.

reddit · r/MachineLearning · /u/Fantastic-Nerve-4056 · Sep 11, 04:09

**Background**: TMLR (Transactions on Machine Learning Research) is a peer-reviewed journal launched in 2022 that emphasizes correctness and reproducibility over novelty, and offers a faster review process than traditional journals. It uses an open review model where reviewers and authors interact, and an Action Editor oversees each submission. Many researchers, especially students, value TMLR for its timely reviews and the credibility it adds to their CVs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/laurent-charlin-5aaa941_thrilled-to-join-tmlr-as-an-editor-in-chief-activity-7414008875080761345-sGSK">Thrilled to join TMLR as an Editor - in - Chief ! It's a wonderful recognition.....</a></li>

</ul>
</details>

**Tags**: `#machine-learning`, `#peer-review`, `#tmlr`, `#academia`, `#publishing`

---

<a id="item-17"></a>
## [Reddit user asks how to handle confounding range variable in radar point cloud classification](https://www.reddit.com/r/MachineLearning/comments/1wdpat4/how_to_handle_cofound_variables_d/) ⭐️ 5.0/10

A Reddit user on r/MachineLearning posted a question about a confounding variable in automotive radar point cloud object classification: adding range as a feature improved F1 scores across all K validation sets and the final test set, but the user worries the model is learning spurious correlations (e.g., larger range means larger object) rather than true class distributions. This is a common and important problem in applied machine learning, especially for sensor-based perception tasks like radar point cloud classification, where physical artifacts (e.g., fewer points at longer range) can create shortcuts that inflate validation performance but fail in deployment. The user notes there is no classical overfitting, yet the improvement may come from the model exploiting the radar artifact that farther objects return fewer points, and asks whether to stress-test by splitting data so range distributions differ, or to drop the feature and accept lower performance.

reddit · r/MachineLearning · /u/Huge-Leek844 · Sep 11, 18:57

**Background**: A confounding variable influences both the input features and the target label, potentially creating spurious associations that do not reflect true causation. In automotive radar point clouds, the number of returned points decreases with distance, so range can correlate with object size or class, making it a potential confounder. Practitioners often use randomization, data splitting, or causal inference methods to detect and control for such confounders.

<details><summary>References</summary>
<ul>
<li><a href="https://machinelearningmastery.com/confounding-variables-in-machine-learning/">The Role of Randomization to Address Confounding Variables in ... Confounding variables in machine learning predictions? Confounders: machine learning’s blindspot - causaLens Confounder Features & Machine Learning Models: Examples Controlling for effects of confounding variables on machine ... Confounding Variable — Machine Learning — DATA SCIENCE</a></li>
<li><a href="https://stats.stackexchange.com/questions/271694/confounding-variables-in-machine-learning-predictions">Confounding variables in machine learning predictions?</a></li>
<li><a href="https://arxiv.org/pdf/2402.12715">The Clever Hans Mirage: A Comprehensive Survey on Spurious ...</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#confounding variables`, `#radar point clouds`, `#object classification`, `#model evaluation`

---

<a id="item-18"></a>
## [Reddit user seeks tools to convert codebases into fine-tuning datasets](https://www.reddit.com/r/MachineLearning/comments/1wd5zkk/any_tools_to_turn_a_codebase_into_a_fine_tuning/) ⭐️ 5.0/10

A Reddit user on r/MachineLearning asked whether any tools or workflows exist to turn existing codebases, such as React/Next.js projects or static HTML sites, into instruction-style fine-tuning datasets for code generation models. They also raised practical questions about preserving context across components and files, incorporating screenshots alongside code, and generating useful instructions rather than generic descriptions. As more developers fine-tune code LLMs on their own repositories, the lack of standardized tooling for turning real-world codebases into high-quality instruction datasets is a growing bottleneck. Solving this could democratize custom code model training and enable better benchmarking of new architectures that aim to improve quality and speed while using less VRAM. The user specifically wants an instruction/prompt-to-code format suitable for instruct, thinking, or diffusion coding models, and is also building a separate model architecture to improve quality and speed with lower VRAM usage, making a solid dataset and benchmark essential. Existing tools like easy-dataset focus on converting domain documents into structured datasets, but no widely known tool directly targets full codebase-to-instruction-dataset conversion.

reddit · r/MachineLearning · /u/ImBadGuyInEveryStory · Sep 11, 04:27

**Background**: Fine-tuning adapts a pre-trained model to a specific domain or task by training it further on a smaller, targeted dataset. For code generation models, instruction tuning uses paired prompts and code outputs so the model learns to follow natural-language requests. Building such datasets from an existing codebase is non-trivial because it requires extracting meaningful units of code, generating accurate natural-language instructions, and preserving cross-file context that real projects depend on.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ConardLi/easy-dataset">GitHub - ConardLi/easy-dataset: A powerful tool for creating ...</a></li>
<li><a href="https://www.ibm.com/think/topics/instruction-tuning">What Is Instruction Tuning ? | IBM</a></li>
<li><a href="https://arxiv.org/pdf/2408.08343">API-guided Dataset Synthesis to Finetune Large Code Models</a></li>

</ul>
</details>

**Tags**: `#fine-tuning`, `#dataset-creation`, `#code-generation`, `#machine-learning`, `#developer-tools`

---

<a id="item-19"></a>
## [Graduate Seeks EMNLP Registration Help After Grant Rejections](https://www.reddit.com/r/MachineLearning/comments/1wdw5o0/confusion_regarding_emnlp_registration_d/) ⭐️ 3.0/10

A recent graduate posted on r/MachineLearning asking for advice on EMNLP registration fees after being rejected for travel grants from both their former undergraduate institution in India and their current Master's university. Their first-author paper was accepted to EMNLP Findings, but they cannot afford the registration and author fees despite having a small emergency fund for travel and lodging. This highlights a common funding gap for early-career researchers, especially those transitioning between institutions, and raises questions about whether co-authors can share registration costs or whether presenting a Findings paper requires separate fees. It affects students and independent researchers who lack institutional travel support. The user has ACL member registration and asks whether they must pay the $350 student registration fee if a co-author already registers, and whether presenting a Findings paper requires separate payment. They have already been rejected twice for D&I grants and have exhausted most funding options.

reddit · r/MachineLearning · /u/Batman_beyond123 · Sep 11, 23:24

**Background**: EMNLP (Empirical Methods in Natural Language Processing) is a major NLP conference organized by ACL's SIGDAT, started in 1996. The Findings track publishes papers that are scientifically sound but not accepted to the main conference; Findings papers are not required to be presented. Conference registration fees and travel grants are typically handled by institutions, but eligibility often depends on current affiliation and student status.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Empirical_Methods_in_Natural_Language_Processing">Empirical Methods in Natural Language Processing - Wikipedia</a></li>
<li><a href="https://aclanthology.org/2025.findings-emnlp.0.pdf">Findings of the Association for Computational Linguistics ...</a></li>

</ul>
</details>

**Tags**: `#academic-conference`, `#EMNLP`, `#registration`, `#funding`, `#student-issues`

---