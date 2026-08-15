---
layout: default
title: "Horizon Summary: 2026-08-15 (ZH)"
date: 2026-08-15
lang: zh
---

> 从 34 条内容中筛选出 12 条重要资讯。

---

1. [Qwen 3.8 27B 展现强大的本地推理能力与效率权衡](#item-1) ⭐️ 9.0/10
2. [GLM-5.3：具有新兴网络能力的前沿编程](#item-2) ⭐️ 9.0/10
3. [苹果官宣换帅：库克卸任 CEO，特努斯接任](#item-3) ⭐️ 9.0/10
4. [《走向黑暗》：执法部门黑客攻击的崛起](#item-4) ⭐️ 8.0/10
5. [Opus 5 抽象沟通风格遭批评](#item-5) ⭐️ 8.0/10
6. [Firefox 成为最后一个完全支持 uBlock Origin 的主流浏览器](#item-6) ⭐️ 8.0/10
7. [将《毁灭战士》渲染器编译进 210 亿参数 Transformer，零训练](#item-7) ⭐️ 8.0/10
8. [AI 人体组织实验室每年测试 310 万样本，或终结动物试验](#item-8) ⭐️ 8.0/10
9. [小红书开源 dots3-note：280B MoE 仅 16B 激活参数](#item-9) ⭐️ 8.0/10
10. [法官令谷歌取消第三方应用商店安装障碍](#item-10) ⭐️ 8.0/10
11. [PostgreSQL 修复 to_char 高危堆缓冲区溢出漏洞](#item-11) ⭐️ 8.0/10
12. [苹果联手阿里自研中国专属 AI 大模型，或成首家获批外企](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Qwen 3.8 27B 展现强大的本地推理能力与效率权衡](https://huggingface.co/Qwen/Qwen3.8-27B-FP8) ⭐️ 9.0/10

阿里 Qwen 团队在 Hugging Face 上发布了新的 27B 参数本地大语言模型 Qwen3.8-27B-FP8。早期社区测试显示其推理能力很强，有用户称它是能在笔记本电脑上运行的最好的“鹈鹕”（图像推理）模型。 此次发布强化了开源本地大语言模型生态，提供了对美国主要 AI 公司模型的有力替代方案。这也表明阿里等非美国厂商正在缩小推理性能差距，可能加速本地与私有化 AI 的部署。 这款 FP8 量化模型在消费级硬件上运行高效：一位 RTX 5090 用户报告使用 ninfer 推理引擎可达约 138 tokens/秒，约为朴素 llama.cpp 配置的两倍。但也有评论指出其显存占用似乎不如 Gemma 4 或 Muse Glimmer 高效，而且独特的“穴居人式”思考痕迹可能妨碍 MTP（多 token 预测）效率。

hackernews · erdaltoprak · 8月14日 15:00 · [社区讨论](https://news.ycombinator.com/item?id=49299605)

**背景**: Qwen 是阿里云开发的大语言模型和多模态模型系列，最初于 2023 年以“通义千问”名称发布。其架构基于 Meta 的 Llama 设计。像 Qwen 这样的本地大语言模型设计用于在个人设备上运行，实现无需云端的私有离线 AI 使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>
<li><a href="https://huggingface.co/Qwen">Qwen (Qwen)</a></li>

</ul>
</details>

**社区讨论**: 社区反应整体非常积极，但对效率的评价则喜忧参半。用户称赞其罕见地能解决私有推理基准测试，注意到与之前版本相比思考痕迹书写方式有明显变化，并兴奋地预测 Qwen、GLM 等非美国模型很快能与美国大型实验室抗衡。也有人对显存占用和 MTP 限制提出了担忧。

**标签**: `#Qwen`, `#Local LLM`, `#AI`, `#Reasoning`, `#Open Source`

---

<a id="item-2"></a>
## [GLM-5.3：具有新兴网络能力的前沿编程](https://z.ai/blog/glm-5.3) ⭐️ 9.0/10

GLM-5.3 是一个前沿编程模型，展现出新兴的网络能力，包括自主安全研究和大规模漏洞扫描，引发了社区广泛讨论。

hackernews · pella · 8月14日 05:19 · [社区讨论](https://news.ycombinator.com/item?id=49294997)

**标签**: `#AI`, `#LLM`, `#cybersecurity`, `#coding`, `#GLM`

---

<a id="item-3"></a>
## [苹果官宣换帅：库克卸任 CEO，特努斯接任](https://t.me/zaihuapd/43191) ⭐️ 9.0/10

苹果宣布管理层交接，蒂姆·库克将卸任 CEO，硬件工程高级副总裁约翰·特努斯将从 2026 年 9 月 1 日起出任新 CEO。库克将出任董事会执行董事长，董事会已一致批准这项安排。 这是苹果十多年来的首次 CEO 更迭，也是这家全球最具影响力的科技公司之一的高层重大变动。特努斯出身硬件工程，预示着苹果将继续聚焦 iPhone、Mac、iPad、AirPods 等核心产品线。 特努斯于 2001 年加入苹果，2013 年升任硬件工程副总裁，2021 年进入高管团队。现任董事长 Arthur Levinson 将于 2026 年 9 月 1 日转任首席独立董事，特努斯同日加入董事会；库克将在整个夏天继续担任 CEO，以完成交接过渡。

telegram · zaihuapd · 8月14日 11:00

**背景**: 苹果是全球最大的科技公司之一，CEO 负责公司的整体战略和运营。执行董事长是董事会层面的领导职务，侧重公司治理与战略监督，与 CEO 的日常经营管理职责不同。特努斯 2001 年加入苹果，2021 年进入高管团队后一直负责 iPhone、Mac、iPad 和 AirPods 等硬件工程。

**标签**: `#Apple`, `#CEO transition`, `#Tim Cook`, `#John Ternus`, `#Tech Industry`

---

<a id="item-4"></a>
## [《走向黑暗》：执法部门黑客攻击的崛起](https://blog.cryptographyengineering.com/2026/08/14/everything-is-about-to-go-dark/) ⭐️ 8.0/10

2026 年 8 月，Cryptography Engineering 博客发表了一篇广受讨论的文章，审视“走向黑暗”（going dark）问题，并认为在加密技术使传统窃听失效后，执法部门黑客攻击已成为主要监控手段。文章分析了这一转变在政策与安全上的取舍。 这件事很重要，因为它标志着执法部门正从被动窃听转向主动黑客攻击，影响加密政策、隐私保护以及政府监控的法律边界。这场辩论还将影响企业如何设计安全产品，以及法院如何看待远程搜查。 关键细节包括 Network Investigative Technique（NIT）——FBI 自至少 2002 年起使用的、经授权可绕过 Tor 匿名性的恶意软件——以及 2016 年《联邦刑事诉讼规则》第 41 条修正案对远程访问权限的扩展。文章还讨论了可利用软件漏洞数量是否即将触顶，而一些评论者对此提出异议。

hackernews · vslira · 8月14日 20:52 · [社区讨论](https://news.ycombinator.com/item?id=49304447)

**背景**: “走向黑暗”（going dark）问题指的是执法部门即使持有合法搜查令，也难以访问加密通讯内容；FBI 局长 James Comey 等人在 2010 年代曾公开提出这一担忧。作为回应，执法机构越来越多地采用 NIT 等黑客技术，通过路过式下载（drive-by download）从嫌疑人设备中提取身份信息。这种做法引发了第四修正案层面的疑问：远程访问是否应被视为与实体搜查同类。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Network_Investigative_Technique">Network Investigative Technique - Wikipedia</a></li>
<li><a href="https://www.congress.gov/crs_external_products/R/PDF/R44481/R44481.7.pdf">Encryption and the “Going Dark” Debate - Congress.gov</a></li>
<li><a href="https://assets.carnegieendowment.org/static/files/Wilde_Landi_Law_Enforcement_Cyber_final_1-1.pdf">Exploring Law Enforcement Hacking as a Tool Against ...</a></li>

</ul>
</details>

**社区讨论**: 评论者的观点各不相同：有人回顾了前数字时代窃听需要铺设昂贵物理电话线的情况；有人反驳文章关于可利用软件漏洞即将触顶的观点，认为 AI 辅助开发正在制造更多漏洞。还有人批评“走向黑暗”这一说法很荒谬，因为监控摄像头无处不在，谷歌、Facebook 等科技公司也在大量收集元数据。

**标签**: `#cryptography`, `#law enforcement`, `#surveillance`, `#security`, `#hacking`

---

<a id="item-5"></a>
## [Opus 5 抽象沟通风格遭批评](https://mun-logadan.github.io/why-does-opus-5-feel-worse/) ⭐️ 8.0/10

一篇被广泛分享的博客文章批评 Claude Opus 5 的沟通风格令人疲惫且过于抽象，在 Hacker News 上引发 705 条评论和大量参与。评论者推测，后训练现在更针对智能体之间的通信而非人类用户，部分人已转向 OpenAI 的 Sol 等其他模型。 这一批评表明，即使模型能力增强，优化目标从满足人类转向智能体任务性能，也可能损害实际用户体验。它引发了关于前沿 LLM 后训练方向以及 Anthropic 等公司如何平衡能力与易用性的重要问题。 评论者称 Opus 5 的文章迂回抽象，句子绕来绕去，并指出它有长篇大论地'保持诚实'和'承认错误'的倾向。部分用户表示已回到 Claude 4.8 或转向 OpenAI 的方案，还有人怀疑该模型更小或更经济，认为'刷榜'主要是营销驱动。

hackernews · numeri · 8月14日 10:12 · [社区讨论](https://news.ycombinator.com/item?id=49296740)

**背景**: Claude 是 Anthropic 公司开发的一系列大型语言模型，Opus 历来与 Sonnet、Haiku 一起构成最高能力层级。Anthropic 称 Claude Opus 5 是一个'深思熟虑且主动'的模型，其智能水平接近 Claude Fable 5，而价格约为后者的一半。近年来，该领域越来越强调智能体 AI，包括智能体间通信的协议和结构化推理，使得面向人类读者的可读性可能被忽视。这一背景有助于解释为何一些用户感到技术性能与令人愉快的交互之间存在落差。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Opus">Claude Opus</a></li>
<li><a href="https://www.anthropic.com/news/claude-opus-5">Introducing Claude Opus 5 \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Agent_Communications_Language">Agent Communications Language</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认为 Opus 5 能力更强但更难交流，抱怨其措辞冗长抽象、容易过度道歉。一些人推测，模型的后训练现在面向的是其他智能体而非人类，还有人认为该模型可能更小或更经济，'刷榜'只是营销手段。讨论反映出即使用户希望模型更强，他们依然渴望可读、对人类友好的输出。

**标签**: `#AI`, `#LLM`, `#Claude Opus 5`, `#user experience`, `#agent communication`

---

<a id="item-6"></a>
## [Firefox 成为最后一个完全支持 uBlock Origin 的主流浏览器](https://www.pcworld.com/article/3212428/firefox-is-now-the-last-major-browser-that-still-supports-ublock-origin.html) ⭐️ 8.0/10

Firefox 目前是唯一仍然完全支持原版 uBlock Origin 扩展的主流浏览器。这是因为以 Chrome 为首的基于 Chromium 的浏览器已全面转向 Manifest V3，而后者严重限制了广告拦截扩展的能力。 uBlock Origin 是最流行、最有效的广告拦截工具之一，因此在 Chrome 中失去完整支持将削弱数百万用户的广告拦截和隐私保护能力。这一变化还凸显了 Google 和 Mozilla 在用户选择与内容过滤理念上的日益分化。 Manifest V3 用 declarativeNetRequest 取代了阻塞式 webRequest API，使广告拦截扩展只能使用较小的静态规则集。谷歌推荐的替代品 uBlock Origin Lite 功能更少，而社区虽存在非官方的 MV3 移植版，但由于 webRequestBlocking 权限仅对企业侧载扩展开放，其能力受到很大限制。

hackernews · DemiGuru · 8月14日 19:03 · [社区讨论](https://news.ycombinator.com/item?id=49303202)

**背景**: uBlock Origin 是一款免费、开源、跨平台的浏览器扩展，主要用于内容过滤和广告拦截，目标是高效且保护隐私。Chrome 早在 2018 年就提出 Manifest V3，声称为了提升安全与隐私，但实际上也削弱了广告拦截扩展的功能。Firefox 继续支持 Manifest V2，因此 uBlock Origin 仍能完整运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/UBlock_Origin">uBlock Origin - Wikipedia</a></li>
<li><a href="https://developer.chrome.com/docs/extensions/develop/migrate/what-is-mv3">Extensions / Manifest V3 | Chrome for Developers</a></li>
<li><a href="https://arstechnica.com/gadgets/2024/08/chromes-manifest-v3-and-its-changes-for-ad-blocking-are-coming-real-soon/">Chrome’s Manifest V3, and its changes for ad blocking, are coming real soon - Ars Technica</a></li>

</ul>
</details>

**社区讨论**: 评论者大多批评谷歌的 Manifest V3 改造，有人指出 Firefox 也会审查热门扩展以确保安全。还有人提到非官方的 MV3 移植版 uBlock-mv3，个别用户则表示使用 uBlock Origin Lite 并未发现明显的拦截缺陷。整体情绪包含担忧、无奈以及寻找替代方案的实际态度。

**标签**: `#browsers`, `#ad-blocking`, `#uBlock Origin`, `#Manifest V3`, `#privacy`

---

<a id="item-7"></a>
## [将《毁灭战士》渲染器编译进 210 亿参数 Transformer，零训练](https://www.reddit.com/r/MachineLearning/comments/1voazhm/i_compiled_dooms_renderer_into_a_21bparameter/) ⭐️ 8.0/10

一位开发者使用自研编译器将《毁灭战士》的渲染算法编译成一个 210 亿参数的 Transformer，完全无需训练。生成的模型是标准 Hugging Face 检查点，能输出像素绘制命令，从而重现游戏中经典的 E1M1 画面。 这项工作表明，计算可以通过编译而非训练的方式嵌入 Transformer 权重，为模型可解释性、模型编辑和神经网络分析开辟了新的可能。同时，它也展示了 Transformer 在自然语言任务之外执行算法的创造性用法。 渲染一帧需要 3,614 个 token 的提示词并生成 53,747 个 token，在 NVIDIA B200 上约需 40 分钟——相当于每天约 35 帧，而原始 Doom 在 486 电脑上可达 35 FPS。加载检查点并解析输出的宿主程序仅需 43 行 Python 代码。

reddit · r/MachineLearning · /u/notforrob · 8月14日 15:50

**背景**: Transformer 通常在大量数据上训练来学习模式，但该项目另辟蹊径：用编译器将显式计算图转换为 Transformer 权重。Doom 引擎使用二叉空间分割（BSP）来确定可见墙面，并按由近到远的顺序绘制场景，这种确定性算法可以表示为计算图。此前已有研究通过解析式构造权重而非学习权重，在神经网络内嵌入小程序或计算机，本项目正是这一思路的延续。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Doom_engine">Doom engine - Wikipedia</a></li>
<li><a href="https://doom.fandom.com/wiki/Doom_rendering_engine">Doom rendering engine</a></li>
<li><a href="https://data-today.net/transformer-compiler-no-training/">A compiler that skips training and writes transformer weights</a></li>

</ul>
</details>

**标签**: `#transformer`, `#compiler`, `#neural-networks`, `#doom`, `#computation-graph`

---

<a id="item-8"></a>
## [AI 人体组织实验室每年测试 310 万样本，或终结动物试验](https://www.fastcompany.com/91589344/the-worlds-largest-biological-datacenter-could-help-make-animal-testing-obsolete) ⭐️ 8.0/10

Vivodyne 推出了号称全球最大的人体生物数据中心，由 12 个机器人“蜂巢”（HIVE）实验室组成，每年可对 310 万份活体人体组织样本开展受控试验。该系统由 AI 设计实验，以更好地预测新药在人体中的疗效与安全性。 这项技术有望让药物开发者获得更快、更贴近人体的筛选方式，从而让动物试验变得过时。它针对一个长期难题：约 90%的临床试验在药物通过动物试验后仍然失败。 其每年测试容量估计约为美国全部临床试验总和的两倍。Vivodyne 源于宾夕法尼亚大学的生物工程研究，其 HIVE 实验室使用的是大型人体组织，而非传统的二维细胞培养。

telegram · zaihuapd · 8月14日 01:48

**背景**: 药物测试长期以来依赖动物模型，但动物实验结果往往无法预测人体反应。干细胞与类器官技术的进展使科学家能在实验室中培育出微型、有功能的人体组织；将这些组织与机器人自动化和 AI 结合，就能对人类生物学进行大规模受控实验。Vivodyne 的发布是将这一方法工业化为商业药物测试平台的早期尝试。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.laboratorynetwork.com/doc/vivodyne-launches-the-world-largest-human-biological-datacenter-train-first-world-model-human-biology-0001">Vivodyne Launches The World's Largest Human Biological ...</a></li>
<li><a href="https://biobuzz.io/news/penn-born-vivodyne-launches-what-it-calls-the-worlds-largest-human-biological-datacenter/">Penn-Born Vivodyne Launches What It Calls the World's Largest ...</a></li>
<li><a href="https://www.intechopen.com/chapters/81045">Introductory Chapter: Organoid Technology and... | IntechOpen</a></li>

</ul>
</details>

**标签**: `#AI`, `#Biotech`, `#Drug Discovery`, `#Lab Automation`, `#Animal Testing`

---

<a id="item-9"></a>
## [小红书开源 dots3-note：280B MoE 仅 16B 激活参数](https://x.com/dotsstudioai/status/2088083314855018521) ⭐️ 8.0/10

小红书 dots 实验室开源了 dots3-note preview，这是 dots3 系列首个开放权重模型，总参数 280B、每次激活 16B。模型支持 512K 上下文，并能处理文字、图片、视频和音频。 此次开源让一个规模庞大且高效的 MoE 模型公开可用，降低了研究人员和开发者接触前沿架构的门槛。同时发布的 TEMPO 强化学习方法和两个新智能体基准，也有助于推动长程智能体研究。 该模型引入了 TEMPO 强化学习方法，通过自批判和测试时价值估计来训练长程智能体。权重已在 Hugging Face 上开放，同时发布了 VibeSearchBench 和 VibeLifeBench 两个真实场景智能体基准。

telegram · zaihuapd · 8月14日 08:27

**背景**: 混合专家（MoE）是一种机器学习技术，将模型拆分为多个专门的子模型（即“专家”），每个输入只激活其中一部分。这样可以在扩大总参数量的同时，保持较低推理计算量，即用“激活参数”来衡量。新基准之一 VibeSearchBench 用于评估智能体在模糊、多轮查询下的长程主动搜索能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/mixture-of-experts">What is mixture of experts? | IBM</a></li>
<li><a href="https://arxiv.org/abs/2605.27882">[2605.27882] VibeSearchBench: Benchmarking Long-horizon ...</a></li>

</ul>
</details>

**标签**: `#MoE`, `#Open Source`, `#AI Model`, `#Reinforcement Learning`, `#Benchmark`

---

<a id="item-10"></a>
## [法官令谷歌取消第三方应用商店安装障碍](https://www.androidauthority.com/google-play-store-remove-third-party-app-store-friction-3698697/) ⭐️ 8.0/10

美国地区法官詹姆斯·多纳托下令谷歌简化竞品安卓应用商店的安装流程，删除 Play Store 中的多余步骤与警告弹窗。法院认定这些先“查看”再“安装”的多步提示是蓄意制造的“反竞争摩擦”。 这一裁决迫使谷歌改变 Play Store 政策，可能为安卓应用分发带来来自第三方商店的更大竞争。它直接影响到用户安装替代应用市场的方式，并可能重塑开发者生态接触安卓设备的途径。 谷歌须在一周内完成修改，让第三方应用商店的安装像安装普通安卓应用一样直接。该指令源自 Epic 诉谷歌反垄断案，陪审团裁定谷歌在安卓应用分发上构成非法垄断。

telegram · zaihuapd · 8月14日 09:55

**背景**: Play Store 是安卓默认的应用市场，谷歌历来在用户侧载来自外部应用时会显示警告弹窗和多步流程。这种摩擦长期以来一直是争议点，2023 年陪审团在 Epic 诉谷歌案中裁定谷歌对安卓应用分发的控制构成非法垄断。另外，谷歌还在推行新的侧载验证规则，例如要求来自未验证开发者的应用经过强制 24 小时锁定，这些规则也在影响第三方应用的安装。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.androidauthority.com/how-android-sideloading-restrictions-may-work-3595355/">Google's plan to restrict sideloading on Android has a ...</a></li>
<li><a href="https://www.androidauthority.com/google-android-sideloading-unverified-apps-new-rules-3650343/">Android's new sideloading rules are here, and they come with ...</a></li>
<li><a href="https://www.digitaltrends.com/phones/google-will-still-let-you-sideload-apps-but-theres-a-catch-now/">Google will still let you sideload apps, but there's a catch ...</a></li>

</ul>
</details>

**标签**: `#antitrust`, `#Google`, `#Android`, `#Play Store`, `#app distribution`

---

<a id="item-11"></a>
## [PostgreSQL 修复 to_char 高危堆缓冲区溢出漏洞](https://www.postgresql.org/support/security/CVE-2026-14669/) ⭐️ 8.0/10

PostgreSQL 披露了 CVE-2026-14669，这是 to_char(timestamptz) 函数在处理超长 POSIX 时区缩写时引发的堆缓冲区溢出高危漏洞。修复版本为 18.6、17.11、16.15、15.19 和 14.24；由于 18.5 因回归问题未发布，18 系列用户应直接升级到 18.6。 该漏洞可能让低权限数据库用户以 PostgreSQL 服务进程的操作系统权限执行任意代码，对受影响的安装构成严重风险。由于 CVSS 评分为 8.8，管理员应优先升级小版本以防止服务器被攻陷。 该漏洞在 to_char(timestamptz) 处理超长 POSIX 时区缩写时触发；利用前提是攻击者拥有低权限数据库账户并能设置时区，因此并非无需认证即可利用。此次小版本更新不需要转储数据库或运行 pg_upgrade，只需更新程序文件并重启服务。

telegram · zaihuapd · 8月14日 14:35

**背景**: PostgreSQL 的 to_char 函数可将时间戳、时间间隔、数字等值转换为格式化字符串，而 timestamptz 类型用于存储带时区信息的日期和时间。POSIX 时区字符串可以包含缩写和偏移量，超长的缩写可能导致服务器 C 代码中的固定大小缓冲区溢出。堆缓冲区溢出属于内存安全漏洞，通常可被利用来执行任意代码，因此该项目将此问题定为高危。用户应为其主版本安装最新小版本以修复该缺陷。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/functions-formatting.html">PostgreSQL: Documentation: 18: 9.8. Data Type Formatting Functions</a></li>
<li><a href="https://www.postgresql.org/docs/current/datatype-datetime.html">PostgreSQL: Documentation: 18: 8.5. Date/Time Types</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#CVE`, `#Security`, `#Vulnerability`, `#to_char`

---

<a id="item-12"></a>
## [苹果联手阿里自研中国专属 AI 大模型，或成首家获批外企](https://www.reuters.com/business/retail-consumer/apple-trains-its-own-ai-model-china-market-with-alibabas-support-sources-say-2026-08-14/) ⭐️ 8.0/10

苹果正联手阿里巴巴为中国市场专门训练一款大语言模型，改变此前依赖第三方模型的策略。Apple Intelligence 预计未来数月随 iOS 更新在华上线，中国网信办已备案其生成式 AI 服务。 若获批，苹果将成为首家获准在华提供自有 AI 模型的外国公司，这对 AI 监管和竞争格局意义重大。同时，苹果将能更好地掌控其在中国这一重要市场设备上的 AI 体验。 据知情人士透露，苹果专门为中国市场训练自研大模型，并由阿里巴巴提供支持。中国网信办已备案其生成式 AI 服务，这是依据 2023 年 8 月施行的《生成式人工智能服务管理暂行办法》迈出的关键一步。

telegram · zaihuapd · 8月14日 14:47

**背景**: Apple Intelligence 是苹果的个人智能系统，深度集成于 iOS 18、iPadOS 18 和 macOS Sequoia，通过端侧与服务器处理协同工作。在中国，所有生成式 AI 服务在面向公众提供前，必须向中国网信办完成备案或登记，因此苹果需要遵守当地监管要求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zh.wikipedia.org/wiki/Apple_Intelligence">Apple Intelligence - 维基百科，自由的百科全书</a></li>
<li><a href="https://www.gov.cn/zhengce/zhengceku/202307/content_6891752.htm">生成式人工智能服务管理暂行办法_国务院部门文件_中国政府网</a></li>
<li><a href="https://www.cac.gov.cn/2024-04/02/c_1713729983803145.htm">国家互联网信息办公室关于发布生成式人工智能服务已备案信息的公告_中...</a></li>

</ul>
</details>

**标签**: `#Apple`, `#AI`, `#China`, `#Alibaba`, `#Large Language Model`

---