---
layout: default
title: "Horizon Summary: 2026-08-29 (ZH)"
date: 2026-08-29
lang: zh
---

> 从 32 条内容中筛选出 11 条重要资讯。

---

1. [Htmx 4.0 发布：hypermedia 库迎来重大更新](#item-1) ⭐️ 9.0/10
2. [Z.ai 发布开源权重模型 GLM-5.3](#item-2) ⭐️ 9.0/10
3. [Triton 3.8.0 发布：新增聚合 API、topk 增强与后端更新](#item-3) ⭐️ 8.0/10
4. [开源工具借助 Apple Virtualization.framework 启动虚拟 iPhone](#item-4) ⭐️ 8.0/10
5. [为什么所有图形界面都应完全支持键盘操作：兼具无障碍与效率](#item-5) ⭐️ 8.0/10
6. [OpenAI 在 SpaceX 收购 Cursor 后切断其接入，称担忧模型蒸馏](#item-6) ⭐️ 8.0/10
7. [美国制裁意大利托管商 Autistici/Inventati 引发基础设施忧虑](#item-7) ⭐️ 8.0/10
8. [含糊的 Bug 传言已足以让 LLM 辅助发掘漏洞](#item-8) ⭐️ 8.0/10
9. [微型潜流变压器在 RP2350 微控制器上生成 128×128 人脸图像](#item-9) ⭐️ 8.0/10
10. [腾讯发布 Hy4 preview 开源 MoE 模型，盲测得分略胜 GLM-5.3 与 Kimi K3](#item-10) ⭐️ 8.0/10
11. [Z.ai 发布 GLM-5.3-Flash：320B MoE 模型，价格仅为上代十分之一](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Htmx 4.0 发布：hypermedia 库迎来重大更新](https://four.htmx.org/announcements/2026-08-28-htmx-4.0.0-is-released) ⭐️ 9.0/10

Htmx 4.0.0 已于 2026 年 8 月 28 日发布，这是该库自创建以来的首次大版本升级。此版本带来了新功能和兼容性修复，包括一个 hx-alpine-compat 属性，用于消除 htmx 与 Alpine.js 之间的兼容性问题。 这次大版本发布对 hypermedia 和服务器端渲染生态来说是一个重要里程碑；随着开发者对重量级客户端 JavaScript 框架的反思，这一领域重新受到关注。对于所有偏好更简单、以 HTML 为中心的方式来构建交互式界面的 Web 开发者而言，这都很重要。 新增的 hx-alpine-compat 属性解决了 htmx 与 Alpine.js（hypermedia 技术栈中常见的一对组合）之间的兼容性问题。htmx 体积很小（gzip 压缩后约 14k）、无依赖、可扩展，并且兼容 IE11。

hackernews · rmsaksida · 8月28日 13:28 · [社区讨论](https://news.ycombinator.com/item?id=49478178)

**背景**: htmx 是一个 JavaScript 库，它通过 HTML 属性让你直接在 HTML 中使用 AJAX、CSS 过渡、WebSockets 和 Server-Sent Events，从而以超文本的简洁和强大来构建现代用户界面。它是作为 intercooler.js 的改进版本而创建的，遵循 HATEOAS 原则（把 hypermedia 作为应用状态的引擎）。该项目在偏好服务器端渲染和更简单前端架构的开发者中广受欢迎。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Htmx">htmx - Wikipedia</a></li>
<li><a href="https://htmx.org/">htmx - high power tools for html</a></li>
<li><a href="https://hypermedia.systems/hypermedia-a-reintroduction/">Hypermedia: A Reintroduction</a></li>

</ul>
</details>

**社区讨论**: 社区反应大体上是正面的，htmx 的 CEO 本人也表达了兴奋之情，还有开发者分享了 Go + htmx + SQLite 这样的技术组合。但也出现了一些相反的观点：一位 .NET/Angular 开发者发现 htmx 用起来更困难，因为它要求把表现层与业务逻辑混在一起；还有用户指出 alpine-ajax 比 htmx 更小，同时提供了他们需要的所有功能。总体而言，评论者称赞了这个库的简洁性和它有机的成长方式。

**标签**: `#htmx`, `#release`, `#web-development`, `#hypermedia`, `#server-side-rendering`

---

<a id="item-2"></a>
## [Z.ai 发布开源权重模型 GLM-5.3](https://huggingface.co/zai-org/GLM-5.3) ⭐️ 9.0/10

Z.ai 已将最新旗舰大语言模型 GLM-5.3 以开放权重形式发布。该模型基于 GLM-5.2 的基础模型构建，所有改进均来自后训练。 GLM-5.3 为封闭模型提供了一个具有竞争力的开放权重替代方案，社区评测者称赞其在编程与推理任务上的表现。此次发布可能会加速开放模型在生产环境中的采用，尤其是希望本地控制或降低 API 成本的用户。 该模型为纯文本模型，延续了 GLM-5.x 系列的设定，并主要面向复杂软件工程与智能体应用场景。社区评测显示，它的 token 效率与易部署性优于部分同类模型，但在原始能力上可能略逊于 Kimi 等顶级模型。

hackernews · jeudesprits · 8月28日 15:20 · [社区讨论](https://news.ycombinator.com/item?id=49479878)

**背景**: 开放权重模型会公开训练后的神经网络权重，允许任何人下载并在本地运行，在可访问性与专有控制之间取得平衡。GLM 是 Z.ai 推出的多款大语言模型产品线，GLM-5.3 与 GLM-5.2 共享同一基础模型，性能提升全部来自后训练。开放权重方式不同于完全开源 AI，后者通常还会发布训练代码与数据。搜索结果将开放权重模型定义为公开发布并可下载的核心组件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/zai-org/GLM-5.3">zai-org/ GLM - 5 . 3 · Hugging Face</a></li>
<li><a href="https://docs.z.ai/guides/llm/glm-5.3">GLM - 5 . 3 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>

</ul>
</details>

**社区讨论**: 社区反应热烈，用户称 GLM-5.3 是'最佳平衡点'的开放权重模型，比某些同类模型更易运行，并在难题上表现出很强的直觉。有人表示其使用体验堪比 Opus 4.8，也有人指出中国模型可能存在'过度思考'的问题，生成比西方模型更多的思考 token，不过第三方服务的价格与速度可能更有优势。整体情绪积极，大家期待这一发布对明年开放模型格局的影响。

**标签**: `#open-weights`, `#LLM`, `#GLM-5.3`, `#AI/ML`, `#HuggingFace`

---

<a id="item-3"></a>
## [Triton 3.8.0 发布：新增聚合 API、topk 增强与后端更新](https://github.com/triton-lang/triton/releases/tag/v3.8.0) ⭐️ 8.0/10

Triton v3.8.0 已发布，带来了新的方言和前端特性，包括公开的 @triton.aggregate 与 @gluon.aggregate API，以及 tl.topk 新增的 descending 参数。同时还包含 AMD/HIP 和 NVIDIA 后端改进、Gluon 布局增强、Proton 性能分析更新以及破坏性变更。 Triton 是 AI/ML 领域广泛用于编写高性能 GPU 内核的核心 GPU 编程语言和编译器，因此本次发布会对许多深度学习和科学计算工作负载产生直接影响。新的聚合 API 和布局改进为高级内核开发者提供了更强的表达能力，而 AMD 与 NVIDIA 后端的更新也扩大了生态系统的适用范围。 值得注意的技术细节包括：JIT 缓存依赖键现在可以确定性地生成、新增自动调优监听器、将多 CTA 支持扩展到布局转换和 TMA gather/scatter，以及为 tma.store_wait 增加 read_only 参数。本次发布还将 LLVM 版本固定到更新后的修订版，以修复 GFX950 BF16 错误编译和 SLP 向量化问题，并包含需要迁移的破坏性变更。

github · warrendeng · 8月28日 18:25

**背景**: Triton 是一种类 Python 的语言和编译器，让开发者能以更高层次编写 GPU 内核，同时仍可获得接近手工调优 CUDA 的性能。Gluon 是 Triton 的底层 GPU 编程模型，直接暴露布局、共享内存、warp 特化和目标相关特性，使高级内核可以在便利性与控制力之间进行取舍。Proton 是 Triton 生态中的性能分析工具，提供一种快速直观的途径来检查内核性能。aggregate 装饰器提供了一种把多个字段打包为内核参数的结构化方式，补充了 Triton 现有的张量和标量参数模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://triton-lang.org/main/gluon/index.html">Gluon Overview — Triton documentation</a></li>
<li><a href="https://www.jokeren.tech/slides/IBM24_slides.pdf">Profiling and Debugging GPU-accelerated AI Applications</a></li>
<li><a href="https://github.com/triton-lang/triton/issues/10860">[RFC] Composable Kernel with runtime aggregate fields · Issue...</a></li>

</ul>
</details>

**标签**: `#Triton`, `#GPU Programming`, `#Compiler`, `#AI/ML`, `#Release Notes`

---

<a id="item-4"></a>
## [开源工具借助 Apple Virtualization.framework 启动虚拟 iPhone](https://github.com/Lakr233/vphone-cli) ⭐️ 8.0/10

vphone-cli 是一款开源命令行工具，可借助 Apple 的 Virtualization.framework 在 Apple Silicon Mac 上启动虚拟 iPhone。它支持越狱版 iOS 26.1 虚拟设备，并可用于本地 CI 和测试工作流。 该项目提供了一条基于 Apple 官方框架的 iOS 虚拟化路径，无需第三方破解手段，有望降低在真实 iOS 环境中进行 CI/测试的门槛。不过，依赖 macOS 主机这一限制仍制约其规模化。 该工具的工作流程包括创建虚拟机 bundle、下载并合并 IPSW、修补引导链、执行 DFU 恢复以及安装自定义固件。它提供五种安全绕过程度递增的 patch 变体，所有数据均存放在 ~/.vphone/ 目录下。

hackernews · hentrep · 8月28日 23:02 · [社区讨论](https://news.ycombinator.com/item?id=49485267)

**背景**: Apple 的 Virtualization.framework 为 Apple silicon 和 Intel Mac 提供用于创建和管理虚拟机的高级 API，但官方并不支持 iOS 虚拟机。vphone-cli 基于该框架，通过修补引导链和使用恢复固件来启动虚拟 iPhone。iOS Simulator 只是在一个模拟环境中运行应用，并非真正的系统级虚拟化，而 vphone-cli 试图提供更接近真机的行为，用于测试和 CI。该项目也被视为对 Corellium 此前在 iOS 虚拟化领域垄断地位的重大打破。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/Lakr233/vphone-cli">GitHub - Lakr233/vphone-cli · GitHub</a></li>
<li><a href="https://developer.apple.com/documentation/virtualization">Virtualization | Apple Developer Documentation</a></li>
<li><a href="https://medium.com/@mrbypass/mastering-vphone-cli-part-1-building-a-jailbroken-ios-26-1-virtual-iphone-on-apple-silicon-06ed5a4b13d2">Mastering vphone-cli (Part 1): Building a Jailbroken iOS 26.1 Virtual iPhone on Apple Silicon | by Akash Katare | Medium</a></li>

</ul>
</details>

**社区讨论**: 评论者大多对该项目持欢迎态度，认为它对本地 CI 是重大利好，同时也提出了不少问题，比如它与 iOS Simulator 的区别、设置时日本或欧盟地区的额外监管检查、是否包含虚拟基带，以及能否用于 localhost 浏览器测试。还有人指出依赖 macOS 主机是规模化的一大限制。

**标签**: `#iOS`, `#virtualization`, `#CI`, `#testing`, `#macOS`

---

<a id="item-5"></a>
## [为什么所有图形界面都应完全支持键盘操作：兼具无障碍与效率](https://ckardaris.com/blog/2026/08/28/keyboard-driven-guis.html) ⭐️ 8.0/10

一篇新文章主张，每种图形用户界面都应做到完全键盘驱动，而不仅仅是兼容键盘。文章认为这能提升所有用户的无障碍体验与操作效率。 键盘驱动的界面对于无法使用鼠标的残障人士至关重要，同时也能让高级用户更快地操作。这场讨论触及了可发现性、易学性与效率之间的基本 UX 权衡。 评论者指出，键盘无障碍常常被忽视，而错误的 Tab 顺序会直接阻断键盘用户的操作。也有人认为，仅仅给按钮分配快捷键只能算‘兼容键盘’，而非真正的键盘驱动，且按钮本身与键盘输入存在根本性不匹配。

hackernews · ckardaris · 8月28日 15:17 · [社区讨论](https://news.ycombinator.com/item?id=49479837)

**背景**: 键盘无障碍意味着界面可以不依赖鼠标、仅通过 Tab、回车、方向键和快捷键完成全部操作。美国《残疾人法案》（ADA）等法规要求组织必须提供无障碍软件。设计师需要在专家用户的效率与初学者的可发现性之间取得平衡，这一权衡使得‘键盘优先’的设计主张颇具争议。

**社区讨论**: 评论中不少人认同键盘支持是无障碍的重要环节，但反对强迫所有用户学习键盘驱动的界面。有用户指出，高级用户的使用体验与普通用户的 UX 不是一回事，开发工具可以做到键盘优先，但消费者应用不应被强制。还有人认为，主流 UI 框架和开发者的选择共同导致了键盘无障碍支持不佳。

**标签**: `#accessibility`, `#keyboard-driven`, `#GUI design`, `#UX`, `#power users`

---

<a id="item-6"></a>
## [OpenAI 在 SpaceX 收购 Cursor 后切断其接入，称担忧模型蒸馏](https://openai.com/index/our-decision-on-cursor-following-its-acquisition-by-spacex/) ⭐️ 8.0/10

OpenAI 已决定在 Cursor 被 SpaceX 收购后切断其对 OpenAI 模型的访问。此举正值外界担忧埃隆·马斯克一直在蒸馏 OpenAI 的模型以训练竞争性 AI 系统之际。 这标志着 AI 模型提供商对落入竞争对手手中的转售商收紧了政策。它将扰乱依赖 OpenAI 模型的 Cursor 用户，并凸显前沿 AI 行业日益激烈的竞争格局。 Cursor 是一款基于 Visual Studio Code 构建的 AI 编程编辑器，其很大一部分价值来自转售 OpenAI 和 Anthropic 等提供商的 API。社区评论指出，Anthropic 此前已因类似的《服务条款》违规行为封禁 xAI，而此次行动直接发生在马斯克承认模型蒸馏之后。

hackernews · meetpateltech · 8月29日 01:47 · [社区讨论](https://news.ycombinator.com/item?id=49486172)

**背景**: Cursor 是一款 AI 优先的代码编辑器和编程智能体，由一家 2022 年成立的旧金山公司打造，估值已达 293 亿美元，年经常性收入超过 30 亿美元。知识蒸馏是一种机器学习技术，让较小的“学生”模型学习复制较大“教师”模型的行为；前沿模型提供商通常禁止未经许可进行此类操作。随着 AI 公司不断整合并走向垂直一体化，使用竞争对手的蒸馏模型已成为一个焦点问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cursor_(code_editor)">Cursor (code editor)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者大多认为此举不可避免，并指出 Anthropic 今年早些时候已因类似的《服务条款》违规行为封禁了 xAI。一些人认为 Cursor 的转售商业模式很脆弱，用户可能会转向 Anthropic，或只能依赖 Grok/Composer；另一些人则争论 Cursor 是否应直接托管更多开源模型。

**标签**: `#AI`, `#OpenAI`, `#Cursor`, `#SpaceX`, `#M&A`

---

<a id="item-7"></a>
## [美国制裁意大利托管商 Autistici/Inventati 引发基础设施忧虑](https://www.inventati.org/) ⭐️ 8.0/10

美国财政部和国务院于 2026 年 8 月将意大利托管服务商 Autistici/Inventati（A/I 团体）及其运营的博客平台 noblogs.org 列为“特别指定全球恐怖分子”实体。这是民用基础设施和隐私服务提供商首次被列入恐怖组织黑名单。 这开创了危险的先例：如果一个提供加密通信、匿名博客和网站托管的非暴力机构可以被认定为恐怖分子，那么许多开源隐私工具及其运营者（如 I2P、Monero、Signal 等）理论上也可能面临类似制裁。这标志着美国对隐私基础设施施压升级，对全球言论自由和安全通信造成寒蝉效应。 这一认定于 2026 年 8 月 26 日前后公布，美国国务院新闻稿同时将 Palestine Action 和 Masar Badil 列为目标。财政部 OFAC 名单现包含 A/I 团体，冻结其在美相关资产并禁止美国人与之进行交易。批评者指出，国务院的说明似乎提到一个由 noblogs.org 托管的网站，他们认为这是不诚实和错误的。

hackernews · exiguus · 8月28日 12:58 · [社区讨论](https://news.ycombinator.com/item?id=49477854)

**背景**: Autistici/Inventati 于 2001 年在意大利由自主反资本主义运动的个人和团体创建。它为全球活动人士提供免费电子邮件、网站托管和博客平台 noblogs.org，并坚持隐私、匿名和无追踪原则。历史上，A/I 参与者曾支持意大利 Indymedia，并在 2001 年热那亚八国集团峰会期间帮助搭建抗议者媒体中心。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.autistici.org/">autistici.org - Welcome to Autistici / Inventati</a></li>
<li><a href="https://www.radiorebelde.cu/english/u-s-designates-palestine-action-masar-badil-and-autistici-inventati-as-terrorist-groups-26082026/">U.S. Designates Palestine Action, Masar Badil, and Autistici Inventati ...</a></li>
<li><a href="https://crimethinc.com/2026/08/27/us-government-designates-host-of-noblogsorg-a-global-terrorist">US Government Designates Host of NoBlogs . org a "Global Terrorist"</a></li>

</ul>
</details>

**社区讨论**: 评论中出现广泛警觉：许多人认为这是对基础设施提供商而非个人的前所未有的打击，担心滑坡效应——I2P、Monero、Veilid、Tox 或 Signal 的用户可能被贴上恐怖分子标签。一些人试图澄清该团体的历史和活动，另一些人则对官方理由表示怀疑，将其比作伊拉克战争前的大规模杀伤性武器说辞。

**标签**: `#sanctions`, `#privacy`, `#infrastructure`, `#free-speech`, `#surveillance`

---

<a id="item-8"></a>
## [含糊的 Bug 传言已足以让 LLM 辅助发掘漏洞](https://anil.recoil.org/notes/rumour-is-the-exploit) ⭐️ 8.0/10

文章认为，如今只需一个含糊的漏洞传言，就足以让 LLM 辅助的攻击者找到并武器化漏洞。rclone 维护者 Nick Craig-Wood 报告称安全披露数量激增：项目前十年约有 20 份披露，而最近一个月就超过 40 份。 LLM 正在降低漏洞利用开发的准入门槛，给开源维护者带来了不对称的负担。这一趋势可能使漏洞报告数量急剧增加，压垮小型项目，并将安全工作量转移给志愿者。 近期 rclone 的披露中约 75% 都含有一点真实问题，维护者无法轻易忽略。评论者指出，虽然“利用传言找漏洞”并不新鲜，但 LLM 已将其规模化并普及为对低价值目标的大规模利用。

hackernews · avsm · 8月28日 15:58 · [社区讨论](https://news.ycombinator.com/item?id=49480466)

**背景**: 传统漏洞研究需要深厚的专业知识，但 LLM 辅助工具已开始将部分工作自动化。Google 的 Project Naptime 以及 Claroty Team82 使用 Claude Opus 4.6 开展的研究，都展示了 LLM 进行漏洞研究的可能性。rclone 案例则展示了这些工具被技能较低的攻击者用于扫描代码库时产生的实际影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2024/06/google-introduces-project-naptime-for.html">Google Introduces Project Naptime for AI-Powered Vulnerability ...</a></li>
<li><a href="https://www.claroty.com/team82/research/hands-free-what-llm-driven-vulnerability-research-looks-like">Hands Free: What LLM Driven Vulnerability Research Looks... | Claroty</a></li>
<li><a href="https://www.praetorian.com/blog/llm-kernel-exploit-development/">FreeBSoD: Can LLMs Actually Write Kernel Exploits? - Praetorian</a></li>

</ul>
</details>

**社区讨论**: nickcw 等维护者描述了自己被安全披露数量压垮的处境，而 godelski 认为真正的瓶颈是组织缺乏修复问题的意愿。bri3d 指出“从传言找漏洞”是古老做法，但 LLM 将其大众化，stephbook 则强调仓促更新带来的部署和供应链风险。另一位评论者 rndhouse 构建了一个工具，用于检测提交中被静默修复的漏洞。

**标签**: `#security`, `#LLMs`, `#exploits`, `#vulnerability research`, `#open source`

---

<a id="item-9"></a>
## [微型潜流变压器在 RP2350 微控制器上生成 128×128 人脸图像](https://www.reddit.com/r/MachineLearning/comments/1w10tax/i_implemented_a_very_tiny_image_generation_model/) ⭐️ 8.0/10

一个参数量仅 2.4–400 万的潜流变压器（latent flow transformer）被量化为 int8，完全在 RP2350 微控制器上运行，约 20 秒生成 128×128 人脸图像。该演示通过 DMA 从闪存流式加载权重，并利用 ReLU²稀疏性跳过不必要的计算。 这展示了先进的生成模型可以被压缩并在微型嵌入式设备上运行，为物联网、可穿戴设备和边缘 AI 中的离线端侧图像生成打开了大门。它也突显了模型压缩和激活稀疏性在服务器 GPU 之外的实用价值。 该模型是一个 12 层变压器，使用 AdaLN-Zero 条件化，并支持无分类器引导（CFG），后者显著提升了图像质量。推理引擎在计算前一层的同时通过 DMA 从闪存流式加载权重，并利用 ReLU²提高稀疏性以跳过计算。

reddit · r/MachineLearning · /u/cpldcpu · 8月28日 19:48

**背景**: 潜流变压器（LFT）是一种较新的架构，它将多个层替换为通过流匹配（flow matching）训练的单个学习传输算子，在保持与原始变压器设计兼容的同时实现显著压缩。AdaLN-Zero 是扩散变压器（DiT）在图像生成中广泛使用的一种自适应层归一化条件化机制。ReLU²是一种能产生高激活稀疏性的激活函数，使硬件可以跳过零值计算。RP2350 是树莓派推出的低成本双核微控制器，RAM 和闪存都很有限，因此在这种设备上实现生成模型尤其具有挑战性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2505.14513">[2505.14513] Latent Flow Transformer</a></li>
<li><a href="https://arxiv.org/abs/2402.03804">[2402.03804] ReLU$^2$ Wins: Discovering Efficient Activation Functions for Sparse LLMs</a></li>
<li><a href="https://openreview.net/forum?id=E4roJSM9RM">Unveiling the Secret of AdaLN-Zero in Diffusion Transformer | OpenReview</a></li>

</ul>
</details>

**标签**: `#embedded-ai`, `#transformers`, `#image-generation`, `#microcontrollers`, `#model-compression`

---

<a id="item-10"></a>
## [腾讯发布 Hy4 preview 开源 MoE 模型，盲测得分略胜 GLM-5.3 与 Kimi K3](https://mp.weixin.qq.com/s/ymr3X878B8oa2XP15CH8TQ) ⭐️ 8.0/10

2026 年 8 月 28 日，腾讯发布了迄今最强的开源模型 Hy4 preview，总参数量 770B，活跃参数 49B，上下文窗口 1M token。在 203 个盲评工程任务中，Hy4 preview 以 2.99 分略胜 GLM 5.3（2.92）与 Kimi K3（2.94）。 该发布标志着开源大语言模型的一个重要里程碑，腾讯的模型在与 GLM-5.3、Kimi K3 等顶级模型竞争时表现出色。其长上下文窗口和 MoE 架构可能降低部署成本，并支持长周期软件工程、文档处理和科学研究等任务。 Hy4 preview 已上线腾讯云、GitHub、HuggingFace、ModelScope、AtomGit、OpenRouter 等渠道。API 定价为每 100 万输入 token 0.834 美元，每 100 万输出 token 2.501 美元。

telegram · zaihuapd · 8月28日 06:11

**背景**: 混合专家（MoE）是一种架构，每个 token 只激活一部分参数（专家），使模型能够扩展到数千亿总参数，同时保持较低的计算成本。总参数指模型的所有权重，而活跃参数是处理单个 token 时实际使用的参数，这一区别对内存和推理效率至关重要。新闻中提到的“盲测”是指在评估模型输出时不知道具体模型身份，从而减少偏见。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/mixture-of-experts">What is mixture of experts? | IBM</a></li>
<li><a href="https://medium.com/@csburakkilic/understanding-moe-architectures-the-difference-between-total-and-active-parameters-ad1d161fccaa">Understanding MoE Architectures: The Difference Between Total and Active Parameters | by Burak Kılıç | Medium</a></li>

</ul>
</details>

**标签**: `#Tencent`, `#LLM`, `#Open Source`, `#MoE`, `#AI Benchmark`

---

<a id="item-11"></a>
## [Z.ai 发布 GLM-5.3-Flash：320B MoE 模型，价格仅为上代十分之一](https://t.me/zaihuapd/43471) ⭐️ 8.0/10

Z.ai 发布了 GLM-5 系列首个原生多模态模型 GLM-5.3-Flash，采用 320B 总参数的 MoE 架构，激活参数仅 18B。该模型在编程和智能体基准上超越 GLM-5.2，而价格仅为上代的大约十分之一，限时输入价格为每百万 tokens 0.075 美元。 此次发布大幅降低了高性能 LLM 推理的成本，让开发者和企业更容易获得先进的 AI 能力。同时，它也加剧了 AI 模型市场的价格竞争，可能促使其他提供商推出更具性价比的方案。 限时促销期间，API 定价为每百万输入 tokens 0.075 美元、每百万缓存输入 tokens 0.015 美元、每百万输出 tokens 0.25 美元，缓存存储暂时免费。在编程和智能体基准上，该模型接近 Claude Opus 4.8 的水平，尽管成本大幅降低。

telegram · zaihuapd · 8月28日 15:32

**背景**: 混合专家（MoE）是一种将神经网络划分为多个专门子模型（即专家）的架构，对于每个输入 token 只激活其中一部分。总参数代表模型的整体规模，而激活参数决定推理速度和计算成本；在密集模型中，每个 token 都会激活所有参数。GLM-5.3-Flash 中 320B 总参数与 18B 激活参数的比例就体现了这种方法，使得一个庞大的模型能够高效运行。API 定价中的缓存输入 tokens 指重复的提示前缀，相比标准输入会以折扣价计费。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-mixture-of-experts">A Visual Guide to Mixture of Experts ( MoE )</a></li>
<li><a href="https://www.f22labs.com/blogs/active-vs-total-parameters-whats-the-difference/">Active vs Total Parameters : What’s the Difference?</a></li>
<li><a href="https://tokenrate.dev/blog/fundamentals/llm-api-pricing-glossary">The LLM API Pricing Glossary: Every Billing Term... | TokenRate</a></li>

</ul>
</details>

**标签**: `#AI`, `#LLM`, `#GLM`, `#MoE`, `#API`

---