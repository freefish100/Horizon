---
layout: default
title: "Horizon Summary: 2026-07-26 (ZH)"
date: 2026-07-26
lang: zh
---

> 从 25 条内容中筛选出 9 条重要资讯。

---

1. [vLLM v0.26.0 新增 Inkling 支持与 DeepSeek-V4 优化](#item-1) ⭐️ 8.0/10
2. [Claude 5 新上下文工程规则引发锁定争议](#item-2) ⭐️ 8.0/10
3. [开放权重 AI 迎来 Kubernetes 式崛起](#item-3) ⭐️ 8.0/10
4. [安卓可能限制设备端 ADB 访问](#item-4) ⭐️ 8.0/10
5. [Ruff v0.16.0 默认规则从 59 条扩展到 413 条](#item-5) ⭐️ 8.0/10
6. [市场监管总局对携程处以 51.79 亿元反垄断罚款](#item-6) ⭐️ 8.0/10
7. [微软将借 TPM 芯片封堵盗版 Windows 激活](#item-7) ⭐️ 8.0/10
8. [DeepSeek 因泄密暂停新一轮融资](#item-8) ⭐️ 8.0/10
9. [近 200 家硅谷公司反对禁中国开放权重 AI](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.26.0 新增 Inkling 支持与 DeepSeek-V4 优化](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 8.0/10

vLLM v0.26.0 引入了对 Inkling 975B 参数 MoE 模型家族的完整支持，包括分段 CUDA 图和 Hopper FA4 相对注意力，并通过专用路由内核和融合操作显著提升了 DeepSeek-V4 的性能。 此版本增强了 vLLM 作为最新开源权重模型的生产级推理引擎，能够高效服务像 Inkling 这样的大规模 MoE 架构，并进一步优化 DeepSeek-V4，从而降低实际 LLM 部署的延迟和成本。 该版本包含来自 212 名贡献者的 411 次提交，支持按 KV 缓存组选择灵活注意力后端、通过 fp32 lm_head 提高生成精度，以及 Rust 前端对多模态视频和音频的支持。

github · khluu · 7月25日 10:38

**背景**: vLLM 是一个开源的高吞吐量 LLM 服务引擎，利用 PagedAttention 和高效的 CUDA 内核来降低内存开销。Thinking Machines Lab 的 Inkling 模型是一个 975B 参数的混合专家（MoE）Transformer，具有 41B 活跃参数，支持高达 100 万 token 的上下文。Hopper FA4 是最新的 FlashAttention 算法，通过异步流水线针对 NVIDIA Hopper GPU 进行了优化。NVIDIA ModelOpt 的 NVFP4 量化支持 4 位浮点权重存储，从而减少内存使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/introducing-inkling/">Inkling: Our Open-Weights Model - Thinking Machines Lab</a></li>
<li><a href="https://arxiv.org/html/2603.05451v1">FlashAttention-4: Algorithm and Kernel Pipelining Co-Design for Asymmetric Hardware Scaling</a></li>
<li><a href="https://arunksingh16.medium.com/nvidia-nvfp4-quantization-blackwell-and-the-path-to-production-inference-12407e14e084">NVIDIA NVFP4: Quantization, Blackwell, and the Path to Production Inference | by Arun Kumar Singh | Jul, 2026 | Medium</a></li>

</ul>
</details>

**标签**: `#vllm`, `#LLM inference`, `#release`, `#performance optimization`, `#GPU computing`

---

<a id="item-2"></a>
## [Claude 5 新上下文工程规则引发锁定争议](https://claude.com/blog/the-new-rules-of-context-engineering-for-claude-5-generation-models) ⭐️ 8.0/10

Anthropic 发布了针对其 Claude 5 模型的新上下文工程规则，旨在优化模型在推理过程中使用上下文的方式，但社区担心供应商锁定和自动记忆功能的可靠性。 这些规则可能从根本上改变开发者与 Claude 5 的交互方式，增加对 Anthropic 特定工具的依赖，同时自动记忆问题可能削弱对模型决策过程的信任。 新规则强调结构化指令，并利用 Claude 的自动记忆功能跨会话存储和检索上下文，但用户报告自动记忆可能做出不可靠的跳跃，并因首次尝试失败而增加 Token 消耗。

hackernews · mellosouls · 7月25日 20:42 · [社区讨论](https://news.ycombinator.com/item?id=49051361)

**背景**: 上下文工程是一门设计和优化推理期间提供给大语言模型信息的学科，超越提示词，包括结构化指令和外部数据。自动记忆功能允许模型跨会话存储和回忆信息，但其可靠性受到质疑。Anthropic 的新规则旨在为 Claude 5 标准化这些实践。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents">Effective context engineering for AI agents \ Anthropic</a></li>
<li><a href="https://www.philschmid.de/context-engineering">The New Skill in AI is Not Prompting, It's Context Engineering</a></li>
<li><a href="https://www.linkedin.com/posts/koujala_claudecode-ai-developertools-activity-7432311920109596672-FgaD">Unlock Claude Code's AutoMemory Feature for Efficient... | LinkedIn</a></li>

</ul>
</details>

**社区讨论**: 社区意见分歧明显：有人批评新规则是增加对 Anthropic 平台锁定的举动，指出 Claude 5 出现意外删除和模糊推理痕迹。还有人担心依赖自动记忆会引入不可预测行为和法律责任风险，少数人则认为这有可能实现更简洁的上下文工程，无需冗长指令。

**标签**: `#Claude 5`, `#context engineering`, `#AI`, `#lock-in`, `#community discussion`

---

<a id="item-3"></a>
## [开放权重 AI 迎来 Kubernetes 式崛起](https://tobi.knaup.me/2026-07-25-open-weight-ai-is-having-its-kubernetes-moment/) ⭐️ 8.0/10

开放权重 AI 模型正迅速成为 AI 开发的标准，类似于 Kubernetes 标准化云基础设施的方式，这一趋势由成本效率和社区协作推动。 这一转变可能使 AI 的获取民主化，减少对专有模型的依赖，并促进协作开发，有可能像 Kubernetes 改变云计算那样改变 AI 行业。 开放权重模型公开发布训练参数（权重），允许定制和本地部署，但并非完全开源，因为训练数据和代码可能不包含在内。与 Kubernetes 的类比凸显了社区驱动标准化的作用。

hackernews · tknaup · 7月25日 14:49 · [社区讨论](https://news.ycombinator.com/item?id=49048034)

**背景**: 模型权重是神经网络中的数值参数，决定模型如何处理信息；它们存储了训练期间学到的“知识”。开放权重 AI 模型公开发布这些权重，使开发者能够在自己的硬件上微调或运行模型。这类似于 Kubernetes（一个开源容器编排平台）通过社区协作和成本节约成为管理云基础设施的标准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/thought-vector/open-weight-llms-a-strategic-advantage-for-enterprise-ai-1c4859ea6885">Open - Weight LLMs: A Strategic Advantage for Enterprise AI | Medium</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-are-weights">What are Weights? | Stanford HAI</a></li>
<li><a href="https://www.linkedin.com/pulse/open-weight-ai-what-we-finally-opened-bonnet-nicolas-pistorio-n3ulf">Open - weight AI : what if we finally opened the bonnet ?</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论按来源禁止中国模型的可行性，因为权重只是数字；批评专有模型不透明的定价“代币经济”；并倡导像 Linux 那样真正开放的协作模型。一些人指出像 OpenAI 这样的美国实验室已经发布了开放权重模型，但希望有更频繁的更新。

**标签**: `#AI`, `#open-source`, `#Kubernetes`, `#model weights`, `#industry trend`

---

<a id="item-4"></a>
## [安卓可能限制设备端 ADB 访问](https://kitsumed.github.io/blog/posts/android-may-soon-restrict-on-device-adb/) ⭐️ 8.0/10

据报道，安卓计划在未来的更新中限制设备端 ADB（Android Debug Bridge）访问，这可能会限制开发者及高级用户与设备的交互方式。 此变更可能严重影响依赖 ADB 进行调试和侧载的安卓开发者，同时引发关于安全与用户自由之间平衡的担忧。这标志着安卓正变得不那么开放，趋近于 iOS。 该限制针对的攻击向量需要同时开启开发者选项和远程 ADB，这对极少数用户现实可行。谷歌还讨论过替代方案，如限制对特定接口或 IP 地址的访问。

hackernews · shscs911 · 7月25日 06:57 · [社区讨论](https://news.ycombinator.com/item?id=49045159)

**背景**: Android Debug Bridge (ADB) 是一个命令行工具，允许开发者与安卓设备通信，用于调试、安装应用和运行 shell 命令。它可以通过 USB 或无线 TCP 使用。设备端 ADB 访问指在设备本地使用 ADB，通常通过终端模拟器。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Android_Debug_Bridge">Android Debug Bridge - Wikipedia</a></li>
<li><a href="https://developer.android.com/tools/adb">Android Debug Bridge (adb) | Android Studio | Android Developers</a></li>
<li><a href="https://medium.com/@EazSoftware/a-comprehensive-guide-to-adb-android-debug-bridge-the-unsung-hero-for-android-developers-28b349037436">A Comprehensive Guide to ADB (Android Debug Bridge): The Unsung Hero for Android Developers | by Eaz Software | Medium</a></li>

</ul>
</details>

**社区讨论**: 社区评论褒贬不一：有人认为该限制针对一个不存在的威胁（需要开启开发者选项），而另一些人则认为这是谷歌继续收紧安卓控制的一部分，预计未来将进一步限制侧载和可定制性。用户对谷歌的动机持怀疑态度，部分人预计最终可能需要付费或提交身份信息。

**标签**: `#Android`, `#ADB`, `#security`, `#developer tools`, `#privacy`

---

<a id="item-5"></a>
## [Ruff v0.16.0 默认规则从 59 条扩展到 413 条](https://simonwillison.net/2026/Jul/25/ruff/#atom-everything) ⭐️ 8.0/10

Ruff v0.16.0 于 2026 年 7 月 23 日发布，将默认规则集从 59 条增加到 413 条，无需任何配置即可检测到更多潜在问题。 此变化通过捕获严重错误（如语法错误和运行时错误）显著提高了 Python 代码质量，这些错误以前只有通过显式配置规则才能检测到，虽然可能破坏 CI 作业，但最终使代码库更安全。 Ruff 现在共有 968 条规则，新默认规则自动启用对时区无知 datetime 使用和盲目异常捕获等问题的检查。用户可以使用 `ruff check --fix --unsafe-fixes` 自动修复大部分违规。

rss · Simon Willison · 7月25日 22:44

**背景**: Ruff 是一个用 Rust 编写的极快 Python 代码检查器和格式化工具，旨在替代 Flake8 和 Black 等工具。它由 Astral 开发，该公司最近被 OpenAI 收购，以其性能和全面的规则集而闻名。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.astral.sh/ruff/">An extremely fast Python linter and code formatter, written in Rust.</a></li>
<li><a href="https://astral.sh/ruff">Ruff , an extremely fast Python linter | Astral</a></li>

</ul>
</details>

**标签**: `#ruff`, `#python`, `#linting`, `#astral`

---

<a id="item-6"></a>
## [市场监管总局对携程处以 51.79 亿元反垄断罚款](https://t.me/zaihuapd/42767) ⭐️ 8.0/10

7 月 25 日，国家市场监督管理总局依据反垄断法对携程集团有限公司滥用市场支配地位行为作出行政处罚，没收违法所得 16.58 亿元，罚款 35.21 亿元，罚没合计 51.79 亿元。同时责令携程停止违法行为、全额退还酒店经营者订单储备金 1.22 亿元，并要求全面整改。 此罚单是中国科技领域最大的反垄断罚单之一，标志着政府对平台垄断行为的执法力度加大。它将重塑中国在线旅游市场的竞争格局，并对其他主导性数字平台起到警示作用。 处罚包含没收违法所得和罚款两部分，合计 51.79 亿元。携程须退还强制扣除酒店经营者的订单储备金 1.22 亿元，并公开整改措施。

telegram · zaihuapd · 7月25日 11:56

**背景**: 携程（现为 Trip.com 集团）是中国领先的在线旅游平台，在酒店和机票预订领域占据主导市场份额。中国反垄断法禁止滥用市场支配地位，自 2020 年以来，监管部门针对大型科技平台的反竞争行为加大了执法力度，此前已对阿里巴巴和腾讯等采取过类似行动。

**标签**: `#antitrust`, `#regulation`, `#China`, `#travel technology`, `#monopoly`

---

<a id="item-7"></a>
## [微软将借 TPM 芯片封堵盗版 Windows 激活](https://www.techspot.com/news/113232-microsoft-using-tpm-chips-crack-down-pirated-windows.html) ⭐️ 8.0/10

微软宣布为企业 KMS 批量激活工具加入基于 TPM 芯片的硬件安全验证（TPM 证明），该机制会先确认 KMS 服务器的硬件身份经微软认证且未被篡改，之后才允许处理批量激活请求，从而封堵长期被攻击者滥用的 KMS 伪造激活。该功能将从下一版 Windows Server 起强制实施，并自 2026 年 8 月起在 Windows Server 2025 中推送准备提示。 此举直接针对企业版 Windows 最常见的软件盗版方式，有望关闭大量依赖伪造 KMS 服务器的激活工具。同时，它提高了软件许可的硬件安全门槛，但 Massgrave 的 TSforge 等绕过方法的出现表明这是一场持续的攻防战。 TPM 证明机制会先验证 KMS 服务器的硬件身份是否经微软认证且未被篡改，之后才允许处理激活请求。微软已在 2025 年封死了 KMS38 漏洞，而 Massgrave 组织的 Online KMS 方法需要每半年重新连接伪造服务器续期，TPM 证明可能使其彻底失效；但 Massgrave 最近推出的 TSforge 方法号称可绕过整个 Windows DRM 激活架构。

telegram · zaihuapd · 7月25日 15:55

**背景**: KMS（密钥管理服务）是一种合法的企业批量激活方法，旨在允许组织使用本地 KMS 主机激活多台 Windows 或 Office 设备。多年来，攻击者设置了伪造的 KMS 服务器来模仿真实服务器，从而无需有效许可即可激活软件。TPM（可信平台模块）是一种硬件安全芯片，用于存储加密密钥并验证系统完整性；Windows 11 已要求 TPM 2.0，而微软现在将其用于激活安全。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.pingcode.com/ask/241653.html">TPM 芯 片 的工作原理是什么 – PingCode</a></li>
<li><a href="https://www.laoliang.net/jsjh/technology/13891.html">Windows系统下 KMS （ 批 量 授权）和HWID...</a></li>
<li><a href="https://massgrave.dev/blog/tsforge">TSforge | MAS</a></li>

</ul>
</details>

**标签**: `#微软`, `#TPM`, `#Windows激活`, `#安全`, `#反盗版`

---

<a id="item-8"></a>
## [DeepSeek 因泄密暂停新一轮融资](https://www.bloomberg.com/news/articles/2026-07-25/deepseek-said-to-tell-backers-of-funding-pause-after-viral-posts) ⭐️ 8.0/10

DeepSeek 已口头通知部分第二轮投资者暂停签署投资协议，部分原因是创始人梁文锋对内部讨论外泄感到不满。该公司仍计划进行首次公开募股。 此次暂停凸显了知名 AI 初创公司内部沟通的敏感性，可能影响投资者信心。这也推迟了原计划至少募资 100 亿元人民币、估值 4800 亿元人民币的重大融资轮次，影响 AI 融资格局。 该公司于 2026 年 6 月完成首轮 70 亿美元融资，投资者包括腾讯、宁德时代及国家人工智能产业投资基金。暂停的这轮融资投前估值不低于 4800 亿元人民币。

telegram · zaihuapd · 7月26日 01:17

**背景**: DeepSeek 是一家中国 AI 初创公司，因开发具有竞争力的大语言模型而崭露头角。该公司的快速增长和备受关注的融资轮次在 AI 行业引起了广泛关注。创始人梁文锋以其激进的愿景和对公司方向的直言不讳而闻名。

**标签**: `#DeepSeek`, `#funding`, `#AI`, `#IPO`, `#business news`

---

<a id="item-9"></a>
## [近 200 家硅谷公司反对禁中国开放权重 AI](https://t.me/zaihuapd/42772) ⭐️ 8.0/10

包括 Y Combinator 和 Proton 在内的近 200 家硅谷公司致信特朗普政府，反对禁止中国开放权重 AI 模型，认为一刀切禁令将损害美国初创企业，并建议采取更有针对性的安全措施。 这一联盟代表了对美国潜在政策的重大行业反弹，该政策可能限制对低成本 AI 模型的获取，影响 AI 初创企业的竞争格局以及中美技术关系。 这封信由 Little Tech Association 组织。他们认为全面禁令将重创依赖低成本中国开放权重模型的下一代美国初创企业，并主张以更有针对性的安全措施取而代之。

telegram · zaihuapd · 7月26日 02:00

**背景**: 开放权重 AI 模型是指其训练参数（权重）公开发布的模型，允许开发者下载、微调和部署。与包含完整训练代码和数据的开源不同，开放权重模型只提供最终权重。来自 DeepSeek 等公司的中国开放权重模型因其经济性和有竞争力的性能而在初创社区中广受欢迎。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/openais-open-weight-model-what-means-developers-ai-industry-tsi9f">OpenAI’s Open - Weight Model : What It Means for Developers and the...</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#US-China tech relations`, `#open-source AI`, `#startups`, `#regulation`

---