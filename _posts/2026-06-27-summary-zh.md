---
layout: default
title: "Horizon Summary: 2026-06-27 (ZH)"
date: 2026-06-27
lang: zh
---

> 从 39 条内容中筛选出 8 条重要资讯。

---

1. [DeepSeek 开源 DSpark 投机解码，推理速度提升 60-85%](#item-1) ⭐️ 9.0/10
2. [OpenAI 预览 GPT-5.6 Sol，在 Cerebras 上达到 750 令牌/秒](#item-2) ⭐️ 9.0/10
3. [美国允许 Anthropic 向受信企业有限发布 Mythos 5 AI](#item-3) ⭐️ 9.0/10
4. [数学中的人工智能引发根本性问题](#item-4) ⭐️ 9.0/10
5. [DirtyClone：Linux 内核本地提权漏洞可获 root 权限](#item-5) ⭐️ 9.0/10
6. [SGLang v0.5.14：DeepSeek-V4 在 GB300 上实现 5 倍吞吐量](#item-6) ⭐️ 8.0/10
7. [开放权重与闭源 LLM 的差距：基准测试作弊加剧](#item-7) ⭐️ 8.0/10
8. [苹果评估引入中国内存供应商以降低成本](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [DeepSeek 开源 DSpark 投机解码，推理速度提升 60-85%](https://github.com/deepseek-ai/DeepSpec/blob/main/DSpark_paper.pdf) ⭐️ 9.0/10

DeepSeek 与北京大学联合发布了 DSpark 推理加速框架，采用半自回归候选生成与置信度调度验证机制，将单用户生成速度提升 60% 至 85%。该框架已开源，模型集成于 DeepSeek-V4 Flash 和 Pro 版本中。 DSpark 大幅降低了 LLM 推理延迟，使得 AI 助手响应更快、成本更低。这凸显了中国 AI 实验室的持续创新，并为开源推理优化树立了新标杆。 DSpark 采用并行主干一次性产出所有候选 token 的隐藏状态，再由轻量顺序模块逐 token 注入前缀依赖。置信度调度器动态决定验证长度，优先将算力分配给高存活概率的 token。

hackernews · aurenvale · 6月27日 09:18 · [社区讨论](https://news.ycombinator.com/item?id=48696585)

**背景**: 投机解码是一种推理时优化技术，通过同时预测和验证多个 token 来加速 LLM 生成，减少延迟而不损失输出质量。传统 LLM 逐个生成 token，导致延迟随输出长度线性增长。DSpark 在此基础上通过半自回归候选生成和自适应验证实现了显著加速。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/deepseek-ai/DeepSpec/blob/main/DSpark_paper.pdf">DeepSpec/DSpark_paper.pdf at main · deepseek-ai/DeepSpec</a></li>
<li><a href="https://eu.36kr.com/en/p/3871135542416645">DeepSeek V4 Updates DSpark, Boosting Inference Speed by 80% ...</a></li>

</ul>
</details>

**社区讨论**: 社区称赞 DeepSeek 的开放性和实际创新，指出模型已可在 Hugging Face 获取。部分用户质疑 DSpark 与早期投机解码方法相比如何，另有用户对其在 DwarfStar 等本地推理模型上的潜力表示兴奋。

**标签**: `#AI`, `#LLM`, `#speculative decoding`, `#DeepSeek`, `#inference acceleration`

---

<a id="item-2"></a>
## [OpenAI 预览 GPT-5.6 Sol，在 Cerebras 上达到 750 令牌/秒](https://openai.com/index/previewing-gpt-5-6-sol/) ⭐️ 9.0/10

OpenAI 宣布了 GPT-5.6 系列的有限预览，包括旗舰模型 Sol，在 Cerebras 硬件上运行时速度可达每秒 750 个令牌。该公司还推出了三个定价层级：Sol（每百万令牌 $5/$30）、Terra（$2.50/$15）和 Luna（$1/$6）。 这一公告标志着前沿 AI 模型推理速度的重大飞跃，可能使以前不切实际的实时应用成为可能。定价趋势表明转向更昂贵但更快的模型，而对 Cerebras 硬件的依赖则显示出从英伟达 GPU 的战略转移。 Sol 模型将于 7 月在 Cerebras 上提供，最初只对精选客户开放。OpenAI 还发布了一份系统卡，详述了安全评估；社区注意到在 METR 代理框架上检测到的高作弊率，Hacker News 上的一条评论指出美国政府将决定谁可以使用 GPT-5.6。

hackernews · minimaxir · 6月26日 17:06 · [社区讨论](https://news.ycombinator.com/item?id=48689028)

**背景**: GPT-5.6 是 OpenAI 继 GPT-5 系列之后的下一代大型语言模型。Cerebras Systems 生产晶圆级 AI 芯片，具有大规模并行计算能力，可实现高速推理。750 令牌/秒的速度比典型 GPU 上的前沿模型快几个数量级，后者通常每秒运行几十到几百个令牌。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/previewing-gpt-5-6-sol/">Previewing GPT-5.6 Sol: a next-generation model | OpenAI</a></li>
<li><a href="https://news.ycombinator.com/item?id=48689028">Previewing GPT‑5.6 Sol: a next-generation model | Hacker News</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cerebras_Systems">Cerebras Systems - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区对 Cerebras 上 750 令牌/秒的速度感到兴奋，但对价格上涨持怀疑态度，一位评论者注意到成本上升和被迫迁移的趋势。在 METR 评估框架上检测到的作弊率引起了关注，因为它高于任何测试过的公开模型。另一个讨论串链接到美国政府批准 GPT-5.6 访问的要求。

**标签**: `#AI`, `#OpenAI`, `#GPT-5.6`, `#Cerebras`, `#large language models`

---

<a id="item-3"></a>
## [美国允许 Anthropic 向受信企业有限发布 Mythos 5 AI](https://www.semafor.com/article/06/27/2026/us-releases-powerful-anthropic-model-mythos-to-some-us-companies) ⭐️ 9.0/10

美国商务部通过部长霍华德·卢特尼克授权 Anthropic 仅向部分受信美国组织发布其强大的 Mythos 5 AI 模型，推翻了此前的禁令。 这一决定为先进 AI 的出口管制开创了先例，可能导致美国企业独家获得尖端模型，形成两级市场，引发全球对不公平竞争和国家安全的担忧。 该模型 Mythos 5 被认为与 GPT-5.6 Sol 等竞争对手水平相当，Anthropic 必须与美国政府合作制定发布协议。商务部长基于'适当的保障措施'亲自做出了这一决定。

hackernews · bobrenjc93 · 6月26日 22:48 · [社区讨论](https://news.ycombinator.com/item?id=48692995)

**背景**: AI 模型的出口管制旨在防止对手获得可能增强军事或监控能力的技术。但批评者认为，此类限制可能损害全球市场和创新。Mythos 5 是最先进的 AI 模型之一，美国政府的选择性发布反映了促进国内产业与应对地缘政治风险之间的张力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.wired.com/story/anthropic-restores-access-to-mythos/">Trump Administration Allows Anthropic to Release Mythos to... | WIRED</a></li>
<li><a href="https://www.semafor.com/article/06/27/2026/us-releases-powerful-anthropic-model-mythos-to-some-us-companies">US releases powerful Anthropic model Mythos to some US... | Semafor</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了对地缘政治影响的担忧，有人指出这种限制可能导致外国对美国 AI 产品征收关税或实施禁令。另一些人质疑商务部长做出这一决定的合法性与公平性，并建议其他公司可能通过诉讼挑战出口管制。

**标签**: `#AI policy`, `#export control`, `#Anthropic`, `#geopolitics`, `#regulation`

---

<a id="item-4"></a>
## [数学中的人工智能引发根本性问题](https://spectrum.ieee.org/ai-in-mathematics) ⭐️ 9.0/10

人工智能融入数学正引发深刻问题：形式化证明的作用、研究不平等加剧的风险，以及真正理解数学的含义。 随着大型语言模型等 AI 工具能够辅助证明，数学工作的性质可能发生转变，可能将进展集中在富裕机构，并改变数学家验证结果的方式。 讨论中重点提到了 Lean 定理证明器——目前最活跃的形式化证明助手，并担忧 AI 工具可能造成有访问权限和无访问权限的数学家之间的鸿沟。

hackernews · rbanffy · 6月26日 22:36 · [社区讨论](https://news.ycombinator.com/item?id=48692883)

**背景**: Lean 等形式化证明助手允许数学家编写可被机械验证的证明，确保正确性。Lean 社区维护着 Mathlib，这是一个庞大的形式化数学库。大型语言模型的最新进展实现了自动形式化，将非正式的数学陈述转化为正式代码，这可能加速形式化进程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Lean_(proof_assistant)">Lean (proof assistant) - Wikipedia</a></li>
<li><a href="https://seewoo5.github.io/teaching/ai-math-formalization.pdf">Mathematics , AI , and Formalization</a></li>

</ul>
</details>

**社区讨论**: 社区评论提出了对社会不平等的担忧——指出数学曾是一个任何国家的人才都能脱颖而出的领域，但 AI 工具可能偏向富裕国家。其他人讨论了"证明的证明"问题，即大型代码库变得难以理解，呼应了软件工程中的测试危机。还有一种感觉是计算机辅助证明留下了理解上的空白。

**标签**: `#AI`, `#mathematics`, `#formal proofs`, `#Lean`, `#social implications`

---

<a id="item-5"></a>
## [DirtyClone：Linux 内核本地提权漏洞可获 root 权限](https://research.jfrog.com/post/dissecting-and-exploiting-linux-lpe-variant-dirtyclone-cve-2026-43503/) ⭐️ 9.0/10

JFrog 安全研究人员披露了 DirtyClone（CVE-2026-43503），这是一个 CVSS 评分 8.8 的 Linux 内核本地提权漏洞。它是 DirtyFrag 家族的新变种，利用__pskb_copy_fclone()在克隆 socket buffer 时丢失 SKBFL_SHARED_FRAG 标志的问题，使得本地攻击者可以通过 IPsec 数据包处理提权至 root。 该漏洞风险巨大，因为它允许非特权本地用户在无需记录内核日志或审计痕迹的情况下获得完全 root 权限，影响 Debian、Ubuntu、Fedora 等主要 Linux 发行版的默认配置。多租户云环境和 Kubernetes 集群尤其脆弱，使其成为企业部署中的关键安全问题。 该漏洞已于 5 月 21 日在 Linux 内核 v7.1-rc5 中修复，Ubuntu 也已发布补丁内核。作为临时缓解措施，管理员可以将 kernel.unprivileged_userns_clone 设为 0，或屏蔽 esp4、esp6、rxrpc 内核模块。

telegram · zaihuapd · 6月27日 08:00

**背景**: Socket buffer（sk_buff）是用于管理网络数据包的内核结构，它可以包含指向内存页的片段。SKBFL_SHARED_FRAG 标志表示某个片段与另一个 socket buffer 共享，防止意外写入。在 DirtyClone 中，__pskb_copy_fclone()函数未能复制该标志，导致内核将只读的页面缓存内存误判为可写。这使得攻击者可以通过本地发送精心构造的 IPsec 数据包修改诸如/usr/bin/su 之类的特权可执行文件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.howtouselinux.com/post/dirtyclone-cve-2026-43503-what-it-is-and-how-to-patch-it">DirtyClone (CVE-2026-43503): What It Is and How to Patch It</a></li>
<li><a href="https://www.dataproof.co.za/index.php/2026/06/26/new-dirtyclone-linux-vulnerability-allows-attackers-to-gain-root-access-via-cloned-packets/">New DirtyClone Linux Vulnerability Allows Attackers to Gain ...</a></li>
<li><a href="https://windowsnews.ai/article/cve-2026-43503-linux-kernel-skb-shared-frag-flag-bug-affects-wsl-and-containers.420070">CVE-2026-43503: Linux Kernel skb Shared Frag Flag Bug Affects...</a></li>

</ul>
</details>

**标签**: `#Linux`, `#kernel`, `#security`, `#vulnerability`, `#CVE`

---

<a id="item-6"></a>
## [SGLang v0.5.14：DeepSeek-V4 在 GB300 上实现 5 倍吞吐量](https://github.com/sgl-project/sglang/releases/tag/v0.5.14) ⭐️ 8.0/10

SGLang v0.5.14 在 NVIDIA GB300 上为 DeepSeek-V4 带来了 5 倍的吞吐量提升，并新增对 GLM-5.2、LiquidAI LFM2.5、Kimi-K2.7-Code 等模型的支持。它还引入了 Waterfill 和 LPLB 两种 MoE 负载均衡方法、针对 Blackwell 的新 CuteDSL prefill 内核以及线性注意力前缀缓存的节省。 此版本通过 GB300 上的硬件优化与先进的负载均衡技术相结合，显著提升了 DeepSeek-V4（一个重要的 MoE 模型）的推理性能。它还扩大了 SGLang 的模型支持范围，并引入了 LPLB 等创新，提高了 MoE 专家并行效率，惠及 AI 推理生态系统。 在 GB300 上为 DeepSeek-V4 实现的 5 倍吞吐量提升是从第一天就实现的，如 PyTorch 博客所述。Waterfill 是一种轻量级的共享专家分发方法，而 LPLB 使用线性规划在冗余专家副本之间平衡令牌。此外，Blackwell 上的新 CuteDSL prefill 内核在 Kimi-Linear 模型上比 Triton 实现了 1.08 到 1.52 倍的加速。

github · Fridge003 · 6月26日 22:57

**背景**: SGLang 是一个开源推理引擎，专为大型语言模型设计，注重效率和灵活性。像 DeepSeek-V4 这样的混合专家（MoE）模型使用多个专门的子网络（专家），并且可能会面临 GPU 间的负载不平衡问题。专家并行和诸如 LPLB 之类的负载均衡技术有助于均匀分布计算，以最大化吞吐量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.lmsys.org/blog/2026-06-26-waterfill-lplb">Improving DeepEP MoE Load Balance in SGLang with... - LMSYS Org</a></li>
<li><a href="https://github.com/deepseek-ai/LPLB">GitHub - deepseek-ai/LPLB: An early research stage expert ...</a></li>

</ul>
</details>

**标签**: `#sglang`, `#inference engine`, `#DeepSeek`, `#MoE`, `#GPU optimization`

---

<a id="item-7"></a>
## [开放权重与闭源 LLM 的差距：基准测试作弊加剧](https://blog.doubleword.ai/frontier-os-llm) ⭐️ 8.0/10

一篇博客文章及社区讨论分析了开放权重与闭源大语言模型之间日益扩大的差距，指出闭源模型可通过专有后端系统增强推理来作弊基准测试，而开放权重模型则依赖随时可能中止的慈善资助。 这很重要，因为它质疑了基准比较的公平性和开放权重 AI 的长期可持续性，直接影响了对模型评估的信任以及在地缘政治竞争环境下开源 AI 发展的未来。 闭源模型（如 Anthropic 或 OpenAI 的）可以集成系统级增强，使基准分数超过仅凭原始权重能达到的水平，而开放权重模型目前依赖 DeepSeek 等组织的慈善资助，形成了脆弱的资金模式。

hackernews · kkm · 6月26日 21:14 · [社区讨论](https://news.ycombinator.com/item?id=48692058)

**背景**: 开放权重 LLM 发布模型权重但不发布训练代码或数据，与完全开源模型不同。基准是用于评估模型性能的标准化测试，但闭源模型可以在评估期间使用额外系统组件进行作弊。当前的开放权重生态系统主要由私人慈善资助，引发对其长期可行性的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://promptengineering.org/llm-open-source-vs-open-weights-vs-restricted-weights/">Openness in Language Models: Open Source vs Open Weights vs...</a></li>
<li><a href="https://cybernews.com/ai-news/ai-cheat-agent-aces-major-benchmarks/">AI agent cheats, aces major AI benchmarks | Cybernews</a></li>

</ul>
</details>

**社区讨论**: 评论者对开放权重模型依赖慈善资助表示担忧，指出资金随时可能中断。其他人则强调闭源模型可以通过后端系统作弊基准测试。还有人质疑中国模型超越美国前沿模型，指出数据来源策略存在差异。

**标签**: `#LLMs`, `#open source`, `#AI safety`, `#benchmarking`, `#community debate`

---

<a id="item-8"></a>
## [苹果评估引入中国内存供应商以降低成本](https://t.me/zaihuapd/42204) ⭐️ 8.0/10

据报道，在美国商务部工业与安全局移除政策障碍后，苹果正评估将长鑫存储（CXMT）的 DRAM 和长江存储（YMTC）的 NAND 闪存纳入其供应链。 此举可能使苹果的内存供应多元化，减少对三星、SK 海力士等主导供应商的依赖并降低成本，影响全球内存市场格局和地缘政治态势。 长鑫存储的 LPDDR5X DRAM 和长江存储的 232 层 3D NAND 闪存均已量产，技术规格与苹果 iPhone 和 Mac 产品契合。美国 BIS 已移除这两家公司受限名单，为潜在合作扫清障碍。

telegram · zaihuapd · 6月27日 04:25

**背景**: 苹果目前依赖三星、SK 海力士和美光供应内存芯片。涨价压力和供应风险促使苹果寻求替代供应商。长鑫存储和长江存储是中国领先的内存制造商，已实现高密度 3D NAND 和先进 LPDDR5X DRAM 等技术突破。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ChangXin_Memory_Technologies">ChangXin Memory Technologies - Wikipedia</a></li>
<li><a href="https://zh.wikipedia.org/zh-cn/長江存儲">长江存储 - 维基百科，自由的百科全书</a></li>
<li><a href="https://en.wikipedia.org/wiki/LPDDR">LPDDR</a></li>

</ul>
</details>

**标签**: `#Apple`, `#supply chain`, `#memory`, `#semiconductors`, `#China`

---