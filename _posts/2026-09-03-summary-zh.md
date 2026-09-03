---
layout: default
title: "Horizon Summary: 2026-09-03 (ZH)"
date: 2026-09-03
lang: zh
---

> 从 38 条内容中筛选出 11 条重要资讯。

---

1. [谷歌发布 Gemini 3.8 Flash 与 3.8 Flash Cyber 模型](#item-1) ⭐️ 9.0/10
2. [Meta 低成本模型 Muse Spark 1.3 刷新 DeepSWE 纪录](#item-2) ⭐️ 8.0/10
3. [报告：AI 生成的“最佳软件”页面操纵 Perplexity 引用](#item-3) ⭐️ 8.0/10
4. [全球最大的暗物质探测器捕捉到单个奇特粒子事件](#item-4) ⭐️ 8.0/10
5. [Paint.NET 用 Claude 重写 Direct2D 支持 Wine，共 18 万行](#item-5) ⭐️ 8.0/10
6. [Jasper Research 发布文生图模型构建手册与数据集](#item-6) ⭐️ 8.0/10
7. [研究：多数开源 AI 检测器无法达到 0.5%误报率](#item-7) ⭐️ 8.0/10
8. [阿里 Qwen3.8-Max-0902 登顶 CodeArena 编程榜](#item-8) ⭐️ 8.0/10
9. [英伟达洽购开源 AI 平台 Hugging Face，估值逾 130 亿美元](#item-9) ⭐️ 8.0/10
10. [月之暗面与微软、亚马逊、谷歌谈判 Kimi K3 分成协议](#item-10) ⭐️ 8.0/10
11. [xAI 发布 Grok 4.6，强化智能体与视觉任务，追平 GPT-5.6 Sol 基准](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [谷歌发布 Gemini 3.8 Flash 与 3.8 Flash Cyber 模型](https://blog.google/innovation-and-ai/models-and-research/gemini-models/3-8-flash-and-3-8-flash-cyber/) ⭐️ 9.0/10

谷歌宣布 Gemini 3.8 Flash 全面上市，并同步推出面向网络安全的 Gemini 3.8 Flash Cyber 版本。这些模型在基准测试中表现强劲，据称 Flash 模型的智能得分与 Opus 5 持平并位居排行榜前列。 此次发布让开发者获得了一个异常快速、成本低廉，但仍在编程和知识基准测试中位居前列的模型，从而扩大了对高端 AI 能力的获取。同时，这也表明谷歌正通过仅限受信任防御者使用的模型布局 AI 网络安全领域。 Gemini 3.8 Flash 被描述为谷歌最智能的 Flash 系列模型，专为长时程软件工程、自主智能体和复杂企业工作流而设计。Flash Cyber 的真实世界漏洞发现率超过 70%，并在 CWE-Bench 补丁基准上处于帕累托前沿；该模型仅通过新的 Fairwind 计划限制访问。

hackernews · bratao · 9月2日 15:12 · [社区讨论](https://news.ycombinator.com/item?id=49537553)

**背景**: Gemini Flash 是谷歌轻量、快速且成本较低的大语言模型层级，定位为更大的 Pro 系列的廉价替代方案，同时仍支持智能体工作流。Gemini 3 系列保持了快速的发布节奏：3.7 Flash 仅在前几个月发布，而此次新模型延续了这一轨迹，专注于软件工程和领先的基准表现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/3-8-flash-and-3-8-flash-cyber/">Introducing Gemini 3.8 Flash and 3.8 Flash Cyber</a></li>
<li><a href="https://deepmind.google/models/model-cards/gemini-3-8-flash/">Gemini 3.8 Flash - Model Card — Google DeepMind</a></li>
<li><a href="https://ai.google.dev/gemini-api/docs/latest-model">What's new in Gemini 3.8 Flash | Gemini API | Google AI for Developers</a></li>

</ul>
</details>

**社区讨论**: 开发者反应热烈：Simon Willison 称赞该模型在速度和 HTML/JavaScript 生成方面的表现，并分享了一个成本仅 1.8 美分的示例。多位评论者强调其基准测试成绩优异（如登上 DeepSwe 榜首、智能得分 59 分与 Opus 5 持平）；同时也有用户质疑 Flash 模型如此高频发布是否意味着递归自我改进，或者只是为了分散大众对迟迟没有新 Pro 模型的注意力。

**标签**: `#gemini`, `#google`, `#llm`, `#benchmarks`, `#ai-models`

---

<a id="item-2"></a>
## [Meta 低成本模型 Muse Spark 1.3 刷新 DeepSWE 纪录](https://developer.meta.com/ai/models/muse-spark/) ⭐️ 8.0/10

Meta 发布了低成本大语言模型 Muse Spark 1.3，在 DeepSWE 长时程编码基准上取得 75.4 分，为目前公开最高分，并超过了 Gemini 3.8 Flash。此次发布还包含 muse-spark-1.3-contributor 变体，以允许 Meta 使用用户数据训练为代价换取更低价格。 Muse Spark 1.3 以很低的推理成本提供了接近前沿的智能体编程性能，使先进的长时程软件工程能力对个人开发者和初创公司更加可用。它的出色成绩加剧了各大 AI 实验室之间的性价比竞争，社区成员预计这将推动模型价格下降。 Muse Spark 1.3 针对长时程编程工作流进行了调优，能够跟踪上下文与之前的结果，处理杂乱或相互矛盾的输入，并在需要时要求用户输入，同时减少不必要的轮次。Meta 还提供了 contributor 定价档位，以更低价格换取用户允许 Meta 将数据用于训练，这种透明做法获得了开发者的认可。

hackernews · bvaldivielso · 9月2日 19:35 · [社区讨论](https://news.ycombinator.com/item?id=49541256)

**背景**: Muse Spark 是 Meta 通过 Meta Superintelligence Labs 开发的大语言模型系列；该系列于 2026 年 4 月推出，Muse Spark 1.1 于 2026 年 7 月 9 日发布。DeepSWE 是 Datacurve 推出的包含 113 个原创长时程软件工程任务的基准测试，在活跃的开源仓库上评估编码智能体，用于替代从 GitHub 已合并修复中挖掘测试的 SWE-bench 式基准。此前 DeepSWE 榜单快照显示 Claude Opus 5 以 73.6 领先，因此 Muse Spark 1.3 的 75.4 是一次明显跃升。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://research.meta.ai/blog/introducing-muse-spark-1-3">Introducing Muse Spark 1.3 | Meta AI Research</a></li>
<li><a href="https://en.wikipedia.org/wiki/Muse_Spark">Muse Spark - Wikipedia</a></li>
<li><a href="https://deepswe.datacurve.ai/">DeepSWE</a></li>

</ul>
</details>

**社区讨论**: 社区反应总体积极：开发者进行了实测，发现 Muse Spark 1.3 比 1.2 输出更好，例如用 38 秒、仅几美分就生成了更干净的鹈鹕骑自行车 SVG。还有评论者强调 75.4 的 DeepSWE 分数并预测竞争将压低价格；也有人称赞透明的 contributor 档位定价，但对 Meta 从用户数据训练中获得的巨大价值表示不安。

**标签**: `#AI`, `#Meta`, `#LLM`, `#Machine Learning`, `#Benchmarks`

---

<a id="item-3"></a>
## [报告：AI 生成的“最佳软件”页面操纵 Perplexity 引用](https://trellner.com/reports/manufactured-sources-behind-ai-recommendations/) ⭐️ 8.0/10

一份报告揭露，三个网站生成了 215,128 个由 AI 撰写的“最佳软件”页面，这些页面经常被 Perplexity 的 AI 答案引用。这暴露了一种针对生成式引擎优化的新型 SEO 操纵手段。 此事意义重大，因为像 Perplexity 这样的 AI 推荐系统可能被大规模生产的 AI 内容系统性影响，削弱人们对 AI 生成答案的信任。它凸显了 LLM 驱动的搜索中日益严重的漏洞，可能误导用户并损害合法内容创作者。 该报告很可能描述了一种程序化 SEO 形式，即自动生成 AI 页面，为无数“最佳软件”查询排名。Perplexity 倾向于引用这些页面，表明它可能偏好 LLM 风格的内容，从而使这种操纵手段有效。

hackernews · jakobgreenfeld · 9月2日 13:59 · [社区讨论](https://news.ycombinator.com/item?id=49536375)

**背景**: 生成式引擎优化（GEO）是一种通过组织内容来提高在 Perplexity、ChatGPT 或 Google AI Overview 等系统生成的 AI 回答中可见度的做法。Google 等搜索引擎已表明，主要使用 AI 自动化来操纵排名违反其垃圾内容政策。然而，AI 回答引擎可能没有同样强大的防御机制，使得本质上是批量生产的内容能够获得引用影响力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Generative_engine_optimization">Generative engine optimization - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2311.09735">[2311.09735] GEO: Generative Engine Optimization</a></li>
<li><a href="https://developers.google.com/search/blog/2023/02/google-search-and-ai-content">Google Search's guidance about AI-generated content | Google Search Central Blog | Google for Developers</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，LLM 通常偏爱 AI 生成的文本或自身输出，例如 Claude 和 Codex 在选择时总是倾向于生成的网站。一些人还分享了 LLM 推荐不存在地点的真实案例，凸显了模型幻觉被这种操纵放大的更广泛问题。另一位用户观察到，Perplexity 为了追求速度而牺牲准确性，导致质量下降，引用的链接常常毫无价值。

**标签**: `#AI`, `#search`, `#LLM`, `#misinformation`, `#SEO`

---

<a id="item-4"></a>
## [全球最大的暗物质探测器捕捉到单个奇特粒子事件](https://www.science.org/content/article/world-s-biggest-dark-matter-detector-spots-single-weird-particle) ⭐️ 8.0/10

全球最大的暗物质探测器 LUX-ZEPLIN（LZ）观测到一次可能预示新物理学的意外粒子事件。物理学家强调，仅凭这一个事件远不足以宣布任何发现。 暗物质从未被直接观测到，因此任何疑似信号都具有很高的科学意义。如果更多数据能重现这一事件，它有望揭示暗物质的粒子本质，或指向超越当前标准模型的新物理；即使无法证实，它也表明新一代探测器已变得非常灵敏。 LZ 使用约 7 吨活性液氙，安装于南达科他州桑福德地下研究设施一座前金矿内约 1,480 米深处，以屏蔽宇宙射线的背景干扰。合作组在预印本中表示已排查过错误重建的事件和非同寻常的背景来源，但据报道团队成员形容这个事件仍令人无法完全理解。

hackernews · randycupertino · 9月2日 13:40 · [社区讨论](https://news.ycombinator.com/item?id=49536079)

**背景**: 暗物质是一种不可见的物质形态，构成了宇宙中的大部分物质，目前只能通过其引力效应来观测。一类主流候选粒子是弱相互作用大质量粒子（WIMP），它们偶尔会与普通原子核发生碰撞。LZ 实验由 LUX 与 ZEPLIN 项目合并而成，利用液氙靶来寻找这种 WIMP 与原子核碰撞产生的反冲信号。它建在极深的地下，正是为了减少宇宙射线背景和其他假信号。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LZ_experiment">LZ experiment - Wikipedia</a></li>
<li><a href="https://lz.lbl.gov/detector/">Detector | The LZ Dark Matter Experiment</a></li>
<li><a href="https://science.nasa.gov/dark-matter/">Dark Matter - NASA Science</a></li>

</ul>
</details>

**社区讨论**: 总的来说，评论者热情但克制：他们赞赏 LZ 预印本中对背景事件细致的核查，并承认其中或许有真正的发现潜力。许多人指出，粒子物理中约 3σ 的异常经常在更多数据到来后被推翻；还有人提到联合创始人坦言单一事件很难解读。另一些评论则乐于看到金矿被改造用于科学研究，并希望这次异常——即便只是设备故障——也能成为改进探测器的学习机会。

**标签**: `#particle physics`, `#dark matter`, `#LZ detector`, `#scientific anomaly`

---

<a id="item-5"></a>
## [Paint.NET 用 Claude 重写 Direct2D 支持 Wine，共 18 万行](https://simonwillison.net/2026/Sep/2/rick-brewster/) ⭐️ 8.0/10

Rick Brewster 宣布 Paint.NET 现在包含一个由 Claude 编写的、从零开始、以“干净室”方式逆向重写的 Direct2D，当应用通过 /wine 参数在 Wine 上运行时使用。这个重写版本位于 PaintDotNet.Windows.Direct2D1.Managed.dll，包含约 18 万行 AI 生成代码，作者称其为“vibe coding”，并且没有经过全面审查。 这是一个新颖且有潜在影响力的实验：用大语言模型以“干净室”方式重实现一个庞大的专有图形 API，从而让 Windows/.NET 应用能够通过 Wine 在 Linux 上运行。它也引发了关于大规模 AI 辅助代码生成的可行性、可靠性，以及真实项目中需要怎样的人工审查等重要问题。 Brewster 将这 18 万行代码与 Paint.NET 其余约 70 万行、历时二十多年写成的代码作对比，并指出他必须不断监督 Claude 处理资源管理——有一段时间它甚至没有对引用计数对象执行 COM 中相当于 AddRef() 的操作。他还提到 Claude 既会做出糟糕的架构决策，也会完成令人印象深刻的逆向工程，例如推导出 Direct2D 内置特效库所需的各种公式。

rss · Simon Willison · 9月2日 05:50

**背景**: Direct2D 是微软的硬件加速 2D 图形 API，而 Wine 对其支持不完整，长期阻碍 Paint.NET 在 Linux 上正常运行。Wine 是一个开源兼容层，通过黑盒逆向工程重实现 Windows API，使 Windows 软件可以运行在 Linux、macOS 等类 Unix 操作系统上。“Vibe coding”指通过自然语言提示让 AI 生成代码，并且开发者往往对自己没有深入理解，也很少进行彻底审查的一种开发方式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Wine_compatibility_layer">Wine compatibility layer</a></li>
<li><a href="https://en.wikipedia.org/wiki/Vibe_coding">Vibe coding - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI code generation`, `#Direct2D`, `#Wine`, `#Paint.NET`, `#software engineering`

---

<a id="item-6"></a>
## [Jasper Research 发布文生图模型构建手册与数据集](https://www.reddit.com/r/MachineLearning/comments/1w5c9rd/detailed_explanation_of_how_to_create_a/) ⭐️ 8.0/10

Jasper Research 发布了一本详尽的技术 cookbook，并配套 nano-t2i 代码库和包含 1.049 亿张图片的 MONET 数据集，让开发者可以从零训练文生图模型。发布内容包含完整推理过程、中间结果以及一个可用于动手训练的小型模型。 该发布降低了大规模、可复现文生图研究的门槛，为从业者和研究者提供了一套接近前沿实验室做法的完整开源方案。同时，它证明了仅用 MONET 训练的 4B 参数模型也能在 GenEval 和 DPG 上取得有竞争力的成绩。 MONET 数据集从 29 亿张图片中筛选、去重并重写多组标题，最终得到 1.049 亿张高质量样本。nano-t2i 是一个极简代码库，旨在单块 GPU 上从零训练出有竞争力的扩散模型。

reddit · r/MachineLearning · /u/dh7net · 9月2日 14:40

**背景**: 文生图（T2I）模型根据文本提示生成图像，扩散模型是实现该任务的常见架构。大规模训练此类模型通常需要海量的图文配对数据集，这限制了开放研究的开展。MONET 是首个公开的、经筛选、去重并为预训练大型文生图模型专门设计的多标题数据集。Jasper 的 cookbook 和代码库将这些数据转化为社区可用的实用配方。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://gojasper.github.io/monet/">A Massive, Open, Non-redundant and Enriched Text - to - image dataset</a></li>
<li><a href="https://www.jasper.ai/blog/monet">Monet Lowering the Barrier to World Class Image ... | The Jasper Blog</a></li>
<li><a href="https://huggingface.co/blog/jasperai/monet">MONET : Lowering the bar for World-Class Image Generation research.</a></li>

</ul>
</details>

**标签**: `#text-to-image`, `#machine learning`, `#tutorial`, `#dataset`, `#model training`

---

<a id="item-7"></a>
## [研究：多数开源 AI 检测器无法达到 0.5%误报率](https://www.reddit.com/r/MachineLearning/comments/1w58erw/most_opensource_ai_detectors_cant_hold_a_05/) ⭐️ 8.0/10

一项对开源 AI 文本检测器的系统性评估发现，六款模型中有四款无法将误报率控制在 0.5%（FPR），OpenAI RoBERTa 等旧检测器在检测现代生成模型文本时表现甚至不如随机猜测。在目标误报率下，表现最好的开源检测器也只能识别 42%的经“人味改写器”（humanizer）改写的 AI 文本。 这项发现对任何使用开源检测器来审查 AI 生成文本的应用都意义重大，因为在规模效应下，即使 0.5%的误报率也可能导致大量人类文章被错误标记。研究还证实这些模型普遍对非英语母语写作者存在偏见，使学校、出版社和内容平台面临更严峻的伦理与法律风险。 评估协议先在同样的 6,930 篇人类文档上把每个模型的阈值统一校准到 0.5%误报率，再分别测量对原始 AI 文本、改写后 AI 文本以及前沿模型（GPT-5.x、Claude Opus 5、Gemini 3.x）文本的召回率。MAGE 在任何阈值下都无法达到 0.5%误报率，会对 26%的普通 LLM 时代前人类网页文本打出超过 0.9999 的高分；OpenAI 的 RoBERTa 检测器 AUC 仅为 0.313。

reddit · r/MachineLearning · /u/grumpyp2 · 9月2日 12:04

**背景**: AI 文本检测器是一类分类器，用于区分人类写作与大型语言模型生成的文本，其误报率决定普通人类写作被错误判为机器文本的频率。像 OpenAI RoBERTa 这样的早期检测器是针对 GPT-2 输出微调的，因此对更新的大模型泛化能力很差；MAGE 则是基于 Longformer 的较新检测框架，在来自 27 个 LLM 的 44.7 万条样本上训练。所谓“人味改写器”工具会重写 AI 文本以绕过检测，因此改写文本上的评估结果会大幅下滑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/openai-community/roberta-large-openai-detector">openai -community/ roberta -large- openai - detector · Hugging Face</a></li>
<li><a href="https://skywork.ai/skypage/en/mage-content-detection/2021154098147848192">A Guide to MAGE : Detecting Content from Any Text Generator in the...</a></li>
<li><a href="https://reliqus.com/top-ai-humanizer-tools/">Top 12 AI Humanizer Tools in 2026 for Natural Text</a></li>

</ul>
</details>

**标签**: `#AI detection`, `#model evaluation`, `#bias`, `#NLP`, `#open-source`

---

<a id="item-8"></a>
## [阿里 Qwen3.8-Max-0902 登顶 CodeArena 编程榜](https://mp.weixin.qq.com/s/BfKRXMAR5ykD58LDkBftLg) ⭐️ 8.0/10

阿里巴巴发布了 Qwen3.8-Max-0902 大语言模型，拥有 2.4 万亿参数和 100 万 token 上下文窗口。该模型在 CodeArena 前端编程总榜中获得 1691 分，比旧版提高 22 分。 该模型在编程基准上领先，且 API 综合均价仅约 5 美元/百万 tokens（输入 2 美元、输出 6 美元），远低于第二名 20 美元和第三名 12 美元的价格，可能重塑大模型 API 定价格局。此次发布还验证了针对特定任务后训练的价值，并强化了阿里通义千问在办公（千问办公、Qoder、千问 App）等场景的生态布局。 该模型在基座模型之上针对编程和专业办公任务做了进一步后训练。API 定价为每百万 tokens 输入 2 美元、输出 6 美元，综合均价约 5 美元，而 CodeArena 榜单第二、第三名模型的综合均价分别为 20 美元和 12 美元；新版本已上线千问 AI 平台，并接入千问办公、Qoder 和千问 App。

telegram · zaihuapd · 9月2日 06:05

**背景**: CodeArena 是一个动态、交互式基准，专门用于评估自主编码智能体——即能够规划、编写、调试和执行代码的 LLM 系统，比静态编程题更贴近真实开发场景。后训练是指在预训练基座模型之上，通过微调、强化学习等方法让模型在特定领域更专业；本次是针对编程和专业办公任务进行后训练。Qwen 是阿里巴巴的大语言模型系列，2.4 万亿参数和 100 万上下文窗口意味着该模型体量庞大，能处理很长的代码或文档。Qoder 则是同一生态下的 AI 智能编程平台，支持对话式、感知上下文的软件开发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ali-codearena.github.io/Ali-CodeArena/">CodeArenaEval</a></li>
<li><a href="https://medium.com/@huguosuo/codearena-a-dynamic-benchmark-for-evaluating-autonomous-coding-agents-501eec40758b">CodeArena : A Dynamic Benchmark for Evaluating... | Medium</a></li>
<li><a href="https://qoder.com/">Qoder - The Agentic Platform</a></li>

</ul>
</details>

**标签**: `#AI`, `#Qwen`, `#Model Release`, `#Coding`, `#NLP`

---

<a id="item-9"></a>
## [英伟达洽购开源 AI 平台 Hugging Face，估值逾 130 亿美元](https://t.me/zaihuapd/43557) ⭐️ 8.0/10

据 Business Insider 报道，英伟达正与开源 AI 平台 Hugging Face 洽谈收购事宜，交易估值可能超过 130 亿美元。双方尚未达成协议，谈判仍可能破裂。 收购 Hugging Face 将使英伟达掌控开源 AI 模型、数据集和开发者工具的最大中心平台之一，可能重塑 AI 模型在其硬件上的分发与部署方式。这也会成为规模最大的 AI 收购之一，可能对整个开源 AI 生态产生深远影响。 英伟达已是 Hugging Face 的股东，曾参与其 2023 年 2.35 亿美元的融资，当时公司估值约 45 亿美元。微软此前也曾接洽过 Hugging Face，但目前谈判已经停止；另有报道称，Hugging Face 去年拒绝了英伟达 5 亿美元的投资要约。

telegram · zaihuapd · 9月2日 06:50

**背景**: Hugging Face 是一个开源 AI 平台，托管着数百万个预训练 AI 模型、数据集和应用程序，涵盖文本、图像、语音等任务。它提供帮助开发者查找、定制、训练和部署 AI 模型的工具，因此成为开源 AI 生态系统的核心枢纽，也是没有深厚编程经验的人构建 AI 应用的热门起点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://builtin.com/articles/what-is-hugging-face">What Is Hugging Face? The Open - Source AI Platform | Built In</a></li>
<li><a href="https://www.datacamp.com/tutorial/what-is-hugging-face">What is Hugging Face ? The AI... | DataCamp</a></li>

</ul>
</details>

**标签**: `#Nvidia`, `#Hugging Face`, `#acquisition`, `#AI industry`, `#open source`

---

<a id="item-10"></a>
## [月之暗面与微软、亚马逊、谷歌谈判 Kimi K3 分成协议](https://www.jiemian.com/article/15040119.html) ⭐️ 8.0/10

据报道，月之暗面正与微软、亚马逊和谷歌进行早期谈判，希望由这三家云巨头托管其开源模型 Kimi K3，并寻求最高 30%的服务总收入分成。若达成，这将成为中国 AI 公司与美国云巨头之间的首个大型模型收入分成协议。 这标志着开放权重 AI 的一种新商业模式：当云巨头转售模型时，开发者也从中获利。它可能为更多中国前沿模型进入西方云平台铺平道路，并重塑开源 AI 的经济模式。 Kimi K3 总参数达 2.8 万亿，是首个达到 3T 参数级别的开源模型，于 2026 年 7 月发布，截至 6 月中旬年度经常性收入已突破 3 亿美元。谈判仍处早期阶段，核心条款未定，各方均拒绝置评。

telegram · zaihuapd · 9月2日 07:36

**背景**: 传统上，开源 AI 模型可免费下载，第三方通过将其作为托管服务提供来盈利，而无需向原始开发者付费。月之暗面正在尝试一种“开放权重但商业受限”的许可模式：凡从 Kimi K3 部署中获得超过 2000 万美元年收入的服务商，须与模型开发者分享最高 30%的服务总收入。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://meyka.com/blog/moonshot-ai-negotiates-revenue-sharing-deals-with-microsoft-amazon-and-google-2608/">Moonshot AI Negotiates Revenue - Sharing Deals With... | Meyka</a></li>
<li><a href="https://techgolly.com/moonshot-ai-weighs-landmark-30-cloud-revenue-sharing-deals-with-us-tech-giants">Moonshot AI Weighs Landmark 30% Cloud Revenue - Sharing Deals ...</a></li>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K 3 Tech Blog: Open Frontier Intelligence</a></li>

</ul>
</details>

**标签**: `#AI`, `#Moonshot AI`, `#Kimi K3`, `#Revenue Sharing`, `#Cloud Providers`

---

<a id="item-11"></a>
## [xAI 发布 Grok 4.6，强化智能体与视觉任务，追平 GPT-5.6 Sol 基准](https://t.me/zaihuapd/43559) ⭐️ 8.0/10

xAI 于 2026 年 8 月 12 日发布 Grok 4.6，在 Grok 4.5 基础上强化了长时间运行的智能体任务、交互与视觉能力。该模型即日在 Cursor、Grok Build 和 API 上线，定价为每百万输入 token 2 美元、每百万输出 token 6 美元，另有双倍价格的快速版。 Grok 4.6 在 Artificial Analysis 智能指数上与 GPT-5.6 Sol 持平，表明 xAI 已跻身头部模型阵营，竞争将进一步加剧。对长时间运行的智能体任务的强化顺应了行业向自主多步工作流演进的方向，将影响 Cursor、Grok Build 和 xAI API 上的开发者与产品。 Artificial Analysis 智能指数综合了九项基准，包括 GDPval-AA v2、τ³-Banking、Terminal-Bench v2.1、SciCode、Humanity's Last Exam、GPQA Diamond、CritPt、AA-Omniscience 与 AA-LCR。报道中的定价为标准版，另有双倍价格的快速版。

telegram · zaihuapd · 9月2日 08:10

**背景**: Artificial Analysis 智能指数是一个综合基准分数，用于衡量模型在推理、编程、知识、指令遵循、科学推理以及多步任务上的能力。智能体任务指 AI 系统在较少人工干预下进行规划、调用工具并完成任务流程。Grok Build 是 xAI 的命令行编程智能体，Cursor 是 AI 辅助代码编辑器；Grok 4.6 在这两个平台上线，突出了 xAI 面向开发者的智能体工作流布局。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/evaluations/artificial-analysis-intelligence-index">Artificial Analysis Intelligence Index v4.1.1 | Artificial Analysis</a></li>
<li><a href="https://www.uipath.com/ai/agentic-ai">What is Agentic AI ? | UiPath</a></li>
<li><a href="https://docs.x.ai/build/overview">Grok Build : SpaceXAI's Coding Agent | SpaceXAI Docs</a></li>

</ul>
</details>

**标签**: `#xAI`, `#Grok`, `#AI models`, `#agents`, `#benchmarks`

---