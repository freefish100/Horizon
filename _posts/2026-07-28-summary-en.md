---
layout: default
title: "Horizon Summary: 2026-07-28 (EN)"
date: 2026-07-28
lang: en
---

> From 31 items, 9 important content pieces were selected

---

1. [Kimi K3: Open-Weight 2.8T Model Tops Frontend Code Arena](#item-1) ⭐️ 9.0/10
2. [Critical gadget-free RCE in Fastjson 1.x (1.2.68-1.2.83), no patch available](#item-2) ⭐️ 9.0/10
3. [Anthropic Clarifies Stance on Open-Weights Models](#item-3) ⭐️ 8.0/10
4. [Judge Rejects Google's DMCA Claim to Block Scraping](#item-4) ⭐️ 8.0/10
5. [Updated guide to AI models emphasizes agentic systems](#item-5) ⭐️ 8.0/10
6. [Structural Admission: Verify Dependency Structure Before Interpreting Learning](#item-6) ⭐️ 8.0/10
7. [Google Reveals Gemini 4 as Most Ambitious Pre-training Yet](#item-7) ⭐️ 8.0/10
8. [SMIC Tests China's First Domestic DUV Lithography Machine](#item-8) ⭐️ 8.0/10
9. [Moonshot AI to Open-Source 3T-Parameter Kimi-K3](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Kimi K3: Open-Weight 2.8T Model Tops Frontend Code Arena](https://t.me/zaihuapd/42793) ⭐️ 9.0/10

Moonshot AI released Kimi K3, an open-weight 2.8 trillion parameter model with novel Kimi Delta Attention and Attention Residuals architecture, achieving the highest score of 1679 in the Frontend Code Arena, surpassing previous leaders. Kimi K3 marks a significant milestone in open-weight large models, demonstrating that innovations in attention architecture can achieve state-of-the-art performance in specialized coding benchmarks, potentially lowering barriers for developers and enterprises. The model features a 1 million token context window and native vision capabilities; its 1.56TB weights are released under a custom license requiring a separate agreement for large-scale Model-as-a-Service providers.

telegram · zaihuapd · Jul 27, 06:27

**Background**: Kimi Delta Attention (KDA) is a linear attention mechanism that extends Gated DeltaNet with fine-grained diagonal gating for efficient memory use. Attention Residuals (AttnRes) replace standard residual connections with learned, input-dependent attention over depth, enabling selective aggregation of earlier representations. These architectural innovations allow K3 to achieve high performance with reduced computational overhead compared to dense transformers.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2510.26692">[2510.26692] Kimi Linear: An Expressive, Efficient Attention ... GitHub - MoonshotAI/Kimi-Linear GitHub - hwilner/kimi-delta-attention: Educational ... Kimi Linear: An Expressive, Efficient Attention Architecture KDA (Kimi Delta Attention) | fla-org/flash-linear-attention ...</a></li>
<li><a href="https://arxiv.org/abs/2603.15031">[2603.15031] Attention Residuals</a></li>
<li><a href="https://aitoolhunt.co/blog/kimi-k3-benchmarks-frontend-code-arena-2026">Kimi K3 Benchmarks: Frontend Leap and Review... | AIToolHunt</a></li>

</ul>
</details>

**Tags**: `#AI/ML`, `#Large Language Models`, `#Open Source`, `#Architecture`, `#Benchmarks`

---

<a id="item-2"></a>
## [Critical gadget-free RCE in Fastjson 1.x (1.2.68-1.2.83), no patch available](https://t.me/zaihuapd/42797) ⭐️ 9.0/10

Security researcher Kirill Firsov disclosed a high-risk remote code execution (RCE) vulnerability in Fastjson versions 1.2.68 through 1.2.83 that requires no gadget chains or autoType support and is exploitable on JDK 8, 17, and 21. Fastjson 1.x is widely used in production, but it reached end-of-life in October 2024, leaving no official patch; the only mitigation is upgrading to Fastjson2, which may cause compatibility issues and urgent deployment pressure. The vulnerability does not require enabling autoType or any specific classpath gadgets, making it a zero-click RCE; it affects the final 1.x release 1.2.83 and earlier versions back to 1.2.68.

telegram · zaihuapd · Jul 27, 10:31

**Background**: Fastjson is a popular Java JSON library developed by Alibaba. Historically, many Fastjson RCE vulnerabilities required either enabling autoType (which allows type specification) or relying on gadget chains (existing classes on the classpath that execute commands during deserialization). This new vulnerability bypasses both requirements, making it significantly easier to exploit.

<details><summary>References</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/fastjson-1x-rce-vulnerability-targeted.html">Fastjson 1.x RCE Vulnerability Targeted in Attacks With No Patched Available</a></li>
<li><a href="https://x.com/k_firsov/status/2078872293745570032">Kirill Firsov on X: "We found a gadget-free RCE in Fastjson 1.2.83 - the final release of the 1.x line, and still one of the most widely-deployed Java JSON libraries in production today, even with 2.x around. No classpath gadget. One payload-> RCE. https://t.co/8pbjl1M8y7" / X</a></li>
<li><a href="https://www.sentinelone.com/vulnerability-database/cve-2025-70974/">CVE-2025-70974: Fastjson AutoType RCE Vulnerability</a></li>

</ul>
</details>

**Discussion**: The disclosure on social media has caused widespread concern, with many developers expressing urgency to migrate to Fastjson2 given the lack of a patch. Some note that the vulnerability underscores the risks of relying on end-of-life libraries.

**Tags**: `#security`, `#rce`, `#fastjson`, `#vulnerability`, `#java`

---

<a id="item-3"></a>
## [Anthropic Clarifies Stance on Open-Weights Models](https://www.anthropic.com/news/position-open-weights-models) ⭐️ 8.0/10

Anthropic released a blog post stating it does not advocate for banning open-weights models, but supports mandatory safety testing for all sufficiently capable AI models, both open and closed. This stance has been criticized by some as de facto regulation that could hinder open-source AI development. This marks a major AI company's explicit policy position on open-weights models, influencing the ongoing debate between open AI development and safety regulation. The policy could set a precedent for how governments and companies treat open-weights models, potentially affecting innovation and accessibility in the AI ecosystem. Anthropic's proposal includes mandatory safety testing for capable models, but does not specify who would administer the tests or what criteria would be used. Critics argue that such testing could become a bureaucratic barrier that disadvantages open-source projects, similar to past government licensing schemes.

hackernews · surprisetalk · Jul 27, 22:03 · [Discussion](https://news.ycombinator.com/item?id=49076057)

**Background**: Open-weights models refer to AI models whose trained parameters (weights) are publicly released, allowing anyone to download, use, and modify them. Unlike open-source models, open-weights models may not include training code or data. The debate around open-weights models centers on balancing innovation and accessibility with risks of misuse, such as generating harmful content or enabling malicious applications.

<details><summary>References</summary>
<ul>
<li><a href="https://allthings.how/what-is-an-open-weight-ai-model-and-how-to-use-one/">What is an Open Weight AI Model and How to Use One</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>

</ul>
</details>

**Discussion**: Community comments are highly critical of Anthropic's position, accusing the company of hypocrisy for supporting chip export bans while opposing open-weights model bans. Commenters like 'cogman10' and 'GodelNumbering' argue that mandatory testing could be used to de facto ban open-weights models, similar to past government actions. Others, such as 'vhantz', suggest Anthropic's true motive is to protect its own closed, expensive models from competition.

**Tags**: `#AI safety`, `#open-weights`, `#regulation`, `#Anthropic`, `#policy`

---

<a id="item-4"></a>
## [Judge Rejects Google's DMCA Claim to Block Scraping](https://www.techdirt.com/2026/07/27/judge-rejects-googles-attempt-to-dmca-its-way-out-of-being-scraped/) ⭐️ 8.0/10

A U.S. federal judge ruled that Google cannot use the Digital Millennium Copyright Act (DMCA) to prevent third parties from scraping its search engine results pages (SERPs). The decision rejects Google's argument that scraping its SERPs constitutes circumvention of a technological protection measure. This ruling clarifies that web scraping of publicly accessible data is not automatically copyright infringement or DMCA circumvention, which has broad implications for data access, competition, and the balance of power between large platforms and smaller data users. It also highlights the tension when companies like Google, built on web crawling, attempt to restrict others from doing the same. The court found that Google's search results are not protected by copyright based on the selection and arrangement of facts, as they lack sufficient originality. Additionally, Google's argument that scraping violated the DMCA by bypassing its rate-limiting and bot detection measures did not hold because those measures were not considered effective technological protection measures under the DMCA.

hackernews · cdrnsf · Jul 27, 18:15 · [Discussion](https://news.ycombinator.com/item?id=49073513)

**Background**: The Digital Millennium Copyright Act (DMCA) is a U.S. law that criminalizes circumvention of technological protection measures (TPM) controlling access to copyrighted works. Web scraping is the automated extraction of data from websites, often used for price comparison, research, and monitoring. Google had argued that its SERPs are a copyrighted database and that measures like CAPTCHAs and rate limits are TPMs, which the court rejected.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Digital_Millennium_Copyright_Act">Digital Millennium Copyright Act</a></li>
<li><a href="https://en.wikipedia.org/wiki/Web_scraping">Web scraping</a></li>

</ul>
</details>

**Discussion**: Commenters expressed mixed reactions: some criticized Google for removing its search API and then suing those who scrape, calling it hypocritical. Others noted the irony that Google's own business model relies on crawling others' content. One comment highlighted the difference between EU and US copyright law regarding database protection. Overall, the sentiment was supportive of the ruling, with skepticism toward Google's tactics.

**Tags**: `#scraping`, `#DMCA`, `#Google`, `#legal`, `#web scraping`

---

<a id="item-5"></a>
## [Updated guide to AI models emphasizes agentic systems](https://simonwillison.net/2026/Jul/27/an-opinionated-guide-to-which-ai-to-use-to-do-stuff/#atom-everything) ⭐️ 8.0/10

Ethan Mollick published an updated opinionated guide on which AI to use for tasks, now focusing on agentic systems like ChatGPT Work and Claude Cowork instead of pure chat. This guide provides a curated, practical overview for users to choose the right AI tool, reflecting a major industry shift towards agentic AI that can autonomously perform hours of human work. The guide notes that Gemini is no longer recommended because Google lacks a competitive entry in the Codex/ChatGPT Work/Cowork category; also, the naming of modes across platforms (Work, Codex, Cowork, Code) is confusing and does not map consistently.

rss · Simon Willison · Jul 27, 21:55

**Background**: Agentic AI systems perceive, think, and act autonomously to achieve user-set goals, moving beyond simple chatbots that only respond to prompts. ChatGPT Work and Claude Cowork are agent modes designed for longer, multi-step tasks with finished deliverables. Google's later entry Gemini Spark is a 24/7 personal AI agent, but it has yet to prove itself in this competitive category.

<details><summary>References</summary>
<ul>
<li><a href="https://help.openai.com/en/articles/20001275-chatgpt-work-and-codex">ChatGPT Work and Codex - OpenAI Help Center</a></li>
<li><a href="https://gemini.google/overview/agent/spark/">Gemini Spark – Your 24/7 personal AI agent for productivity</a></li>
<li><a href="https://www.relativity.com/blog/agentic-ai-is-in-the-air/">Agentic AI is in the aiR | Relativity Blog</a></li>

</ul>
</details>

**Tags**: `#AI`, `#LLMs`, `#Agentic AI`, `#Productivity`

---

<a id="item-6"></a>
## [Structural Admission: Verify Dependency Structure Before Interpreting Learning](https://www.reddit.com/r/MachineLearning/comments/1v8insy/structural_admission_verify_a_sequential_tasks/) ⭐️ 8.0/10

A new Python harness called Structural Admission allows researchers to verify claimed dependency structures in sequential tasks before interpreting learning results, using a calibration and oracle-based procedure. This tool addresses a critical methodological gap in causal inference and reinforcement learning, preventing over-interpretation of learning curves, transfer, or emergence as evidence for causal structures that may not exist. The tool enforces calibration seeds disjoint from rollout seeds, uses a Conditional Mutual Information (CMI) threshold calibrated from synthetic data, and tests under both random and scripted oracle policies, reporting Admitted, Rejected, or Inconclusive.

reddit · r/MachineLearning · /u/willybbrown · Jul 28, 00:39

**Background**: In sequential decision-making tasks, researchers often interpret agent behavior as evidence of internal causal structures, but such claims require verification under the same observation and action interfaces the learner faces. Structural Admission provides a standardized, preregistered verification pipeline to ensure that any dependency structure claimed is actually present before learning experiments are interpreted.

**Tags**: `#reinforcement learning`, `#causal inference`, `#machine learning`, `#verification`, `#emergence`

---

<a id="item-7"></a>
## [Google Reveals Gemini 4 as Most Ambitious Pre-training Yet](https://9to5google.com/2026/07/26/google-gemini-4-teases/) ⭐️ 8.0/10

Google CEO Sundar Pichai announced during the Alphabet Q2 2026 earnings call that Gemini 4, the company's next major AI model, has entered pre-training, calling it their most ambitious pre-training project to date, with a target release in late 2026. This announcement signals Google's continued heavy investment in frontier AI, potentially accelerating progress towards artificial general intelligence (AGI) and maintaining competitive pressure on rivals like OpenAI and Anthropic. Pichai stated that Google will prioritize compute allocation for cutting-edge AGI R&D to ensure Gemini 4 remains at the forefront upon release, while the Gemini 3.x Flash series will continue monthly iterations focusing on capabilities like intelligent coding.

telegram · zaihuapd · Jul 27, 04:06

**Background**: Pre-training is the initial phase of training large language models on vast amounts of unlabeled data to capture general knowledge and patterns. AGI (Artificial General Intelligence) is a hypothetical AI that matches or surpasses human cognitive abilities across virtually all tasks. Google's Gemini series competes with models like GPT-4 and Claude.

<details><summary>References</summary>
<ul>
<li><a href="https://www.geeksforgeeks.org/artificial-intelligence/what-is-pre-training-and-its-objective/">What is Pre Training and its Objective - GeeksforGeeks</a></li>
<li><a href="https://en.wikipedia.org/wiki/Artificial_general_intelligence">Artificial general intelligence - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Google`, `#Gemini 4`, `#AI`, `#Large Language Model`, `#Pre-training`

---

<a id="item-8"></a>
## [SMIC Tests China's First Domestic DUV Lithography Machine](https://t.me/zaihuapd/42800) ⭐️ 8.0/10

SMIC is reportedly trial-running China's first advanced deep ultraviolet (DUV) lithography machine developed by Shanghai startup Yuliangsheng, aiming to produce 28nm chips and explore 7nm via multi-patterning. This milestone signals China's push for semiconductor self-sufficiency, potentially reducing reliance on imports like ASML's DUV equipment, though it will take years to match commercial viability. The machine uses mostly domestic components but still relies on some imported parts; SMIC targets mass production by 2027, with current trials at 28nm and lower yields for 7nm.

telegram · zaihuapd · Jul 27, 14:10

**Background**: Deep ultraviolet (DUV) lithography uses 193nm or 248nm light to pattern circuits on silicon wafers, and is widely used for mature nodes (28nm and above). Multi-patterning can extend DUV to produce features as small as 7nm by splitting a single layer into multiple exposures. In contrast, EUV lithography uses 13.5nm light and is required for advanced nodes like 5nm, but is barred from sale to China due to US export controls.

<details><summary>References</summary>
<ul>
<li><a href="https://eureka.patsnap.com/article/what-is-deep-ultraviolet-lithography-duv-and-how-does-it-work">What is Deep Ultraviolet Lithography (DUV) and how does it work?</a></li>
<li><a href="https://en.wikipedia.org/wiki/Multiple_patterning">Multiple patterning - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/EUV_lithography">EUV lithography - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#DUV lithography`, `#China tech`, `#SMIC`, `#chip manufacturing`

---

<a id="item-9"></a>
## [Moonshot AI to Open-Source 3T-Parameter Kimi-K3](https://t.me/zaihuapd/42802) ⭐️ 8.0/10

Moonshot AI announced it will open-source Kimi-K3, a 3-trillion-parameter frontier model, on Hugging Face, with weights expected to be released on July 27, 2026. The model introduces a novel architecture featuring Kimi Delta Attention and Attention Residuals, and offers built-in agentic capabilities for tool calling, web browsing, and multi-step planning. This is a significant milestone as it would be the largest open-source model by parameter count (3T), potentially democratizing access to frontier-scale AI. It could accelerate research in long-context coding, knowledge work, and complex reasoning, and set a new standard for open-source model capabilities. Kimi-K3 uses Kimi Delta Attention, a delta-rule based linear attention mechanism with channel-wise forgetting for fine-grained memory updates, and Attention Residuals (AttnRes), which replace standard residual connections with learned attention over depth. The model is designed for repository-level code understanding with an extended context window.

telegram · zaihuapd · Jul 27, 15:15

**Background**: Large language models (LLMs) typically use attention mechanisms to process sequences, but standard attention scales quadratically with sequence length. Linear attention variants like Mamba and Gated DeltaNet aim to reduce this cost. Kimi Delta Attention improves on these with fine-grained decay, while Attention Residuals enhance depth-wise information flow. Open-sourcing models at this scale (3T parameters) is rare; previous largest open-source models are around 400B parameters.

<details><summary>References</summary>
<ul>
<li><a href="https://jianyuh.github.io/attention/2025/12/13/KDA.html">Linear Attention : Kimi Delta Attention | Jianyu Huang’s Blog</a></li>
<li><a href="https://arxiv.org/abs/2603.15031">[2603.15031] Attention Residuals - arXiv.org GitHub - MoonshotAI/Attention-Residuals Attention Residuals - arXiv.org Attention Residuals wdlctc/open-attention-residuals - GitHub Attention Residuals - openlm.ai Attention Residuals Explained: Rethinking Transformer Depth</a></li>
<li><a href="https://github.com/MoonshotAI/Attention-Residuals">GitHub - MoonshotAI/Attention-Residuals</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#large language model`, `#Kimi-K3`, `#Moonshot AI`, `#3T parameters`

---