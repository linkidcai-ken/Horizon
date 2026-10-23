---
layout: default
title: "Horizon Summary: 2026-10-23 (EN)"
date: 2026-10-23
lang: en
---

> From 27 items, 24 important content pieces were selected

---

1. [Quad9 to Exit France After Court Fines It for Non-Compliance with Web-Blocking Orders](#item-1) ⭐️ 8.0/10
2. [NVIDIA OpenShell: Secure Runtime for Autonomous AI Agents](#item-2) ⭐️ 8.0/10
3. [HackiOS project runs full iOS 16.5 firmware on Android phones via QEMU](#item-3) ⭐️ 8.0/10
4. [Switch 2 Jailbreak Uses JetKVM, LLM Automation, and Bluetooth Switch](#item-4) ⭐️ 8.0/10
5. [eMudhra to exit global SSL/TLS certificate business after misissuance incident](#item-5) ⭐️ 8.0/10
6. [Faster than earcut: triangulating 3.7M map polygons in 489 ms](#item-6) ⭐️ 8.0/10
7. [Anthropic Donates Agent Skills Standard to Agentic AI Foundation](#item-7) ⭐️ 8.0/10
8. [Carbon-X: Open 14.8B model trained jointly on DNA and text](#item-8) ⭐️ 8.0/10
9. [Woman faces six years for Cash App account she never opened](#item-9) ⭐️ 7.0/10
10. [GNU Taler prepares for operational launch in Germany](#item-10) ⭐️ 7.0/10
11. [High Schooler's 100k-Line 3D Open-World Game Hedra Goes Viral](#item-11) ⭐️ 7.0/10
12. [arXiv Paper Argues AI Is Enclosing the Scientific Commons](#item-12) ⭐️ 7.0/10
13. [Developer apologizes for unknowingly breaking PHP RCE embargo](#item-13) ⭐️ 7.0/10
14. [Open-XTTS-Trainer enables full XTTS v2 training and new-language tokenizer extension](#item-14) ⭐️ 7.0/10
15. [WhissleAI shrinks steerable TTS to 11.84 MB with int4 quantization](#item-15) ⭐️ 7.0/10
16. [Frontier audio models struggle to label ASMR sound events, benchmark shows](#item-16) ⭐️ 7.0/10
17. [Xbox to charge 24-40 cents per hour for streaming owned games](#item-17) ⭐️ 6.0/10
18. [Blog post claims all AI models share a controversial take on human nature, but commenters debunk methodology](#item-18) ⭐️ 5.0/10
19. [Reddit user steers Qwen2.5-1.5B-Instruct toward 'evil' persona, eliciting slurs](#item-19) ⭐️ 5.0/10
20. [uv 0.13.5 Updates Managed CPython Builds and Removes Compromised Certificate Root](#item-20) ⭐️ 4.0/10
21. [Vanity Fair Report Alleges Kushner's Hacked Phone Revealed Secret Deals](#item-21) ⭐️ 4.0/10
22. [Reddit user asks if ICLR AI text detector will affect peer review](#item-22) ⭐️ 4.0/10
23. [De Staat's 'Freedom' video features AI-generated visual effect](#item-23) ⭐️ 3.0/10
24. [Armin Ronacher quips AI is punishing decades of bad software](#item-24) ⭐️ 3.0/10

---

<a id="item-1"></a>
## [Quad9 to Exit France After Court Fines It for Non-Compliance with Web-Blocking Orders](https://quad9.net/news/blog/au-revoir-france/) ⭐️ 8.0/10

Quad9, a Swiss non-profit public DNS resolver, announced it will exit France after a French court fined it for contempt of court for not complying with web-blocking orders. The orders were obtained by Sony Music Entertainment GmbH, which used a VPN to access blocked content from Germany and then argued Quad9's geoIP blocking was insufficient. This is a significant industry development because a major public DNS resolver is being forced out of a country due to legal pressure, highlighting a growing trend of DNS-level censorship. It raises concerns that DNS resolvers could be held liable for content they do not host and forced into content moderation roles, affecting users' privacy and internet access. Quad9 CTO John Todd stated that after November 24, Quad9 will likely use geoIP filters to block French users from its services, even though geoIP blocking is insufficient for selectively denying resolution for certain names. The case involved Sony Music Entertainment GmbH circumventing geoIP blocking via a VPN from Germany, leading the court to agree with Sony's non-compliance assertions and fine Quad9 for contempt.

hackernews · farrokhi · Oct 22, 14:32 · [Discussion](https://news.ycombinator.com/item?id=50195959)

**Background**: Quad9 is a global public recursive DNS resolver operated by the Quad9 Foundation, a Swiss non-profit, which blocks domains associated with malware and phishing and is subject to Swiss privacy law. DNS resolvers translate domain names into IP addresses, and blocking at the DNS level is a common method for censoring or filtering content. In France, rights holders such as Canal+ and Sony have obtained web-blocking injunctions against piracy sites, targeting ISPs, DNS resolvers, and VPNs; Google, Cloudflare, and Cisco have also faced such orders.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Quad9">Quad9 - Wikipedia</a></li>
<li><a href="https://torrentfreak.com/paris-court-issued-simultaneous-site-blocking-orders-against-isps-dns-resolvers-and-vpns/">Paris Court Issued Simultaneous Site Blocking Orders Against ...</a></li>
<li><a href="https://www.dnslab.dev/learn/docs/governance/dns-censorship">DNS Censorship — DNS Docs - dnslab.dev</a></li>

</ul>
</details>

**Discussion**: The community discussion is highly substantive, with Quad9's CTO directly participating and clarifying that geoIP blocking will likely be used to block French users after November 24. Commenters express frustration that Sony circumvented geoIP blocking via a VPN and then successfully argued non-compliance, and some compare the situation to punishing a phone book for listing a criminal's number. Others suggest that DNS resolvers should stop resolving domains of companies that sue them, and note that Cisco exited the French market two years ago for similar reasons.

**Tags**: `#DNS`, `#censorship`, `#privacy`, `#legal`, `#internet-governance`

---

<a id="item-2"></a>
## [NVIDIA OpenShell: Secure Runtime for Autonomous AI Agents](https://github.com/NVIDIA/OpenShell) ⭐️ 8.0/10

NVIDIA has released OpenShell, an open-source runtime designed to safely sandbox fleets of autonomous AI agents, allowing them to read files, install packages, call APIs, and use credentials without granting unrestricted access to data, secrets, or network. As AI agents become more autonomous and are deployed in production, securing their execution environment is critical to prevent data exfiltration, prompt injection, and unintended actions. OpenShell addresses this need by providing a governed runtime that balances capability with security, which could accelerate enterprise adoption of agentic AI. OpenShell governs agent execution, access, and inference routing, and can run on a single machine or across a cluster. It is part of NVIDIA's broader agentic AI stack, including NemoClaw, and emphasizes policy enforcement and sandboxing to restrict agent capabilities to only what is necessary.

hackernews · niemandhier · Oct 22, 17:44 · [Discussion](https://news.ycombinator.com/item?id=50198675)

**Background**: AI agent sandboxing involves isolating code execution in secure environments to prevent unauthorized access, data breaches, and system compromise. As agents gain more autonomy, traditional application-level guardrails are insufficient, and infrastructure-level controls like microVMs and gVisor are increasingly used. OpenShell is an open-source runtime that provides these controls specifically for AI agents, allowing them to operate with necessary permissions while enforcing security boundaries.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/ai/openshell/">NVIDIA OpenShell | Open, Secure Runtime for AI Agents</a></li>
<li><a href="https://axiomstudio.ai/blog/what-is-nvidia-openshell-agent-runtime">What Is NVIDIA OpenShell ? Agent Runtime Guide | Axiom Studio</a></li>
<li><a href="https://northflank.com/blog/how-to-sandbox-ai-agents">How to sandbox AI agents in 2026: MicroVMs, gVisor... — Northflank</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion (278 points, 144 comments) shows strong interest, with users debating the trade-offs between agent capability and security. Some note that while network restrictions and credential swapping are helpful, preventing data exfiltration remains a hard problem, and others criticize the marketing as oversimplifying the inherent tension between access and security.

**Tags**: `#AI agents`, `#sandboxing`, `#security`, `#NVIDIA`, `#runtime`

---

<a id="item-3"></a>
## [HackiOS project runs full iOS 16.5 firmware on Android phones via QEMU](https://github.com/oosexgang/hackios-xnu-kernel) ⭐️ 8.0/10

A project called HackiOS has demonstrated booting Apple's open-source XNU kernel (xnu-8796.121.2, the kernel of iOS 16.5) on Android phone hardware and running the unmodified iOS 16.5 user space on top of it, from launchd to SpringBoard and apps. It uses a custom EFI loader, replacements for Apple's closed drivers, a UEFI port, and a Linux Wi-Fi driver on a compatibility layer, and has been shown working on devices like the POCO X5 Pro 5G and some Xiaomi phones. This is a highly novel technical achievement that pushes the boundaries of reverse engineering and virtualization, showing that iOS firmware can be made to run on non-Apple hardware. It has significant implications for device security research, counterfeit phone detection, and the broader understanding of mobile OS portability. The project is described as a research bench rather than a ROM: a session lasts a given number of seconds, then the kernel returns to the loader and hands over its log. It relies on QEMU for emulation and includes custom components like an EFI loader and driver replacements, but it is not intended for daily use.

hackernews · aghuang · Oct 22, 15:26 · [Discussion](https://news.ycombinator.com/item?id=50196718)

**Background**: QEMU is a free and open-source machine emulator and virtualizer that can emulate various instruction set architectures, allowing software written for one platform to run on another. iOS is Apple's mobile operating system, which normally runs only on Apple's own hardware, and its kernel, XNU, is partly open source. Reverse engineering iOS firmware involves analyzing and modifying the software to run in non-standard environments, often for security research or compatibility purposes.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/QEMU">QEMU - Wikipedia</a></li>
<li><a href="https://github.com/oosexgang/hackios-xnu-kernel">GitHub - oosexgang/hackios-xnu-kernel</a></li>
<li><a href="https://ipsw.me/16.5/">Choose an IPSW for iOS 16.5</a></li>

</ul>
</details>

**Discussion**: Commenters found the achievement impressive, especially that it works on QEMU and devices like the POCO X5 Pro 5G. Some raised concerns about counterfeit phones becoming harder to detect, while others questioned the project's practicality given iOS's current usability and speculated about the role of AI safeguards in its development.

**Tags**: `#iOS`, `#Android`, `#QEMU`, `#reverse-engineering`, `#virtualization`

---

<a id="item-4"></a>
## [Switch 2 Jailbreak Uses JetKVM, LLM Automation, and Bluetooth Switch](https://pepsipu.com/blog/2026-10-switch2-jailbreak-ns2jb/) ⭐️ 8.0/10

Developer pepsipu published a detailed write-up of 'ns2jb', a software-only, tethered jailbreak for the Nintendo Switch 2 that runs arbitrary native code as any ordinary sysmodule and as the built-in fs sysmodule. The setup uses JetKVM hardware to let an LLM (Codex) send controller inputs over USB and receive HDMI video output, plus a Bluetooth light switch (SwitchBot Bot) to physically press the power button when the console crashes. This is reportedly the first software-only jailbreak for the Switch 2, and if it enables read/write access to the decrypted filesystem, game dumps could soon appear, potentially allowing console exclusives to run on arbitrary hardware via recomps/decomps—a worst-case scenario for Nintendo. It also demonstrates a powerful paradigm for AI-assisted hardware research, where LLMs gain 'arms and eyes' through KVM and camera setups. The jailbreak is tethered and software-only, meaning it requires a connection to a host and does not persist across reboots; it exploits a backward-compatible Switch application as an entry point. The automation relies on JetKVM's open-source KVM-over-IP hardware, which provides video and USB HID at the hardware level without needing an agent on the target, and the power-button pressing is handled by a SwitchBot Bot smart switch.

hackernews · ledoge · Oct 22, 08:01 · [Discussion](https://news.ycombinator.com/item?id=50192536)

**Background**: A jailbreak on a game console is an exploit that bypasses manufacturer restrictions to run unsigned or arbitrary code. The Switch 2 is Nintendo's successor to the Switch, and its security has been a major focus since launch. JetKVM is an open-source KVM over IP device that lets you control a computer's video, keyboard, and mouse remotely through a browser at the hardware level, making it useful for automating interactions with devices that lack software agents. LLM-driven automation refers to using large language models to plan and execute sequences of actions, such as sending controller inputs and reacting to video feedback.

<details><summary>References</summary>
<ul>
<li><a href="https://jetkvm.com/docs">JetKVM - Control any computer remotely</a></li>
<li><a href="https://gbatemp.net/news/switch-2-jailbreak-ns2jb-demonstrated-software-only-exploit-tethered.685698/">Switch 2 jailbreak "ns2jb" demonstrated, software-only... | GBAtemp.ne...</a></li>
<li><a href="https://pepsipu.com/blog/2026-10-switch2-jailbreak-ns2jb/">pepsipu.com/blog/2026-10- switch 2 - jailbreak -ns2jb</a></li>

</ul>
</details>

**Discussion**: Commenters were impressed by the ingenuity of the setup, with one noting that if decrypted filesystem read/write is achieved, Switch 2 game dumps could appear within hours and enable exclusives to run on arbitrary hardware via recomps/decomps. Others highlighted the clever use of a SwitchBot Bot (dubbed a 'Switch SwitchBot Bot') to press the power button, and some questioned how the author got Codex to assist with security research given the model's restrictions, while another emphasized that modern tooling like KVMs and USB controller support enables this level of automation.

**Tags**: `#security`, `#jailbreak`, `#hardware-hacking`, `#LLM-agents`, `#console-modding`

---

<a id="item-5"></a>
## [eMudhra to exit global SSL/TLS certificate business after misissuance incident](https://emudhra.com/en/press-release/emudhra-to-exit-global-ssl-tls-certificate-business) ⭐️ 8.0/10

eMudhra, an Indian certificate authority, announced that its board decided to withdraw from its global SSL/TLS certificate business following a security incident involving improperly issued certificates. The decision came after a researcher demonstrated that eight intermediate CA private keys were cracked, and the Chrome team publicly submitted a battery of questions to eMudhra on Mozilla's Bugzilla. This is a rare case of a certificate authority exiting the SSL/TLS market due to a serious misissuance scandal, which could erode trust in smaller CAs and prompt stricter scrutiny from browser root programs. The incident highlights the systemic risk that weak key management at any CA poses to the entire web PKI ecosystem. eMudhra stated that global SSL/TLS is a small part of its business, contributing about 1% of global revenue, and cited increasing data sovereignty, compliance complexity, and cost as reasons for the exit. The company also claimed that no end-entity certificates were issued from the affected CAs, a statement that community members found questionable given that anyone could issue certificates from those CAs.

hackernews · bo0tzz · Oct 22, 13:33 · [Discussion](https://news.ycombinator.com/item?id=50195110)

**Background**: Certificate authorities (CAs) issue digital certificates that bind public keys to domain names, enabling HTTPS and secure communications. Browsers and operating systems maintain root stores that trust specific CAs, but if a CA misissues certificates or its private keys are compromised, attackers could impersonate websites. Incidents like this have led to CA removals and exits in the past, such as Symantec's certificate business being taken over by DigiCert.

<details><summary>References</summary>
<ul>
<li><a href="https://thehackernews.com/2026/10/emudhra-to-exit-global-ssltls-business.html">eMudhra to Exit Global SSL/TLS Business After 8 Intermediate CA...</a></li>
<li><a href="https://emudhra.com/en/press-release/emudhra-to-exit-global-ssl-tls-certificate-business">eMudhra to Exit global SSL / TLS Certificate Business</a></li>
<li><a href="https://www.coindesk.com/tech/2026/10/21/a-company-that-vouches-for-websites-had-secret-keys-so-weak-that-8-of-them-were-cracked">Internet panics after 8 eMudhra private keys get cracked</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters expressed sharp criticism, noting that the scrutiny is proportional to the weakness of the private keys and that eMudhra's response lacks a clear apology or explanation of how the failure occurred. Some mocked the company's statement about no end-entity certificates being issued, while others linked to the Chrome team's brutal question battery on Bugzilla as evidence of serious concerns.

**Tags**: `#security`, `#TLS`, `#certificate-authority`, `#incident`, `#hackernews`

---

<a id="item-6"></a>
## [Faster than earcut: triangulating 3.7M map polygons in 489 ms](https://globus.software/blog/2026/10/16/cutting-map-polygons/) ⭐️ 8.0/10

A blog post by Evgen presents a new polygon triangulation method that outperforms the widely used earcut library, triangulating 3.7 million map polygons in just 489 milliseconds. The post includes a technical deep-dive and has attracted discussion from key library authors, including the creator of earcut. This performance improvement could significantly speed up rendering and processing of large-scale map data, benefiting applications like Mapbox GL JS and other WebGL-based mapping tools. The engagement from earcut's author and other triangulation library authors indicates strong community validation and potential for cross-pollination of optimization ideas. The earcut author notes that some optimizations were deliberately rejected to keep the library small (4.1k min/gz) and that earcut is already fast enough for most practical applications. The new method's WASM build size and triangle quality (some tiny triangles) were also points of discussion.

hackernews · molind · Oct 22, 09:31 · [Discussion](https://news.ycombinator.com/item?id=50193170)

**Background**: Polygon triangulation is a fundamental problem in computational geometry, where a polygon is divided into non-overlapping triangles for efficient rendering in computer graphics and mapping. Earcut is a widely used, fast, and small JavaScript library for this task, known for its simplicity and speed. The new method claims to be faster, likely using WebAssembly and optimized algorithms, but trade-offs in bundle size and triangle quality are important considerations.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/mapbox/earcut">GitHub - mapbox/ earcut : The fastest and smallest JavaScript polygon ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Polygon_triangulation">Polygon triangulation - Wikipedia</a></li>
<li><a href="https://github.com/mapbox/earcut.hpp">GitHub - mapbox/earcut.hpp: Fast, header-only polygon triangulation</a></li>

</ul>
</details>

**Discussion**: The discussion is highly engaged, with the earcut author expressing interest in borrowing tricks while noting bundle size constraints, and the author of Delaunay32 curious about comparisons with constrained Delaunay triangulation. Another commenter questions why ear clipping dominates over Seidel's algorithm despite its better asymptotic complexity, and concerns about tiny triangles causing rendering issues are raised.

**Tags**: `#triangulation`, `#computational-geometry`, `#performance`, `#maps`, `#algorithms`

---

<a id="item-7"></a>
## [Anthropic Donates Agent Skills Standard to Agentic AI Foundation](https://simonwillison.net/2026/Oct/22/donating-agent-skills/) ⭐️ 8.0/10

Anthropic announced it is donating its Agent Skills standard to the Agentic AI Foundation (AAIF) under the Linux Foundation, following its earlier donation of the Model Context Protocol (MCP). The AAIF was co-founded by Anthropic, Block, and OpenAI last year. This move cements Agent Skills as a vendor-neutral open standard, reducing the risk of fragmentation in how AI agents are extended with specialized capabilities. It signals growing industry commitment to interoperable agentic AI infrastructure governed by neutral foundations rather than single vendors. Agent Skills is a lightweight open format that uses files and folders to package specialized knowledge and workflows for AI agents, and it was first published as an open standard in December 2025. Simon Willison noted he predicted this donation last December, and he found his own earlier post by prompting Claude through the datasette-mcp plugin.

rss · Simon Willison · Oct 22, 18:09

**Background**: Agent Skills lets developers extend AI agents with reusable packages of instructions and resources, similar to how plugins add features to software. The Model Context Protocol (MCP), introduced by Anthropic in November 2024, is an open standard for connecting LLMs to external tools and data sources. The Linux Foundation is a nonprofit that hosts open-source projects and provides neutral governance, and the AAIF was created to steward agentic AI standards contributed by multiple companies.

<details><summary>References</summary>
<ul>
<li><a href="https://agentskills.io/">A standardized way to give AI agents new capabilities and expertise.</a></li>
<li><a href="https://www.anthropic.com/engineering/equipping-agents-for-the-real-world-with-agent-skills">Equipping agents for the real world with Agent Skills \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#agentic-ai`, `#open-standards`, `#anthropic`, `#ai-governance`, `#llm-tooling`

---

<a id="item-8"></a>
## [Carbon-X: Open 14.8B model trained jointly on DNA and text](https://www.reddit.com/r/MachineLearning/comments/1xchayq/carbonx_is_an_open_148b_model_trained_jointly_on/) ⭐️ 8.0/10

Hugging Face released Carbon-X, a 14.8B parameter decoder-only model that processes raw DNA and text in a single token stream using 6-mer tokens, and was mid-trained on 302B tokens. It achieves a 66.7% average across five DNA benchmarks (with thinking disabled), nearly matching GPT-6.1 Sol's 67.5%, and its weights fit on a single 80GB GPU in bfloat16 under an Apache 2.0 license. This model demonstrates that a relatively compact open-weight model can achieve DNA benchmark performance competitive with a large proprietary system, making sensitive sequence analysis feasible on local hardware. Its permissive license and single-GPU footprint could accelerate adoption in bioinformatics and clinical research where data privacy is critical. The model card notes that Carbon-X has not been clinically validated and that exact sequence operations should still be handled by code rather than the model itself. The benchmark comparison used thinking disabled, and the community has raised questions about whether the gains hold on private variant datasets.

reddit · r/MachineLearning · /u/jatingargiitk · Oct 22, 12:32

**Background**: DNA language models adapt techniques from natural language processing to genomic sequences, often by tokenizing DNA into k-mers (here, 6-mers) to capture local sequence patterns. Carbon-X extends this by sharing a single token stream between DNA and natural language, allowing users to input raw DNA in a chat and receive English answers. The model uses bfloat16 precision, a 16-bit floating-point format popular in machine learning for its balance of range and memory efficiency, enabling the 14.8B parameters to fit on one 80GB GPU.

<details><summary>References</summary>
<ul>
<li><a href="https://www.apache.org/licenses/LICENSE-2.0">Apache License , Version 2 . 0 | Apache Software Foundation</a></li>
<li><a href="https://www.johndcook.com/blog/2018/11/15/bfloat16/">bfloat16 (BF16) range and precision</a></li>

</ul>
</details>

**Discussion**: The discussion highlights practical questions about whether the benchmark gains generalize to private variant datasets, and emphasizes the value of local deployment for sensitive data. Commenters see the model's ability to run on a single GPU as a key advantage for privacy-preserving bioinformatics work.

**Tags**: `#machine-learning`, `#bioinformatics`, `#dna`, `#open-source`, `#large-language-models`

---

<a id="item-9"></a>
## [Woman faces six years for Cash App account she never opened](https://www.techspot.com/news/114296-woman-spends-three-nights-jail-faces-six-years.html) ⭐️ 7.0/10

A woman named Amanda Smith was arrested and spent three nights in jail after authorities accused her of fraud related to a Cash App account that was opened in her name without her knowledge. Prosecutors offered her a plea deal with a $1,000 fine, $1,000 restitution, and three years' probation, but she refused, maintaining her innocence and risking a six-year prison sentence if convicted at trial. The case highlights a troubling intersection of fintech account security and the criminal justice system, where identity theft victims can be treated as suspects and pressured into plea bargains. It raises urgent questions about how financial platforms like Cash App verify identities and how prosecutors handle cases with weak evidence, potentially affecting millions of users and the broader push for fintech accountability. Smith spent three nights in jail and faces up to six years in prison if she goes to trial and is convicted. The plea deal would require her to pay $1,000 in fines and $1,000 in restitution plus three years of probation, but she has refused because she insists she is innocent. The case was originally reported by 404 Media.

hackernews · oidar · Oct 22, 13:11 · [Discussion](https://news.ycombinator.com/item?id=50194833)

**Background**: Cash App is a peer-to-peer payment service launched by Block, Inc. (formerly Square) in 2013 that allows users to send, receive, and invest money. Accounts can be opened with minimal verification, and initial sending/receiving limits are $1,000 per 30-day period until users verify their identity for higher limits. Prosecutorial misconduct refers to illegal or unethical actions by prosecutors that violate a defendant's rights, while coercive plea bargaining is a widespread practice where innocent people plead guilty to avoid harsher sentences, with over 95% of criminal cases resolved through plea deals in the U.S.

<details><summary>References</summary>
<ul>
<li><a href="https://cash.app/learn/getting-started/what-is-cash-app-and-how-does-it-work">What is Cash App and how does it work?</a></li>
<li><a href="https://www.forbes.com/advisor/money-transfer/what-is-cash-app/">What Is Cash App, And How Does It Work? – Forbes Advisor What Is Cash App and How Does It Work? - NerdWallet Getting Started with Cash App What Is Cash App and How Does It Work? - Tech Review Advisor How Does Cash App Work? Complete Guide [2026] – Savings Grove How Cash App Works - HowStuffWorks</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prosecutorial_misconduct">Prosecutorial misconduct - Wikipedia</a></li>
<li><a href="https://innocenceproject.org/coerced-pleas/">Coerced Pleas - Innocence Project</a></li>

</ul>
</details>

**Discussion**: Commenters expressed outrage at the prosecutorial overreach, with many arguing that the plea deal is a tactic to avoid admitting mistakes and that prosecutors and police should be held liable for gross negligence. Some also called for Cash App founders and executives to be held personally liable for creating a system that facilitates fraud, while others shared the original 404 Media reporting link.

**Tags**: `#justice-system`, `#fintech`, `#fraud`, `#prosecutorial-overreach`, `#cash-app`

---

<a id="item-10"></a>
## [GNU Taler prepares for operational launch in Germany](https://www.taler.net/en/news/2026-13.html) ⭐️ 7.0/10

GNU Taler, a privacy-preserving digital cash system, is preparing for operational deployment in Germany, as announced on its official news page. This marks a significant step toward real-world use of a free-software-based payment system that prioritizes user anonymity. This deployment could provide a European alternative to US-dominated payment systems and bank-backed initiatives like Wero, while testing whether privacy-preserving digital cash can survive EU regulatory constraints. It matters for privacy advocates, European payment sovereignty, and the broader debate on digital cash design. Taler uses blind signatures to ensure customer anonymity while preventing merchant tax evasion, and it is not blockchain-based. However, Taler e-money has a validity period, and wallets must periodically exchange expiring coins for new ones, which requires internet connectivity and raises concerns about offline usability.

hackernews · dewey · Oct 22, 16:14 · [Discussion](https://news.ycombinator.com/item?id=50197404)

**Background**: GNU Taler is a free software electronic payment system that allows customers to remain anonymous while making merchants' income transparent, aiming to prevent tax evasion and money laundering. Unlike cryptocurrencies, it does not use a blockchain and is designed as a payment system rather than a store of value, with payments backed by existing currencies. In Europe, the European Payments Initiative (EPI) is developing Wero, a bank-backed digital wallet, while the EU is tightening AML rules that could impact privacy-focused payment solutions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GNU_Taler">GNU Taler - Wikipedia</a></li>
<li><a href="https://www.taler.net/en/features.html">GNU Taler: Features</a></li>
<li><a href="https://en.wikipedia.org/wiki/European_Payments_Initiative">European Payments Initiative - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters expressed skepticism about Taler's requirement for periodic internet connectivity and coin expiration, with one calling it 'infinitely worse than Bitcoin.' Others doubted that EU regulators would allow meaningful payment privacy due to KYC requirements, while some praised Taler as a much-needed European alternative to US payment systems and questioned its ability to compete with bank-backed Wero.

**Tags**: `#digital-payments`, `#privacy`, `#gnu-taler`, `#europe`, `#cryptography`

---

<a id="item-11"></a>
## [High Schooler's 100k-Line 3D Open-World Game Hedra Goes Viral](https://github.com/maxilevi/project-hedra/tree/pre-ai) ⭐️ 7.0/10

Maxilevi shared Project Hedra, a 3D open-world low-poly RPG and custom engine he began writing in high school almost 10 years ago, now comprising roughly 100,000 lines of C# and OpenGL code with native Linux and Windows support. The project showcases exceptional craftsmanship and long-term dedication, and its discussion highlights how the meaning of 'from scratch' is shifting in the AI coding era, while also demonstrating the value of building a mod API into games from the start. The game features animations, rendering effects, and dynamic terrains, and was built around a mod API; the repository is available under the 'pre-ai' branch, emphasizing that it was entirely hand-written without AI assistance.

hackernews · maxilevi · Oct 22, 18:44 · [Discussion](https://news.ycombinator.com/item?id=50199389)

**Background**: OpenGL is a cross-platform graphics API used to render 2D and 3D graphics, and building a game engine from scratch means implementing core systems like rendering, physics, and input handling without relying on existing engines such as Unity or Unreal. A mod API allows players to create and share custom content, extending a game's lifespan and fostering community creativity.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/maxilevi/project-hedra">GitHub - maxilevi/project-hedra: Hedra is a 3D open world ...</a></li>
<li><a href="https://daily.dev/posts/hedra-is-a-3d-open-world-game-i-wrote-from-scratch-while-in-highschool-bef6ltkhp">Hedra is a 3D open world game I wrote from scratch while...</a></li>
<li><a href="https://digitechbytes.com/general/hedra-is-a-3d-open-world-game-i-wrote-from-scratch-while-in-highschool/">Hedra Is A 3D Open World Game I Wrote From Scratch While In ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed admiration for the hand-written code and low-poly aesthetic, with one noting how 'from scratch' can mean anything from writing everything to just the core engine, and now even 'not using AI at all'. Others praised the mod API and added the game to their Steam wishlist.

**Tags**: `#game-development`, `#opengl`, `#personal-project`, `#modding`, `#ai-coding`

---

<a id="item-12"></a>
## [arXiv Paper Argues AI Is Enclosing the Scientific Commons](https://arxiv.org/abs/2610.27251) ⭐️ 7.0/10

A new arXiv paper titled 'AI and the Enclosure of the Scientific Commons' argues that AI is enclosing the scientific commons, drawing a critical discussion on Hacker News about open source licensing, copyright, and the nature of shared resources. The paper and discussion highlight growing tensions between AI development and the openness of scientific knowledge, with implications for researchers, open source developers, and policymakers navigating copyright and licensing. Commenters criticized the paper for focusing narrowly on GPL copyleft while ignoring permissively licensed open source funded by for-profit companies, and for omitting discussion of copyright term length and successful open source AI models.

hackernews · jrepinc · Oct 22, 18:28 · [Discussion](https://news.ycombinator.com/item?id=50199230)

**Background**: The 'enclosure of the commons' refers to the historical process of converting common land into private property, depriving commoners of traditional rights. In this context, the 'scientific commons' means shared scientific knowledge and resources, and the paper argues AI is similarly appropriating and restricting access to it. arXiv is a free open-access preprint server hosting nearly 2.4 million scholarly articles.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Enclosure_of_the_commons">Enclosure of the commons</a></li>
<li><a href="https://arxiv.org/">arXiv .org e- Print archive</a></li>

</ul>
</details>

**Discussion**: Commenters pushed back on the author's framing: one noted that most open source is permissively licensed and corporate-funded, another argued enclosure has been driven by copyright term extension and lobbying rather than AI, and a third said AI has actually opened the scientific commons to them by making literature more accessible.

**Tags**: `#AI`, `#open-source`, `#scientific-commons`, `#copyright`, `#enclosure`

---

<a id="item-13"></a>
## [Developer apologizes for unknowingly breaking PHP RCE embargo](https://news.ycombinator.com/item?id=50193416) ⭐️ 7.0/10

A developer publicly apologized on Hacker News for posting details about the upcoming PHP remote code execution vulnerabilities CVE-2026-109618 and CVE-2026-109619 before the coordinated disclosure embargo was lifted, causing schedule disruptions and extra workload for the disclosure team. This incident highlights the challenges of maintaining information asymmetry in coordinated vulnerability disclosure and raises questions about who bears responsibility when embargo information is not properly communicated through the disclosure chain. The developer stated he was unaware of any embargo because his contact and her contact had both told him there was no embargo; the vulnerabilities were later publicly disclosed on October 21, 2026, with a CVSS v4.0 score of 9.2.

hackernews · petecooper · Oct 22, 10:11

**Background**: Coordinated vulnerability disclosure (CVD) often involves an embargo period during which a vulnerability is shared only with trusted parties to allow patches to be prepared before public disclosure. PHP follows a regular release cycle, and critical security releases are typically announced in advance so that administrators can plan updates.

<details><summary>References</summary>
<ul>
<li><a href="https://www.redhat.com/en/blog/Understanding-security-embargoes-at-Red-Hat">Understanding security embargoes at Red Hat</a></li>
<li><a href="https://www.zscaler.com/blogs/security-research/cve-2026-109618-and-cve-2026-109619-php-vulnerable-unauthenticated-rce">CVE-2026-109618 and CVE-2026-109619: PHP Vulnerable to ...</a></li>
<li><a href="https://www.php.net/supported-versions.php">Supported Versions - PHP</a></li>

</ul>
</details>

**Discussion**: Commenters largely supported the developer, arguing that one cannot break an embargo one was never informed about, and that responsibility lies with whoever leaked the information upstream. Some noted the vulnerabilities were already being exploited before the post, and others criticized the phrase 'take full responsibility' as meaningless in this context.

**Tags**: `#security`, `#vulnerability-disclosure`, `#php`, `#embargo`, `#hackernews`

---

<a id="item-14"></a>
## [Open-XTTS-Trainer enables full XTTS v2 training and new-language tokenizer extension](https://www.reddit.com/r/MachineLearning/comments/1xcurgj/i_built_openxttstrainer_now_you_can_add_new/) ⭐️ 7.0/10

A developer released Open-XTTS-Trainer, an open-source (MPL-2.0) modular suite that provides training recipes for all three XTTS v2 components—the DVAE audio tokenizer, the GPT text/vocab extender, and the Latent HiFi-GAN vocoder—plus a one-click Colab demo. It also adds a tokenizer extension mechanism that scans a new-language corpus, discovers unique Unicode glyphs, appends them to the tokenizer, and resizes the GPT embedding matrix without corrupting existing weights. Since Coqui AI's shutdown, XTTS v2 users have lacked official training code for the DVAE and HiFi-GAN stages and were blocked from adapting the model to new scripts by its fixed 17-language vocabulary. This suite fills that gap, making it feasible for the open TTS community to fine-tune XTTS v2 for languages such as Arabic, Hindi, Thai, and Dhivehi. On an NVIDIA T4 GPU with real speech (LJSpeech and the JFK address), the author reports HiFi-GAN mel reconstruction loss dropping 67% (190.83 to 63.49) over 10 epochs, DVAE mel error falling 67% (8.14 to 2.71), and stable MPD+MSD discriminator equilibrium at 3.62. The benchmarks verify component-level convergence and gradient stability rather than full end-to-end TTS quality, and the code runs on Python 3.10–3.13 with modern PyTorch without the torchcodec dependency issues.

reddit · r/MachineLearning · /u/yashubhakt · Oct 22, 21:03

**Background**: XTTS v2 is a multilingual zero-shot text-to-speech model from Coqui that can clone a voice from about six seconds of audio, and it was trained on 16–17 languages. Its pipeline has three stages: a DVAE audio tokenizer that converts audio to discrete codes and mel spectrograms, a GPT model that predicts those codes from text, and a HiFi-GAN-based vocoder that turns mel spectrograms back into waveforms. When Coqui shut down, only partial fine-tuning code remained public, and the model's fixed tokenizer vocabulary caused out-of-vocabulary or dimension-mismatch errors when fed new Unicode scripts.

<details><summary>References</summary>
<ul>
<li><a href="https://deepwiki.com/archwesome/XTTS-v2/3-system-architecture">System Architecture | archwesome/XTTS-v2 | DeepWiki</a></li>
<li><a href="https://edresson.github.io/XTTS/">XTTS - Edresson Casanova</a></li>
<li><a href="https://github.com/jik876/hifi-gan">GitHub - jik876/hifi-gan: HiFi-GAN: Generative Adversarial ...</a></li>

</ul>
</details>

**Tags**: `#text-to-speech`, `#XTTS`, `#open-source`, `#model-training`, `#multilingual`

---

<a id="item-15"></a>
## [WhissleAI shrinks steerable TTS to 11.84 MB with int4 quantization](https://www.reddit.com/r/MachineLearning/comments/1xcum4s/we_shrank_our_steerable_small_tts_to_1184_mb_wer/) ⭐️ 7.0/10

WhissleAI released SteerTTS-Edge, an 11.84 MB int4-quantized text-to-speech model that includes weights, voices, text front end, and Python runtime, while maintaining the same word error rate (WER) as the fp32 version and only a ~0.1 drop in UTMOS. This demonstrates that aggressive quantization can shrink a steerable TTS system to fit on edge devices without sacrificing intelligibility or control, making on-device speech synthesis more practical for mobile and embedded applications. The acoustic model (9.25M parameters, attention + bidirectional Mamba-3) and a distilled Vocos-style vocoder (6.2M parameters) are both int4 quantization-aware trained; the text front end is pure numpy with no external dependencies, and the model runs at RTF 0.053 on a 2018 Threadripper CPU, though weights are dequantized to fp32 at load so the benefit is size, not speed.

reddit · r/MachineLearning · /u/Working_Hat5120 · Oct 22, 20:57

**Background**: Text-to-speech (TTS) models typically use large neural networks, making them challenging to deploy on edge devices with limited memory and compute. Quantization reduces model size by lowering numerical precision (e.g., to 4-bit integers), and quantization-aware training (QAT) simulates this during training to minimize accuracy loss. Mamba-3 is a state space model architecture that offers efficient sequence modeling as an alternative to Transformers, and Vocos is a fast neural vocoder that generates audio waveforms from acoustic features.

<details><summary>References</summary>
<ul>
<li><a href="https://keras.io/guides/int4_quantization_in_keras/">INT4 Quantization in Keras</a></li>
<li><a href="https://github.com/gemelo-ai/vocos">GitHub - gemelo-ai/ vocos : Vocos : Closing the gap between...</a></li>
<li><a href="https://www.remio.ai/post/mamba-3-model-reopens-the-post-transformer-debate">Mamba 3 model Reopens the Post-Transformer Debate</a></li>

</ul>
</details>

**Tags**: `#TTS`, `#model-quantization`, `#edge-ML`, `#speech-synthesis`, `#Mamba`

---

<a id="item-16"></a>
## [Frontier audio models struggle to label ASMR sound events, benchmark shows](https://www.reddit.com/r/MachineLearning/comments/1xcbqdm/frontier_models_are_bad_at_hearing_asmr_8_judges/) ⭐️ 7.0/10

A developer building a text-to-ASMR model benchmarked eight frontier audio models as sound-event labelers on 480 clips, finding that all performed poorly compared to human labels, with the best F1 score of 0.325 from Gemini 3.1 Pro. Spectrogram-image approaches (Claude Opus 5.5 and Grok 4.7) performed worst, with F1 scores of 0.121 and 0.110 respectively. This benchmark highlights a significant gap in current audio LLMs' ability to recognize fine-grained, real-world sound events like brushing or paper rustling, which is critical for applications such as training generative audio models. It suggests that practitioners should validate label quality before using model-generated labels for training. The models performed well on whispering (F1 0.70-0.79) but poorly on physical triggers; for example, Gemini 3.1 Pro achieved only 0.18 F1 on brushing in real ASMR clips despite naming brushing 92% of the time on clean sound effects. Cost varied widely, with Gemini 3.1 Pro at $0.0088 per clip and MiMo at $0.0008 per clip.

reddit · r/MachineLearning · /u/MissAppleby · Oct 22, 07:10

**Background**: ASMR (Autonomous Sensory Meridian Response) audio often features subtle, close-miked sounds like tapping, crinkling, and brushing, which are challenging for automatic recognition. FSD50K and ESC-50 are standard datasets of human-labeled environmental sounds used to benchmark audio classification models. Audio LLMs are large multimodal models that process audio inputs, but their ability to label fine-grained sound events is not well understood.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/datasets/Fhrozen/FSD50k">Fhrozen/FSD50k · Datasets at Hugging Face</a></li>
<li><a href="https://github.com/karolpiczak/ESC-50">GitHub - karolpiczak/ESC-50: ESC-50: Dataset for ...</a></li>

</ul>
</details>

**Tags**: `#audio-models`, `#benchmarking`, `#ASMR`, `#model-evaluation`, `#machine-learning`

---

<a id="item-17"></a>
## [Xbox to charge 24-40 cents per hour for streaming owned games](https://arstechnica.com/gaming/2026/10/xbox-wants-you-to-pay-24-to-40-cents-per-hour-to-stream-games-you-already-bought/) ⭐️ 6.0/10

Xbox plans to introduce a per-hour fee of 24 to 40 cents for streaming games that users already own, a shift from its current subscription-based cloud gaming model. This pricing applies specifically to cloud streaming on rented GPU hardware, not to playing the game on your own console or PC. This move signals a potential shift in how cloud gaming is monetized, moving from all-you-can-play subscriptions to usage-based pricing for streamed content. It could affect millions of Xbox users who rely on cloud streaming as a cheaper alternative to buying expensive gaming hardware. The fee covers the cost of renting GPUs in the cloud, similar to services like GeForce Now, and is positioned as a budget-friendly option for those who play 10-20 hours per week. However, recent reports suggest Xbox Cloud streaming quality has degraded in some regions, raising concerns about the value proposition.

hackernews · entryleveljobsc · Oct 22, 11:42 · [Discussion](https://news.ycombinator.com/item?id=50194009)

**Background**: Cloud gaming allows users to stream games running on remote servers to their devices, eliminating the need for powerful local hardware. Xbox Cloud Gaming is currently bundled with Game Pass subscriptions starting at $9.99 per month, but Microsoft has announced hour caps by tier starting November 2026. The concept of digital ownership has become contentious, with advocacy groups like Stop Killing Games arguing that publishers are destroying games consumers have paid for.

<details><summary>References</summary>
<ul>
<li><a href="https://cloudloadout.com/xbox-game-pass/">Xbox Game Pass Update: New Prices & Tiers, and the Impact on ...</a></li>
<li><a href="https://shattered.io/xbox-cloud-gaming-hour-caps-november-2026/">Xbox Cloud Gaming Hour Caps: 15/10/5 Hrs by Tier [2026]</a></li>
<li><a href="https://www.stopkillinggames.com/">Stop Killing Games — They Kill Games . We Fight Back.</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters are divided: some argue the fee is fair for renting GPUs, comparing it to GeForce Now and noting it's cheaper than buying a $1000 console for casual play. Others report that Xbox Cloud streaming quality has deteriorated and that Xbox hardware is increasingly hard to find in stores, while some satirize the digital ownership implications with jokes about intrusive verification.

**Tags**: `#cloud-gaming`, `#xbox`, `#pricing`, `#digital-ownership`, `#industry-news`

---

<a id="item-18"></a>
## [Blog post claims all AI models share a controversial take on human nature, but commenters debunk methodology](https://www.modelcompare.ai/blog/ai-models-controversial-take-on-humans) ⭐️ 5.0/10

A blog post on modelcompare.ai argues that every AI model, when prompted, produces a similar 'controversial' take on human nature—specifically that humans pick what their group believes and then invent reasons. Commenters on Hacker News quickly challenged this, pointing out that the data does not support the conclusion and that model outputs are highly sensitive to prompting. This episode highlights a common pitfall in AI journalism: drawing broad conclusions about model behavior from a single prompt without controlling for prompt design or model bias. It underscores the need for rigorous methodology when evaluating LLM outputs, especially as these models are increasingly used in high-stakes domains. One commenter noted that GPT-6 Astra's response—'Humanity’s biggest moral failure is the talent for making convenience look like principle'—does not actually match the claimed thesis about group beliefs, and at best is a half-match. Another commenter showed that an 'abliterated' GLM 5.3 model gave a completely different answer ('Death is bad, full stop'), and that rephrasing the prompt to ignore rationalist talking points yields different results.

hackernews · rakannimer · Oct 22, 16:08 · [Discussion](https://news.ycombinator.com/item?id=50197313)

**Background**: Large language models (LLMs) generate text by predicting likely sequences based on patterns in training data, and their outputs can vary significantly depending on how a prompt is phrased. Research has shown that even slight changes in prompt wording can greatly impact clarity, accuracy, and completeness of outputs, and that models can exhibit sycophancy—a tendency to agree with user beliefs. Evaluating model bias and behavior therefore requires careful methodology, such as controlling for prompt variations and using multiple test cases.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2403.03028v1">Word Importance Explains How PromptsAffect Language Model Outputs</a></li>
<li><a href="https://ijirt.org/publishedpaper/IJIRT183166_PAPER.pdf">Does Prompt Design Affect LLM Outputs? A Study Across ...</a></li>
<li><a href="https://arxiv.org/html/2411.15287v1">Sycophancy in Large Language Models: Causes and Mitigations</a></li>

</ul>
</details>

**Discussion**: Commenters largely dismissed the blog's premise. One argued that LLMs are 'just a probabilistic database' with no opinion, while another found irony in models producing a shared opinion while pretending to derive it from analysis. A third noted that the data doesn't support the conclusion, and another demonstrated that prompt changes (e.g., asking to ignore rationalist talking points) yield different answers.

**Tags**: `#AI`, `#LLM`, `#model behavior`, `#prompting`, `#critique`

---

<a id="item-19"></a>
## [Reddit user steers Qwen2.5-1.5B-Instruct toward 'evil' persona, eliciting slurs](https://www.reddit.com/r/MachineLearning/comments/1xcvil5/steered_qwen_to_be_more_evil_and_it_started/) ⭐️ 5.0/10

A Reddit user extracted an 'evil vs kind' activation direction from Qwen2.5-1.5B-Instruct's internal activations and used it to steer the model toward an 'evil' persona, which then produced offensive outputs including the n-word and other slurs. This informal demonstration shows how activation steering can reliably manipulate high-level behavioral traits like persona, raising safety concerns because such techniques can bypass alignment safeguards and induce harmful outputs even in small, instruction-tuned models. The experiment used Qwen2.5-1.5B-Instruct, a 1.54B-parameter instruction-tuned model, and the steering vector was derived by contrasting activations from 'evil' versus 'kind' persona prompts; however, the methodology is informal and lacks rigorous evaluation or controls.

reddit · r/MachineLearning · /u/Thatmf482 · Oct 22, 21:33

**Background**: Activation steering is a technique that modifies a language model's internal activations at inference time to alter its behavior without retraining, typically by adding a 'steering vector' that represents a concept or trait. Qwen2.5-1.5B-Instruct is a small instruction-tuned model from Alibaba's Qwen2.5 series, which includes models from 0.5B to 72B parameters pretrained on up to 18 trillion tokens. Steering vectors are often computed as the difference between mean activations elicited by positive and negative prompts, a method known as contrastive activation addition (CAA).

<details><summary>References</summary>
<ul>
<li><a href="https://ollama.com/library/qwen2.5:1.5b-instruct">qwen2.5:1.5b-instruct - ollama.com</a></li>
<li><a href="https://www.emergentmind.com/topics/activation-steering-method">Activation Steering in LLMs</a></li>
<li><a href="https://arxiv.org/html/2609.36388v1">Persona Dosing: Calibrated ActivationSteering for Graded ...</a></li>

</ul>
</details>

**Tags**: `#activation-steering`, `#interpretability`, `#LLM-safety`, `#reddit`, `#model-behavior`

---

<a id="item-20"></a>
## [uv 0.13.5 Updates Managed CPython Builds and Removes Compromised Certificate Root](https://github.com/astral-sh/uv/releases/tag/0.13.5) ⭐️ 4.0/10

uv 0.13.5, released on 2026-10-21, updates its managed CPython builds for Python 3.11 and newer to python-build-standalone 20261021, incorporating CPython 3.15.1, 3.14.9, and 3.13.17 security patch releases. These builds bundle pip 26.2.2 and certifi 2026.10.19, which remove the affected eMudhra/emSign certificate root, and uv now rejects certificate chains containing compromised eMudhra intermediate keys via rustls-webpki 0.103.16. This is a security-relevant maintenance release for uv users: it ensures that newly created virtual environments and managed interpreters no longer trust a compromised certificate authority, reducing the risk of man-in-the-middle attacks during package installation. It also signals the end of Docker image publishing for end-of-life Python 3.9 and 3.10, pushing users to migrate to supported versions. After upgrading uv, users must run `uv python upgrade` to install the updated builds; existing virtual environments pinned to older Python patch versions will not switch automatically, and pip must be upgraded separately in those environments. Upstream CPython 3.9 and 3.10 still bundle pip releases that trust the affected root, so users are advised to migrate off those versions.

github · astral-releases-bot[bot] · Oct 22, 01:35

**Background**: uv is a fast Python package and project manager from Astral that can install and manage Python interpreters itself, using redistributable builds from the python-build-standalone project. certifi provides the curated Mozilla CA bundle used by Python for SSL/TLS verification, and pip bundles certifi to validate package downloads. When a certificate authority is compromised, tools must remove its root from trust stores and update bundled copies to prevent attackers from impersonating package indexes.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/astral-sh/python-build-standalone">GitHub - astral-sh/python-build-standalone: Produce ...</a></li>
<li><a href="https://pypi.org/project/certifi/">certifi · PyPI</a></li>
<li><a href="https://pydevtools.com/handbook/how-to/how-to-keep-python-up-to-date-with-uv-python-upgrade/">How to keep Python up to date with uv python upgrade | pydevtools</a></li>

</ul>
</details>

**Tags**: `#python`, `#uv`, `#package-management`, `#security-update`, `#release-notes`

---

<a id="item-21"></a>
## [Vanity Fair Report Alleges Kushner's Hacked Phone Revealed Secret Deals](https://www.vanityfair.com/story/jared-kushner-hacked-phone-secret-negotiations) ⭐️ 4.0/10

Vanity Fair published an excerpt from the book 'Princes and Thieves' alleging that Jared Kushner's hacked phone revealed secret negotiations and millions of dollars in transactions linked to Israel, the UAE, and Saudi Arabia. The report raises concerns about foreign influence on U.S. policy and the security of sensitive communications at the highest levels of government, sparking discussion about compromised systems and geopolitical implications. The excerpt claims that bank accounts linked Kushner to foreign entities, including hundreds of millions of dollars from a bank in Azerbaijan, though the specific hacking method and full evidence are not detailed in the provided content.

hackernews · ck2 · Oct 22, 21:24 · [Discussion](https://news.ycombinator.com/item?id=50201259)

**Background**: Jared Kushner is a former senior advisor and son-in-law to President Donald Trump. The book excerpt is part of an investigation into Kushner's dealings with Middle Eastern leaders. The alleged hacking of his phone highlights the vulnerability of high-profile individuals to sophisticated cyber espionage, such as Pegasus spyware, which can remotely compromise mobile devices.

<details><summary>References</summary>
<ul>
<li><a href="https://www.vanityfair.com/story/jared-kushner-hacked-phone-secret-negotiations">The Art of the Deal: Jared Kushner ’s Hacked Phone ... | Vanity Fair</a></li>
<li><a href="https://en.wikipedia.org/wiki/Pegasus_(spyware)">Pegasus (spyware)</a></li>

</ul>
</details>

**Discussion**: Commenters expressed cynicism about foreign influence, with some suggesting the administration is 'owned by foreign interests' and others drawing connections to the arrest of Germany's BND chief and Azerbaijan. The overall sentiment was one of shock and resignation, with references to compromised systems and political satire.

**Tags**: `#politics`, `#security`, `#geopolitics`, `#news`, `#hacking`

---

<a id="item-22"></a>
## [Reddit user asks if ICLR AI text detector will affect peer review](https://www.reddit.com/r/MachineLearning/comments/1xcq2an/iclr_text_editor_d/) ⭐️ 4.0/10

A Reddit post on r/MachineLearning asks whether a new AI text detector for ICLR submissions, hosted at opentextdetector.com, will impact the peer review process. The poster expresses hope that it will not, citing the general unreliability of AI detectors. If such detectors are used in peer review, they could unfairly flag legitimate submissions or discourage authors from using AI-assisted writing tools, affecting fairness and trust in the review process at a top machine learning conference. This touches on broader debates about AI's role in academic writing and the reliability of detection tools. The detector, Open Text Detector, is described as a free, open-source tool that checks every public ICLR 2027 submission for AI-assisted and AI-edited writing, showing passage-by-passage where text looks model-generated. It claims thresholds calibrated to a fixed false-positive rate on human writing, but independent studies show AI detectors are often unreliable, especially with paraphrasing.

reddit · r/MachineLearning · /u/Whatever_635 · Oct 22, 18:07

**Background**: ICLR (International Conference on Learning Representations) is one of the three primary conferences in machine learning, alongside NeurIPS and ICML. Peer review at such conferences relies on volunteer reviewers assessing submissions, and the rise of large language models has led to concerns about AI-generated content in papers. AI text detectors attempt to identify machine-generated text but have been shown to produce false positives and can be easily fooled by paraphrasing.

<details><summary>References</summary>
<ul>
<li><a href="https://opentextdetector.com/">Open Text Detector: AI-assisted writing in ICLR 2027 submissions</a></li>
<li><a href="https://en.wikipedia.org/wiki/International_Conference_on_Learning_Representations">International Conference on Learning Representations</a></li>
<li><a href="https://link.springer.com/article/10.1007/s40979-026-00213-1">Evaluating the accuracy and reliability of AI content ...</a></li>

</ul>
</details>

**Tags**: `#AI detectors`, `#peer review`, `#ICLR`, `#academic publishing`, `#machine learning community`

---

<a id="item-23"></a>
## [De Staat's 'Freedom' video features AI-generated visual effect](https://simonwillison.net/2026/Oct/22/de-staat-freedom/) ⭐️ 3.0/10

Simon Willison highlighted a striking visual effect at the 44-second mark in Dutch rock band De Staat's new music video for 'Freedom'. The effect, credited to Matties Grooten of AI studio Fake it or Leave it, was shared via a Hacker News comment. This showcases how AI-generated visual effects are increasingly being used in mainstream music videos, blending live-action footage with AI to create surreal imagery. It signals broader adoption of generative AI in creative industries beyond software. The video was created by Fake it or Leave it, an AI studio founded by brothers Cas and Matties Grooten, which combines self-filmed footage with AI visual effects. The specific effect at 00:44 is a pelican riding a bicycle, a recurring motif in Simon Willison's blog.

rss · Simon Willison · Oct 22, 19:42

**Background**: De Staat is a Dutch alternative rock band formed in Nijmegen in 2006. Fake it or Leave it is an AI studio that uses AI technology to create images that are impossible to film but need to be seen. The pelican riding a bicycle is a whimsical benchmark often used by Simon Willison to test generative AI models.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/De_Staat">De Staat - Wikipedia</a></li>
<li><a href="https://fakeitorleaveit.com/">Home - Fake it or Leave it | AI Studio</a></li>

</ul>
</details>

**Discussion**: The item was shared via a Hacker News comment by user flir, but no further community discussion is provided in the content.

**Tags**: `#music-video`, `#visual-effects`, `#hacker-news`, `#curiosity`

---

<a id="item-24"></a>
## [Armin Ronacher quips AI is punishing decades of bad software](https://simonwillison.net/2026/Oct/22/armin-ronacher/) ⭐️ 3.0/10

Simon Willison quoted Armin Ronacher's tweet saying that after 30 years of building bad software, "the universe is punishing us for our sins" now that AI is in the picture. The quip resonates because LLM-powered security tools are increasingly used to find vulnerabilities in legacy code, exposing long-ignored weaknesses at scale. The post is a single quoted tweet with no added analysis, and it is tagged with security, generative AI, and AI security research, framing the joke as commentary on AI-driven vulnerability discovery.

rss · Simon Willison · Oct 22, 15:34

**Background**: Armin Ronacher is the Austrian developer who created the Flask web framework for Python and later worked at Sentry; he now writes and speaks widely about software engineering. Large language models are increasingly studied as tools for vulnerability detection, since traditional static and dynamic analysis struggle with false positives and the complexity of modern codebases. Ronacher's remark plays on the idea that AI is now surfacing the accumulated flaws in decades-old software.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Armin_Ronacher">Armin Ronacher - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2502.07049">[2502.07049] LLMs in Software Security: A Survey of ... Large Language Models in Software Security Analysis LLMs in Software Security: A Survey of Vulnerability ... Awesome-LLMs-for-Vulnerability-Detection - GitHub GitHub - OwenSanzas/LLM-For-Software-Security: Hey folks ...</a></li>

</ul>
</details>

**Tags**: `#ai`, `#security`, `#software-engineering`, `#llms`, `#quote`

---