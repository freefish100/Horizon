---
layout: default
title: "Horizon Summary: 2026-07-28 (ZH)"
date: 2026-07-28
lang: zh
---

> 从 31 条内容中筛选出 9 条重要资讯。

---

1. [Kimi K3：开源 2.8T 参数模型登顶前端编程挑战赛](#item-1) ⭐️ 9.0/10
2. [Fastjson 1.x (1.2.68-1.2.83) 存在无 gadget 高危 RCE 漏洞，无补丁可用](#item-2) ⭐️ 9.0/10
3. [Anthropic 阐明对开放权重模型的立场](#item-3) ⭐️ 8.0/10
4. [法官驳回 Google 利用 DMCA 阻止爬取的诉讼](#item-4) ⭐️ 8.0/10
5. [AI 模型更新指南：强调自主代理系统](#item-5) ⭐️ 8.0/10
6. [Structural Admission：在解释学习前验证依赖结构](#item-6) ⭐️ 8.0/10
7. [谷歌揭示 Gemini 4 为迄今最雄心预训练项目](#item-7) ⭐️ 8.0/10
8. [中芯国际测试中国首台国产 DUV 光刻机](#item-8) ⭐️ 8.0/10
9. [月之暗面将开源 3T 参数模型 Kimi-K3](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Kimi K3：开源 2.8T 参数模型登顶前端编程挑战赛](https://t.me/zaihuapd/42793) ⭐️ 9.0/10

月之暗面发布了 Kimi K3，这是一个拥有 2.8 万亿参数的开源权重模型，采用创新的 Kimi Delta Attention 和 Attention Residuals 架构，在 Frontend Code Arena 中获得 1679 分，排名第一，超越了之前的领先者。 Kimi K3 标志着开源权重大模型的一个重要里程碑，表明注意力架构的创新可以在专业化编程基准测试中取得最先进性能，可能降低开发者和企业的使用门槛。 该模型支持 100 万 token 的上下文窗口和原生视觉能力；其 1.56TB 的权重在自定义许可证下发布，要求大规模模型即服务提供商签署单独协议。

telegram · zaihuapd · 7月27日 06:27

**背景**: Kimi Delta Attention（KDA）是一种线性注意力机制，通过细粒度对角门控扩展了 Gated DeltaNet，以实现高效的内存使用。Attention Residuals（AttnRes）用学习到的、输入相关的深度注意替代了标准的残差连接，使得能够选择性聚合早期表示。这些架构创新使得 K3 能够在比密集 Transformer 更低的计算开销下实现高性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2510.26692">[2510.26692] Kimi Linear: An Expressive, Efficient Attention ... GitHub - MoonshotAI/Kimi-Linear GitHub - hwilner/kimi-delta-attention: Educational ... Kimi Linear: An Expressive, Efficient Attention Architecture KDA (Kimi Delta Attention) | fla-org/flash-linear-attention ...</a></li>
<li><a href="https://arxiv.org/abs/2603.15031">[2603.15031] Attention Residuals</a></li>
<li><a href="https://aitoolhunt.co/blog/kimi-k3-benchmarks-frontend-code-arena-2026">Kimi K3 Benchmarks: Frontend Leap and Review... | AIToolHunt</a></li>

</ul>
</details>

**标签**: `#AI/ML`, `#Large Language Models`, `#Open Source`, `#Architecture`, `#Benchmarks`

---

<a id="item-2"></a>
## [Fastjson 1.x (1.2.68-1.2.83) 存在无 gadget 高危 RCE 漏洞，无补丁可用](https://t.me/zaihuapd/42797) ⭐️ 9.0/10

Fastjson 1.x 在生产环境中广泛使用，但已于 2024 年 10 月停止维护，官方不会发布补丁；唯一缓解措施是升级到 Fastjson2，这可能引发兼容性问题并带来紧急部署压力。 该漏洞无需启用 autoType 或任何特定 classpath gadget，属于零点击远程代码执行；影响范围从 1.2.68 到最终的 1.2.83 版本。

telegram · zaihuapd · 7月27日 10:31

**背景**: Fastjson 是由阿里巴巴开发的流行 Java JSON 库。历史上，许多 Fastjson RCE 漏洞要么需要开启 autoType（允许指定类型），要么依赖 gadget 链（classpath 上现有类在反序列化期间执行命令）。这个新漏洞绕过了这两个要求，使其更容易被利用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/fastjson-1x-rce-vulnerability-targeted.html">Fastjson 1.x RCE Vulnerability Targeted in Attacks With No Patched Available</a></li>
<li><a href="https://x.com/k_firsov/status/2078872293745570032">Kirill Firsov on X: "We found a gadget-free RCE in Fastjson 1.2.83 - the final release of the 1.x line, and still one of the most widely-deployed Java JSON libraries in production today, even with 2.x around. No classpath gadget. One payload-> RCE. https://t.co/8pbjl1M8y7" / X</a></li>
<li><a href="https://www.sentinelone.com/vulnerability-database/cve-2025-70974/">CVE-2025-70974: Fastjson AutoType RCE Vulnerability</a></li>

</ul>
</details>

**社区讨论**: 该披露在社交媒体上引起广泛关注，许多开发者因无补丁而表达紧急升级到 Fastjson2 的意愿。部分人士指出，该漏洞凸显了依赖已停止维护库的风险。

**标签**: `#security`, `#rce`, `#fastjson`, `#vulnerability`, `#java`

---

<a id="item-3"></a>
## [Anthropic 阐明对开放权重模型的立场](https://www.anthropic.com/news/position-open-weights-models) ⭐️ 8.0/10

Anthropic 发布博客文章，声明不主张禁止开放权重模型，但支持对所有足够强大的 AI 模型（包括开放和封闭的）进行强制性安全测试。这一立场被一些人批评为事实上的监管，可能阻碍开源 AI 发展。 这标志着一家主要 AI 公司对开放权重模型的明确政策立场，影响关于开放 AI 开发与安全监管的持续辩论。该政策可能为政府和公司如何对待开放权重模型树立先例，潜在影响 AI 生态系统的创新和可获取性。 Anthropic 的提议包括对强大模型进行强制性安全测试，但未指定由谁管理测试或使用什么标准。批评者认为，这种测试可能成为官僚障碍，对开源项目不利，类似于过去的政府许可计划。

hackernews · surprisetalk · 7月27日 22:03 · [社区讨论](https://news.ycombinator.com/item?id=49076057)

**背景**: 开放权重模型是指其训练参数（权重）公开发布的 AI 模型，允许任何人下载、使用和修改。与开源模型不同，开放权重模型可能不包括训练代码或数据。关于开放权重模型的辩论集中在平衡创新和可访问性与误用风险（如生成有害内容或助力恶意应用）之间。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://allthings.how/what-is-an-open-weight-ai-model-and-how-to-use-one/">What is an Open Weight AI Model and How to Use One</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>

</ul>
</details>

**社区讨论**: 社区评论对 Anthropic 的立场高度批评，指责该公司支持芯片出口禁令的同时反对开放权重模型禁令是虚伪的。评论者如'cogman10'和'GodelNumbering'认为，强制性测试可能被用于事实上禁止开放权重模型，类似于过去的政府行动。其他人如'vhantz'则认为 Anthropic 的真正动机是保护自己的封闭高价模型免受竞争。

**标签**: `#AI safety`, `#open-weights`, `#regulation`, `#Anthropic`, `#policy`

---

<a id="item-4"></a>
## [法官驳回 Google 利用 DMCA 阻止爬取的诉讼](https://www.techdirt.com/2026/07/27/judge-rejects-googles-attempt-to-dmca-its-way-out-of-being-scraped/) ⭐️ 8.0/10

美国联邦法官裁定，Google 不能利用《数字千年版权法》（DMCA）阻止第三方爬取其搜索引擎结果页面（SERPs）。该判决驳回了 Google 关于爬取其 SERPs 构成规避技术保护措施的主张。 该裁决明确，对公开可访问数据的网页爬取并不自动构成版权侵权或违反 DMCA，这对数据获取、竞争以及大型平台与小型数据使用者之间的权力平衡具有广泛影响。它也凸显了像 Google 这样建立在网络爬取基础上的公司，试图限制他人进行同样行为时存在的矛盾。 法院认为，Google 的搜索结果在事实的选择和编排上缺乏足够的原创性，因此不受版权保护。同时，Google 关于爬取绕过其速率限制和机器人检测措施因而违反 DMCA 的论点不成立，因为这些措施不被视为 DMCA 下的有效技术保护措施。

hackernews · cdrnsf · 7月27日 18:15 · [社区讨论](https://news.ycombinator.com/item?id=49073513)

**背景**: 《数字千年版权法》（DMCA）是美国法律，将规避控制访问受版权作品的技术保护措施（TPM）定为犯罪。网页爬取是从网站自动提取数据，常用于价格比较、研究和监控。Google 曾主张其 SERPs 是受版权保护的数据库，而 CAPTCHA 和速率限制等措施属于 TPM，但法院驳回了这些论点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Digital_Millennium_Copyright_Act">Digital Millennium Copyright Act</a></li>
<li><a href="https://en.wikipedia.org/wiki/Web_scraping">Web scraping</a></li>

</ul>
</details>

**社区讨论**: 评论者反应不一：有人批评 Google 先移除搜索 API，再起诉爬取者，认为这是虚伪的。还有人指出，Google 自身的商业模式就依赖于爬取他人内容，这具有讽刺意味。一条评论强调了欧盟与美国在数据库保护方面的版权法差异。总体来看，舆论支持该裁决，并对 Google 的策略持怀疑态度。

**标签**: `#scraping`, `#DMCA`, `#Google`, `#legal`, `#web scraping`

---

<a id="item-5"></a>
## [AI 模型更新指南：强调自主代理系统](https://simonwillison.net/2026/Jul/27/an-opinionated-guide-to-which-ai-to-use-to-do-stuff/#atom-everything) ⭐️ 8.0/10

Ethan Mollick 发布了更新的 AI 使用指南，重点转向了如 ChatGPT Work 和 Claude Cowork 等自主代理系统，而非纯聊天模式。 该指南为用户提供了实用的 AI 工具选择参考，反映了行业向自主代理 AI 的重大转变，这类 AI 能自动完成数小时的人类工作。 指南指出，由于谷歌在 Codex/ChatGPT Work/Cowork 类别中缺乏竞争力，Gemini 已不再推荐；同时，各平台模式命名混乱（Work、Codex、Cowork、Code），无对应关系。

rss · Simon Willison · 7月27日 21:55

**背景**: 自主代理 AI 系统能够感知、思考并自主行动以实现用户设定的目标，超越了仅回应提示的简单聊天机器人。ChatGPT Work 和 Claude Cowork 是为长周期、多步骤任务设计的代理模式，能产出最终成果。谷歌晚些推出的 Gemini Spark 是一个 24/7 个人 AI 代理，但尚未在此竞争类别中证明自己。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://help.openai.com/en/articles/20001275-chatgpt-work-and-codex">ChatGPT Work and Codex - OpenAI Help Center</a></li>
<li><a href="https://gemini.google/overview/agent/spark/">Gemini Spark – Your 24/7 personal AI agent for productivity</a></li>
<li><a href="https://www.relativity.com/blog/agentic-ai-is-in-the-air/">Agentic AI is in the aiR | Relativity Blog</a></li>

</ul>
</details>

**标签**: `#AI`, `#LLMs`, `#Agentic AI`, `#Productivity`

---

<a id="item-6"></a>
## [Structural Admission：在解释学习前验证依赖结构](https://www.reddit.com/r/MachineLearning/comments/1v8insy/structural_admission_verify_a_sequential_tasks/) ⭐️ 8.0/10

一个名为 Structural Admission 的新 Python 工具使研究人员能够在解释学习结果之前验证顺序任务中声称的依赖结构，使用校准和基于先知（oracle）的程序。 该工具解决了因果推断和强化学习中的一个关键方法论空白，防止将学习曲线、迁移或涌现现象过度解释为可能不存在的因果结构的证据。 该工具强制要求校准种子与滚动种子不重叠，使用从合成数据校准的条件互信息（CMI）阈值，并在随机和脚本先知策略下进行测试，报告结果为通过（Admitted）、拒绝（Rejected）或不确定（Inconclusive）。

reddit · r/MachineLearning · /u/willybbrown · 7月28日 00:39

**背景**: 在顺序决策任务中，研究人员常常将智能体行为解释为内部因果结构的证据，但这种声称需要在学习者面对的相同观察和动作接口下进行验证。Structural Admission 提供了一个标准化的预注册验证流程，确保在解释学习实验之前，所声称的依赖结构确实存在。

**标签**: `#reinforcement learning`, `#causal inference`, `#machine learning`, `#verification`, `#emergence`

---

<a id="item-7"></a>
## [谷歌揭示 Gemini 4 为迄今最雄心预训练项目](https://9to5google.com/2026/07/26/google-gemini-4-teases/) ⭐️ 8.0/10

谷歌 CEO Sundar Pichai 在 Alphabet 2026 年第二季度财报电话会议上宣布，下一代大模型 Gemini 4 已进入预训练阶段，称这是公司迄今为止最具雄心的预训练项目，目标在 2026 年底发布。 这一声明表明谷歌继续大力投资前沿 AI，可能加速通用人工智能的进展，并对 OpenAI 和 Anthropic 等竞争对手保持竞争压力。 Pichai 表示，谷歌将优先将算力分配给前沿的 AGI 研发，以确保 Gemini 4 在发布时仍处于前沿地位，同时 Gemini 3.x Flash 系列将继续保持每月一次的迭代频率，重点提升智能编码等能力。

telegram · zaihuapd · 7月27日 04:06

**背景**: 预训练是大型语言模型在大量无标签数据上学习的初始阶段，旨在捕捉通用知识和模式。AGI（通用人工智能）是一种假设性的 AI，能够在几乎所有任务上匹配或超越人类认知能力。谷歌的 Gemini 系列与 GPT-4、Claude 等模型竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.geeksforgeeks.org/artificial-intelligence/what-is-pre-training-and-its-objective/">What is Pre Training and its Objective - GeeksforGeeks</a></li>
<li><a href="https://en.wikipedia.org/wiki/Artificial_general_intelligence">Artificial general intelligence - Wikipedia</a></li>

</ul>
</details>

**标签**: `#Google`, `#Gemini 4`, `#AI`, `#Large Language Model`, `#Pre-training`

---

<a id="item-8"></a>
## [中芯国际测试中国首台国产 DUV 光刻机](https://t.me/zaihuapd/42800) ⭐️ 8.0/10

据报道，中芯国际正在试运行中国首台由上海初创公司宇量昇研发的先进深紫外（DUV）光刻机，旨在生产 28 纳米芯片，并尝试通过多重图形化工艺实现 7 纳米。 这一里程碑标志着中国推动半导体自给自足的进程，可能减少对 ASML 等进口 DUV 设备的依赖，尽管需要数年才能达到商业可行性。 该光刻机大部分零部件已国产化，但仍依赖部分进口；中芯国际目标 2027 年量产，目前在 28 纳米试产，7 纳米良率较低。

telegram · zaihuapd · 7月27日 14:10

**背景**: 深紫外（DUV）光刻使用 193nm 或 248nm 的光在硅片上印制电路，广泛用于成熟节点（28nm 及以上）。多重图形化技术通过将单层拆分为多次曝光，可将 DUV 延伸至 7nm 等更小特征尺寸。相比之下，极紫外（EUV）光刻使用 13.5nm 光，是 5nm 等先进节点所必需的，但因美国出口管制被禁止对华销售。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://eureka.patsnap.com/article/what-is-deep-ultraviolet-lithography-duv-and-how-does-it-work">What is Deep Ultraviolet Lithography (DUV) and how does it work?</a></li>
<li><a href="https://en.wikipedia.org/wiki/Multiple_patterning">Multiple patterning - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/EUV_lithography">EUV lithography - Wikipedia</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#DUV lithography`, `#China tech`, `#SMIC`, `#chip manufacturing`

---

<a id="item-9"></a>
## [月之暗面将开源 3T 参数模型 Kimi-K3](https://t.me/zaihuapd/42802) ⭐️ 8.0/10

月之暗面宣布将在 Hugging Face 上开源 Kimi-K3，这是一个 3 万亿参数的前沿模型，预计于 2026 年 7 月 27 日发布权重。该模型采用了包含 Kimi Delta Attention 和 Attention Residuals 的全新架构，并原生支持工具调用、网页浏览和多步规划等智能体能力。 这是一个重要里程碑，因为它将成为参数规模最大的开源模型（3T），有可能使前沿 AI 的访问民主化。它可能加速长程编程、知识工作和复杂推理领域的研究，并为开源模型能力设定新标准。 Kimi-K3 采用 Kimi Delta Attention，这是一种基于 delta 规则的线性注意力机制，具有通道级遗忘功能以实现精细记忆更新；以及 Attention Residuals（AttnRes），它用学习到的深度注意力取代标准残差连接。该模型专为仓库级代码理解设计，具有扩展的上下文窗口。

telegram · zaihuapd · 7月27日 15:15

**背景**: 大型语言模型（LLM）通常使用注意力机制处理序列，但标准注意力机制的计算量随序列长度二次增长。线性注意力变体如 Mamba 和 Gated DeltaNet 旨在降低这一成本。Kimi Delta Attention 通过细粒度衰减改进了这些方法，而 Attention Residuals 增强了深度方向的信息流。开源如此规模的模型（3T 参数）很少见；此前最大的开源模型约为 400B 参数。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://jianyuh.github.io/attention/2025/12/13/KDA.html">Linear Attention : Kimi Delta Attention | Jianyu Huang’s Blog</a></li>
<li><a href="https://arxiv.org/abs/2603.15031">[2603.15031] Attention Residuals - arXiv.org GitHub - MoonshotAI/Attention-Residuals Attention Residuals - arXiv.org Attention Residuals wdlctc/open-attention-residuals - GitHub Attention Residuals - openlm.ai Attention Residuals Explained: Rethinking Transformer Depth</a></li>
<li><a href="https://github.com/MoonshotAI/Attention-Residuals">GitHub - MoonshotAI/Attention-Residuals</a></li>

</ul>
</details>

**标签**: `#open-source`, `#large language model`, `#Kimi-K3`, `#Moonshot AI`, `#3T parameters`

---