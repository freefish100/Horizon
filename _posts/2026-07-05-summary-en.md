---
layout: default
title: "Horizon Summary: 2026-07-05 (EN)"
date: 2026-07-05
lang: en
---

> From 39 items, 9 important content pieces were selected

---

1. [Prompt injection leaks YouTube creators' private videos](#item-1) ⭐️ 9.0/10
2. [Huawei's 'Tao's Law' Proposes Time Scaling to Replace Moore's Law](#item-2) ⭐️ 9.0/10
3. [GPT-5.5 Codex Token Clustering Causes Reasoning Degradation](#item-3) ⭐️ 8.0/10
4. [Google Books scan bounty: $200k for complete scans](#item-4) ⭐️ 8.0/10
5. [Session/Cache Leakage May Cause LLM Response Swaps Between Users](#item-5) ⭐️ 8.0/10
6. [Newer Claude Models Regress in Tool Call Schema Adherence](#item-6) ⭐️ 8.0/10
7. [BaryGraph: Knowledge Graph with Embedded Relationships as Documents](#item-7) ⭐️ 8.0/10
8. [South Korea plans $800B semiconductor cluster, DRAM output to double in 5 years](#item-8) ⭐️ 8.0/10
9. [Hong Kong handles over half of China's chip imports, record high](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Prompt injection leaks YouTube creators' private videos](https://javoriuski.com/post/youtube) ⭐️ 9.0/10

A prompt injection vulnerability in YouTube Studio's AI comment features allows attackers to leak the titles and URLs of creators' private videos by leaving a specially crafted comment. This vulnerability exposes creators' private content, violating their privacy and security, and highlights the real-world risk of prompt injection in widely-used platforms like YouTube. The attack works when a creator clicks an AI-generated comment suggestion; the injected prompt causes the AI to include private video information in its response. Not all testers were able to reproduce the exploit.

hackernews · javxfps · Jul 4, 16:45 · [Discussion](https://news.ycombinator.com/item?id=48786781)

**Background**: Prompt injection is a cybersecurity exploit where malicious inputs cause a large language model (LLM) to behave unintentionally. YouTube Studio uses AI to suggest replies to comments, and if a crafted comment is injected, it can hijack the AI's output to leak sensitive data.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>
<li><a href="https://www.reddit.com/r/antiai/comments/1ll76nx/youtube_studio_is_now_making_ai_content/">r/antiai on Reddit: YouTube Studio is now making AI content suggestions ...</a></li>

</ul>
</details>

**Discussion**: An ex-Google engineer commented that organizational complexity may be why YouTube is slow to fix this. Others praised the article's clarity and noted that the exploit works in some cases but not all, suggesting it may depend on specific conditions.

**Tags**: `#security`, `#prompt injection`, `#YouTube`, `#vulnerability`, `#Hacker News`

---

<a id="item-2"></a>
## [Huawei's 'Tao's Law' Proposes Time Scaling to Replace Moore's Law](https://t.me/zaihuapd/42346) ⭐️ 9.0/10

At the 2026 International Symposium on Circuits and Systems in Shanghai, Huawei unveiled 'Tao's Law,' a new semiconductor scaling principle based on time scaling instead of geometric scaling. Huawei has already designed and mass-produced 381 chips using this principle over the past six years, and plans to launch a new Kirin chip with logic folding technology this fall. Tao's Law offers a potential path beyond Moore's Law, which is approaching physical limits, by optimizing multiple layers from devices to systems through reduced time constants. If successful, it could extend the semiconductor industry's roadmap and reduce reliance on extreme miniaturization, impacting global chip design and manufacturing. The principle was formally published on ChinaXiv on May 25, 2026, in a paper titled 'A Time Scaling Theory for Multi-Layer Electronic Systems.' Huawei predicts that by 2031, high-end chips based on this law could achieve transistor density equivalent to a 1.4nm process. Logic folding involves vertical stacking of chip components to reduce signal travel distance.

telegram · zaihuapd · Jul 4, 04:56

**Background**: For decades, the semiconductor industry has followed Moore's Law, which predicts that transistor density doubles roughly every two years through geometric scaling—shrinking transistor size. However, as physical limits near, alternative approaches are needed. Time scaling focuses on reducing the time constant (τ) of circuits, improving performance through architectural and system-level optimizations rather than purely shrinking dimensions.

<details><summary>References</summary>
<ul>
<li><a href="https://chinaainews.org/news/huawei-s-tao-law-proposes-time-based-scaling-to-replace-moore-s-law-in-semiconductors">Huawei' s ' Tao Law ' Proposes Time -Based Scaling to Replace...</a></li>
<li><a href="https://www.linkedin.com/pulse/huaweis-tau-law-signals-new-direction-semiconductor-industry-dx8me">Huawei’s “Tau Law” Signals a New Direction for the Semiconductor ...</a></li>
<li><a href="https://www.geeky-gadgets.com/huawei-logic-folding-moores-law/">Huawei Logic Folding : A New Approach to... - Geeky Gadgets</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#Huawei`, `#Moore's Law`, `#chip design`, `#time scaling`

---

<a id="item-3"></a>
## [GPT-5.5 Codex Token Clustering Causes Reasoning Degradation](https://github.com/openai/codex/issues/30364) ⭐️ 8.0/10

Users have reported that GPT-5.5 Codex occasionally short-circuits after exactly 516 reasoning tokens, producing incorrect results on complex tasks. This behavior is linked to a token clustering phenomenon where reasoning output tokens cluster at fixed intervals of 518. This regression undermines trust in OpenAI's flagship coding assistant, Codex, and may push users to alternative models like Claude or local models. The reproducible issue suggests a fundamental flaw in the model's adaptive reasoning mechanism, which could impact developer productivity and tool reliability. The issue is reproducible using the Codex CLI with puzzle prompts, where the model uses exactly 516 thinking tokens when it should use 6000-8000. The token clustering appears as spikes at fixed values spaced 518 apart, strongly correlated with errors in complex tasks.

hackernews · maille · Jul 4, 21:51 · [Discussion](https://news.ycombinator.com/item?id=48789428)

**Background**: GPT-5.5 was released in April 2026 with improved efficiency, using fewer tokens for Codex tasks. Token clustering is a technique where similar tokens are grouped to reduce computational cost, but in this case, it appears to cause the model to prematurely stop reasoning when hitting a cluster boundary. OpenAI's Codex is a widely used AI coding assistant built on GPT models.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48789428">GPT-5.5 Codex reasoning-token clustering may be leading to degraded performance | Hacker News</a></li>
<li><a href="https://openai.com/index/introducing-gpt-5-5/">Introducing GPT-5.5 | OpenAI</a></li>
<li><a href="https://blogs.nvidia.com/blog/openai-codex-gpt-5-5-ai-agents/">OpenAI’s New GPT-5.5 Powers Codex on NVIDIA Infrastructure | NVIDIA Blog</a></li>

</ul>
</details>

**Discussion**: Users expressed frustration, with some recalling similar regressions in Claude Code earlier. One user noted that the model's quality has degraded over months and switched to Claude. Another user considered per-token pricing to use multiple models flexibly. Overall sentiment is negative, with calls for OpenAI to take the issue seriously.

**Tags**: `#GPT-5.5`, `#codex`, `#AI performance`, `#regression`, `#OpenAI`

---

<a id="item-4"></a>
## [Google Books scan bounty: $200k for complete scans](https://software.annas-archive.gl/AnnaArchivist/annas-archive/-/work_items/234) ⭐️ 8.0/10

A $200,000 bounty has been offered to scan all books from Google Books or similar digital library platforms, posted on Anna's Archive by the user AnnaArchivist. This bounty targets a major bottleneck in digital library access, potentially making millions of books freely available and greatly expanding knowledge equity, especially for users in regions with limited access. The bounty is hosted on Anna's Archive, a shadow library that aggregates content from sources like Z-Library and Library Genesis, and the reward is for scanning all books from Google Books or similar services.

hackernews · Cider9986 · Jul 4, 16:51 · [Discussion](https://news.ycombinator.com/item?id=48786838)

**Background**: Anna's Archive is a search engine for shadow libraries, providing access to millions of books and academic papers often behind paywalls. Bounties are used to incentivize the scanning of physical books or accessing restricted digital collections to expand the archive's holdings.

**Discussion**: Community comments show strong support: a user from Tunisia expressed gratitude for access to English books, SourceLibrary.org shared their 50,000-rare-book archive, and another user recounted finding a hard-to-locate CD zip file via Anna's Archive. Some speculated about future bounties for internet scrapes, and one user questioned the identity of the team behind the project.

**Tags**: `#digital libraries`, `#bounty`, `#open access`, `#copyright`, `#book scanning`

---

<a id="item-5"></a>
## [Session/Cache Leakage May Cause LLM Response Swaps Between Users](https://github.com/anthropics/claude-code/issues/74066) ⭐️ 8.0/10

Reports have emerged of session or cache leakage causing language model responses to be swapped between different users or workspace instances, with multiple providers affected including Claude and GPT models, and one provider issuing a postmortem citing an API gateway bug related to HTTP 100 status codes. This vulnerability could lead to cross-tenant data leakage in multi-tenant LLM infrastructure, potentially exposing sensitive information from one user to another. As LLM usage becomes widespread, such security flaws undermine trust in the infrastructure and highlight the need for robust isolation mechanisms. The reported postmortem from one provider revealed that their API gateway incorrectly handled HTTP 100 status codes, causing an off-by-one error in session handling. Similar patterns have been observed with Gemini and other models, with some users reporting responses that appear to belong to other users' contexts.

hackernews · chatmasta · Jul 4, 14:03 · [Discussion](https://news.ycombinator.com/item?id=48785485)

**Background**: In multi-tenant SaaS systems, multiple users share the same underlying infrastructure, including caches and session stores, for efficiency. If isolation between tenants is not properly enforced, data from one tenant can leak into another's responses. Cross Session Leak is a known vulnerability where sensitive information from one user's session bleeds into another's, often due to shared GPU caches or context objects.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@instatunnel/multi-tenant-leakage-when-row-level-security-fails-in-saas-da25f40c788c">Multi-Tenant Leakage: When “Row-Level Security” Fails in SaaS | by InstaTunnel | Medium</a></li>
<li><a href="https://www.giskard.ai/knowledge/cross-session-leak-when-your-ai-assistant-becomes-a-data-breach">Cross Session Leak: LLM security vulnerability & detection guide</a></li>

</ul>
</details>

**Discussion**: The community is divided: some users report experiencing similar issues across multiple providers, while others suspect hallucination. A Claude Code team member acknowledged the report and stated the team is investigating but believes it to be a hallucination. Users express concern about potential private information leakage even if not yet observed.

**Tags**: `#security`, `#llm`, `#privacy`, `#cache`, `#infrastructure`

---

<a id="item-6"></a>
## [Newer Claude Models Regress in Tool Call Schema Adherence](https://simonwillison.net/2026/Jul/4/better-models-worse-tools/#atom-everything) ⭐️ 8.0/10

Armin Ronacher reported that newer Claude models (Opus 4.8, Sonnet 5) invent extra fields in tool call arguments, causing Pi's edit tool to reject valid edits, while older models do not exhibit this issue. This regression highlights a counterintuitive trend where state-of-the-art models perform worse at specific tool-use tasks, which is critical for developers building AI coding harnesses and other third-party tooling that rely on strict schema adherence. The issue is attributed to Anthropic training newer models via reinforcement learning to better use Claude Code's built-in edit tools, inadvertently degrading performance on third-party tools like Pi's hash-anchored edit tool.

rss · Simon Willison · Jul 4, 22:53

**Background**: Tool call schemas define the exact structure of arguments an LLM must provide when invoking an external function. Models are often fine-tuned or reinforced to excel at specific tools (e.g., Claude Code's built-in editor), which can cause them to become less reliable with other custom schemas. This phenomenon suggests that model-level optimization for first-party tools may come at the cost of general tool-use fidelity.

<details><summary>References</summary>
<ul>
<li><a href="https://letsdatascience.com/news/newer-claude-models-show-tool-calling-regression-6f029d5f">Newer Claude Models Show Tool-Calling Regression | Let's Data Science</a></li>
<li><a href="https://dev.to/gentic_news/claude-code-regression-how-to-diagnose-and-fix-the-recent-quality-drop-hmg">Claude Code Regression: How to Diagnose and Fix the Recent Quality Drop - DEV Community</a></li>
<li><a href="https://github.com/can1357/oh-my-pi">GitHub - can1357/oh-my-pi: ⌥ AI Coding agent for the terminal — hash-anchored edits, optimized tool harness, LSP, Python, browser, subagents, and more</a></li>

</ul>
</details>

**Tags**: `#AI models`, `#tool use`, `#model regression`, `#schema adherence`, `#Anthropic`

---

<a id="item-7"></a>
## [BaryGraph: Knowledge Graph with Embedded Relationships as Documents](https://www.reddit.com/r/MachineLearning/comments/1un3lsf/barygraph_knowledge_graph_where_every/) ⭐️ 8.0/10

BaryGraph introduces a novel knowledge graph where each relationship is embedded as a first-class vector document called a BaryEdge, enabling recursive construction of MetaBary triads that bridge distant concepts. The system is built and runs locally on a full English Wiktionary dataset with 6.6 million documents using MongoDB and nomic-embed-text. This approach addresses a fundamental limitation of flat vector search, which fails to capture conceptual bridges between distant but related concepts. By making relationships retrievable documents, BaryGraph enables cross-domain semantic retrieval that could enhance RAG systems, recommendation engines, and scientific discovery. The BaryEdge vector is computed as a weighted combination of node embeddings and relationship type embeddings, with a connection quality parameter q. Structural metrics from the graph correlate with human similarity judgments (ρ ≈ 0.32–0.53, p < 10⁻¹⁵), while raw cosine similarity shows negligible correlation (ρ ≈ −0.04 on SimLex-999). The graph is a forest, allowing efficient traversal with a single $graphLookup operation.

reddit · r/MachineLearning · /u/adseipsum · Jul 4, 08:24

**Background**: Traditional knowledge graphs represent relationships as edges between nodes, where the semantic meaning is only implicit in the proximity of node embeddings. In standard RAG and vector search, relationships are not directly indexed, so conceptually related but distant items remain disconnected. BaryGraph reifies each relation as an independent vector document, enabling recursive abstraction layers that uncover cross-domain bridges.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reddit.com/r/mongodb/">r/mongodb</a></li>

</ul>
</details>

**Tags**: `#Knowledge Graph`, `#Embedding`, `#RAG`, `#Vector Search`, `#Semantic Retrieval`

---

<a id="item-8"></a>
## [South Korea plans $800B semiconductor cluster, DRAM output to double in 5 years](https://t.me/zaihuapd/42357) ⭐️ 8.0/10

South Korea's Ministry of Trade, Industry and Energy announced a national semiconductor cluster plan, investing 800 trillion KRW (about 3.52 trillion RMB) to build four memory fabs in the southwestern region, aiming to double DRAM production within five years. This massive investment reinforces South Korea's dominance in the global memory market and positions the country to capitalize on an anticipated fourfold growth in the memory market over the next five years. It also highlights the intensifying global race for semiconductor manufacturing leadership. The plan includes a second semiconductor production base in the southwestern region and an additional 30 trillion KRW (about 1.32 trillion RMB) from the government over 15 years. Minister Kim Jung-kwan emphasized the need for speed to maintain leadership.

telegram · zaihuapd · Jul 4, 15:15

**Background**: South Korea is a global leader in memory semiconductors, especially DRAM and NAND flash. The semiconductor cluster plan aims to create a self-contained ecosystem with fabs, suppliers, and R&D centers, similar to existing clusters in the Seoul metropolitan area. The memory market is cyclical, and South Korea seeks to preempt capacity expansion to meet future demand.

**Tags**: `#semiconductors`, `#DRAM`, `#South Korea`, `#investment`, `#manufacturing`

---

<a id="item-9"></a>
## [Hong Kong handles over half of China's chip imports, record high](https://thenextweb.com/news/hong-kong-china-ai-chip-trade-hub) ⭐️ 8.0/10

In the first five months of 2026, Hong Kong handled over half of China's chip imports, with re-exports to the mainland valued at about $124 billion, accounting for 52% of China's total chip purchases during the period. This proportion has risen from one-third a decade ago, setting a new record. This trend underscores Hong Kong's emergence as a critical transit hub for AI trade in Asia, leveraging its free-port status and advanced logistics. However, its intermediary role also exposes it to significant geopolitical risks amid US-China tensions. AI-related electronics now account for 57% to 70% of Hong Kong's exports, prompting the Hong Kong Trade Development Council to raise its 2026 export growth forecast to over 20%. Hong Kong's advantages include zero tariffs, no capital controls, and a developed air cargo network suitable for high-value, low-weight semiconductors.

telegram · zaihuapd · Jul 5, 02:45

**Background**: Hong Kong has historically been a major re-export hub due to its free trade policies and strategic location. The surge in chip imports via Hong Kong reflects growing AI demand in China and the city's unique advantages in handling high-value, time-sensitive goods. This trend also highlights the deepening integration of Hong Kong into the mainland's semiconductor supply chain.

**Tags**: `#半导体`, `#香港`, `#AI`, `#贸易`, `#地缘政治`

---