---
layout: default
title: "Horizon Summary: 2026-07-10 (ZH)"
date: 2026-07-10
lang: zh
---

> 从 38 条内容中筛选出 10 条重要资讯。

---

1. [OpenAI 发布 GPT-5.6，在 ARC-AGI-3 上创下新 SOTA](#item-1) ⭐️ 10.0/10
2. [欧盟议会通过漏洞批准聊天控制 1.0](#item-2) ⭐️ 9.0/10
3. [TypeScript 7.0 正式发布：Go 重写带来最高 12 倍速度提升](#item-3) ⭐️ 9.0/10
4. [蚂蚁开源灵波视频：首个 MoE 具身视频模型](#item-4) ⭐️ 9.0/10
5. [Rust 重写 PostgreSQL 通过全部回归测试](#item-5) ⭐️ 8.0/10
6. [Meta 发布 Muse Spark 1.1 代理型 AI 模型](#item-6) ⭐️ 8.0/10
7. [Meta 超级智能更新：RL 创业公司、算力激增与建议](#item-7) ⭐️ 8.0/10
8. [大疆 EV50 垂直起降无人机飞越珠峰 8861 米](#item-8) ⭐️ 8.0/10
9. [国家超算互联网核心节点郑州上线，提供超 10 万卡国产算力](#item-9) ⭐️ 8.0/10
10. [OpenAI 与美国战争部拟禁止 AI 监控公民](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI 发布 GPT-5.6，在 ARC-AGI-3 上创下新 SOTA](https://openai.com/index/gpt-5-6/) ⭐️ 10.0/10

OpenAI 发布了其最新的前沿模型 GPT-5.6，在 ARC-AGI-3 基准测试上取得了 7.8% 的新 SOTA 分数，并引入了意图理解和原始图像细节保留等功能。该模型提供三种尺寸：Luna、Terra 和 Sol。 此次发布推动了 AI 推理和代理能力的前沿发展，因为 GPT-5.6 是首个在 ARC-AGI-3 游戏中获胜的经过验证的前沿模型。改进的意图理解能力减少了对显式逐步指令的需求，可能降低复杂任务自动化的门槛。 三种模型尺寸的定价为：Luna 每百万输入/输出 token 1 美元/6 美元，Terra 2.50 美元/15 美元，Sol 5 美元/30 美元。GPT-5.6 在 BenchCAD 上也取得了高分，表明它在编程 CAD 数据上接受了专门训练。

hackernews · logickkk1 · 7月9日 17:04 · [社区讨论](https://news.ycombinator.com/item?id=48849066)

**背景**: ARC-AGI-3 是一个交互式推理基准测试，挑战 AI 智能体在抽象的回合制游戏中探索新环境、推断目标并规划行动。它旨在衡量类人智能和代理能力。像 GPT-5.6 这样的前沿模型代表了最先进的 AI 系统，通常结合大规模预训练和推理技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>
<li><a href="https://arxiv.org/abs/2603.24621">[2603.24621] ARC-AGI-3: A New Challenge for Frontier Agentic Intelligence</a></li>

</ul>
</details>

**社区讨论**: 社区反应普遍积极，称赞意图理解和图像保留功能，以及在 ARC-AGI-3 上取得的 SOTA。一些用户指出，OpenAI 在生物学基准测试中省略了与 Fable 5 的比较，因为 Fable 5 拒绝回答高级生物学问题。开发者们也在争论是否要从 Claude Code 切换到 OpenAI 的 codex 模型。

**标签**: `#GPT-5.6`, `#OpenAI`, `#AI`, `#frontier model`, `#ARC-AGI-3`

---

<a id="item-2"></a>
## [欧盟议会通过漏洞批准聊天控制 1.0](https://www.patrick-breyer.de/en/eu-parliament-greenlights-chat-control-1-0-breyer-our-children-lose-out/) ⭐️ 9.0/10

欧洲议会批准了‘聊天控制 1.0’的延期，该法规允许美国科技公司在无需授权的情况下扫描私人信息直至 2028 年，尽管多数欧洲议会议员投票反对（314 票反对，276 票赞成，17 票弃权）。由于否决该法规的动议未能获得所需的 361 票绝对多数，该措施得以通过。 这一决定为欧盟的数字隐私和加密技术树立了一个令人担忧的先例，可能削弱端到端加密并导致大规模监控。它影响到 Instagram、Discord、Snapchat、Gmail 和 iCloud 等平台上的数百万用户，并可能助长其他地区采取类似措施。 该法规被称为‘聊天控制 1.0’，最初是 2021 年的临时措施，原定到期，但其延期被加速推进并于 2026 年 7 月 9 日通过，使用了需要绝对多数才能否决的紧急程序。该法律允许对私人信息进行客户端扫描以查找儿童性虐待材料，但批评者认为这实际上强制实施大规模监控并破坏加密。

hackernews · rapnie · 7月9日 11:03 · [社区讨论](https://news.ycombinator.com/item?id=48843923)

**背景**: 聊天控制是欧盟旨在打击网络儿童性虐待的法规，要求数字平台检测并报告此类材料。公民社会组织认为该提案削弱了端到端加密并侵犯基本隐私权。第一个版本（聊天控制 1.0）是临时措施，于 2026 年 3 月结束，但现在被恢复至 2028 年。更全面的聊天控制 2.0 仍在讨论中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control_1.0">Chat Control 1.0</a></li>
<li><a href="https://www.techtimes.com/articles/320010/20260709/eu-parliament-passes-chat-control-default-314-meps-couldnt-block-scanning-law.htm">EU Parliament Passes Chat Control by Default: 314 MEPs Couldn ...</a></li>
<li><a href="https://samsungmagazine.eu/en/2026/07/09/chat-control/">The end of privacy on the internet. Chat Control passed the ...</a></li>

</ul>
</details>

**社区讨论**: 社区评论强烈批评议会程序是不民主的诡计，指出投票安排在暑假前，且需要绝对多数才能否决，导致少数人通过了该法律。评论者担心这为欧盟的‘极权主义’开创了危险先例，并破坏了欧盟项目的合法性。

**标签**: `#privacy`, `#EU regulation`, `#mass surveillance`, `#encryption`, `#digital rights`

---

<a id="item-3"></a>
## [TypeScript 7.0 正式发布：Go 重写带来最高 12 倍速度提升](https://devblogs.microsoft.com/typescript/announcing-typescript-7-0/) ⭐️ 9.0/10

微软正式发布 TypeScript 7.0，这是用 Go 语言重写的原生版本，完整构建速度比旧版快 8 到 12 倍，并支持共享内存多线程。用户可通过 LSP 在主流编辑器中使用新的语言服务器。 这是 TypeScript 工具链的范式转变，通过大幅缩短构建时间并支持并行项目构建，显著提升开发者生产力。Go 重写标志着一次重大的架构变革，可能影响其他编译器项目。 TypeScript 7.0 引入了 --checkers 和 --builders 参数以自定义并行度，但 Vue、Svelte 等嵌入式语言工具链目前尚未支持，仍需使用 TypeScript 6。同时提供了兼容包以实现与 TypeScript 6 并存安装。

telegram · zaihuapd · 7月9日 04:01

**背景**: TypeScript 是 JavaScript 的类型超集，可编译为纯 JavaScript，广泛用于大规模 Web 开发。语言服务器协议（LSP）标准化了编辑器与语言服务器之间的通信，支持自动补全和诊断等功能。之前的 TypeScript 版本由 TypeScript 自身编写，在大项目中存在性能瓶颈。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://devblogs.microsoft.com/typescript/announcing-typescript-7-0/">Announcing TypeScript 7.0 - TypeScript</a></li>
<li><a href="https://en.wikipedia.org/wiki/Language_Server_Protocol">Language Server Protocol - Wikipedia</a></li>
<li><a href="https://devblogs.microsoft.com/typescript/announcing-typescript-7-0-rc/">Announcing TypeScript 7.0 RC - TypeScript</a></li>

</ul>
</details>

**标签**: `#TypeScript`, `#Microsoft`, `#Performance`, `#Compiler`

---

<a id="item-4"></a>
## [蚂蚁开源灵波视频：首个 MoE 具身视频模型](https://www.qbitai.com/2026/07/446458.html) ⭐️ 9.0/10

蚂蚁灵波开源了全球首个基于 MoE 架构的具身智能视频生成基础模型 LingBot-Video。该模型总参数量 300 亿，生成时仅激活约 30 亿，推理效率约为同等规模 Dense 架构的 3 倍。 这代表了具身智能领域的重大突破，为机器人动作预测、仿真数据生成和世界模型研究提供了更高效、能力更强的基础模型。开源举措有望加速机器人和具身智能领域的整体发展。 模型采用 DiT+MoE 架构、7 万小时具身数据引擎（涵盖灵巧操作、机器人移动和第一视角交互），并引入多维强化学习奖励系统，关注物理合理性和任务完成度。它以 Apache 2.0 许可证在 GitHub 开源。

telegram · zaihuapd · 7月9日 04:30

**背景**: 混合专家（MoE）架构通过使用多个专门的子网络（专家）和一个路由器，每输入只激活相关专家，从而以较低计算成本实现更大模型。DiT（扩散 Transformer）将扩散模型与 Transformer 架构结合，用于高质量视频生成。具身智能是指能够感知并在物理世界中行动的 AI 系统，例如机器人。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/mixture-of-experts/">What Is Mixture of Experts (MoE) and How It Works?</a></li>
<li><a href="https://huggingface.co/docs/diffusers/api/pipelines/dit">DiT · Hugging Face</a></li>

</ul>
</details>

**标签**: `#MoE`, `#具身智能`, `#视频生成`, `#机器人`, `#开源`

---

<a id="item-5"></a>
## [Rust 重写 PostgreSQL 通过全部回归测试](https://github.com/malisper/pgrust) ⭐️ 8.0/10

一位开发者成功用 Rust 重写了 PostgreSQL，借助大语言模型生成的代码，100%通过了官方回归测试套件。 这表明用内存安全语言重写成熟复杂数据库系统的可行性，有望在保持完全兼容的同时提升安全性和性能。 该项目 pgrust 使用 LLM 在一个月内生成了 7101 次提交，引发了关于代码审查和长期可维护性的讨论。

hackernews · SweetSoftPillow · 7月9日 06:18 · [社区讨论](https://news.ycombinator.com/item?id=48841676)

**背景**: PostgreSQL 是一个有 30 年历史的用 C 编写的关系型数据库。回归测试套件是一套全面的 SQL 测试，确保正确性。Rust 是一种以无垃圾回收的内存安全著称的系统编程语言。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/malisper/pgrust">GitHub - malisper/pgrust: Postgres rewritten in Rust, now ...</a></li>
<li><a href="https://malisper.me/pgrust-rebuilding-postgres-in-rust-with-ai/">pgrust: Rebuilding Postgres in Rust with AI - malisper.me</a></li>
<li><a href="https://www.postgresql.org/docs/current/regress.html">PostgreSQL: Documentation: 18: Chapter 31. Regression Tests</a></li>

</ul>
</details>

**社区讨论**: 社区成员表达了对单人重写、可维护性以及使用 AI 生成代码的担忧，建议在实际工作负载下测试，并对长期可行性表示怀疑。

**标签**: `#PostgreSQL`, `#Rust`, `#database`, `#rewrite`, `#LLM`

---

<a id="item-6"></a>
## [Meta 发布 Muse Spark 1.1 代理型 AI 模型](https://ai.meta.com/blog/introducing-muse-spark-meta-model-api/) ⭐️ 8.0/10

Meta 宣布推出全新代理型 AI 模型 Muse Spark 1.1，并同步发布 API 定价、评估报告和开发者资源。该模型支持文本、图像和语音输入，上下文窗口达 262k 个 token。 此次发布标志着 Meta 进入商用代理型 AI 市场，其定价远低于 Anthropic 和 OpenAI 等竞争对手。这可能会使编程代理商品化，并促使其他供应商降低价格。 定价为输入每百万 token 1.25 美元，输出 4.5 美元，缓存输入仅 0.15 美元。该模型具备工具使用、视觉思维链和多代理编排能力，但并非开源。

hackernews · ot · 7月9日 14:10 · [社区讨论](https://news.ycombinator.com/item?id=48846184)

**背景**: 代理型 AI 指能够使用工具、规划并自主行动以实现目标的系统。Meta 以往的 AI 模型多为开放权重，但 Muse Spark 闭源且通过 API 访问，反映了其向商业化转型的战略。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ai.meta.com/blog/introducing-muse-spark-meta-model-api/">Introducing Muse Spark 1.1</a></li>
<li><a href="https://artificialanalysis.ai/models/muse-spark">Muse Spark - Intelligence, Performance & Price Analysis</a></li>
<li><a href="https://agentic.ai/what-is-agentic-ai">What Is Agentic AI? Definition, 6 Levels & Examples (2026)</a></li>

</ul>
</details>

**社区讨论**: 开发者对基准测试的有效性提出质疑，指出评估任务超出了资源限制。另有人赞赏其低廉定价和实用易用性，同时也有批评其闭源做法，认为闭源领域只有 Anthropic 和 OpenAI 值得关注。

**标签**: `#AI`, `#Meta`, `#Muse Spark`, `#agentic model`, `#open source`

---

<a id="item-7"></a>
## [Meta 超级智能更新：RL 创业公司、算力激增与建议](https://newsletter.semianalysis.com/p/the-future-of-meta-superintelligence) ⭐️ 8.0/10

Meta 的超级智能项目中诞生了一家顶级强化学习环境创业公司，同时出现了迄今为止最激进的算力激增，跨 2000 公里以上的规模扩展，以及针对 Google DeepMind 的直接建议。 这一更新标志着 Meta 向超级智能的全力冲刺，可能重塑 AI 实验室之间的竞争格局，并推动前所未有的基础设施投资。 算力激增包括一种新的‘帐篷’数据中心设计，可实现快速扩展；RL 环境创业公司被描述为‘凭空出现’，很可能涉及人才收购或内部拆分。

rss · Semianalysis · 7月9日 19:16

**背景**: 强化学习（RL）环境是虚拟沙盒，AI 模型在其中通过采取行动并获得评分来学习。跨规模网络将相距数百公里的数据中心互联，形成一个超级计算机。Meta 的超级智能项目旨在实现通用人工智能（AGI）或更高水平，需要巨大的算力和专门的基础设施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://benanderson.work/blog/dont-build-rl-env-startup/">Don't Build an RL Environment Startup</a></li>
<li><a href="https://www.broadcom.com/topics/what-is-scale-across-networking-for-ai-clusters">Scale-across Networking | AI Clusters | AI Infrastructure</a></li>
<li><a href="https://www.keysight.com/blogs/en/inds/ai/ai-infrastructure-scaling-domains">AI Infrastructure Scaling Domains</a></li>

</ul>
</details>

**标签**: `#AI`, `#Meta`, `#superintelligence`, `#reinforcement learning`, `#compute infrastructure`

---

<a id="item-8"></a>
## [大疆 EV50 垂直起降无人机飞越珠峰 8861 米](https://www.163.com/dy/article/L1CUCV940514R9OJ.html) ⭐️ 8.0/10

大疆尚未发布的 EV50 垂直起降运载无人机飞越珠穆朗玛峰海拔 8861 米，创下高海拔无人机飞行纪录，并在 8000 米以上获取大气数据。 此次成就证明了大疆在极端环境下的工程能力，并展示了垂直起降无人机在高海拔物流和科研领域的潜力。 EV50 是一款复合翼无人机，可垂直起降并切换至固定翼巡航。在为期 12 天的任务中，它完成了 32 架次起降，连续爬升 3730 米，返程时剩余 30%电量。

telegram · zaihuapd · 7月9日 06:00

**背景**: 垂直起降无人机结合了多旋翼的灵活性和固定翼飞机的效率。在 8000 米以上高空飞行面临空气稀薄和极端低温等挑战，需要强劲的动力和电池系统。大疆以消费级无人机闻名，如今正进入货运无人机市场。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dronexl.co/2026/07/09/dji-ev50-evtol-delivery-drone-everest/">DJI EV50 Debuts As Company's First EVTOL Delivery Drone With ...</a></li>
<li><a href="https://pandaily.com/dji-ev50-everest-vtol-cargo-drone-jul2026">DJI Unreleased EV50 VTOL Cargo Drone Flies Above Everest ...</a></li>
<li><a href="https://aviationweek.com/business-aviation/aircraft-propulsion/dji-enters-fixed-wing-evtol-cargo-drone-market">DJI Enters Fixed-Wing eVTOL Cargo Drone Market</a></li>

</ul>
</details>

**标签**: `#drone`, `#VTOL`, `#high-altitude`, `#logistics`, `#DJI`

---

<a id="item-9"></a>
## [国家超算互联网核心节点郑州上线，提供超 10 万卡国产算力](https://36kr.com/newsflashes/3887797387344387) ⭐️ 8.0/10

2026 年 7 月 9 日，国家超算互联网核心节点在郑州正式上线运行，可对外提供超过 10 万卡的国产人工智能算力。这是该平台上线以来接入的最大规模单体国产 AI 算力资源池。 这一里程碑显著增强了中国在 AI 算力基础设施上的自主可控能力，为全国计算资源提供统一调度体系。通过提供大规模国产算力，将加速 AI 研发、工业仿真和科学计算等应用。 该核心节点集成了超过 10 万张国产 AI 加速卡（如寒武纪、华为昇腾等），承担国家超算互联网平台的运营管理和资源调度核心功能。同时整合供需对接、产业孵化等综合服务。

telegram · zaihuapd · 7月9日 07:00

**背景**: 国家超算互联网是由科技部牵头建设的国家级项目，于 2023 年 4 月启动，旨在将全国超算中心连接成一体化服务网络。其目标是打破各算力中心之间的孤岛，实现计算资源的高效调度，服务于科学研究、AI 训练和工业应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://local.cctv.com/2026/07/09/ARTIGxl4CPHCEclGCTrNzq34260709.shtml">国内首个十万卡级超智融合算力资源池在郑上线_地方频道_央视网 (cct...</a></li>
<li><a href="https://baike.baidu.com/item/国家超算互联网/62902938">国家超算互联网 - 百度百科 国家超算互联网 - 高性能计算服务与 AI 服务平台 - AIHub 国家超算互联网平台上线 - 中国政府网 超算互联网 - 百度百科 国家超算互联网用户规模破百万 - 中国政府网 国家超算互联网正式上线 DeepSeek，全民可用！国家队强势助力！</a></li>
<li><a href="https://www.scnet.cn/home/internet/index.html">超算互联网 - scnet.cn</a></li>

</ul>
</details>

**标签**: `#supercomputing`, `#AI infrastructure`, `#domestic chips`, `#China`, `#national computing network`

---

<a id="item-10"></a>
## [OpenAI 与美国战争部拟禁止 AI 监控公民](https://t.me/zaihuapd/42459) ⭐️ 8.0/10

OpenAI 与美国战争部（原国防部）已同意修改双方的人工智能合作协议，增加禁止使用 AI 对美国公民进行蓄意监控的条款，该提议由 OpenAI 首席执行官 Sam Altman 主动提出。 此举回应了公众对 AI 被军方用于大规模监控的担忧，为政府 AI 合同中的伦理边界树立了先例，也与其竞争对手 Anthropic 与战争部搁置的类似协议形成对比。 修订后的条款明确禁止 AI 系统用于对美国公民的蓄意监控，并禁止利用商业获取的个人身份信息进行追踪或监测。目前该修正案尚未正式签署。

telegram · zaihuapd · 7月9日 13:22

**背景**: 美国战争部是国防部的前身，其参与 AI 合作以用于国家安全。此前有报道称其他 AI 公司如 Anthropic 因类似的军事合同引发争议，导致对 AI 监控的担忧加剧。OpenAI 的提议旨在确保 AI 在负责任的前提下使用，不侵犯公民自由。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>
<li><a href="https://www.anthropic.com/">Home \ Anthropic</a></li>

</ul>
</details>

**标签**: `#AI ethics`, `#OpenAI`, `#US government`, `#surveillance`, `#policy`

---