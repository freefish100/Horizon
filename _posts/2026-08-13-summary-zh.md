---
layout: default
title: "Horizon Summary: 2026-08-13 (ZH)"
date: 2026-08-13
lang: zh
---

> 从 35 条内容中筛选出 10 条重要资讯。

---

1. [Qwen 发布 Qwen3.8-2.4T-A95B：2.4 万亿参数开源权重 MoE 模型](#item-1) ⭐️ 9.0/10
2. [DeepSeek V4 Pro 0813 上线 OpenRouter，社区反响热烈](#item-2) ⭐️ 8.0/10
3. [Zed 发布 Delta：实时协作式 AI 代理对话](#item-3) ⭐️ 8.0/10
4. [Tailscale 将数据库损坏追踪到 16 年前的 SQLite WAL 重置 Bug](#item-4) ⭐️ 8.0/10
5. [xAI 发布 Grok 4.6，引发基准测试与 API 争议](#item-5) ⭐️ 8.0/10
6. [uBlock Origin 放弃对抗 Facebook 广告拦截](#item-6) ⭐️ 8.0/10
7. [AI 正在移除软件工程的中产阶级。](#item-7) ⭐️ 8.0/10
8. [Adam 的逐坐标自适应性破坏因子模型的低秩偏差](#item-8) ⭐️ 8.0/10
9. [微信发布 WeLM 系列，主打资源效率的大语言模型](#item-9) ⭐️ 8.0/10
10. [DeepSeek 上线 V4-Flash 正式版 API 公测，Agent 能力大幅增强](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Qwen 发布 Qwen3.8-2.4T-A95B：2.4 万亿参数开源权重 MoE 模型](https://huggingface.co/Qwen/Qwen3.8-2.4T-A95B) ⭐️ 9.0/10

Qwen 发布了 Qwen3.8-2.4T-A95B，这是一个开放权重的混合专家（MoE）大语言模型，总参数达 2.4 万亿，激活参数为 950 亿，并提供 BF16 和 FP8 格式。该模型被定位为前沿规模发布，模型卡声称其性能可与顶级商业模型媲美。 这是迄今发布的最大开源权重模型之一，大幅提升了开源 AI 的门槛，让开发者和研究者能够获得前沿规模的模型能力。它也加剧了开源权重生态系统的竞争，直接挑战 Kimi K3、DeepSeek 以及闭源商业系统。 本次仅发布了 BF16 和 FP8 检查点，因此 4 比特使用依赖训练后量化；4 比特版本约为 1.3TB，而极度压缩的 1 比特版本约为 397GB。开源权重模型缺少视觉输入、非思考模式以及商用 Qwen3.8-Max 才拥有的 1M 上下文长度，许可证则允许内部使用或年收入低于 5000 万美元的公司免费使用。

hackernews · Philpax · 8月12日 15:01 · [社区讨论](https://news.ycombinator.com/item?id=49273478)

**背景**: 混合专家（MoE）模型通过稀疏路由，只激活全部参数中的一部分（例如 2.4 万亿中的 950 亿）来处理每个 token，从而在较低的每 token 计算成本下实现大规模容量。开源权重模型会发布训练好的权重，让用户可以下载并自行部署，但由于训练数据和代码可能不公开，它们并非完全开源。高效服务此类巨型模型通常依赖 FP8 等低位量化，但在更低位宽下保持精度通常需要量化感知训练。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://researchaudio.io/p/mixture-of-experts-moe-in-large-language-models">Mixture of Experts ( MoE ) in Large Language Models</a></li>
<li><a href="https://www.ai21.com/glossary/foundational-llm/open-weights-model/">What is an Open - Weights Model ? | AI 21</a></li>
<li><a href="https://arxiv.org/html/2303.17951v2">FP 8 versus INT8 for efficient deep learning inference</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：一些评论者兴奋地认为，重度量化可能将接近前沿的性能带到普通消费者可负担的硬件上，而另一些人则担心服务成本和功能缺失。NitpickLawyer 指出，由于没有 QAT 4 比特权重且许可证有限制，该模型比 Kimi K3 更难部署；l72 指出开源模型缺少商用 Max 版本中的视觉和 1M 上下文支持；dhx 则提到了竞争对手 DeepSeek 的基准测试消息。XCSme 还指出，当前推理价格很高，大约是 Grok 4.6 的两倍。

**标签**: `#AI`, `#LLM`, `#Qwen`, `#MoE`, `#open-weights`

---

<a id="item-2"></a>
## [DeepSeek V4 Pro 0813 上线 OpenRouter，社区反响热烈](https://openrouter.ai/deepseek/deepseek-v4-pro-0813) ⭐️ 8.0/10

DeepSeek 的新模型 V4 Pro 0813 现已通过 OpenRouter 以 API 形式提供，距离 4 月的 V4 Pro 和 7 月的更新已有数月。目前没有官方公告页面，是否发布开放权重也尚未确认。 这次发布表明 DeepSeek 正以快速节奏持续推出高性价比的前沿模型，并立即引发开发者社区的实际测试。社区的高度关注意味着它有望成为 Claude Sonnet、GPT-5 Opus 等更昂贵模型之外的热门低成本选择。 该模型上线时仅提供 API，由于 DeepSeek 没有专门的公告页面，报道只能链接到 OpenRouter 的页面，而该页面没有对比基准。早期用户反馈提到约 12.50 美元处理 2B tokens（50% 缓存命中），并在交通模拟器和分布式物理引擎负载上取得了显著收益。

hackernews · explosion-s · 8月12日 16:04 · [社区讨论](https://news.ycombinator.com/item?id=49274600)

**背景**: DeepSeek 是一家中国 AI 公司，由梁文锋于 2023 年 7 月创立；2025 年 1 月因 DeepSeek-R1 模型及其聊天机器人而引发全球关注。该公司以开放模型权重和异常低廉的 API 价格著称，因此其模型深受注重成本的开发者和研究者欢迎。其面向消费者的产品在政治敏感话题上遵循中国的内容监管规定，与其他中国 AI 服务类似。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>
<li><a href="https://www.deepseek.com/en/">DeepSeek</a></li>

</ul>
</details>

**社区讨论**: 社区反应总体积极：一位开发者报告称，在自己的交通模拟器和物理引擎上运行该模型一整天后取得了显著收益；另一位评论者称赞上一版 Flash 更新让繁重的开发任务变得非常便宜。也有人建议提供官方基准链接而非 OpenRouter 页面，还有人分享了自己偏爱低成本高能力模型、而非追求顶级智能的通用选择标准。

**标签**: `#DeepSeek`, `#LLM`, `#AI`, `#Model Release`

---

<a id="item-3"></a>
## [Zed 发布 Delta：实时协作式 AI 代理对话](https://zed.dev/blog/introducing-delta) ⭐️ 8.0/10

Zed 推出了 Delta 功能，使编辑器内能够实时协作进行 AI 代理对话。该功能还支持“会话即文档”能力，可将聊天记录视为可持久化、可编辑的文档。 Delta 将 Zed 的多人协作能力从纯人工协作扩展到 AI 代理，可能改变团队审查、调试和学习 AI 生成代码的方式。它在指导初级开发者以及透明化展示 AI 代理如何生成拉取请求方面尤其有价值。 该功能的两大核心是实时多人代理对话和“会话即文档”，用户可在代理聊天记录中内联评论。Zed 是一款基于 Rust 的跨平台开源代码编辑器，支持 Linux、macOS 和 Windows，主打速度以及与人类和 AI 的协作。

hackernews · khy · 8月12日 18:19 · [社区讨论](https://news.ycombinator.com/item?id=49276574)

**背景**: Zed 是一款开源的跨平台代码编辑器，使用 Rust 编程语言编写，支持 Linux、macOS 和 Windows。它由 Atom 的创建者之一 Nathan Sobo 创立，并由 Zed Industries 开发。该编辑器定位为“为速度以及与人类和 AI 的协作而生”。“会话即文档”将对话日志视为持久化产物，是文档中心化 AI 辅助领域的新兴模式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zed_(text_editor)">Zed (text editor) - Wikipedia</a></li>
<li><a href="https://zed.dev/">Zed — Your last next editor</a></li>
<li><a href="https://arxiv.org/pdf/2002.00747">Conversations with Documents An Exploration of Document-Centered Assistance</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一但思考深入。一些用户质疑多人编码的必要性，称其为“单机游戏”；另一些人则担心 AI 对代码的总结过于冗长或遗漏边界情况。但也有一些评论者认为实时协作在指导和追溯 AI 代理如何生成 PR 方面有真正价值，还有人称赞内联评论的设计。此外，有用户抱怨博客页面文字对比度偏低，影响阅读。

**标签**: `#Zed`, `#AI`, `#code editor`, `#collaboration`, `#developer tools`

---

<a id="item-4"></a>
## [Tailscale 将数据库损坏追踪到 16 年前的 SQLite WAL 重置 Bug](https://tailscale.com/blog/sqlite-wal-reset-bug) ⭐️ 8.0/10

Tailscale 发现其数据库损坏问题是由一个存在 16 年的 SQLite WAL 重置竞态条件导致的。他们与 SQLite 团队合作修复了该 Bug，并资助了一个开源的 VFS shim，用于快速定位该竞态条件，未来也有助于调试类似问题。 该 Bug 可能导致 SQLite 应用程序（即使是采用推荐的单写者模式）出现无征兆的数据库损坏。这次修复以及资助的调试工具让整个 SQLite 生态受益，也展示了企业可以有效回馈开源基础设施。 Tailscale 将 SQLite 用作 tailnet 控制面的数据库，并且手动控制检查点过程且非常激进地进行检查点，因此更容易触发该 Bug。修复方案在 checkpoint 函数中增加了一个检测机制，可以识别 WAL 是否已被其他线程重置，从而避免竞态条件。

hackernews · ropbear · 8月12日 14:22 · [社区讨论](https://news.ycombinator.com/item?id=49272832)

**背景**: SQLite 是一种广泛使用的嵌入式数据库。在 WAL（Write-Ahead Logging，预写日志）模式下，写入先进入单独的 WAL 文件，之后再被检查点合并到主数据库。VFS（Virtual File System，虚拟文件系统）shim 是一个拦截文件操作的层，Tailscale 资助了一个校验和 VFS shim 用于检测页面级损坏。WAL 重置 Bug 是检查点进程重置 WAL 文件与其他连接读取它之间的竞态条件，可能导致数据库损坏。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tailscale.com/blog/sqlite-wal-reset-bug">How Tailscale helped find the SQLite WAL-Reset bug</a></li>
<li><a href="https://www.sqlite.org/walformat.html">WAL-mode File Format</a></li>
<li><a href="https://sqlite.org/cksumvfs.html">The Checksum VFS Shim - SQLite</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞了这篇写得很好文章，以及公司资助开源工具并保持 SQLite 支持合同的决定。一些人讨论了 SQLite 在高并发系统中的适用性，有评论认为它不适合显著并发的场景，并建议使用 Postgres 进行在线连续备份。也有人赞赏这种调试方法论，并提醒即使经过大量测试的软件也可能存在隐蔽 Bug。

**标签**: `#sqlite`, `#database`, `#bug`, `#tailscale`, `#debugging`

---

<a id="item-5"></a>
## [xAI 发布 Grok 4.6，引发基准测试与 API 争议](https://x.ai/news/grok-4-6) ⭐️ 8.0/10

xAI 发布了新一代前沿模型 Grok 4.6，并附有 Artificial Analysis 的基准测试与分析文章。此次发布迅速在 Hacker News 上引发 390 条评论，讨论 API 行为、基准测试真实性与竞争影响。 Grok 4.6 是主要 AI 实验室的一次重要更新，加剧了前沿模型提供商之间的竞争。社区关于基准可信度与 API 行为的争论，可能影响用户评估和采用前沿模型的方式。 Hacker News 评论者指出，xAI 的 API 似乎会添加默认系统提示词，可能覆盖用户关于讨论系统提示词的指令。评论者还猜测基准测试污染或技术快速传播，并将 Grok 4.6 与 GPT-5.6-Sol、Claude 4.8/5 等模型进行了比较。

hackernews · iLuddite · 8月12日 15:32 · [社区讨论](https://news.ycombinator.com/item?id=49274027)

**背景**: 前沿模型是指某个时期能力最先进、用途最广的 AI 系统，以推理、多模态理解和自主任务执行为特征。Artificial Analysis 是一个独立平台，提供透明且不易受主观偏好影响的基准测试，衡量速度、成本和可靠性，而非主观喜好。基准测试污染——即评估数据混入训练语料——日益令人担忧，因为它会让模型看似理解了其实只是记住的问题，从而削弱基准测试的有效性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/">AI Model & API Providers Analysis | Artificial Analysis</a></li>
<li><a href="https://arxiv.org/html/2605.19999v1">LLM Benchmark Datasets Should Be Contamination-Resistant</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/frontier-models/">What Are Frontier AI Models and How They Work | NVIDIA Glossary</a></li>

</ul>
</details>

**社区讨论**: Hacker News 评论者大多积极但观点不一：有人批评 xAI 的 API 注入默认系统提示词，也有人质疑快速提升的基准成绩是否源于蒸馏或基准测试作弊。还有人称赞 Grok 简洁直白的风格，并承认尽管其声誉两极分化，Grok 仍带来了良性竞争。

**标签**: `#AI`, `#LLM`, `#Grok`, `#xAI`, `#benchmarks`

---

<a id="item-6"></a>
## [uBlock Origin 放弃对抗 Facebook 广告拦截](https://digitalescapetools.com/2026/08/ublock-origin-stops-chasing-facebook-ads.html) ⭐️ 8.0/10

uBlock Origin 的开发者决定停止在 Facebook 上过滤广告，理由是平台采取了激进且不断演变的反广告拦截措施。这标志着广告拦截器与大型社交媒体平台之间持续斗争中的一次明显退让。 这件事很重要，因为它凸显了广告拦截器与大型平台之间不断升级的军备竞赛，并表明在 Facebook 等网站上，基于过滤列表的传统拦截方式可能不再奏效。数百万依赖 uBlock Origin 保护隐私和无广告浏览的用户将受到影响，可能推动讨论转向基于 AI 的广告检测解决方案。 据报道，Facebook 使用反广告拦截技术，例如频繁更新代码（有时甚至每小时更新），并部署针对性代码来规避过滤列表；同时，当检测到拦截器时，还会弹出覆盖提示并强制自动播放视频。uBlock Origin 团队认为，继续跟上这些对策的代价已经不值得。

hackernews · Markoff · 8月12日 11:28 · [社区讨论](https://news.ycombinator.com/item?id=49270726)

**背景**: 像 uBlock Origin 这样的广告拦截器依赖过滤列表（如 EasyList），通过匹配 URL 模式和页面元素来隐藏或拦截广告。网站和平台开发了反广告拦截脚本，可以检测这些列表并破坏页面功能，或以过滤列表难以捕捉的方式投放广告。因此，在大型平台上维持有效的拦截已经成为一场持续且耗费心血的猫鼠游戏。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://support.adblockultimate.net/en/articles/9240458-anti-adblock-techniques">Anti - adblock techniques | AdBlocker Ultimate Help Center</a></li>
<li><a href="https://lifetips.alibaba.com/tech-efficiency/facebook-now-blocks-ad-blockers">Facebook Now Blocks Ad Blockers: What Works in 2024 (Evidence-Based)</a></li>
<li><a href="https://www.facebook.com/help/920247859773192">About ad blockers on Facebook | Facebook Help Center</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论了未来可能的对策，例如操作系统级或基于计算机视觉的广告检测——无需检查应用代码，直接在广告上画一个矩形框。有人赞同这一决定，认为避免 Facebook 广告的唯一可靠方法就是离开该平台；还有人指出这场军备竞赛的“猫鼠游戏”本质，并对 Facebook 的黑暗模式表示不满。

**标签**: `#privacy`, `#ad-blocking`, `#facebook`, `#ublock-origin`, `#tech-news`

---

<a id="item-7"></a>
## [AI 正在移除软件工程的中产阶级。](https://blog.florianherrengt.com/ai-removing-middle-class-software-engineering.html) ⭐️ 8.0/10

一篇博客文章认为，AI 正在通过自动化常规编码任务，不成比例地淘汰中级软件工程岗位。作者强调，工程师必须保持批判性思维，避免过度依赖 AI。 这很重要，因为它涉及行业内关于 AI 对科技就业和职业发展影响的紧迫争论。这一观点可能影响工程师和公司如何看待 AI 采用与技能发展。 文章警告说，过度依赖 AI 可能让“糟糕的工程师”将糟糕的工作放大十倍，并强调“垃圾进、垃圾出”的原则依然适用。它还指出，在学习过程中走捷径使用 AI 会阻碍批判性判断力的培养。

hackernews · florianherrengt · 8月12日 13:20 · [社区讨论](https://news.ycombinator.com/item?id=49271994)

**背景**: AI 编码助手（如 GitHub Copilot、Codeium 和 Tabnine）可以根据提示生成代码、补全样板代码，甚至建议修复方案，将许多常规开发任务自动化。AI 工具也越来越多地用于 CI/CD 流水线中的自动测试生成和预测性调试。随着这些工具的成熟，以常规编码为主要工作的工程师需求可能会减少，而强调判断力、架构设计和问题解决能力的角色则变得更加有价值。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/sourcegraph/awesome-code-ai">GitHub - sourcegraph/awesome-code-ai: A list of AI coding tools (assistants, completions, refactoring, etc.) · GitHub</a></li>
<li><a href="https://cloud.google.com/use-cases/ai-code-generation">AI Code Generation: Definition, Uses and Tools | Google Cloud</a></li>
<li><a href="https://ghaznix.com/blogs/ai-and-modern-software-development/">AI and Modern Software Development : The Great Transformation</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认同文章的前提，有人指出“糟糕的工程师”现在可以将糟糕的输出在组织内放大。还有人将 AI 比作“Stack Overflow 工程师的自动化”，并强调永远不要把批判性思维外包给 LLM。也有历史视角认为，几十年来技术一直在重塑中产阶级，从而将这一争论置于更广泛的经济背景中。

**标签**: `#AI`, `#Software Engineering`, `#Career Impact`, `#Automation`, `#Tech Industry`

---

<a id="item-8"></a>
## [Adam 的逐坐标自适应性破坏因子模型的低秩偏差](https://www.reddit.com/r/MachineLearning/comments/1vmjb3p/the_loss_does_not_see_the_basis_but_adam_does_r/) ⭐️ 8.0/10

一项关于欠定矩阵感知的研究表明，Adam 的逐坐标二阶矩估计打破了因子模型中的旋转不变性，而 GD、Muon 和 Shampoo 则不会。在匹配训练损失下比较了九种更新规则，结果分为两个清晰的聚类，并指出各向异性是关键的罪魁祸首。 这一发现将优化器的选择与隐式低秩偏差联系起来，而低秩偏差会影响矩阵分解和深度线性网络的泛化性能。它可能指导新优化器的设计，并帮助解释为什么自适应方法有时在结构化任务上表现不佳。 该研究使用仅训练集的学习率规则在超光谱数据上实现了 43-44%的留出误差降低，该规则让 Adam 在其自身网格上获得最差的学习率；当每种方法自行选择最佳学习率时，差距会缩小。理论分析仅涵盖无记忆更新规则，而动量的结果是经验性的。

reddit · r/MachineLearning · /u/EtherealGlyph · 8月12日 16:39

**背景**: 在 W = UV^T 的因子模型中，损失函数对旋转(U,V) → (UQ, VQ)具有不变性，梯度下降尊重这一对称性。Adam 的逐坐标归一化依赖于因子的基，破坏了旋转不变性，并导致丢失 GD 通常具有的隐式低秩偏差。Muon 和 Shampoo 是保持结构特性的矩阵感知优化器，而隐式低秩偏差已在 SGD 噪声和矩阵分解的背景下被研究。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/1802.09568">[1802.09568] Shampoo: Preconditioned Stochastic Tensor Optimization</a></li>
<li><a href="https://www.emergentmind.com/topics/muon-optimizer">Muon Optimizer : Matrix-Aware Learning</a></li>
<li><a href="https://cbmm.mit.edu/publications/sgd-noise-and-implicit-low-rank-bias-deep-neural-networks">SGD Noise and Implicit Low - Rank Bias in Deep Neural Networks</a></li>

</ul>
</details>

**标签**: `#optimizers`, `#Adam`, `#low-rank bias`, `#matrix factorization`, `#deep learning theory`

---

<a id="item-9"></a>
## [微信发布 WeLM 系列，主打资源效率的大语言模型](https://x.com/Weixin_WeChat/status/2087509298310209718) ⭐️ 8.0/10

微信团队发布了 WeLM 大语言模型系列，其中 WeLM-80B（激活参数 30 亿）已应用于微信内 AI 智能体小微，而基于 MoE 架构的 WeLM-617B（激活参数 230 亿）正在研发中。 此次发布凸显了业界对资源高效型大语言模型的日益关注，这类模型能够以可承担的成本运行。它也展示了大型模型如何融入日常消费产品，可能影响其他科技公司在大众市场应用中部署 AI 助手的方式。 WeLM-80B 虽然总参数为 800 亿，但仅激活 30 亿参数；WeLM-617B 将采用混合专家（MoE）架构，激活 230 亿参数。即将推出的 617B 模型旨在处理微信生态中的复杂任务，如小程序智能开发和小工具生成。

telegram · zaihuapd · 8月12日 13:58

**背景**: WeLM 是微信自研的大语言模型系列，最初于 2022 年 9 月发布。传统的稠密大语言模型在处理每个词元时激活全部参数，随着模型规模增长计算成本会变得很高。MoE 架构将网络拆分为多个专门化的“专家”，并通过路由器只激活最相关的部分，从而以极低的计算成本实现大规模扩展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.theblockbeats.news/flash/361266">WeChat Introduces WeLM Dual Model : 80B Model Empowering Mini...</a></li>
<li><a href="https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-mixture-of-experts">A Visual Guide to Mixture of Experts ( MoE )</a></li>
<li><a href="https://eu.36kr.com/en/p/3865706037924872">The Most In - depth Network - wide Experience of WeChat AI: I'm in...</a></li>

</ul>
</details>

**标签**: `#LLM`, `#WeChat`, `#MoE`, `#resource efficiency`, `#AI`

---

<a id="item-10"></a>
## [DeepSeek 上线 V4-Flash 正式版 API 公测，Agent 能力大幅增强](https://t.me/zaihuapd/43149) ⭐️ 8.0/10

2026 年 7 月 31 日，DeepSeek 上线 V4-Flash 正式版 API 公测，原生支持 Responses API 格式，并针对 Codex 做了适配。该模型的 Agent 能力大幅增强，Terminal Bench 2.1（82.7）、CyberGym（76.7）、DSBench-FullStack（68.7）、DSBench-Hard（59.6）等基准成绩全面超越 V4-Pro-Preview。 此次发布标志着 DeepSeek 在智能体（Agent）AI 与工具调用场景上的加码，而这正是前沿模型厂商竞争的关键方向。正式版公测让开发者能提前使用一款体积更小、但 Agent 性能接近旗舰级的“Flash”档模型，有望降低构建自主编程、终端操作等工作流的成本。 公告公布的基准成绩为：Terminal Bench 2.1 达 82.7，CyberGym 达 76.7，DSBench-FullStack 达 68.7，DSBench-Hard 达 59.6。模型原生支持 Responses API 格式并针对 Codex 做了定制适配；公告未完整披露模型结构与尺寸等细节。

telegram · zaihuapd · 8月12日 15:30

**背景**: Terminal-Bench 是一个开源基准测试，用于评估 AI 智能体在终端/命令行环境中完成复杂真实任务的能力，其 2.0 版本包含 89 个源自真实工作流的精选高难度任务。CyberGym 是一个面向智能体 AI 网络安全能力的评估框架，利用大型软件项目中真实的 OSS-Fuzz 漏洞来构建基准。这些基准反映了行业趋势：评估模型不再只看静态知识，而是更看重其在交互式环境中自主行动的能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/Terminal-Bench">Terminal-Bench</a></li>
<li><a href="https://hugobowne.github.io/mythos-preview-model-card/entities/cybergym">CyberGym</a></li>
<li><a href="https://www.tbench.ai/">Terminal-Bench</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#API`, `#AI model`, `#agent`, `#benchmarks`

---