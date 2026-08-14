---
layout: default
title: "Horizon Summary: 2026-08-14 (ZH)"
date: 2026-08-14
lang: zh
---

> 从 34 条内容中筛选出 10 条重要资讯。

---

1. [DRAM“面条化”攻击暴露隐藏 CPU 功能](#item-1) ⭐️ 9.0/10
2. [DeepMind 发布手语转文字模型 SL2T 落地 Pixel 11](#item-2) ⭐️ 9.0/10
3. [DeepSeek 开源 Harness 并开放 V4-Pro-0813 权重](#item-3) ⭐️ 9.0/10
4. [谷歌推出 Gemini 3.7 Flash：视觉转 HTML 与大幅折扣引热议](#item-4) ⭐️ 8.0/10
5. [Cerebras 与 OpenAI 称 GPT-5.6 Sol Ultrafast 推理速度提升约 7 倍](#item-5) ⭐️ 8.0/10
6. [理解力成为软件工程的新瓶颈](#item-6) ⭐️ 8.0/10
7. [选择无聊技术：丹·麦金利谈创新代币](#item-7) ⭐️ 8.0/10
8. [特朗普签署备忘录授权私企开展政府背书的网络攻击](#item-8) ⭐️ 8.0/10
9. [谷歌发布 Gemini 3.6 Flash，Gemini 4 已开始预训练](#item-9) ⭐️ 8.0/10
10. [X 扩大算法开源范围，新增影子封禁查看工具](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [DRAM“面条化”攻击暴露隐藏 CPU 功能](https://github.com/xoreaxeaxeax/skitter-creek-bath-salts) ⭐️ 9.0/10

安全研究员 Christopher Domas 演示了一种名为“Spaghettifying DRAM”的新型硬件攻击，通过操纵 DRAM 来暴露隐藏的处理器功能并绕过 CPU 保护环。该攻击是在 AMD Family 16h CPU 上开发和测试的。 这项研究揭示了 DRAM 子系统可能被武器化，从而破坏处理器的安全边界，可能威胁依赖环保护的游戏机和其他系统。它强调了 DRAM 在硬件安全领域中正成为日益增长的攻击面。 该攻击针对 DRAM 控制器的转换寄存器，AMD Family 16h 的数据手册显示这些寄存器无法被锁定。根据 README，Zen 3 的内存控制器寄存器基地址不同，因此对较新 CPU 的具体影响尚不明确。

hackernews · matt_d · 8月13日 14:17 · [社区讨论](https://news.ycombinator.com/item?id=49286341)

**背景**: “面条化”（Spaghettification）是一个物理学术语，描述极端潮汐力将物体拉伸成细长形状的过程。在计算领域，未文档化的 CPU 指令是指硬件中存在但官方文档未记录的操作码，有时可以绕过软件防护。该攻击借用这个比喻来描述操纵 DRAM 行为以到达隐藏的特权处理器状态，显示底层硬件细节如何成为安全漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49286341">Spaghettifying DRAM | Hacker News</a></li>
<li><a href="https://en.wikipedia.org/wiki/Spaghettification">Spaghettification - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Illegal_opcode">Illegal opcode - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论称赞 Christopher Domas 是一流的安全研究员，并期待他的 Black Hat 演讲。一些人担心一旦获得 ring-0 权限，该技术可能危及 Xbox 和 PlayStation 的安全，另一些人则质疑除了 AMD Jaguar 之外还有哪些较新的 CPU 家族受影响。

**标签**: `#security`, `#hardware`, `#DRAM`, `#exploitation`, `#reverse engineering`

---

<a id="item-2"></a>
## [DeepMind 发布手语转文字模型 SL2T 落地 Pixel 11](https://deepmind.google/blog/putting-sign-language-ai-into-users-hands/) ⭐️ 9.0/10

DeepMind 发布了大规模多语言手语转文字模型 SL2T，现已登陆 Pixel 11 的 Gboard 和 Live Transcribe，支持美国手语转英语。这是手语 AI 首次进入消费级产品。 SL2T 是无障碍领域的重大进步，为聋人和听障用户提供了内置的实时手语翻译工具。它在 FLEURS-ASL 上取得 70 BLEURT 的零样本成绩，表明该技术有望扩展到更多手语和设备。 该模型使用了超过 10 万小时、涵盖 50 多种手语的数据进行训练。为了保护隐私，它只处理手部和身体姿态关键点，而不读取原始视频。

telegram · zaihuapd · 8月13日 08:55

**背景**: 手语翻译系统技术难度很高，因为它需要捕捉手势形状、运动轨迹和语法，而这些都是非语音信息。FLEURS-ASL 是基于 FLEURS 框架构建的美国手语翻译基准测试集，由持证聋人翻译员参与开发。BLEURT 是一种学习型评估指标，通过比较候选译文与参考译文来评价翻译质量。SL2T 的零样本得分意味着它可以翻译未经专门微调的语言，这对扩展到多种手语至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://explainx.ai/blog/google-sl2t-asl-sign-language-text-pixel-11-2026">Google SL2T: ASL -to-Text Comes to Pixel 11 | explainx.ai... | explainx.ai</a></li>
<li><a href="https://arxiv.org/html/2408.13585">FLEURS - ASL : Including American Sign Language in Massively...</a></li>
<li><a href="https://github.com/google-research/bleurt">GitHub - google-research/ bleurt : BLEURT is a metric for Natural...</a></li>

</ul>
</details>

**标签**: `#AI`, `#Sign Language`, `#DeepMind`, `#Accessibility`, `#Speech-to-Text`

---

<a id="item-3"></a>
## [DeepSeek 开源 Harness 并开放 V4-Pro-0813 权重](https://mp.weixin.qq.com/s/mANdGRI4fO_sEbC1ECEoZQ) ⭐️ 9.0/10

DeepSeek 发布了以 MIT 协议开源的智能体框架应用 DeepSeek Harness，同时在 Hugging Face 开放了 DeepSeek-V4-Pro-0813 的权重。GitHub 仓库现已公开，不过 Hugging Face 页面曾短暂出现 404，随后恢复。 作为顶尖 AI 实验室的发布，这为开发者提供了一个开源且与模型无关的选择，可替代 Claude Code、Codex 等专有智能体基础设施。这可能加速社区的实验和自托管智能体开发。 DeepSeek Harness（dsh）采用“一切皆插件”的架构，由 Cordis 插件框架驱动，提供标准、PTC（Programmatic Tool Calling）、极简和创造四种运行模式。DeepSeek-V4-Pro-0813 的权重在短暂中断后已可在 Hugging Face 获取。

telegram · zaihuapd · 8月13日 12:39

**背景**: 智能体框架（agent harness）是将 AI 模型与工具、会话、存储和用户界面连接起来的基础设施，使智能体能够执行复杂的多步任务。DeepSeek Harness 将其实现为一组可替换的插件，底层框架 Cordis 支持在不重启进程的情况下热加载和干净卸载插件。DeepSeek-V4-Pro-0813 是 DeepSeek 新发布的模型，权重已开放供直接使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.deepseek.com/harness/en/">DeepSeek Harness developer preview: Everything is a plugin</a></li>
<li><a href="https://github.com/deepseek-ai/deepseek-harness/tree/master">GitHub - deepseek-ai/deepseek-harness: DeepSeek Harness: Everything is ...</a></li>
<li><a href="https://www.npmjs.com/package/@deepseek-ai/cordis">@deepseek-ai/cordis - npm</a></li>

</ul>
</details>

**社区讨论**: Hacker News 评论者总体积极但保持谨慎：一位作者表示这只是早期开发者预览版，仍有粗糙之处；另有人称赞可追溯的只追加（append-only）会话日志，认为这是相比美国模型加密轨迹的“杀手级特性”。还有人讨论了底层 Cordis 插件框架，也有人对“一切皆插件”的架构表示“插件疲劳”。

**标签**: `#DeepSeek`, `#AI`, `#Open Source`, `#Model Release`, `#Harness`

---

<a id="item-4"></a>
## [谷歌推出 Gemini 3.7 Flash：视觉转 HTML 与大幅折扣引热议](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/) ⭐️ 8.0/10

谷歌发布了 Gemini 3.7 Flash，这是 Gemini Flash 系列最新款“主力”模型，推理、文档理解能力提升，并具备强大的视觉转 HTML 能力。该模型以深度折扣的首发价格提供，预计在 2026 年底的促销期结束后上调价格。 Gemini Flash 系列是谷歌面向高吞吐、低延迟场景的高性价比主力模型，此次在推理和视觉转代码能力上的明显提升，可能改变开发者的选型，并给整个大模型市场带来定价压力。它同时也表明与 GPT-5.6 Luna、Anthropic Opus 等模型的竞争正在加剧。 据谷歌数据，3.7 Flash 在 GDP.pdf 文档基准上大幅超过 3.6 Flash（34.0% 对 22.0%），在 AutomationBench 商业流程基准上也超过 3.6 Flash（30.4% 对 17.0%）。该模型的首发价格异常低，并计划在 2027 年初上调；其发布距离 3.6 Flash 仅约三周。

hackernews · thisisauserid · 8月13日 17:23 · [社区讨论](https://news.ycombinator.com/item?id=49289112)

**背景**: Gemini 是 Google DeepMind 开发的多模态大语言模型系列，最初于 2023 年 12 月发布，并支持 Gemini 聊天机器人。Flash 层级定位为更便宜、更快、面向开发者的“主力”模型，同时支持图像、音频和文本输入。谷歌近期的模型迭代节奏很快，用较低的首发价格吸引开发者使用新版本也是常见策略。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/">Gemini 3.7 Flash: our most intelligent workhorse model</a></li>
<li><a href="https://deepmind.google/models/gemini/flash/">Gemini 3.7 Flash — Google DeepMind</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gemini_2.5_Flash_Image">Gemini 2.5 Flash Image</a></li>

</ul>
</details>

**社区讨论**: 评论者积极对模型进行测试，尤其是视觉转 HTML：有测试发现 Anthropic 的 Opus 5 仍在该任务领先，但 Gemini 3.7 Flash 在其价位上表现不错。Simon Willison 认为首发定价“很奇怪”，因为模型可能在涨价前就被新版本取代；也有评论者认为 GPT-5.6 Luna 在 DeepSWE 1.1 基准上仍更优。总体情绪偏正面但克制，部分人认为在折扣价下这是一次扎实的发布，但错失了更大规模冲击市场的机会。

**标签**: `#Gemini`, `#AI model`, `#Google`, `#LLM`, `#announcement`

---

<a id="item-5"></a>
## [Cerebras 与 OpenAI 称 GPT-5.6 Sol Ultrafast 推理速度提升约 7 倍](https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai) ⭐️ 8.0/10

Cerebras 与 OpenAI 宣布推出由 Cerebras 晶圆级引擎驱动的 GPT-5.6 Sol Ultrafast 模式，输出速度最高可达每秒 750 个 token。在对比测试中，Ultrafast 在 11 小时 11 分钟内完成了全部 2,500 道 Humanity's Last Exam 题目，而 Claude Fable 5 耗时 78 小时 27 分钟，在准确率相当的情况下实现了近 7 倍的速度提升。 这一里程碑表明，前沿 AI 推理速度可以大幅提升，有望让高端模型在交互式和迭代式工作流中变得更加实用。同时，它也凸显了推理优化作为与模型原始质量并列的竞争前沿，其重要性正在不断上升。 Cerebras 报告称，根据 Artificial Analysis 的输出速度数据，Ultrafast 模式比 Fable 5 快 11 倍，比 Fast 模式下的 Opus 4.8 快 5 倍。OpenAI 的公告还提到，相比标准模式，Ultrafast 的 token 输出速度最高可提升 14 倍，但目前尚未公布定价信息。

hackernews · pr337h4m · 8月13日 18:10 · [社区讨论](https://news.ycombinator.com/item?id=49289844)

**背景**: Cerebras 制造晶圆级引擎，这是一种将整个硅晶圆整合为单芯片的巨大 AI 处理器——CS-3 包含 4 万亿个晶体管、90 万个 AI 优化核心和 44GB 片上 SRAM，提供每秒 21 PB 的内存带宽。这种架构非常有利于低延迟推理，因为它避免了 GPU 系统中常见的内存瓶颈。GPT-5.6 Sol 是 OpenAI 的前沿模型，Ultrafast 模式是 Cerebras 托管的一个服务层，可以极快的速度运行该模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai">Accelerating GPT - 5 . 6 Sol Ultrafast with OpenAI</a></li>
<li><a href="https://openai.com/index/previewing-ultrafast/">Previewing Ultrafast mode: GPT - 5 . 6 Sol at up to 14X the... | OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cerebras_Systems">Cerebras Systems - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者对这一合作感到兴奋，但对性能一致性持怀疑态度：有用户指出，Cerebras 和 OpenAI 都没有明确表示 Ultrafast 在所有设置下都能产生与普通 Sol 完全相同的结果。另一些人则指出，速度本身可以通过实现迭代修正来提高输出质量，同时他们也注意到缺乏定价信息，并质疑这是否真的是 1:1 的替代品。

**标签**: `#LLM inference`, `#performance optimization`, `#OpenAI`, `#Cerebras`, `#GPT`

---

<a id="item-6"></a>
## [理解力成为软件工程的新瓶颈](https://www.geoffreylitt.com/2026/07/02/understanding-is-the-new-bottleneck) ⭐️ 8.0/10

Geoffrey Litt 认为，随着 LLM 自动化代码生成，软件开发的关键瓶颈正在转向对现有代码库和意图的理解。文章指出，开发者工作流需要调整，优先重视代码理解而非编写代码。 这一重新定义对开发者生产力和 AI 工具设计有重要影响：如果理解力是瓶颈，那么提升代码理解能力的工具可能比代码生成模型更有价值。它也凸显了自动化与人类监督需求之间日益增长的张力。 这篇文章引发了 200 分、111 条评论的社区讨论，表明读者参与度很高。评论指出，LLM 生成的 PR 描述常常因缺乏动机而遭反感，而且人类仍需阅读代码来验证 LLM 的输出。

hackernews · sebg · 8月13日 18:47 · [社区讨论](https://news.ycombinator.com/item?id=49290299)

**背景**: 几十年来，软件工程中的主要瓶颈被认为是编写代码。随着 AI 代码生成器的进步，这一瓶颈正被大量自动化，从而暴露出代码理解是新的限制因素。理解现有代码库、意图和系统行为，如今被认为是开发者面临的关键挑战。

**社区讨论**: 评论者意见不一：有人认为这个问题在 LLM 出现之前就存在，反映了工程领导力的长期挑战；也有人担心用 LLM 来进行理解会形成循环验证问题。少数评论者持怀疑态度，要求提供更多证据说明瓶颈究竟在哪里。总体而言，大家强烈认同即使在 AI 辅助下，人类仍然要为代码的后果负责。

**标签**: `#LLM`, `#software engineering`, `#code comprehension`, `#AI tools`, `#developer productivity`

---

<a id="item-7"></a>
## [选择无聊技术：丹·麦金利谈创新代币](https://mcfunley.com/choose-boring-technology) ⭐️ 8.0/10

丹·麦金利于 2015 年发表的文章主张，公司应默认使用成熟、无惊喜的“无聊”技术，并以“创新代币”这一固定预算来节制地引入新工具。这篇文章已成为工程战略领域的经典，至今仍被广泛引用。 该框架为工程领导者提供了一种简单的方式来权衡新技术带来的隐性成本；在团队面对 AI 和快速演进的工具时，其影响力依然持续。它塑造了许多公司进行技术选型和取舍的方式。 曾就职于 Etsy 的麦金利提出，每家公司大约只有三个创新代币，且在一段时间内数量固定；使用新奇或新技术会消耗代币，而无趣成熟的技术则免费。文章强调应把创新花在业务差异点上，而不是基础设施上。

hackernews · tosh · 8月13日 17:48 · [社区讨论](https://news.ycombinator.com/item?id=49289512)

**背景**: 这篇文章源于麦金利在 Etsy 的经历，并于 2015 年发布；当时许多创业公司过早采用时髦的数据库和工具。这里的“无聊”并非指过时，而是指经过验证、文档完善、被广泛理解的技术，如 PostgreSQL 或 MySQL。创新代币隐喻表达了每个组织对复杂性的接纳能力有限这一观点。这篇文章既启发了实际应用，也引发了直接批评，例如 Glyph 在 2024 年的文章《反对创新代币》。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.lessannoyingbusiness.com/post/innovation-tokens">Innovation Tokens - When to break from the status quo</a></li>
<li><a href="https://hybridcopynet.wordpress.com/2026/01/04/innovation-tokens/">Innovation Tokens – Hybrid Copy</a></li>
<li><a href="https://blog.glyph.im/2024/07/against-innovation-tokens.html">Deciphering Glyph :: Against Innovation Tokens</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论者大多称赞这篇文章；NickNaraghi 称其是工程领导者最实用的概念之一，theptip 则将其应用到 AI 智能体时代，主张智能体应使用“无聊”的分布内技术。然而，insanitybit 提出反对，认为“创新代币”是武断且不严肃的，工程师应直接权衡需求与风险，而不应以新奇性作为粗略指标。

**标签**: `#software-engineering`, `#technology-strategy`, `#engineering-culture`, `#essay`, `#hacker-news`

---

<a id="item-8"></a>
## [特朗普签署备忘录授权私企开展政府背书的网络攻击](https://www.bloomberg.com/news/articles/2026-08-13/trump-enlists-private-sector-to-boost-cyber-offensive-arsenal) ⭐️ 8.0/10

特朗普总统签署备忘录，授权私营企业在联邦政府的直接控制和监督下开展海外监控和网络攻击。国土安全部将负责运行该项目，并与司法部协调监督。 此举标志着一项重大政策转变，将私营部门纳入进攻性网络行动，可能重塑网络安全和科技行业格局。同时，它也引发了关于非国家行为体开展政府背书监视活动所带来的法律、隐私和问责方面的严重担忧。 参与企业须维持至少 100 万美元的保证金或托管款，如不遵守合同约定，该款项将被没收。该项目针对的是伤害美国人的外国网络化跨国犯罪组织。

telegram · zaihuapd · 8月13日 05:10

**背景**: 传统上，进攻性网络行动一直属于政府情报和军事机构的职责范围。这份备忘录正式授权私营企业在政府指导下开展此类活动，由国土安全部监督、司法部协调，标志着一种转变。此举反映了网络安全领域公私合作的更广泛趋势，但也引发了关于政府权力边界以及私营部门参与进攻性行动的法律框架的疑问。

**标签**: `#cybersecurity`, `#policy`, `#surveillance`, `#private-sector`, `#government`

---

<a id="item-9"></a>
## [谷歌发布 Gemini 3.6 Flash，Gemini 4 已开始预训练](https://t.me/zaihuapd/43177) ⭐️ 8.0/10

谷歌发布了主打效率提升的 Gemini 3.6 Flash，并同期推出面向高吞吐、低延迟场景的 Gemini 3.5 Flash。官方还透露下一代 Gemini 4 已启动预训练。 Gemini 是许多开发者广泛使用的主流大模型，此次效率提升以及 Gemini 4 预训练的确认，都表明谷歌在激烈的大模型竞争中持续推进。输出 Token 减少约 17%，对高用量应用来说可能显著降低成本。 据官方公告，Gemini 3.6 Flash 通过更少的推理步骤和工具调用来完成多步任务，并在代码生成、知识工作和计算机操作方面有所提升。其知识截止日期更新至 2026 年 3 月，API 定价为每百万输入 Token 1.5 美元、每百万输出 Token 7.5 美元。

telegram · zaihuapd · 8月13日 17:32

**背景**: 大语言模型通常先通过在海量文本上进行预训练来获取广泛的语言和世界知识，因此“Gemini 4 已开始预训练”这一消息具有重要意义。公告中提到的“更少的推理步骤”与链式思考（chain-of-thought）技术相关，即模型将复杂任务拆解为中间步骤；而“工具调用”则指大模型能够接入外部工具或 API 来更高效地完成任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepchecks.com/llm-training-pipelines-pretraining-guide/">LLM Training Pipelines: Key Facts About Pretraining | Deepchecks</a></li>
<li><a href="https://en.wikipedia.org/wiki/Chain-of-thought_reasoning">Chain-of-thought reasoning</a></li>
<li><a href="https://zilliz.com/blog/harnessing-function-calling-to-build-smarter-llm-apps">Understanding Function Calling in LLMs - Zilliz blog</a></li>

</ul>
</details>

**标签**: `#Gemini`, `#Google`, `#AI`, `#LLM`, `#Model Release`

---

<a id="item-10"></a>
## [X 扩大算法开源范围，新增影子封禁查看工具](https://techcrunch.com/2026/08/13/x-open-sources-its-ranking-algorithm-letting-users-see-if-theyve-been-shadowbanned/) ⭐️ 8.0/10

X 于周四宣布大幅扩大开源代码库，将“为你推荐”时间线的排序算法及核心排名引擎以 Apache 2.0 许可证发布到 GitHub，代码规模约为此前的 10 至 15 倍。公司还在设置中推出了透明度工具，符合条件的用户可下载 JSON 文件，查看自己的账号或帖子是否被排名系统标记。 这一举措是向算法透明度和平台问责制迈出的重要一步，让用户和研究者得以了解 X 如何对内容排序，以及账号是否被“影子封禁”。这可能重塑公众对算法偏见的讨论，并影响其他平台对待透明度的方式，尽管它并未公开所有审核环节。 该透明度工具目前仅向注册满一年、且近一个月发帖至少 10 次的测试用户开放。用于判断违规内容的部分 Grok 系统并未随代码一并公开，因此相关审核逻辑仍不透明。

telegram · zaihuapd · 8月14日 01:03

**背景**: X（前身为 Twitter）长期以来一直面临压力，需要解释其“为你推荐”时间线如何对帖子排序，而关于“影子封禁”（即用户不知情的情况下被降低内容可见性）的担忧也普遍存在。这次开源排序算法是继 2023 年规模较小的开源之后的又一次尝试，旨在提供外部可验证性。影子封禁是一种有争议的做法，平台会在不通知用户的情况下限制内容的触达范围。Grok 是 xAI 开发的大语言模型，其部分输出被用于 X 的内容审核流程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/08/13/x-open-sources-its-ranking-algorithm-letting-users-see-if-theyve-been-shadowbanned/">X open sources its ranking algorithm , letting users see... | TechCrunch</a></li>
<li><a href="https://github.com/twitter/the-algorithm">GitHub - twitter/the- algorithm : Source code for the...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Grok_(chatbot)">Grok (chatbot) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#open-source`, `#algorithmic-transparency`, `#social-media`, `#ranking-algorithm`, `#platform-accountability`

---