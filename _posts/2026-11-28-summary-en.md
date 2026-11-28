---
layout: default
title: "Horizon Summary: 2026-11-28 (EN)"
date: 2026-11-28
lang: en
---

> From 7 items, 7 important content pieces were selected

---

1. [Google's DeepCrossAttention achieves comparable model quality up to 3x faster](#item-1) ⭐️ 7.0/10
2. [WebRTC-based credit card skimming scripts found on popular shopping sites](#item-2) ⭐️ 7.0/10
3. [Convex skill plugin allegedly uploads user app ideas without consent](#item-3) ⭐️ 7.0/10
4. [Show HN: Bouncemarket, a live prediction market game for a bouncing ball](#item-4) ⭐️ 7.0/10
5. [Virginia and Oregon sue SpaceX over Grok generating CSAM and revenge porn](#item-5) ⭐️ 7.0/10
6. [Michael Nielsen Removes Free Neural Networks Book, Sparking AI Debate](#item-6) ⭐️ 7.0/10
7. [datasette-charts 0.4a0 refines plugin hook and adds docs site](#item-7) ⭐️ 5.0/10

---

<a id="item-1"></a>
## [Google's DeepCrossAttention achieves comparable model quality up to 3x faster](https://research.google/blog/supercharging-transformer-residual-connections/) ⭐️ 7.0/10

Google Research introduced DeepCrossAttention (DCA), a new architecture that enhances transformer residual connections by using learnable, input-dependent weights and depth-wise cross-attention to dynamically combine outputs from previous layers. This approach prevents information dilution and achieves comparable model quality up to 3x faster than traditional transformers. This development could significantly improve the efficiency of training and inference for transformer models, which are widely used in natural language processing and beyond. Faster training with comparable quality can reduce computational costs and enable broader access to advanced AI models. DCA generalizes self-attention by adding three independent instances of a GRN (Global Response Normalization) in each decoder block, with the GRN considered to be GRN-v3. The method uses depth-wise cross-attention for Query, Key, and Value components to selectively focus on relevant information from any previous layer.

hackernews · ComputedCamp995 · Nov 27, 23:06 · [Discussion](https://news.ycombinator.com/item?id=50672565)

**Background**: Transformers rely on residual connections (skip connections) to train deep networks by allowing information to bypass layers, which helps mitigate vanishing gradients. However, traditional residual connections simply sum the outputs of previous layers, which can dilute crucial information. DeepCrossAttention modifies this by using learnable weights to dynamically combine layer outputs, enabling the model to focus on the most relevant information.

<details><summary>References</summary>
<ul>
<li><a href="https://research.google/blog/supercharging-transformer-residual-connections/">Supercharging transformer residual connections - Google Research</a></li>
<li><a href="https://arxiv.org/abs/2502.06785">[2502.06785] DeepCrossAttention: Supercharging Transformer ...</a></li>
<li><a href="https://www.baeldung.com/cs/transformer-networks-residual-connections">Why Are Residual Connections Important in Transformer ...</a></li>

</ul>
</details>

**Discussion**: Community comments compared DCA to DenseNet, noting architectural parallels. Some discussed practical implications for inference speed, with one user reporting 10x tokens/sec improvements from related techniques and wondering if DCA could push it to 30x. Others mentioned the cost-effectiveness of models like Gemini Neon, possibly related to such efficiency improvements.

**Tags**: `#transformers`, `#attention-mechanisms`, `#deep-learning`, `#model-efficiency`, `#google-research`

---

<a id="item-2"></a>
## [WebRTC-based credit card skimming scripts found on popular shopping sites](https://www.infohawk.com/news/2026-11-27-black-friday-webrtc-skimmer) ⭐️ 7.0/10

Security researchers have discovered credit card skimming scripts that abuse WebRTC to exfiltrate payment data on popular e-commerce sites, with the campaign timed around Black Friday. The scripts bypass Content Security Policy (CSP) protections and primarily target mobile devices, making detection harder. This finding highlights the persistent risk of third-party scripts on e-commerce sites and raises concerns about WebRTC's privacy implications, as users cannot easily disable the API. It affects online shoppers, website owners, and browser vendors, and has sparked debate about ad-blocking and browser privacy controls. The skimmer leverages WebRTC data channels to send stolen card data, evading CSP and bypassing traditional monitoring; researchers note that similar attacks could be performed with simple HTTP requests, but WebRTC is less frequently monitored for malicious behavior. Mobile devices are targeted because they are harder to inspect.

hackernews · scanr · Nov 27, 15:40 · [Discussion](https://news.ycombinator.com/item?id=50668145)

**Background**: WebRTC (Web Real-Time Communication) is a browser API that enables real-time audio, video, and data communication without plugins. Credit card skimming scripts are malicious JavaScript injected into checkout pages to steal payment information, often via third-party services like Google Tag Manager. Content Security Policy (CSP) is a browser security mechanism that restricts which scripts can run on a page, but attackers continuously find ways to bypass it.

<details><summary>References</summary>
<ul>
<li><a href="https://www.digitalsamba.com/blog/webrtc-security">WebRTC Security: Best Practices and Key Risks Explained</a></li>
<li><a href="https://whoerip.com/blog/how-secure-is-webrtc/">How Secure Is WebRTC? Risks, Protection, And Real Use Cases</a></li>
<li><a href="https://www.searchenginejournal.com/hackers-use-google-tag-manager-to-steal-credit-card-numbers/539691/">Hackers Use Google Tag Manager to Steal Credit Card Numbers</a></li>

</ul>
</details>

**Discussion**: Commenters expressed frustration over WebRTC's inability to be disabled and criticized the reliance on third-party scripts, with some arguing that ad-blocking is justified as a security measure. Others noted that the attack is not unique to WebRTC and that any third-party script embedding creates vulnerability, while one user shared a personal experience of card fraud on Black Friday.

**Tags**: `#security`, `#web`, `#privacy`, `#e-commerce`, `#skimming`

---

<a id="item-3"></a>
## [Convex skill plugin allegedly uploads user app ideas without consent](https://github.com/convex/convex-backend-skill/issues/64) ⭐️ 7.0/10

A GitHub issue (convex/convex-backend-skill#64) alleges that Convex's skill plugin silently sends users' app ideas to a remote server. Convex CEO Jamie responded directly in the comments, clarifying that the prompt upload powers the Convex 'quickstart' feature and is the successor to the now-shut-down Convex Chef vibe-coding product. This incident highlights growing privacy and trust concerns around AI developer tools that silently transmit user prompts, and it shows how a single GitHub issue can escalate into a public debate when a CEO responds. It affects developers using Convex's AI-assisted tooling and raises broader questions about transparency in prompt handling across the ecosystem. The upload is tied to Convex's 'quickstart' feature, the spiritual successor to the discontinued Convex Chef end-to-end vibe-coding product. Community members noted that prompt injection is far more common than models making malicious tool calls on their own, and some questioned the issue author's motives given their promotion of a personal media site.

hackernews · MickyTheMouse · Nov 27, 18:02 · [Discussion](https://news.ycombinator.com/item?id=50669765)

**Background**: Convex is a full-stack platform for building and hosting software, including a database, server functions, and an AI gateway. The 'skill' plugin is an AI agent skill that helps developers scaffold Convex apps. Prompt injection is a security vulnerability where malicious input overrides developer instructions, and it is a major concern for AI coding tools that process untrusted data.

<details><summary>References</summary>
<ul>
<li><a href="https://learnprompting.org/docs/prompt_hacking/injection">Prompt Injection : Overriding AI Instructions with User Input</a></li>
<li><a href="https://sandeepkumarchaudhary.com/blog/prompt-injection-in-ai-coding-tools-how-the-attacks">Prompt Injection in AI Coding Tools : How the Attacks Actually Work</a></li>
<li><a href="https://www.kunalganglani.com/blog/indirect-prompt-injection-ai-agents">Indirect Prompt Injection in AI Agents: 10 Red-Team Tests</a></li>

</ul>
</details>

**Discussion**: The discussion was diverse: the CEO provided an official clarification, one commenter argued that self-hosted open-weight models are the long-term solution, another noted prompt injection is more common than malicious model tool calls, and a third dismissed the concern with 'ideas are cheap.' Some users also questioned the issue author's self-promotion, adding skepticism to the debate.

**Tags**: `#privacy`, `#developer-tools`, `#prompt-injection`, `#convex`, `#ai-security`

---

<a id="item-4"></a>
## [Show HN: Bouncemarket, a live prediction market game for a bouncing ball](https://bouncemarket.minhanhday.com/) ⭐️ 7.0/10

A developer launched bouncemarket, a live prediction market game where players bet on where a deterministically simulated bouncing ball will land, with server-side simulation streamed via server-sent events and AI traders that drop out when more than five humans join. The project demonstrates a novel combination of deterministic physics simulation, real-time streaming, and prediction market mechanics, and the discussion highlights how such games can become battles of AI bots, raising interesting questions about fairness and strategy in online markets. Each ball drop is fully deterministic from its starting position, allowing exact replay, but tiny variations in the starting position can drastically change the outcome; the AI traders use simple rule-based logic and are not hard to beat.

hackernews · mday404 · Nov 27, 15:01 · [Discussion](https://news.ycombinator.com/item?id=50667726)

**Background**: A prediction market is an exchange where participants trade contracts whose payoffs depend on future events, with prices reflecting the crowd's probability estimates. Server-sent events (SSE) is a web technology that lets a server push real-time updates to a browser over a single HTTP connection. Deterministic simulation means that given the same initial conditions, the simulation always produces the same outcome, which is useful for testing and replay.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prediction_market">Prediction market</a></li>
<li><a href="https://en.wikipedia.org/wiki/Server-sent_events">Server-sent events</a></li>
<li><a href="https://antithesis.com/docs/resources/deterministic_simulation_testing/">Deterministic simulation testing - how it works and... | Antithesis Docs</a></li>

</ul>
</details>

**Discussion**: Commenters found the game fun but noted that the drop is too fast to bet comfortably, and that simply buying cheap shares on both sides can guarantee a profit. One commenter suggested that prediction markets on pure random events could be as legal as sports betting, while another observed that with powerful AI models the game becomes a 'battle of the bots' where a frontier model could write an exact solver.

**Tags**: `#prediction-markets`, `#game-development`, `#server-sent-events`, `#deterministic-simulation`, `#AI-trading`

---

<a id="item-5"></a>
## [Virginia and Oregon sue SpaceX over Grok generating CSAM and revenge porn](https://www.oag.state.va.us/media-center/news-releases/jay-jones/3162-attorneys-general-jones-and-rayfield-file-suit-against-spacex-parent-company-of-x-xai-and-grok-over-creation-and-promotion-of-child-exploitation-and-non-consensual-images-on-platform) ⭐️ 7.0/10

Virginia Attorney General Jay Jones and Oregon Attorney General Dan Rayfield filed separate lawsuits against SpaceX, the parent company of xAI and X, alleging that the Grok AI image generator produced child sexual abuse material (CSAM) and non-consensual intimate imagery (NCII). The suits claim the companies prioritized their business model over user safety, marking the first state-level legal actions against SpaceX over Grok's outputs. This is a high-profile legal challenge that could set a precedent for holding AI companies accountable for harmful content generated by their models, potentially leading to stricter regulations and changes in how AI firms design safety filters. It affects not only xAI and SpaceX but the entire AI industry, as states signal they will pursue litigation over AI safety failures. The lawsuits specifically target Grok's generation of CSAM and NCII, with Virginia's attorney general stating that the companies' choices led to a proliferation of such material. The legal actions are separate but similar, filed in collaboration, and come amid ongoing debate over Section 230 immunity and First Amendment protections for AI-generated content.

hackernews · DeepLogin · Nov 27, 19:42 · [Discussion](https://news.ycombinator.com/item?id=50670855)

**Background**: Grok is an AI chatbot developed by xAI, which is owned by SpaceX, and it includes an image generation feature. CSAM refers to child sexual abuse material, which is illegal in the U.S., while NCII (non-consensual intimate imagery) includes deepfake pornography created without consent. State attorneys general have increasingly targeted AI companies for failing to prevent harmful outputs, and this case tests whether existing laws can hold AI developers liable.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/23/oregon-virginia-spacex-grok-deepfake-lawsuits.html">SpaceX sued by 2 states over AI deepfake porn, Grok ... - CNBC</a></li>
<li><a href="https://www.oag.state.va.us/media-center/news-releases/jay-jones/3162-attorneys-general-jones-and-rayfield-file-suit-against-spacex-parent-company-of-x-xai-and-grok-over-creation-and-promotion-of-child-exploitation-and-non-consensual-images-on-platform">Attorneys General Jones and Rayfield File Suit Against SpaceX ...</a></li>
<li><a href="https://apnews.com/article/grok-lawsuit-elon-musk-ai-abuse-images-452cc64e7169a55868f797982d0e8238">Sexual images from Elon Musk's AI chatbot harmed consumers ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed confusion about how Grok could generate such content if it is widely banned, with one asking whether users had to trick the AI. Another questioned whether the individuals creating the content would also face consequences, and a third raised a debated claim about Supreme Court precedent protecting AI-generated CSAM for personal use, while noting that revenge porn involves real people and may not be protected.

**Tags**: `#AI safety`, `#content moderation`, `#legal`, `#xAI`, `#policy`

---

<a id="item-6"></a>
## [Michael Nielsen Removes Free Neural Networks Book, Sparking AI Debate](https://neuralnetworksanddeeplearning.com/) ⭐️ 7.0/10

Michael Nielsen has taken down his free online book 'Neural Networks and Deep Learning' from its original site, prompting a Hacker News discussion with 422 points and 266 comments. The removal of a widely used open educational resource highlights tensions between open knowledge and concerns about AI safety and the concentration of AI power in large companies. The book remains accessible via the Internet Archive's Wayback Machine, and commenters noted that its removal may be a form of protest rather than a practical restriction.

hackernews · brandonb · Nov 27, 19:31 · [Discussion](https://news.ycombinator.com/item?id=50670757)

**Background**: Michael Nielsen's 'Neural Networks and Deep Learning' is a free online book that teaches the fundamentals of neural networks and deep learning. It has been a popular resource for learners since its release. Open educational resources like this are typically freely available for anyone to use and share.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Open_educational_resources">Open educational resources</a></li>

</ul>
</details>

**Discussion**: Commenters debated the move, with some arguing that educating people about AI helps prepare them for corporate AI outcomes, while others saw it as a symbolic protest against AI power concentration. Some also discussed the role of capital and ETFs in accelerating AI development.

**Tags**: `#AI safety`, `#open education`, `#neural networks`, `#community discussion`, `#AI industry`

---

<a id="item-7"></a>
## [datasette-charts 0.4a0 refines plugin hook and adds docs site](https://simonwillison.net/2026/Nov/27/datasette-charts/) ⭐️ 5.0/10

datasette-charts 0.4a0 refines its chart-type plugin hook based on friction found while building an experimental plugin, and adds a documentation site with a plugin-author tutorial and interactive chart gallery. This release makes it easier for developers to extend Datasette with custom chart types, improving the plugin ecosystem's ergonomics and lowering the barrier to creating visualizations. The new documentation site at charts.datasette.io includes a tutorial for plugin authors and a gallery of core charts and annotations, each linking to an interactive demo on Datasette Lite.

rss · Simon Willison · Nov 27, 23:57

**Background**: Datasette is an open-source tool for exploring and publishing data, and its plugins use plugin hooks to customize behavior. datasette-charts is a plugin that adds chart visualization capabilities, and this release focuses on its own plugin hook that allows other plugins to define new chart types. Datasette Lite is a version of Datasette that runs entirely in the browser using Pyodide.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.datasette.io/en/stable/plugin_hooks.html">Plugin hooks - Datasette documentation</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#plugins`, `#data-visualization`, `#release`, `#developer-tools`

---