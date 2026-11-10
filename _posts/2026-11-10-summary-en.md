---
layout: default
title: "Horizon Summary: 2026-11-10 (EN)"
date: 2026-11-10
lang: en
---

> From 27 items, 25 important content pieces were selected

---

1. [Anthropic releases Claude Fable 5.2 and Mythos 5.2](#item-1) ⭐️ 8.0/10
2. [E-means clustering claims to beat k-means with one-tenth the epochs](#item-2) ⭐️ 8.0/10
3. [Infineon produces first functional power devices on 300mm SiC wafers](#item-3) ⭐️ 8.0/10
4. [Google Unveils TPU 8tx and 8i Max for Agentic AI](#item-4) ⭐️ 8.0/10
5. [Google Gemini routes personal Drive files and emails to human annotators](#item-5) ⭐️ 8.0/10
6. [Browser tool finds every satellite that passed over any place in the last week](#item-6) ⭐️ 8.0/10
7. [LingBot-Touch: JEPA-style tactile pretraining outperforms reconstruction for dexterous manipulation](#item-7) ⭐️ 8.0/10
8. [USPS Releases Official ZIP Code Boundary Polygons with Steep Price Tag](#item-8) ⭐️ 7.0/10
9. [Payments Canada launches Real-Time Rail payment system](#item-9) ⭐️ 7.0/10
10. [Semi-transparent colored CdTe panels tested for agrivoltaics](#item-10) ⭐️ 7.0/10
11. [Meta releases Muse Ember, its smallest and most efficient model](#item-11) ⭐️ 7.0/10
12. [Simon Willison uses Claude Code to build Beep Locator](#item-12) ⭐️ 7.0/10
13. [XGBoost model forecasts new county-level power outages 2 hours ahead, beating NWS/SPC baselines by 2.4× PR-AUC](#item-13) ⭐️ 7.0/10
14. [SwarmEvolve uses latent-agent swarms for faster math discovery](#item-14) ⭐️ 7.0/10
15. [Twindex: Exact, Replayable Proofs of Parameter Non-Identifiability](#item-15) ⭐️ 7.0/10
16. [Blog Post: Fable 5.2 One-Shots Nephew's Dream Game](#item-16) ⭐️ 6.0/10
17. [Claude Ports Three.js Fabergé Egg Demo to Vanilla WebGL](#item-17) ⭐️ 6.0/10
18. [Simon Willison: Hide verbose AI PR descriptions behind <details><summary>](#item-18) ⭐️ 6.0/10
19. [Reddit discussion revisits why BatchNorm works](#item-19) ⭐️ 6.0/10
20. [Paper-mining tool adds 2026 ICML/CVPR/ICLR/AAAI results, flags baseline inconsistencies](#item-20) ⭐️ 6.0/10
21. [Reddit user fails to reproduce 'lost in the middle' on current models for easy retrieval](#item-21) ⭐️ 6.0/10
22. [Foldable Flight paper airplane site sparks nostalgic Hacker News discussion](#item-22) ⭐️ 5.0/10
23. [Reddit User Asks About Building Image Diffusion Generator from Scratch on Home Hardware](#item-23) ⭐️ 4.0/10
24. [Reddit user seeks advice for Amazon applied science PhD internship interview](#item-24) ⭐️ 3.0/10
25. [EACL 2027 Acceptance Decisions to Be Announced Thursday](#item-25) ⭐️ 3.0/10

---

<a id="item-1"></a>
## [Anthropic releases Claude Fable 5.2 and Mythos 5.2](https://www.anthropic.com/claude-fable-and-mythos-5-2) ⭐️ 8.0/10

Anthropic released Claude Fable 5.2 and Claude Mythos 5.2, two configurations of a new large language model, with Fable 5.2 available for general use and Mythos 5.2 restricted to verified organizations. According to Anthropic, Fable 5.2 sets a new bar in coding, finance, and the sciences. This release intensifies competition among frontier AI labs and affects developers and enterprises choosing models for demanding technical tasks. The community's scrutiny of benchmark methodology and model tiering also highlights growing demand for transparency in how AI capabilities are measured and marketed. Fable 5.2 includes additional safeguards that prevent it from performing certain tasks in high-risk, dual-use domains such as biology and cybersecurity, while Mythos 5.2 is the same underlying model without those restrictions and is available only through Anthropic's verification programs. Anthropic's published scores show results with safeguards on and at each model's highest-available effort unless otherwise noted.

hackernews · lairv · Nov 9, 18:01 · [Discussion](https://news.ycombinator.com/item?id=50429068)

**Background**: Anthropic is an AI safety and research company that develops the Claude family of large language models. In recent releases, it has offered models in tiers such as Opus and Sonnet, and with Fable and Mythos it is introducing a new naming scheme where the same model is released in a general-use version (Fable) and a restricted version for vetted organizations (Mythos). Benchmarks are standardized tests used to compare model capabilities, but their methodology is often debated because results can be sensitive to settings like effort level and task selection.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/claude-fable-and-mythos-5-2">Introducing Claude Fable 5.2 and Claude Mythos 5.2 \ Anthropic</a></li>
<li><a href="https://platform.claude.com/docs/en/models/fable-5-2/overview">Claude Fable 5.2 - Claude Platform Docs</a></li>
<li><a href="https://platform.claude.com/docs/en/models/mythos-5-2/overview">Claude Mythos 5.2 - Claude Platform Docs</a></li>

</ul>
</details>

**Discussion**: Commenters shared hands-on impressions, with one noting that Anthropic's models now feel well balanced across tiers, though Fable 5.2 requires more ambitious prompts to clearly separate from Opus 5.5. Others questioned benchmark methodology, asking why Fable xHigh was compared against Carbon Med, why Carbon's effort-intel curve seemed anomalous, and why Carbon was omitted from a cyber benchmark comparison. Some speculated about release strategy and expressed concern about possible model nerfing over time.

**Tags**: `#AI/ML`, `#LLM`, `#Anthropic`, `#model-release`, `#benchmarks`

---

<a id="item-2"></a>
## [E-means clustering claims to beat k-means with one-tenth the epochs](https://e-means.github.io/) ⭐️ 8.0/10

A new clustering algorithm called E-means has been presented, which reportedly outperforms the classic k-means algorithm while requiring only one-tenth the number of epochs. The announcement has sparked community experiments and theoretical discussion, with practitioners reporting significant speedups in real-world applications. If validated, E-means could significantly reduce computational costs for clustering tasks, which are fundamental in machine learning, data mining, and vector search. This could impact a wide range of applications from customer segmentation to large-scale indexing systems. Community members have adapted E-means to various use cases: one reported 2.5x faster bulk reindexing for hierarchical balanced incremental clustering, another achieved a 146x GPU speedup on an IVF index, and a third found it not better for mesh relaxation. Theoretical discussions suggest the algorithm may be equivalent to expectation-maximization with a friction term, and its update rule keeps centroids within the convex hull.

hackernews · porridgeraisin · Nov 9, 18:45 · [Discussion](https://news.ycombinator.com/item?id=50429734)

**Background**: K-means is a widely used clustering method that partitions data into k clusters by minimizing within-cluster variances, typically using Lloyd's algorithm which iteratively assigns points to nearest centroids and updates centroids. It is known to be efficient but can require many iterations to converge. E-means appears to be a variant that accelerates convergence, possibly by modifying the update rule to allow larger steps while maintaining stability.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/K-means_clustering">k-means clustering - Wikipedia</a></li>
<li><a href="https://www.geeksforgeeks.org/machine-learning/epoch-in-machine-learning/">Epoch in Machine Learning - GeeksforGeeks</a></li>

</ul>
</details>

**Discussion**: The community response is largely positive, with practitioners reporting impressive speedups in real-world applications such as bulk reindexing and GPU-accelerated IVF indexes. However, one user found it less effective for mesh relaxation, and others are discussing its theoretical connections to EM and simulated annealing. There is also hope that it gets added to scipy for wider accessibility.

**Tags**: `#clustering`, `#k-means`, `#machine-learning`, `#algorithms`, `#vector-search`

---

<a id="item-3"></a>
## [Infineon produces first functional power devices on 300mm SiC wafers](https://www.infineon.com/press-release/2026/infpr202611-028) ⭐️ 8.0/10

Infineon announced on November 9, 2026, that it has fabricated the industry's first functional power devices on 300-millimeter silicon carbide (SiC) wafers. This milestone demonstrates the feasibility of processing SiC power devices on larger-diameter wafers, a key step toward commercial-scale manufacturing. Transitioning SiC power devices from 200mm to 300mm wafers could significantly reduce manufacturing costs and increase output, accelerating the adoption of wide-bandgap semiconductors in electric vehicles, industrial power supplies, and renewable energy systems. This affects the entire power electronics supply chain, from wafer suppliers to automakers. Infineon notes that the 300mm SiC process leverages existing 300mm silicon equipment, though adapting processes such as crystal growth and epitaxy for SiC remains challenging. The announcement focuses on functional devices, not yet on high-volume production or yield metrics.

hackernews · sshah03 · Nov 9, 18:25 · [Discussion](https://news.ycombinator.com/item?id=50429430)

**Background**: Silicon carbide is a wide-bandgap semiconductor with a bandgap of about 3 eV, enabling devices that operate at higher voltages, temperatures, and frequencies than traditional silicon. These properties make SiC attractive for power electronics, particularly in electric vehicles where efficiency and thermal management are critical. Historically, SiC devices have been manufactured on 150mm or 200mm wafers, while silicon has used 300mm wafers for years to reduce cost per chip.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Silicon_carbide">Silicon carbide - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Wide-bandgap_semiconductor">Wide-bandgap semiconductor</a></li>
<li><a href="https://www.sic-wafers.com/300-mm-silicon-carbide-wafers-materials-manufacturing-barriers-and-the-path-to-industrial-scale-wide-bandgap-semiconductors/">300 mm Silicon Carbide Wafers: Materials, Manufacturing ...</a></li>

</ul>
</details>

**Discussion**: Commenters highlighted the significance of the milestone for national security and industrial applications, while questioning why the transition to 300mm took so long given that much equipment is shared with silicon. Some also noted Infineon's broader role in European semiconductor manufacturing and expressed interest in AI hardware development.

**Tags**: `#semiconductors`, `#silicon-carbide`, `#power-electronics`, `#manufacturing`, `#wide-bandgap`

---

<a id="item-4"></a>
## [Google Unveils TPU 8tx and 8i Max for Agentic AI](https://blog.google/innovation-and-ai/infrastructure-and-cloud/global-network/tpu-8i-max-and-8tx/) ⭐️ 8.0/10

Google announced two new eighth-generation TPU systems, the TPU 8tx for secure inference and the TPU 8i Max for massive context workloads, expanding its custom AI accelerator lineup for the agentic AI era. This strengthens Google's position in the AI infrastructure market by offering purpose-built silicon for inference and secure computing, directly challenging NVIDIA's dominance and giving cloud customers more specialized options for deploying AI agents. The TPU 8tx is optimized for secure inference with sensitive data, while the 8i Max targets massive context windows needed by complex AI agents; however, Google has not yet disclosed performance metrics such as watts per token or cost per token.

hackernews · _benx_ · Nov 9, 21:56 · [Discussion](https://news.ycombinator.com/item?id=50432831)

**Background**: TPUs (Tensor Processing Units) are Google's custom-designed ASICs for accelerating machine learning workloads, now in their eighth generation. The agentic AI era refers to AI systems that can autonomously perform multi-step tasks, which demand efficient inference on long contexts and secure handling of sensitive data. Google offers TPUs through its Cloud platform rather than as standalone hardware products.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/infrastructure-and-cloud/global-network/tpu-8i-max-and-8tx/">Introducing TPU 8 tx and TPU 8 i Max</a></li>
<li><a href="https://www.servethehome.com/google-tpu-8i-for-inference-and-tpu-8t-for-training-announced/">Google TPU 8 i for Inference and TPU 8 t for Training... - ServeTheHome</a></li>

</ul>
</details>

**Discussion**: Community members questioned the lack of cost and performance metrics, asking for watts/token and $/token comparisons against NVIDIA equivalents. Others expressed frustration that Google Colab still only offers the older v6e-1 TPU, and one commenter asked why Google doesn't sell these chips directly.

**Tags**: `#TPU`, `#AI hardware`, `#Google Cloud`, `#AI infrastructure`, `#NVIDIA competition`

---

<a id="item-5"></a>
## [Google Gemini routes personal Drive files and emails to human annotators](https://github.com/thisisme6598/gemini_files/) ⭐️ 8.0/10

A GitHub report reveals that consumer Google Gemini with Connected Apps can route personal Drive files and emails to human annotators for review, sparking privacy concerns. This occurs when users authorize apps like Gmail, allowing Gemini to load data that may be subject to human review. This revelation highlights a significant privacy risk for consumers using Gemini's connected apps, as personal data may be exposed to human reviewers. It also underscores the growing tension between AI convenience and data privacy, potentially affecting user trust and adoption of such features. The human review applies specifically to consumer Gemini with Connected Apps, while Workspace Gemini and Workspace Intelligence for enterprise claim not to be subject to human review. Users should be aware that authorizing apps like Gmail may lead to their data being used for product improvement, including human annotation.

hackernews · gf74918 · Nov 9, 18:24 · [Discussion](https://news.ycombinator.com/item?id=50429426)

**Background**: Google Gemini is an AI assistant that can connect to various Google services like Gmail and Drive through Connected Apps, allowing it to access and use personal data to perform tasks. Human annotation involves people reviewing data to improve AI models, which is common in AI training but raises privacy concerns when applied to personal information. Google's privacy policies differ between consumer and enterprise versions, with consumer data potentially used for training and review.

<details><summary>References</summary>
<ul>
<li><a href="https://support.google.com/gemini/answer/16836988?hl=en-TJ">About personalisation with Connected Apps - Gemini Apps Help</a></li>
<li><a href="https://www.deai.org/news/does-google-gemini-train-on-your-data">Does Google Gemini Train on Your Data? What the Policy Says ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed frustration and concern, noting that consumer Gemini with Connected Apps is subject to human review while enterprise versions are not. Some shared anecdotes of Gemini responses that seemed eerily tuned to their emails, and others criticized the erosion of privacy norms and the use of human annotators for AI training.

**Tags**: `#privacy`, `#Google Gemini`, `#AI data handling`, `#human annotation`, `#consumer AI`

---

<a id="item-6"></a>
## [Browser tool finds every satellite that passed over any place in the last week](https://www.watched.earth/) ⭐️ 8.0/10

A new Show HN project called Watched Earth lets users type any location and see every satellite that passed over it in the last 7 days, along with actual Sentinel-2, Landsat, and NASA imagery from those passes. The tool runs SGP4 orbit propagation on the CelesTrak catalog entirely in the browser, completing the search in about half a second. This tool makes satellite imagery accessible to a broad audience by combining precise orbital mechanics with real imagery, which is valuable for geospatial professionals, outdoor planners, and anyone curious about what has photographed their area. It demonstrates how complex orbital computations can be performed efficiently in a web browser, potentially inspiring similar interactive geospatial applications. The pass search is verified against brute force at poles, the antimeridian, and tiny swaths with zero missed passes, and all ~17k objects are rendered on the GPU by solving Kepler's equation every frame. The tool only labels a location as 'watched' if a real image exists, and it does not store user locations; the developer notes that Sentinel-2 timestamps are often 5-10 minutes off from actual overpass time.

hackernews · a585gupt · Nov 9, 17:51 · [Discussion](https://news.ycombinator.com/item?id=50428907)

**Background**: SGP4 is a widely used orbit propagation algorithm that takes a Two-Line Element (TLE) set and predicts a satellite's position over time, accounting for perturbations like atmospheric drag and Earth's oblateness. CelesTrak is a public catalog that provides TLE data for thousands of satellites. Kepler's equation relates the geometry of an orbit to time and must be solved numerically for elliptical orbits, which is computationally intensive when done for many objects every frame.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Simplified_perturbations_models">Simplified perturbations models - Wikipedia</a></li>
<li><a href="https://celestrak.org/satcat/">CelesTrak : Satellite Catalog (SATCAT)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Kepler's_equation">Kepler ' s equation - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters enthusiastically praised the project, with one calling it 'the best combination of style and substance I have ever seen.' A geospatial professional noted it stands out from other satellite overview sites because it shows the exact image taken, and another user found it great for planning backpacking trips, saying it offers more data and easier access than Copernicus.

**Tags**: `#satellite-imagery`, `#geospatial`, `#webgl`, `#orbital-mechanics`, `#show-hn`

---

<a id="item-7"></a>
## [LingBot-Touch: JEPA-style tactile pretraining outperforms reconstruction for dexterous manipulation](https://www.reddit.com/r/MachineLearning/comments/1xs05uo/latent_prediction_beats_reconstruction_for/) ⭐️ 8.0/10

Robbyant released LingBot-Touch, a JEPA-style self-supervised tactile encoder that predicts latent representations of masked contact instead of reconstructing raw sensor signals, with inference code and checkpoints publicly available. On tactile-to-video top-5 recall at 1K hours, it achieves 32.1% versus 5.6% for MAE and 4.4% for VAE, and at 4K hours it reaches 49.3% while MAE stays under 9% and VAE drops to 3.1%. This work provides strong empirical evidence that latent prediction objectives, as in JEPA, are substantially more effective than reconstruction-based objectives like MAE and VAE for learning from sparse tactile signals, which could shift the design of self-supervised pretraining for robotic manipulation. The public release of code and checkpoints enables reproducibility and further research in tactile representation learning. The masking ratio warms up from 40% to 80% over 300 steps to avoid gradient explosions caused by hiding all contacting taxels in sparse signals, and three sensor types (magnetic, piezoresistive, visuotactile) are unified through canonical fingertip coordinates with 5D RoPE (time, finger, 3D position). On 26 real robot tasks with 4 policies, frozen encoder features scored highest in 89 of 104 policy-task combinations, and on a magnetic hand unseen during pretraining, LingBot-VLA improved from 57.21 to 75.04.

reddit · r/MachineLearning · /u/Zealousideal-War7154 · Nov 9, 18:52

**Background**: JEPA (Joint Embedding Predictive Architecture) is a self-supervised learning approach that predicts abstract representations of masked input rather than reconstructing raw data, as popularized by I-JEPA for images. Masked autoencoders (MAE) and variational autoencoders (VAE) are reconstruction-based methods that learn by recovering the original input from a corrupted version. Tactile sensors, such as magnetic, piezoresistive, and visuotactile types, produce sparse signals where most of a clip is near-zero background, making reconstruction objectives potentially misleading.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2301.08243">[2301.08243] Self-Supervised Learning from Images with a ...</a></li>
<li><a href="https://www.turingpost.com/p/jepa">JEPA: Joint Embedding Predictive Architecture Explained</a></li>
<li><a href="https://cs.brown.edu/media/filer_public/31/63/316378e6-8031-46cf-8f32-c3a13269e5bf/ghandikota.pdf">The ’Ill-Posed’ Reconstruction Gap of Masked Autoencoders</a></li>

</ul>
</details>

**Tags**: `#self-supervised-learning`, `#tactile-sensing`, `#JEPA`, `#robotics`, `#dexterous-manipulation`

---

<a id="item-8"></a>
## [USPS Releases Official ZIP Code Boundary Polygons with Steep Price Tag](https://postalpro.usps.com/zcb) ⭐️ 7.0/10

The United States Postal Service has released an official national dataset of ZIP Code boundary polygons through its PostalPro portal, with annual license tiers priced at $10,000, $33,000, and $150,000. The data includes four quarterly updates and is positioned as the ground truth for ZIP Code boundaries. This release addresses a long-standing need for authoritative ZIP Code boundaries used in mapping, logistics, insurance, and real estate, but its paywalled nature challenges federal open-data norms and may push many developers to continue using free but less precise Census ZCTAs. The pricing debate highlights broader tensions over public access to government geospatial data. The dataset is based on USPS delivery-address and location information and offers different limits on distribution and publication across the three tiers. Census ZCTAs remain a free alternative, though they are generalized areal representations built from census blocks and may lack some commercial-only ZIP Codes.

hackernews · munro · Nov 9, 19:58 · [Discussion](https://news.ycombinator.com/item?id=50431058)

**Background**: ZIP Codes were introduced in 1963 as delivery route identifiers, not as true geographic polygons, which makes representing them as boundaries inherently approximate. The Census Bureau created ZIP Code Tabulation Areas (ZCTAs) for statistical purposes, but these are generalized and not official USPS boundaries. Federal geospatial data is often expected to be freely available under open-data norms, making paid access to USPS boundaries controversial.

<details><summary>References</summary>
<ul>
<li><a href="https://postalpro.usps.com/zcb">USPS® ZIP Code Boundaries | PostalPro</a></li>
<li><a href="https://www.census.gov/programs-surveys/geography/guidance/geo-areas/zctas.html">ZIP Code Tabulation Areas (ZCTAs) - Census.gov</a></li>
<li><a href="https://runtimewire.com/article/usps-zip-code-boundary-polygons-license-price">USPS sells official ZIP Code boundary polygons at $10,000 to ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed frustration over the high price, arguing that federal data should be free for accountability and transparency, and questioned whether FOIA could apply. Others noted that free Census ZCTAs are close enough for many uses, while some pointed out the conceptual mismatch between ZIP Codes as delivery routes and polygons.

**Tags**: `#geospatial`, `#open-data`, `#government`, `#gis`, `#data-licensing`

---

<a id="item-9"></a>
## [Payments Canada launches Real-Time Rail payment system](https://www.payments.ca/canada-launches-real-time-rail-bringing-247-payment-infrastructure-national-economy) ⭐️ 7.0/10

Payments Canada has announced the launch of Canada's Real-Time Rail (RTR), a new 24/7 real-time payment system that enables irrevocable payments using the ISO 20022 messaging standard. The initial cohort of active participants includes Wealthsimple, Questbank, Peoples Trust Company, Paramount Commerce, KOHO, DoBusiness.com, Digital Commerce Bank, and Bank of America. The RTR provides a public real-time payment infrastructure that any bank or fintech can build on, potentially modernizing Canada's payment landscape and reducing reliance on proprietary systems like Interac e-Transfer. It also positions Canada alongside other countries with real-time payment rails, such as the UK's Faster Payments and India's UPI. The RTR uses the ISO 20022 financial messaging standard for all transactions and supports irrevocable payments 24/7/365. Notably, Canada's major banks are not among the initial participants, which may affect adoption and rollout speed.

hackernews · ocd · Nov 9, 16:00 · [Discussion](https://news.ycombinator.com/item?id=50427362)

**Background**: Real-time payment systems allow money to be transferred between accounts instantly and are increasingly being adopted globally. Payments Canada is the organization responsible for Canada's payment clearing and settlement infrastructure, and the RTR is its initiative to modernize the country's payments. The ISO 20022 standard is a global messaging standard for financial transactions that aims to improve data richness and interoperability.

<details><summary>References</summary>
<ul>
<li><a href="https://www.payments.ca/systems-services/payment-systems/real-time-rail-payment-system">Real - Time Rail payment system | Payments Canada</a></li>
<li><a href="https://www.payments.ca/real-time-rail-payment-system-0">Real - Time Rail payment system | Payments Canada</a></li>
<li><a href="https://www.finder.com/ca/banking/your-guide-to-real-time-rail-payments-in-canada">Real - Time Rail Payments : RTR Explained | Finder Canada</a></li>

</ul>
</details>

**Discussion**: Commenters generally view the RTR positively, with one Canadian noting it feels like a public version of Interac e-Transfer and praising the partnership with Interac. Others point out that major Canadian banks are absent from the initial participant list, and some compare it to other systems like M-PESA and criticize the US's FedNow for limited bank support and fees.

**Tags**: `#payments`, `#fintech`, `#real-time-payments`, `#canada`, `#infrastructure`

---

<a id="item-10"></a>
## [Semi-transparent colored CdTe panels tested for agrivoltaics](https://www.anthropocenemagazine.org/2026/10/magenta-solar-panels-may-be-agrivoltaics-cleverest-trick-yet/) ⭐️ 7.0/10

A study published in Cell Reports Physical Science evaluated land productivity using semi-transparent, magenta-colored cadmium telluride (CdTe) thin-film frameless photovoltaic panels (model ASP-LAM2 from Advanced Solar Power, Hangzhou) in an agrivoltaic setting. The colored layer is made of PVB encapsulant, and the panels allow some light through for crops while generating electricity. Agrivoltaics aims to resolve land competition between solar energy and agriculture, and semi-transparent colored panels could make dual use viable in greenhouses and on farmland by meeting crops' photosynthetic needs. If proven economically and agronomically sound, this approach could diversify farmer income and expand solar deployment without displacing food production. The panels are frameless CdTe thin-film modules with a magenta PVB encapsulant layer, supplied by Advanced Solar Power (Hangzhou, China). CdTe is a thin-film technology that is cheaper than crystalline silicon but typically 1–6% less efficient, and the semi-transparent design further reduces power output roughly in proportion to the light allowed through.

hackernews · speckx · Nov 9, 14:31 · [Discussion](https://news.ycombinator.com/item?id=50426175)

**Background**: Agrivoltaics (also called agrisolar or dual-use solar) is the practice of using the same land for both solar energy and agriculture, with panels installed between crops, elevated above them, or on greenhouses. Because panels consume light, there are trade-offs between crop yield and energy production, though some shade-tolerant crops can benefit. Cadmium telluride (CdTe) is a leading thin-film photovoltaic technology with a high optical absorption coefficient and a near-optimal bandgap of ~1.45 eV, allowing very thin films to absorb most of the solar spectrum; it holds over 30% of the U.S. utility-scale PV market. Semi-transparent colored solar cells are being explored specifically for greenhouse agrivoltaics, where they convert some light to electricity while transmitting enough for photosynthesis.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sciencedirect.com/science/article/pii/S2666386426004613">Evaluating land productivity with semi-transparent colored ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Agrivoltaics">Agrivoltaics</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cadmium_telluride_photovoltaics">Cadmium telluride photovoltaics - Wikipedia</a></li>

</ul>
</details>

**Discussion**: HN commenters were divided: a specialty cut flower grower noted that their USDA contact is skeptical of agrivoltaics due to past dealings with solar companies and a lack of reliable public data, while others argued that farmland is not dimensionally constrained in the U.S. and that 'stacking' solutions often introduce more problems than they solve. Counterpoints included that agrivoltaics is not an either-or question—individual farm owners may want extra revenue—and that a large share of U.S. corn is grown for ethanol, so replacing it with solar would not necessarily threaten food supply.

**Tags**: `#agrivoltaics`, `#solar-energy`, `#photovoltaics`, `#agriculture`, `#renewable-energy`

---

<a id="item-11"></a>
## [Meta releases Muse Ember, its smallest and most efficient model](https://research.meta.ai/blog/muse-ember) ⭐️ 7.0/10

Meta announced Muse Ember, its smallest and most efficient model to date, available via the Meta Model API at $0.10 per million input tokens and $0.50 per million output tokens. The model is designed for complex reasoning execution and high-volume agentic workflows such as repeated coding subtasks, tool calls, routing, and document processing. This release signals Meta's continued push into cost-efficient, agent-oriented models, but it also highlights growing competition in the small-model space where pricing and real-world utility are key differentiators. Developers building high-volume agent pipelines will need to weigh Ember's benchmark performance against cheaper alternatives and the lack of open weights. Muse Ember offers six effort levels (minimal, low, medium, high, xhigh, max) for reasoning, and Meta's benchmarks show its best results on the mini-swe-agent harness rather than Meta's own agent harness. The model is closed-weight, and community members note that competing models like DeepSeek V4.1 Flash can be accessed for less via OpenRouter.

hackernews · dvaplima · Nov 9, 17:58 · [Discussion](https://news.ycombinator.com/item?id=50429024)

**Background**: Meta Superintelligence Lab has been releasing a family of Muse models (including Spark and Wonder) that compete with other frontier LLMs. Small, efficient models are increasingly targeted at agentic workloads, where many low-cost calls are made for tasks like tool use and routing. The Meta Model API is Meta's platform for accessing these models, and pricing per token is a major factor for developers choosing between providers.

<details><summary>References</summary>
<ul>
<li><a href="https://research.meta.ai/blog/muse-ember">Introducing Our Smallest, Most Efficient Model: Muse Ember</a></li>
<li><a href="https://techcrunch.com/2026/11/09/meta-releases-muse-ember-a-new-lightweight-model-for-agent-execution/">Meta releases Muse Ember, a new lightweight model for agent ...</a></li>
<li><a href="https://dev.meta.ai/models/muse-ember">Muse Ember | Meta</a></li>

</ul>
</details>

**Discussion**: Commenters expressed skepticism about Muse Ember's real-world utility, with one noting that Meta's Muse models seem 'benchmaxxed' and not as useful in practice as benchmarks suggest. Others criticized the pricing as uncompetitive with alternatives like DeepSeek V4.1 Flash and lamented the lack of open weights, while one user observed that more reasoning tokens did not correlate with better SVG output in a visual test.

**Tags**: `#llm`, `#meta`, `#model-release`, `#efficiency`, `#benchmarks`

---

<a id="item-12"></a>
## [Simon Willison uses Claude Code to build Beep Locator](https://simonwillison.net/2026/Nov/9/mysterious-beeps/) ⭐️ 7.0/10

Simon Willison used Claude Code to build Beep Locator, a Python web app that triangulates a mysterious intermittent beep using multiple devices (phones, tablets, laptops) as microphones, locating the source to within about 40 cm. This project demonstrates how AI-assisted development can turn a frustrating real-world problem into a working multi-device acoustic sensing system in a short time, highlighting the practical potential of tools like Claude Code for rapid prototyping. The system uses a Python server with WebSocket-connected listeners that record 60-second audio buffers, and includes features like rough mode for manual device placement, clapping mode for testing, and frequency-specific detection; it successfully found an old carbon monoxide detector with low batteries.

rss · Simon Willison · Nov 9, 23:57

**Background**: Acoustic triangulation determines a sound's location by comparing the arrival times of the sound at multiple microphones. Claude Code is Anthropic's terminal-based AI coding agent that can autonomously write and run code. Beep Locator builds on research like BeepBeep, which uses acoustic signals for high-accuracy ranging between devices.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Nov/9/mysterious-beeps/">Locating the source of a mysterious beep with Claude</a></li>
<li><a href="https://en.wikipedia.org/wiki/Acoustic_location">Acoustic location - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>

</ul>
</details>

**Tags**: `#ai-assisted-development`, `#claude-code`, `#acoustic-triangulation`, `#web-app`, `#side-project`

---

<a id="item-13"></a>
## [XGBoost model forecasts new county-level power outages 2 hours ahead, beating NWS/SPC baselines by 2.4× PR-AUC](https://www.reddit.com/r/MachineLearning/comments/1xs4hq8/forecasting_new_power_outages_per_county_hourly_2/) ⭐️ 7.0/10

A new applied ML project forecasts the probability that at least 5% of a county's customers will experience new power outages in the 6-hour window starting 2 hours ahead, using XGBoost trained on HRRR storm data for 216 counties in Missouri and Illinois. On a held-out 2025 test year, the model achieved a PR-AUC of 0.094 versus 0.039 for a baseline combining NWS warnings and SPC Day 1 outlook, a ratio of about 2.4× (95% bootstrap range 2.0–3.3×). This work demonstrates that a gradient-boosted model using high-resolution weather forecasts can substantially outperform traditional alert-based baselines for predicting new power outages, which could improve pre-storm resource allocation for utilities. The open-source write-up, code, and leakage audit also provide a reproducible benchmark for applied ML in critical infrastructure. The model is trained on 2020–2024 data and tested on 2025 using HRRR forecasts as issued (mean of the last 5 runs) rather than observed weather, and it targets only new outages to avoid the trivial task of predicting ongoing ones. At equal alert volume, it catches 30% of new outages versus 17% for the baseline, with precision of 15% versus 11% against a base rate of 0.5% county-hours; an early transfer test to Iowa, Indiana, and Michigan showed 31% versus 19% recall.

reddit · r/MachineLearning · /u/CarRepresentative843 · Nov 9, 21:34

**Background**: The HRRR (High-Resolution Rapid Refresh) is a NOAA-operated weather model with high spatial resolution that provides short-range forecasts up to about 15–18 hours, often used for storm-related variables like wind gusts, shear, CAPE, and icing. XGBoost is an optimized gradient boosting library that builds an ensemble of decision trees sequentially to correct errors, widely used for tabular data. PR-AUC (area under the precision-recall curve) is a summary metric for imbalanced classification, where a high score indicates good performance in identifying rare positive events.

<details><summary>References</summary>
<ul>
<li><a href="https://windy.app/blog/nam-vs-hRrr-weather-models.html">NAM vs HRRR . Compare the major regional weather models for North...</a></li>
<li><a href="https://en.wikipedia.org/wiki/XGBoost">XGBoost - Wikipedia</a></li>
<li><a href="https://www.geeksforgeeks.org/machine-learning/precision-recall-curve-ml/">Precision-Recall Curve - ML - GeeksforGeeks</a></li>

</ul>
</details>

**Tags**: `#machine-learning`, `#power-outages`, `#forecasting`, `#xgboost`, `#applied-ml`

---

<a id="item-14"></a>
## [SwarmEvolve uses latent-agent swarms for faster math discovery](https://www.reddit.com/r/MachineLearning/comments/1xrunu7/using_latentagent_swarms_for_math_discovery_and/) ⭐️ 7.0/10

SwarmEvolve introduces a scalable framework that runs swarms of hundreds of latent-reasoning agents on Qwen3 8B, 14B, and 32B models, reaching scores in about 5 minutes that took OpenEvolve, ShinkaEvolve, and CodeEvolve over an hour. The agents reason in latent space and pass KV caches to each other, inspired by LatentMAS, enabling faster and cheaper math discovery and optimization. This work shows that combining latent-space reasoning with agent swarms can dramatically reduce the cost and time of LLM-driven program search, making evolutionary math discovery more accessible to researchers without massive compute. It also suggests a path toward applying such frameworks to real scientific problems in materials science, biology, and beyond. The framework works at every model size tested, and with just the 8B model it matched the best known circle packing result; it has also been extended to Qwen3.5 and Muse models with even better performance. The code is not yet publicly available but will be released on GitHub, and the approach relies on KV-cache passing between agents, which may raise interpretability and integrity concerns noted in related work.

reddit · r/MachineLearning · /u/QileHQ · Nov 9, 15:30

**Background**: AlphaEvolve, introduced by Google DeepMind, uses LLMs to write programs, score them, and iteratively improve them—an evolutionary approach that famously found a faster way to multiply 4x4 complex matrices, beating a record from 1969. However, AlphaEvolve runs on Gemini models, and open-source implementations like OpenEvolve are often slow and expensive. Latent reasoning refers to having LLMs reason in their hidden states rather than generating explicit text tokens, which can increase bandwidth and reduce generation steps, while LatentMAS is a multi-agent framework where agents communicate by passing latent thoughts instead of text.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/Gen-Verse/LatentMAS">GitHub - Gen-Verse/LatentMAS: [ICML 2026 Spotlight] Latent ...</a></li>
<li><a href="https://arxiv.org/html/2510.15522v1">Latent Reasoning in LLMs as a Vocabulary-Space Superposition</a></li>
<li><a href="https://arxiv.org/html/2511.09149v1">Enabling Agents to Communicate Entirely in Latent Space</a></li>

</ul>
</details>

**Tags**: `#AI/ML`, `#math discovery`, `#optimization`, `#LLM agents`, `#latent reasoning`

---

<a id="item-15"></a>
## [Twindex: Exact, Replayable Proofs of Parameter Non-Identifiability](https://www.reddit.com/r/MachineLearning/comments/1xryhhg/twindex_exact_replayable_proofs_that_your_data/) ⭐️ 7.0/10

Twindex is a new tool that finds 'twin' parameter sets which fit data equally well and produces exact, replayable JSON certificates proving this, demonstrated on SIR models and PINNs. A standard-library Python checker using rational arithmetic verifies each proof as VALID, INVALID, or INCONCLUSIVE. This addresses a fundamental gap in scientific machine learning: estimators like PINNs and Bayesian fits return a single parameter without proving that other very different parameters couldn't fit the data equally well. Twindex provides a rigorous, portable way to bound parameter recoverability, which could improve trust in models used for policy and scientific inference. The tool covers ODE models with polynomials, division, exp, sin, and cos (e.g., Michaelis-Menten, Hill, SIR, PK, predator-prey), 1-D/2-D elliptic and heat-equation PDEs, and any Python simulator as a numerical audit. Limitations include a bounded-noise assumption (not statistical), proofs conditional on the stated model and noise bound, scaling difficulty beyond a few parameters, and no independent expert audit yet.

reddit · r/MachineLearning · /u/Longjumping_Glass852 · Nov 9, 17:50

**Background**: Parameter identifiability is the property that determines whether model parameters can be uniquely estimated from data; failure to ensure it can lead to misleading estimates and unreliable policy recommendations, especially in epidemic models like SIR. Physics-informed neural networks (PINNs) are a type of universal function approximator that embeds physical laws (ODEs/PDEs) into the loss function to guide learning. Twindex builds on established bounded-error estimation with validated integration, adding portable exact certificates and a small checker that runs locally in the browser via Pyodide (WebAssembly).

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Physics-informed_neural_networks">Physics-informed neural networks - Wikipedia</a></li>
<li><a href="https://link.springer.com/article/10.1186/s13662-017-1078-5">Estimation of parameters in a structured SIR model</a></li>
<li><a href="https://pyodide.org/en/stable/index.html">Pyodide — Version 314.0.7</a></li>

</ul>
</details>

**Tags**: `#identifiability`, `#PINNs`, `#ODE`, `#PDE`, `#certificates`

---

<a id="item-16"></a>
## [Blog Post: Fable 5.2 One-Shots Nephew's Dream Game](https://notesbylex.com/fable-5-2-one-shotted-my-nephews-dream-game) ⭐️ 6.0/10

A blog post by Lex describes how the LLM Fable 5.2 generated his nephew's dream game in a single shot, sparking a Hacker News discussion with 158 comments comparing models and debating the significance of one-shot generation. This anecdotal example highlights the growing capability of LLMs like Fable 5.2 to produce complete, playable games from a single prompt, which could lower the barrier to entry for hobbyist game development and influence how AI-assisted coding tools are perceived. Commenters noted that one-shot success often depends on the harness and internal prompting that burns extra tokens to test everything, and that cost can be significant—one user spent $200 in credits on a single project. Others shared examples comparing Fable 5.2 with Opus 5.5, finding the latter more fun despite Fable's technical superiority.

hackernews · lexandstuff · Nov 9, 23:08 · [Discussion](https://news.ycombinator.com/item?id=50433659)

**Background**: Fable 5.2 is a large language model released by Anthropic, positioned as its most capable model for demanding technical work, with improvements in coding, reasoning, and vision over Fable 5.1. One-shot generation refers to an LLM producing a complete output in a single inference pass without iterative refinement. AI-assisted game development uses such models to prototype and build games, often via chat interfaces that generate code artifacts.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/claude-fable-and-mythos-5-2">Introducing Claude Fable 5 . 2 and Claude Mythos 5 . 2 \ Anthropic</a></li>
<li><a href="https://digifella.github.io/ai-wiki/concepts/one-shot-generation">one-shot-generation · NemoClaw</a></li>
<li><a href="https://tiorai.com/glossary/ai-assisted-game-development/">AI - assisted Game Development - TiorAI</a></li>

</ul>
</details>

**Discussion**: Commenters had mixed views: some enjoyed one-shotting simple games but cautioned against overemphasizing first-try success, noting that harness effects and token costs matter. Others shared personal experiences, such as building a WhatsApp sticker maker with Fable 5.1 credits but preferring a later Rust-based replacement built with less budget, and comparing Fable 5.2 with Opus 5.5 on a breakout game.

**Tags**: `#LLM`, `#game-development`, `#AI-assisted-coding`, `#one-shot-generation`, `#hacker-news`

---

<a id="item-17"></a>
## [Claude Ports Three.js Fabergé Egg Demo to Vanilla WebGL](https://simonwillison.net/2026/Nov/9/hn-50421091/) ⭐️ 6.0/10

Simon Willison asked Claude Opus 5.5 (Medium) to port a Three.js Nudibranch-themed Fabergé egg demo to vanilla JavaScript and WebGL, and the model produced a working 98KB version without Three.js. The original Three.js version was 77KB, and Willison noted the two are not identical. This demonstrates that a general-purpose LLM can handle low-level 3D graphics programming, potentially lowering the barrier for developers who want to avoid heavy libraries like Three.js. It also highlights how AI-assisted coding can quickly translate between abstraction layers in a real project. The ported version is larger (98KB vs 77KB) and not pixel-identical to the original; Willison says he doesn't fully understand why they differ and finds the Three.js code slightly easier to read himself. The demo was built in a regular Claude Chat thread, and a public transcript of the exchange is available.

rss · Simon Willison · Nov 9, 04:32

**Background**: Three.js is a popular JavaScript library that simplifies creating 3D graphics in the browser using WebGL, the low-level JavaScript API for GPU-accelerated rendering. Writing raw WebGL requires managing shaders and buffers manually, so libraries like Three.js are commonly used to abstract that complexity. A nudibranch is a colorful sea slug, and a Fabergé egg is an ornate jeweled egg, together forming the theme of the demo.

<details><summary>References</summary>
<ul>
<li><a href="https://threejs.org/">Three.js – JavaScript 3D Library</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/WebGL_API">WebGL : 2D and 3D graphics for the web - Web APIs | MDN</a></li>
<li><a href="https://en.wikipedia.org/wiki/Jorunna_funebris">Jorunna funebris - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#ai-assisted-coding`, `#threejs`, `#webgl`, `#claude`, `#hacker-news`

---

<a id="item-18"></a>
## [Simon Willison: Hide verbose AI PR descriptions behind <details><summary>](https://simonwillison.net/2026/Nov/9/details-summary/) ⭐️ 6.0/10

Simon Willison proposes wrapping lengthy AI-generated pull request descriptions in HTML <details><summary> tags so reviewers see a short human-written summary first and can expand the full agent-written text on demand. He now uses this pattern for PRs opened by Claude Code and Codex, labeling the collapsed section with the model name and effort level, such as "Claude Opus 5.5 Medium". As coding agents like Claude Code and Codex increasingly author PRs, their accurate but exhaustive descriptions can trigger reviewer fatigue and read like AI slop, discouraging careful review. This low-effort convention restores human editorial judgment at the top of a PR while preserving the detailed agent output for those who want it. The <details><summary> elements are supported in GitHub Markdown, so the tags can be dropped directly into PR descriptions or issue comments and render as a collapsed heading with an expansion arrow. Willison keeps a carefully written opening paragraph and sometimes a screenshot as the high-level explanation, with the full agent essay hidden below.

rss · Simon Willison · Nov 9, 04:25

**Background**: Coding agents such as Anthropic's Claude Code and OpenAI's Codex can open pull requests on a developer's behalf, bundling commits and writing detailed descriptions of the problem, solution, and verification steps. The HTML <details> element creates a disclosure widget whose visible heading is defined by its first child <summary> element, and GitHub renders this markup in Markdown fields. "Slop" refers to low-quality, mass-produced AI content, and reviewers increasingly associate long AI-written PR text with that label.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/summary">HTML disclosure summary element - HTML | MDN</a></li>
<li><a href="https://code.claude.com/">Claude Code by Anthropic | AI coding agent and assistant</a></li>
<li><a href="https://github.com/openai/codex">GitHub - openai/ codex : Lightweight coding agent that runs in your...</a></li>

</ul>
</details>

**Tags**: `#ai-coding-agents`, `#pull-requests`, `#developer-workflow`, `#code-review`, `#html`

---

<a id="item-19"></a>
## [Reddit discussion revisits why BatchNorm works](https://www.reddit.com/r/MachineLearning/comments/1xsasyf/did_we_ever_really_get_to_the_bottom_of_why/) ⭐️ 6.0/10

A Reddit post on r/MachineLearning asks whether the deep learning community ever truly resolved why Batch Normalization works, noting that the technique has fallen out of favor for being inconvenient despite its historical success. BatchNorm is one of the most widely used and empirically successful techniques in deep learning, yet its theoretical justification remains unsettled, which matters for researchers seeking principled architecture design and for practitioners choosing normalization methods. The original 2015 paper by Ioffe and Szegedy attributed BatchNorm's success to reducing internal covariate shift, but later work, including a 2018 MIT study, showed that BatchNorm does not actually solve internal covariate shift, leaving alternative explanations such as smoothing the loss landscape still debated.

reddit · r/MachineLearning · /u/XTXinverseXTY · Nov 10, 02:07

**Background**: Batch Normalization is a layer that normalizes the inputs to each network layer by re-centering and re-scaling them, introduced by Sergey Ioffe and Christian Szegedy in 2015. It became a standard component in deep networks because it sped up training and made initialization less sensitive, but its use has declined in some settings due to practical inconveniences such as dependence on batch size and different behavior at training versus inference time.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Batch_normalization">Batch normalization - Wikipedia</a></li>
<li><a href="https://arxiv.org/html/2003.00152">Training BatchNorm and Only BatchNorm :On the Expressive Power...</a></li>
<li><a href="https://www.analyticsvidhya.com/blog/2021/03/introduction-to-batch-normalization/">Introduction to Batch Normalization : Understanding the Basics</a></li>

</ul>
</details>

**Tags**: `#BatchNorm`, `#deep learning`, `#normalization`, `#machine learning theory`, `#Reddit discussion`

---

<a id="item-20"></a>
## [Paper-mining tool adds 2026 ICML/CVPR/ICLR/AAAI results, flags baseline inconsistencies](https://www.reddit.com/r/MachineLearning/comments/1xs6494/followup_2026_papers_are_finally_in_the_topic/) ⭐️ 6.0/10

A follow-up Reddit post announces that the Atlas paper-mining tool now covers 2026 ICML, CVPR, ICLR, and AAAI papers, extracting roughly one million 'tried X, got Y' benchmark findings from about 101k full texts. The author also published 'newspaper' summaries for ICML, CVPR, and ICLR 2026 comparing this year's trends with last year's. This tool gives ML researchers a centralized way to compare benchmark results across venues and years, and it highlights that reported baselines for the same method can vary widely, which complicates claims of improvement. The trend summaries also quantify shifts such as the growth of LLM agents and multimodal LLMs in top conferences. Coverage is nearly complete for ICML, CVPR, and AAAI 2026, with about 4.1k of 5.4k ICLR papers included, while NeurIPS 2026 is only over half done because many PDFs are not yet public. The author cautions that the numbers are AI-extracted without manual verification and that papers tend to over-report successful results, so the data should be used as a starting point rather than a leaderboard.

reddit · r/MachineLearning · /u/latenticlabs · Nov 9, 22:39

**Background**: Gaussian splatting is a volume rendering technique that represents 3D scenes with anisotropic 3D Gaussians, enabling real-time novel-view synthesis; it gained popularity after the seminal 3D Gaussian Splatting paper in 2023. Standard benchmarks like Mip-NeRF 360, Tanks & Temples, and Deep Blending are commonly used to evaluate such methods, but different implementations often use varying dataset loaders, evaluation protocols, and metrics, which makes cross-paper comparisons difficult.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gaussian_splatting">Gaussian splatting</a></li>
<li><a href="https://nerfbaselines.github.io/">NerfBaselines</a></li>
<li><a href="https://nerfbaselines.github.io/mipnerf360">NerfBaselines: Dataset Mip-NeRF 360</a></li>

</ul>
</details>

**Tags**: `#machine-learning`, `#research-tools`, `#benchmarks`, `#paper-mining`, `#reddit`

---

<a id="item-21"></a>
## [Reddit user fails to reproduce 'lost in the middle' on current models for easy retrieval](https://www.reddit.com/r/MachineLearning/comments/1xrn7lo/i_tried_to_reproduce_lost_in_the_middle_on/) ⭐️ 6.0/10

A Reddit user attempted to reproduce the 'lost in the middle' position bias on Claude Haiku 4.5 and Sonnet 5 using a synthetic needle-in-a-haystack test with 5, 15, and 30 documents, and found zero position sensitivity for easy single-fact retrieval. The only apparent flips at 30 documents (~4%) were due to formatting differences like '3' vs 'three', which disappeared after semantic comparison. This informal experiment challenges the assumption that the 'lost in the middle' effect is still a major issue for current models on simple retrieval tasks, suggesting that practitioners may not need to worry about document ordering for easy single-fact lookups. It also highlights the importance of using semantic rather than exact-string evaluation to avoid false positives. The test used made-up facts to prevent memorization, placed the answer document at every position among distractors, and compared model answers for consistency. The author notes caveats: only easy single-fact retrieval with short documents was tested, and the effect may still appear with long documents, multi-hop reasoning, or less obvious relevant information.

reddit · r/MachineLearning · /u/Beneficial_Use2116 · Nov 9, 09:22

**Background**: The 'lost in the middle' phenomenon refers to LLMs performing worse when relevant information is placed in the middle of a long context compared to the beginning or end, often visualized as a U-shaped curve. It was popularized by a 2023 paper and has been a concern for retrieval-augmented generation (RAG) systems, where document ordering might affect answer quality. Current models like Claude Haiku 4.5 and Sonnet 5 are recent releases with improved long-context capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/lost-in-the-middle">Lost in the Middle: Positional Bias in LLMs - emergentmind.com</a></li>
<li><a href="https://machinelearningplus.com/gen-ai/lost-in-the-middle-position-bias/">Lost-in-the-Middle: Fix LLM Position Bias (Python ...</a></li>
<li><a href="https://www.anthropic.com/claude/sonnet">Claude Sonnet \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#evaluation`, `#retrieval`, `#position bias`, `#reproducibility`

---

<a id="item-22"></a>
## [Foldable Flight paper airplane site sparks nostalgic Hacker News discussion](https://www.foldableflight.com/) ⭐️ 5.0/10

Foldable Flight, a website offering paper airplane designs and step-by-step video tutorials, was featured on Hacker News and garnered 884 points and 141 comments. The site's creator, Kyle, joined the discussion to share his passion for designing paper airplanes since childhood. The discussion highlights how simple, well-crafted hobbyist content can foster community and evoke nostalgia, even on a tech-focused forum like Hacker News. It underscores the enduring appeal of hands-on, screen-free activities in an increasingly digital world. The site features a large database of paper airplanes with video tutorials, including a 'Very Easy' 1-minute plane called Mystic that uses A4 paper. Community members shared personal stories about paper airplanes, and the creator, Kyle, actively engaged with comments.

hackernews · vismit2000 · Nov 9, 12:19 · [Discussion](https://news.ycombinator.com/item?id=50424581)

**Background**: Paper airplanes are a classic childhood craft, often made from a simple sheet of paper. Foldable Flight is a website that curates paper airplane designs and provides instructional videos, aiming to be the world's largest database of paper airplanes. Hacker News is a popular forum for technology and startup discussions, where off-topic but engaging content occasionally goes viral.

<details><summary>References</summary>
<ul>
<li><a href="https://www.foldableflight.com/">Foldable Flight: The Best Paper Airplanes in the World!</a></li>
<li><a href="https://www.foldnfly.com/">Fold 'N Fly » Paper Airplane Folding Instructions</a></li>

</ul>
</details>

**Discussion**: The discussion was overwhelmingly positive and nostalgic, with users sharing personal stories about making paper airplanes as children. Many appreciated the site's clear tutorials and the creator's engagement, and some expressed a desire to pass on the hobby to younger generations.

**Tags**: `#paper-airplanes`, `#hobbies`, `#nostalgia`, `#community-discussion`

---

<a id="item-23"></a>
## [Reddit User Asks About Building Image Diffusion Generator from Scratch on Home Hardware](https://www.reddit.com/r/MachineLearning/comments/1xs78e3/has_anyone_here_ever_built_an_image_generator/) ⭐️ 4.0/10

A Reddit user on r/MachineLearning asked whether anyone has built and trained an image diffusion generator from scratch on a home rig, and what model size and image quality they achieved. This question reflects growing interest among hobbyists in training generative models locally, which could democratize AI research and reduce reliance on large-scale compute. The post specifically asks for model size and whether coherent images were produced, indicating a focus on practical feasibility rather than theoretical novelty.

reddit · r/MachineLearning · /u/TheRPGGamerMan · Nov 9, 23:23

**Background**: Diffusion models are a class of generative models that learn to reverse a noise-adding process to create images, and they underpin popular systems like Stable Diffusion. Training such models from scratch typically requires significant computational resources, but recent work like the Home-made Diffusion Model (HDM) aims to make training feasible on consumer-grade hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Diffusion_model">Diffusion model - Wikipedia</a></li>
<li><a href="https://arxiv.org/html/2509.06068v1">Home-made Diffusion Model from Scratch to Hatch - arXiv.org</a></li>
<li><a href="https://medium.com/@thibaut.chauffier/training-diffusion-models-from-scratch-21d7a1f18e9e">Training Diffusion Models from Scratch - Medium</a></li>

</ul>
</details>

**Tags**: `#diffusion-models`, `#image-generation`, `#machine-learning`, `#home-training`, `#reddit-discussion`

---

<a id="item-24"></a>
## [Reddit user seeks advice for Amazon applied science PhD internship interview](https://www.reddit.com/r/MachineLearning/comments/1xrkiaw/amazon_applied_science_intern_interview_next_week/) ⭐️ 3.0/10

A Reddit user posted in r/MachineLearning asking for advice on preparing for an upcoming Amazon applied science PhD internship interview in the EU, specifically the DSA/coding portion they have never practiced. This post highlights the common challenge PhD candidates face when transitioning to industry roles that require coding interview preparation, even for research-oriented positions. The user has two interviews scheduled next week and feels confident about the machine learning breadth portion but anxious about the DSA/coding part, having never studied it or used LeetCode and relying on AI for coding recently.

reddit · r/MachineLearning · /u/ade17_in · Nov 9, 06:31

**Background**: Amazon's applied science internships are research-oriented roles that typically involve machine learning projects. However, interviews often include a coding component testing data structures and algorithms (DSA), commonly prepared via platforms like LeetCode. Many PhD students with strong ML backgrounds may lack recent coding practice, creating a gap between their research skills and interview expectations.

<details><summary>References</summary>
<ul>
<li><a href="https://igotanoffer.com/en/advice/amazon-applied-scientist-interview">Amazon Applied Scientist Interview (process, questions, prep)</a></li>
<li><a href="https://en.wikipedia.org/wiki/LeetCode">LeetCode</a></li>

</ul>
</details>

**Tags**: `#career-advice`, `#interview-preparation`, `#amazon`, `#machine-learning`, `#reddit`

---

<a id="item-25"></a>
## [EACL 2027 Acceptance Decisions to Be Announced Thursday](https://www.reddit.com/r/MachineLearning/comments/1xrv8mp/eacl_2027_decisions_thread_r/) ⭐️ 3.0/10

A Reddit thread on r/MachineLearning notes that EACL 2027 acceptance decisions will be released on Thursday, though no specific date or further details are provided. This announcement is significant for authors who submitted papers to EACL 2027, as it marks the moment they will learn whether their work has been accepted for presentation at the conference in Athens, Greece, in March 2027. EACL 2027 will take place in Athens, Greece, from March 9–14, 2027, and acceptance decisions are made by Senior Area Chairs and Program Chairs based on ARR reviews and meta-reviews after authors commit their reviewed articles to the venue.

reddit · r/MachineLearning · /u/Dry_Theme_7508 · Nov 9, 15:52

**Background**: EACL is the flagship conference of the European Chapter of the Association for Computational Linguistics, covering a broad spectrum of computational approaches to natural language. The conference uses a review process where papers are first reviewed through ACL Rolling Review (ARR), and authors then commit their reviewed papers to a specific venue like EACL for acceptance decisions.

<details><summary>References</summary>
<ul>
<li><a href="https://2027.eacl.org/">2027.eacl.org - The 20th Conference of the European Chapter</a></li>
<li><a href="https://2027.eacl.org/calls/papers/">EACL 2027 Call for Papers</a></li>
<li><a href="https://eacl.org/conferences/">EACL</a></li>

</ul>
</details>

**Tags**: `#EACL`, `#academic-conference`, `#NLP`, `#peer-review`, `#reddit`

---