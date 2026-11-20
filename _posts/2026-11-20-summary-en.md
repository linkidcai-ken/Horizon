---
layout: default
title: "Horizon Summary: 2026-11-20 (EN)"
date: 2026-11-20
lang: en
---

> From 12 items, 12 important content pieces were selected

---

1. [Anthropic says Claude solved two open problems in black hole physics](#item-1) ⭐️ 9.0/10
2. [PostgreSQL 19 Released with WAIT FOR LSN for Read-Your-Writes Consistency](#item-2) ⭐️ 9.0/10
3. [Anthropic's Nasdaq Debut Sparks AI Valuation Debate](#item-3) ⭐️ 8.0/10
4. [Experimental virus injection halts pancreatic cancer in three patients](#item-4) ⭐️ 8.0/10
5. [Java4Shell OpenJDK Vulnerability Reported via GitHub PR, Oracle Takes Over](#item-5) ⭐️ 8.0/10
6. [UK government admits issuing secret encryption order to Apple](#item-6) ⭐️ 8.0/10
7. [Gemini 4 Neon Tops Models Engineering Index, Sparking Opus 5.5 Comparisons](#item-7) ⭐️ 7.0/10
8. [Essay Calls Paid Advertising a 98% Extraction Tax, Sparking Debate](#item-8) ⭐️ 7.0/10
9. [Synology warns of command injection flaw in OAuth Service package](#item-9) ⭐️ 6.0/10
10. [Ransomware Gang n0n Leaks Data of 16,000 JPMorgan, Visa, Mastercard Customers](#item-10) ⭐️ 6.0/10
11. [Cornhole News: A Hacker News-Inspired Site for the Midwest](#item-11) ⭐️ 5.0/10
12. [Browser app turns a single A4 sheet into an 8-page foldable zine](#item-12) ⭐️ 5.0/10

---

<a id="item-1"></a>
## [Anthropic says Claude solved two open problems in black hole physics](https://www.anthropic.com/research/claude-black-hole-physics) ⭐️ 9.0/10

Anthropic announced that its frontier model Claude Fable 5.2 solved two open problems in theoretical physics, both related to black holes and quantum gravity. One problem, concerning the Hawking-Page phase transition, had reportedly remained unsolved for 23 years. This claim, if validated, represents a significant milestone for AI-for-science, showing that large language models can contribute to advanced theoretical physics. It could reshape how researchers approach open problems and accelerate discovery in fields like quantum gravity. The results are theoretical and do not describe our own universe directly, nor do they have practical applications. Notably, the blog post and papers do not mention the prompts used, raising questions about the human role in guiding the AI.

hackernews · cybermango · Nov 19, 17:30 · [Discussion](https://news.ycombinator.com/item?id=50563148)

**Background**: Black holes are regions of spacetime where gravity is so strong that nothing can escape, and understanding them requires reconciling general relativity with quantum mechanics. The Hawking-Page phase transition describes when a hot gas of particles in anti-de Sitter space collapses into a black hole. The 'bootstrap method' is a technique in theoretical physics that uses consistency conditions to determine properties of theories, often without detailed calculation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/research/claude-black-hole-physics">Claude Fable 5.2 solves two open problems in the physics of black ...</a></li>
<li><a href="https://www.youtube.com/watch?v=oBH1xKzOdk0">Anthropic Just Solved a 23-Year-Old Black Hole Problem - YouTube</a></li>
<li><a href="https://nerdzap.com/news/claude-fable-mythos-5-2-black-hole-physics/">Claude Fable 5.2 Cracks Two Black Hole Problems , Then Builds an OS</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters debated the framing of 'Claude solves', with some criticizing the anthropomorphizing of the AI and noting the absence of prompt details. Others highlighted the technical substance, such as Claude proving an upper mass limit consistent with a given central charge, while some lamented that few comments actually discussed the papers themselves.

**Tags**: `#AI-for-science`, `#LLM`, `#physics`, `#black-holes`, `#research`

---

<a id="item-2"></a>
## [PostgreSQL 19 Released with WAIT FOR LSN for Read-Your-Writes Consistency](https://simonwillison.net/2026/Nov/19/postgresql-19/) ⭐️ 9.0/10

PostgreSQL 19 was released in November 2026, two months later than the usual September schedule, and introduces the WAIT FOR LSN command that lets a standby session wait until it has replayed the write-ahead log up to a specified log sequence number before running a query. This enables read-your-writes consistency for applications that send reads to standbys. This feature solves a long-standing problem for applications that offload reads to asynchronous replicas, where a user might not see data they just wrote on the primary. It brings a built-in, standardized solution to PostgreSQL, replacing hand-rolled workarounds and benefiting backend and systems engineers who rely on read scaling with strong consistency guarantees. The command can be used with an optional timeout, such as WAIT FOR LSN '0/0306EE20' WITH (TIMEOUT '0.1s'), which raises an error if the standby does not catch up in time. The LSN value can be obtained via pg_current_wal_insert_lsn() and stored, for example, in a signed cookie for use on subsequent requests.

rss · Simon Willison · Nov 19, 20:43

**Background**: PostgreSQL uses write-ahead logging (WAL) to ensure data integrity, and each WAL record has a log sequence number (LSN) that increases monotonically. In streaming replication, a standby server replays WAL from the primary, but replication lag means a read on the standby may not immediately reflect a recent write on the primary. The read-your-writes consistency problem occurs when an application writes to the primary and then reads from a standby, potentially missing the just-written data. MediaWiki has long implemented a similar pattern against MySQL replication by saving the primary binlog position and waiting for the replica to catch up.

<details><summary>References</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/19/sql-wait.html">PostgreSQL: Documentation: 19: WAIT</a></li>
<li><a href="https://clickhouse.com/blog/postgresql-19-wait-for-read-your-writes">Read your writes: WAIT FOR in PostgreSQL 19 - ClickHouse</a></li>
<li><a href="https://www.postgresql.org/docs/current/wal-internals.html">PostgreSQL: Documentation: 18: 28.6. WAL Internals</a></li>

</ul>
</details>

**Tags**: `#PostgreSQL`, `#databases`, `#replication`, `#consistency`, `#release`

---

<a id="item-3"></a>
## [Anthropic's Nasdaq Debut Sparks AI Valuation Debate](https://www.reuters.com/business/finance/anthropics-historic-debut-put-ais-promise-peril-wall-st-test-2026-11-19/) ⭐️ 8.0/10

Anthropic made its historic Nasdaq debut on November 19, 2026, opening at $111.5 per share after pricing its IPO at $83, but the stock closed at $97.17, down 12.85% from its opening price. The first half hour of trading was reportedly the worst start for a major IPO since 2008. As one of the highest-profile AI companies to go public, Anthropic's debut serves as a major test of whether public markets will validate the lofty valuations that private AI companies have commanded. The weak aftermarket performance could pressure other AI firms, including OpenAI, and signals investor caution about the AI sector's growth expectations. While the stock was up 17.07% from its IPO price of $83 to its closing price of $97.17, it was down 12.85% from its opening price of $111.5, meaning most first-day buyers who didn't get shares at the IPO price lost money. The valuation fell to $1.26 trillion, well below the $2 trillion-plus that some had hoped for just weeks earlier.

hackernews · wslh · Nov 19, 17:02 · [Discussion](https://news.ycombinator.com/item?id=50562754)

**Background**: Anthropic is an AI safety and research company known for its Claude family of large language models, and it is structured as a public benefit corporation. An IPO (initial public offering) is the process by which a private company first sells shares to the public on a stock exchange like Nasdaq, transitioning to a publicly traded company. Valuing AI startups is notoriously difficult because their key assets—models, data, and talent—are intangible and traditional metrics like discounted cash flow often fail to capture their potential.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nasdaq.com/products/listings/ipo">IPO Process | Guide to Going Public on Nasdaq</a></li>
<li><a href="https://eqvista.com/how-to-value-ai-startup/">How to Value an AI Startup in 2026? | Eqvista AI Startup Valuation 2026: Multiples, Methods | GetDeal.AI Understanding AI Startup Valuations: Trends and Insights for ... AI Startups Valuation Multiples: Key Considerations for 2026 AI Startup Valuation: How AI Companies Are Valued in 2026 AI Business Valuation Model 2026: Methods, Metrics & Trends ... AI Startup Valuations 2025-2026: How VCs Price AI Companies ...</a></li>
<li><a href="https://www.anthropic.com/">Home \ Anthropic</a></li>

</ul>
</details>

**Discussion**: Commenters expressed anxiety about the future of software engineering careers, with some veteran developers describing the end of a lucrative era and uncertainty for juniors. Others focused on the disappointing market performance, noting the valuation drop from earlier hopes and suggesting it bodes poorly for OpenAI and the broader AI investment landscape.

**Tags**: `#Anthropic`, `#AI industry`, `#IPO`, `#software engineering careers`, `#market valuation`

---

<a id="item-4"></a>
## [Experimental virus injection halts pancreatic cancer in three patients](https://www.newscientist.com/article/2528235-pancreatic-cancer-halted-by-virus-injection-in-three-patients/) ⭐️ 8.0/10

A New Scientist report describes how an experimental oncolytic virus injection halted the progression of pancreatic cancer in three patients, according to a small early-stage study. The news sparked extensive discussion on Hacker News, where readers shared personal experiences and tried to identify the specific clinical trial. Pancreatic cancer has one of the poorest prognoses of any cancer, with most patients diagnosed at an advanced stage and few effective treatment options. If the results hold up in larger trials, oncolytic virus therapy could offer a new approach for a disease where conventional treatments often fail. The report is based on only three patients, so the findings are preliminary and cannot establish efficacy or safety; the specific virus, dosing, and trial protocol were not clearly identified in the article. Community members noted that numerous clinical trials of oncolytic viruses for pancreatic cancer are already underway, and that the lead physician-researcher has published reviews on the general concept.

hackernews · cybermango · Nov 19, 17:25 · [Discussion](https://news.ycombinator.com/item?id=50563066)

**Background**: Oncolytic viruses are viruses that preferentially infect and kill cancer cells, and as the infected cells are destroyed they release new virus particles that help destroy the remaining tumor and stimulate anti-tumor immune responses. Several oncolytic viruses have been clinically tested, and one (T-VEC, a modified herpes simplex virus) was approved in the US and EU in 2015 for advanced melanoma. Pancreatic cancer is notoriously difficult to treat because it is often detected late and traditional chemotherapy has limited effectiveness.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Oncolytic_virus">Oncolytic virus - Wikipedia</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC12025738/">Recent Advances and Challenges in the Treatment of Advanced ...</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion was emotionally charged, with several commenters sharing stories of family members who died of pancreatic cancer and expressing hope that such research could help others. Others focused on technical aspects, with one commenter unable to identify the exact trial from the limited information and linking to 25 clinical trials of oncolytic viral therapies for pancreatic cancer, while another noted the slow pace of progress against the disease.

**Tags**: `#oncology`, `#medical-research`, `#oncolytic-virus`, `#pancreatic-cancer`, `#biotech`

---

<a id="item-5"></a>
## [Java4Shell OpenJDK Vulnerability Reported via GitHub PR, Oracle Takes Over](https://github.com/openjdk/jdk/pull/32781) ⭐️ 8.0/10

A critical OpenJDK vulnerability dubbed Java4Shell (CVE-2026-114938) was reported through a GitHub pull request, with the reporter later noting that Oracle took over the issue and asked them not to proceed until approval. The vulnerability is a memory corruption flaw in OpenJDK's Base64 decoder that can lead to remote code execution. This vulnerability affects a core component of Java, potentially impacting millions of servers running OpenJDK, and its disclosure process raises questions about AI-assisted vulnerability discovery and the role of major vendors like Oracle in coordinating fixes. The flaw is rated 9.2 under CVSS v4.0 and can allow unauthenticated remote code execution, crash the JVM, or expose sensitive memory data. The disclosure timeline is complex, with independent discoveries and speculation that an LLM may have been involved in finding the bug.

hackernews · notmine1337 · Nov 19, 11:47 · [Discussion](https://news.ycombinator.com/item?id=50558906)

**Background**: Java deserialization vulnerabilities have been a major security concern, allowing attackers to execute arbitrary code. OpenJDK is the open-source implementation of Java, and Oracle oversees its development. The term 'Java4Shell' is a play on 'Log4Shell', highlighting the severity of the flaw.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sophos.com/en-us/security-advisories/sophos-sa-20261118-java4shell">Advisory: OpenJDK Base64 Vulnerability - Java4Shell (CVE-2026 ...</a></li>
<li><a href="https://cybersecuritynews.com/java4shell/">Critical Java4Shell Flaw Lets Hackers Execute Code Without ...</a></li>
<li><a href="https://blog.qualys.com/vulnerabilities-threat-research/2026/11/17/how-to-find-mitigate-and-patch-the-critical-java4shell-flaw-cve-2026-114938-now">How to Find, Mitigate, and Patch the Critical Java4Shell Flaw ...</a></li>

</ul>
</details>

**Discussion**: Commenters debated whether an LLM used by researchers may have read a previous bug report and not independently discovered the flaw, while another researcher claimed to have found it independently via fuzzing. Some noted that simultaneous disclosures are now common and that Oracle's commit message was identical to the PR description.

**Tags**: `#security`, `#java`, `#openjdk`, `#vulnerability-disclosure`, `#ai-assisted-discovery`

---

<a id="item-6"></a>
## [UK government admits issuing secret encryption order to Apple](https://macanorak.com/uk-government-forced-to-admit-it-issued-apple-a-secret-encryption-order/) ⭐️ 8.0/10

The UK government was forced to admit it issued a secret technical capability notice to Apple demanding encryption access, as revealed through a tribunal judgment. The Investigatory Powers Tribunal confirmed the notice, which had been kept secret for nearly two years, after media learned of it through confidential security briefings. This case sets a precedent for government surveillance overreach and could influence similar demands from other countries, affecting encryption and privacy protections for users worldwide. It highlights the tension between national security and tech companies' ability to secure user data. The technical capability notice was issued under section 253 of the Investigatory Powers Act 2016, which allows the Secretary of State to compel telecommunications operators to build capabilities for lawful interception. The contents of the notice remain secret, and the tribunal ruling only addressed the government's attempt to keep the order's existence confidential, not the legality of the demand itself.

hackernews · Terretta · Nov 19, 16:21 · [Discussion](https://news.ycombinator.com/item?id=50562113)

**Background**: The Investigatory Powers Act 2016, often called the 'Snoopers' Charter,' grants UK intelligence agencies broad surveillance powers, including the ability to issue secret technical capability notices to companies. These notices can require operators to modify their systems to enable data collection, and non-compliance can lead to significant penalties. Apple has challenged such orders, arguing they undermine end-to-end encryption and user privacy.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/11/19/u-k-government-forced-to-disclose-secret-apple-backdoor-order/">UK government forced to disclose secret Apple backdoor order</a></li>
<li><a href="https://therecord.media/apple-uk-encryption-notice">UK court confirms British government served Apple with secret ...</a></li>
<li><a href="https://www.legislation.gov.uk/ukpga/2016/25/section/253">Investigatory Powers Act 2016 - Legislation.gov.uk</a></li>

</ul>
</details>

**Discussion**: Commenters expressed concern that Apple has weakened its security assurances, with one noting that device-held keys are likely key encryption keys that unlock other keys, complicating claims that Apple cannot access data. Others criticized the UK's intense surveillance stance and questioned why it is so overt compared to other Western countries, while some saw the admission as confirming long-suspected government overreach.

**Tags**: `#encryption`, `#privacy`, `#surveillance`, `#UK government`, `#Apple`

---

<a id="item-7"></a>
## [Gemini 4 Neon Tops Models Engineering Index, Sparking Opus 5.5 Comparisons](https://git-aarvin.github.io/mei/) ⭐️ 7.0/10

Google's Gemini 4 Neon has reportedly taken the #1 spot on the Models Engineering Index, a benchmark that compares language models on engineering tasks by cost and token use. The ranking, which drew 152 points and 92 comments on Hacker News, prompted practitioners to share hands-on comparisons with Anthropic's Claude Opus 5.5 on coding and long-running language-porting work. If the results hold up, Neon gives Google a credible contender in the high-end coding model market, where Anthropic's Opus line has been a common default for agentic development workflows. The discussion suggests speed and cost, not just raw quality, are becoming decisive factors for developers choosing a model. Commenters note that Neon 'high' appears faster and cheaper than Opus 5.5 'medium' with similar results on long-running language porting in a large monorepo, though skepticism remains about benchmark validity and limited hands-on access. Google's model lineup also includes Gemini 4 Carbon for the hardest long-horizon projects and Hydrogen for fast everyday execution, with Neon positioned to balance depth and efficiency.

hackernews · hn-aarvin · Nov 19, 23:35 · [Discussion](https://news.ycombinator.com/item?id=50568130)

**Background**: The Models Engineering Index is a benchmark that evaluates language models on engineering work, including engineering knowledge, science, reasoning, agentic coding, and agentic knowledge work, while also comparing cost and token use. Gemini 4 Neon is a Google DeepMind model built for complex coding, analytical reasoning, and production-grade enterprise workflows, available through the Gemini API and AI Studio. Claude Opus 5.5 is Anthropic's flagship Opus-tier model for complex reasoning and coding tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://git-aarvin.github.io/mei/">Models Engineering Index</a></li>
<li><a href="https://deepmind.google/models/model-cards/gemini-4-neon/">Gemini 4 Neon - Model Card — Google DeepMind</a></li>
<li><a href="https://platform.claude.com/docs/en/models/opus-5-5/overview">Claude Opus 5.5 - Claude Platform Docs</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree Neon is a strong contender: one calls it their favorite model, equivalent to Opus 5.5 for coding and excellent for documentation, while another reports switching from Opus after Neon proved faster and cheaper with similar results on long-running porting work. Several note that few commenters have actually used the model due to Google's costly access, and one highlights that Neon is now included in the Gemini quota of Google's AI subscription plans.

**Tags**: `#llm`, `#benchmarks`, `#google-gemini`, `#ai-coding`, `#model-evaluation`

---

<a id="item-8"></a>
## [Essay Calls Paid Advertising a 98% Extraction Tax, Sparking Debate](https://globalcommercegraph.com/writing/the-ninety-eight-percent-slot-machine) ⭐️ 7.0/10

An essay published on Global Commerce Graph argues that paid advertising functions as an extraction tax, likening it to a 98% slot machine where advertisers rarely recoup their spending. The piece sparked a substantive Hacker News discussion with 212 points and 112 comments, where commenters challenged the analogy and debated the effectiveness of internet advertising. This debate matters because digital advertising is a massive industry, and if paid ads often fail to deliver returns, it suggests significant economic inefficiency and raises questions about the sustainability of ad-funded business models. It also touches on broader concerns about ad-tech economics and whether platforms extract value from advertisers without providing commensurate benefits. The essay's central analogy compares ad auctions to a slot machine with a 98% house edge, implying advertisers almost always lose. However, commenters noted that ad auctions are marketplaces connecting advertisers to third-party customers, not a direct zero-sum game against the platform, and that the scarcity of attention drives up prices for those who can monetize it best.

hackernews · dev1one1 · Nov 19, 18:35 · [Discussion](https://news.ycombinator.com/item?id=50564159)

**Background**: Programmatic advertising automates the buying and selling of digital ad space using data and machine learning, often through real-time auctions. In this system, advertisers bid for impressions targeted at specific users, and platforms like Google and Meta take a cut of each transaction. The essay's 'extraction tax' framing draws on the idea of a severance tax on resource extraction, suggesting that ad platforms extract value from advertisers much like a tax on a natural resource.

<details><summary>References</summary>
<ul>
<li><a href="https://taxfoundation.org/blog/bottled-water-subject-severance-extraction-excise-tax/">Should Bottled Spring Water Be Subject to Excise... - Tax Foundation</a></li>
<li><a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5610930">Data Extraction Taxes by Andrew D. Appleby :: SSRN</a></li>
<li><a href="https://boldonlinemarketing.com/are-online-ads-effective/">Are Online Ads Still Effective | Bold Online Marketing</a></li>

</ul>
</details>

**Discussion**: Commenters largely pushed back on the analogy: hatthew argued that casinos are engineered for the house to win because they pay customers directly, whereas ad auctions are marketplaces where the advertiser's win comes from a third party. Others, like nukanse, contended that if customers lose money buying from you they go bankrupt, so the real dynamic is scarcity of attention being allocated to those who can best monetize it. hackthemack noted that the effectiveness of internet advertising has been debated since at least 2019, referencing a Freakonomics podcast on the topic.

**Tags**: `#advertising`, `#ad-tech`, `#economics`, `#internet`, `#hn-discussion`

---

<a id="item-9"></a>
## [Synology warns of command injection flaw in OAuth Service package](https://www.synology.com/en-uk/security/advisory/Synology_SA_26_21) ⭐️ 6.0/10

Synology published security advisory SA_26_21 for a command injection vulnerability (CWE-88) in the OAuth Service package, which is installed by default on many DiskStation Manager (DSM) systems. The advisory recommends uninstalling or stopping the OAuth Service package as a mitigation for affected devices. Because the OAuth Service package is installed by default and often left unconfigured, many Synology NAS owners may be exposed without realizing it, and exploitation could lead to remote code execution on internet-facing devices. This highlights the risk of default-enabled services on widely used network-attached storage. The vulnerability is classified as CWE-88 (Improper Neutralization of Argument Delimiters in a Command), a sub-class of command injection that can occur even without a shell. Synology's advised mitigation is to remove or stop the OAuth Service package via Package Center, and users of older units may see a fix status of 'Ongoing'.

hackernews · choult · Nov 19, 22:13 · [Discussion](https://news.ycombinator.com/item?id=50567209)

**Background**: Synology NAS devices run DiskStation Manager (DSM) and support add-on packages, including an OAuth Service package that implements the OAuth 2.0 standard for third-party authorization without sharing credentials. CWE-88 refers to argument injection, where user input is improperly neutralized before being passed to a command, potentially allowing attackers to inject additional arguments. Synology periodically issues security advisories for its packages and DSM, and users are expected to apply updates or follow mitigations.

<details><summary>References</summary>
<ul>
<li><a href="https://cwe.mitre.org/data/definitions/88">CWE - CWE - 88 : Improper Neutralization of Argument Delimiters in...</a></li>
<li><a href="https://www.synology.com/en-us/dsm/packages/OAuthService">OAuth Service - Add-on Packages | Synology Inc.</a></li>
<li><a href="https://mariushosting.com/critical-apache-and-nginx-flaws-what-synology-nas-users-must-do-now/">Critical Apache and NGINX Flaws, What Synology NAS Users Must...</a></li>

</ul>
</details>

**Discussion**: Commenters emphasized practical mitigations: uninstalling or stopping the OAuth Service package via Package Center, and putting NAS devices behind a VPN rather than exposing them to the internet. Some also raised broader questions about root causes of CVEs, wondering how many essential categories of software weaknesses exist, and speculated that the OAuth API was building shell commands from user input.

**Tags**: `#security`, `#vulnerability`, `#synology`, `#nas`, `#cwe-88`

---

<a id="item-10"></a>
## [Ransomware Gang n0n Leaks Data of 16,000 JPMorgan, Visa, Mastercard Customers](https://www.wsj.com/finance/banking/visa-mastercard-and-jpmorgan-customer-data-leaked-by-hackers-3b5a0f87) ⭐️ 6.0/10

The n0n ransomware gang published the names, email addresses, and phone numbers of roughly 16,000 customers of JPMorgan Chase, Visa, and Mastercard, data it obtained by breaching a third-party marketing vendor. JPMorgan confirmed the leak in a statement on X, noting that the exposed information was marketing data held by the vendor. The breach highlights the systemic risk that third-party marketing vendors pose to major financial institutions, even when the banks' own defenses are strong. It also fuels debate over whether customers meaningfully consent to their data being shared with such vendors and who should bear liability when it leaks. The leaked data is limited to names, emails, and phone numbers, which are considered low-value compared to financial records, and the WSJ report is paywalled. The n0n gang has listed 91 victims on its leak site, with activity concentrated in sectors such as maritime and logistics.

hackernews · mikhael · Nov 19, 23:32 · [Discussion](https://news.ycombinator.com/item?id=50568082)

**Background**: Ransomware gangs like n0n steal data and threaten to publish it unless a ransom is paid, a tactic known as double extortion. Third-party vendors—such as marketing firms—often hold customer data for multiple large brands, so a single breach can expose customers of many companies at once. Regulations like GDPR and CCPA require informed consent for data sharing, but enforcement and practical transparency remain uneven.

<details><summary>References</summary>
<ul>
<li><a href="https://www.breachsense.com/ransomware-groups/n0n/">n0n Ransomware: Victims and Activity | Breachsense</a></li>
<li><a href="https://securityarsenal.com/blog/n0n-ransomware-gang-claims-50-victims-in-coordinated-maritime-and-logistics-leak-site-campaign-sector-analysis-and-detection-rules">N0N Ransomware Gang Claims 50 Victims in Coordinated Maritime ...</a></li>
<li><a href="https://www.brightside.net/2025/11/12/mango-data-breach-exposes-sensitive-customer-information/">Mango Data Breach Exposes Sensitive... | Brightside IT Solutions</a></li>

</ul>
</details>

**Discussion**: Commenters questioned whether the leaked data has any real value and criticized the banks for implying more sensitive information was taken. Others raised concerns about informed consent for data sharing with third-party vendors and proposed treating customer data as a liability, such as charging companies per row of data held to fund breach compensation.

**Tags**: `#security`, `#data-breach`, `#privacy`, `#fintech`, `#ransomware`

---

<a id="item-11"></a>
## [Cornhole News: A Hacker News-Inspired Site for the Midwest](https://cornholenews.news/) ⭐️ 5.0/10

A new Show HN project called Cornhole News launched as a text-only news aggregator for the American Midwest, mimicking Hacker News's minimalist design and community-driven voting. The site aims to serve regional news with a focus on local businesses and includes a politics filter. This project demonstrates how the Hacker News model can be adapted to local and regional news, potentially filling gaps left by traditional media. It also sparks discussion about content moderation, monetization, and the definition of politics in news aggregation. The site plans to monetize with two small ads on the homepage reserved for Midwestern businesses, and community members have raised questions about moderation policies and the challenge of accurately filtering political content.

hackernews · cornholemedia · Nov 19, 15:38 · [Discussion](https://news.ycombinator.com/item?id=50561515)

**Background**: Hacker News is a popular technology-focused news aggregator run by Y Combinator, known for its minimalist text-only interface and community upvoting. Many clones and inspired sites have emerged, but few focus on specific geographic regions like the Midwest.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/topics/hackernews-clone">hackernews-clone · GitHub Topics · GitHub</a></li>
<li><a href="https://github.com/soragui/hacker-clone">Hacker News Clone - GitHub</a></li>

</ul>
</details>

**Discussion**: Commenters appreciated the text-only approach and expressed interest in similar sites for other regions, while questioning how 'politics' is defined and filtered. Concerns were raised about moderation plans and whether the site would be for-profit or just cover costs.

**Tags**: `#hacker-news`, `#news-aggregation`, `#show-hn`, `#community`, `#web-app`

---

<a id="item-12"></a>
## [Browser app turns a single A4 sheet into an 8-page foldable zine](https://krthr.co/paper-folds-and-whats-new-in-fanzines-app/) ⭐️ 5.0/10

A blog post introduces a browser-based app that generates an 8-page foldable zine from a single A4 sheet, handling the page layout and folding pattern automatically. The post also covers recent updates to the fanzine app, and Hacker News commenters shared related tools and techniques. This project lowers the barrier to creating and printing zines, making a traditionally fiddly layout process accessible to anyone with a browser. It also highlights a broader community interest in impositioning tools and simple paper-craft workflows. The app specifically targets the 8-page single-sheet fold, where pages must be reordered and some rotated so they read correctly after folding and cutting. Commenters noted that this is a form of impositioning, and similar tools like Bookbinder JS and PocketMod exist, though they may not use the exact same folding algorithm.

hackernews · krthr · Nov 19, 13:18 · [Discussion](https://news.ycombinator.com/item?id=50559719)

**Background**: Impositioning is the process of arranging pages on a printed sheet so that after folding and binding they appear in the correct order. For a single-sheet 8-page zine, the sheet is folded and cut so that the eight panels form a small booklet. Tools like PocketMod and Dirty Little Zine popularized this format for quick, disposable notebooks.

<details><summary>References</summary>
<ul>
<li><a href="https://snipzine.com/">snipzine — free mini zine maker (one sheet , 8 pages )</a></li>
<li><a href="https://dirtylittlezine.com/">Dirty Little Zine — Free 8-Page Printable Zine Maker</a></li>
<li><a href="https://news.ycombinator.com/item?id=50559719">Making 8-page foldable zines from a single A4 sheet ... | Hacker News</a></li>

</ul>
</details>

**Discussion**: Commenters shared related tools like Bookbinder JS, PocketMod, and Dirty Little Zine, and one noted that the general process is called impositioning. Some felt the post should have credited PocketMod for the folding idea, while another suggested a simpler CLI or browser tool that only combines PDF pages into the layout without a full editor.

**Tags**: `#web-app`, `#paper-crafts`, `#zines`, `#impositioning`, `#hacker-news`

---