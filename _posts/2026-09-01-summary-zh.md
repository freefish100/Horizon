---
layout: default
title: "Horizon Summary: 2026-09-01 (ZH)"
date: 2026-09-01
lang: zh
---

> 从 35 条内容中筛选出 5 条重要资讯。

---

1. [谷歌从 Chrome 网上应用店移除 MV2 扩展，包括 uBlock Origin](#item-1) ⭐️ 8.0/10
2. [带 sinks 的滑动窗口注意力在长上下文推理上胜过线性注意力](#item-2) ⭐️ 8.0/10
3. [OpenClaw 2.0 发布：汇集逾 1.6 万个拉取请求的大更新](#item-3) ⭐️ 8.0/10
4. [苹果换帅：库克卸任 CEO，特努斯 2026 年接任](#item-4) ⭐️ 8.0/10
5. [DeepSeek 上线视觉语言模型 deepseek-v4-flash-vision-exp API](#item-5) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [谷歌从 Chrome 网上应用店移除 MV2 扩展，包括 uBlock Origin](https://webiterate.dev/google-removed-extensions-ublock-origin-108/) ⭐️ 8.0/10

谷歌已从 Chrome 网上应用店移除所有剩余的 Manifest V2 扩展，包括广受欢迎的广告拦截工具 uBlock Origin。这一移除遵循官方弃用时间表，并开始对大多数用户生效。 这一变化严重削弱了 Chrome 中有效广告拦截和隐私保护的能力，因为 Manifest V3 限制了扩展检查与阻断网络请求的功能。数百万依赖 uBlock Origin 等扩展来保障安全和获得更干净浏览体验的用户将直接受到影响。 已安装在 Chrome 138 或更早版本上的 Manifest V2 扩展仍然保留，但无法再接收更新，一旦卸载也无法重新安装。在 Manifest V3 下，广告拦截器最多只能加载 30,000 条规则，而有效的广告拦截器通常需要 300,000 条或更多，并且必须使用 declarativeNetRequest 而非功能更强的 WebRequest API。

hackernews · twapi · 8月31日 21:10 · [社区讨论](https://news.ycombinator.com/item?id=49514878)

**背景**: Chrome 扩展通过清单文件声明其功能。Manifest V2 允许 uBlock Origin 等扩展使用 WebRequest API 实时拦截和阻断网络请求。Manifest V3 于 2020 年推出，将后台脚本迁移到 service worker，并用 declarativeNetRequest 取代 WebRequest，虽然灵活性降低，但旨在提升性能和安全性。谷歌多年来一直在逐步淘汰 Manifest V2，并计划于 2026 年 7 月 8 日将其从 Chrome 网上应用店彻底移除。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.chrome.com/docs/extensions/develop/migrate/mv2-deprecation-timeline">Manifest V2 support timeline | Chrome for Developers</a></li>
<li><a href="https://developer.chrome.com/docs/extensions/develop/migrate/what-is-mv3">Extensions / Manifest V3 | Chrome for Developers</a></li>
<li><a href="https://nordvpn.com/blog/manifest-v3-ad-blockers/">Is Google's Manifest V3 the end of ad blockers? | NordVPN</a></li>

</ul>
</details>

**社区讨论**: 评论者绝大多数批评谷歌的这一举动，许多人表示他们已经转向 Firefox 或计划这样做。一些人强调广告拦截是一个安全问题，尤其对年纪较大或不太懂技术的用户而言，他们可能误点恶意广告；评论者认为 Firefox 是唯一真正的替代选择。

**标签**: `#Chrome`, `#Manifest V3`, `#uBlock Origin`, `#Ad Blocking`, `#Browser Extensions`

---

<a id="item-2"></a>
## [带 sinks 的滑动窗口注意力在长上下文推理上胜过线性注意力](https://www.reddit.com/r/MachineLearning/comments/1w3j1vw/slidingwindow_attention_beats_linear_on/) ⭐️ 8.0/10

一篇由 Alexia Jolicoeur-Martineau 及其同事撰写的新 arXiv 预印本报告称，带注意力汇（sinks）的滑动窗口注意力（SWA）在长上下文推理任务上能够匹配或超越经过后训练的线性注意力模型。在 Needle-in-a-Haystack 和 BABILong 基准测试中，SWA 的性能比线性注意力变体高出 2 到 10 倍。 这一结果挑战了高效大语言模型部署中常见的线性注意力范式，后者通常依赖昂贵的后训练成本。这表明，像带 sinks 的 SWA 这样简单且无需后训练的基线方法，可能会重新引导长期上下文模型的研究重点与实务建议。 论文指出，线性注意力的研究路线尚未与更简单的基线进行适当比较。作者表示，线性注意力模型可能需要从头训练或大量后训练才能达到 SWA 的水平，并强烈建议改用 SWA 而非后训练的线性模型。

reddit · r/MachineLearning · /u/Justgototheeffinmoon · 8月31日 16:35

**背景**: 标准 softmax 注意力在序列长度上具有二次计算成本，使得长上下文推理开销巨大。线性注意力变体降低了这一成本，但往往需要额外训练以保持质量。滑动窗口注意力（SWA）将每个 token 的注意力限制在局部窗口内，注意力汇（sinks）是用于吸收多余注意力并稳定训练/生成的特殊 token。BABILong 是一种采用大海捞针方式测试长文档推理能力的基准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2608.28444v1">Sliding - window beats linear attention</a></li>
<li><a href="https://carnotresearch.medium.com/let-the-chaos-sink-in-481c8a37471e">Let the Chaos Sink In. Balancing attention in transformers | Medium</a></li>
<li><a href="https://github.com/booydar/babilong">GitHub - booydar/babilong: BABILong is a benchmark for LLM evaluation using the needle-in-a-haystack approach. · GitHub</a></li>

</ul>
</details>

**标签**: `#attention mechanisms`, `#long-context reasoning`, `#LLM efficiency`, `#linear attention`, `#arXiv preprint`

---

<a id="item-3"></a>
## [OpenClaw 2.0 发布：汇集逾 1.6 万个拉取请求的大更新](https://openclaw.ai/blog/openclaw-2-accidentally) ⭐️ 8.0/10

OpenClaw 于 8 月 30 日发布史上最大更新 2.0，汇集了 933 名贡献者（含 569 名首次参与者）提交的逾 1.6 万个拉取请求。此次更新全面革新了安装、消息、记忆、技能、模型、浏览器、插件与安全等环节，并新增共享云端会话以支持多人协作。 此次发布代表了开源 AI agent 项目中最活跃的一个重大里程碑，彰显了社区主导开发的力量。贡献规模之大——约占项目全部拉取请求的一半——标志着生态正在成熟，并可能推动自主 agent 领域的竞争。 团队特意暂停了近七周的新版本发布，以整合这些改动。主要亮点包括简化安装流程、重建浏览器端体验，以及支持实时协作的共享云端会话。

telegram · zaihuapd · 8月31日 04:38

**背景**: OpenClaw 是一个免费开源的自主 AI agent，通过大型语言模型（LLM）执行任务，并以消息平台作为其主要用户界面。它运行在用户自己的机器上，可配合用户已有的聊天应用使用，降低了 AI 自动化的门槛。拉取请求是开发者协作软件开发时提交并合并代码更改的标准方式，此次逾 1.6 万个 PR 代表了来自社区的众多改进。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenClaw">OpenClaw - Wikipedia</a></li>
<li><a href="https://openclaw.ai/">OpenClaw — Open -Source AI Assistant</a></li>

</ul>
</details>

**标签**: `#OpenClaw`, `#release`, `#open-source`, `#AI`, `#major-update`

---

<a id="item-4"></a>
## [苹果换帅：库克卸任 CEO，特努斯 2026 年接任](https://t.me/zaihuapd/43516) ⭐️ 8.0/10

苹果宣布管理层交接：现任 CEO 蒂姆·库克将卸任，出任董事会执行董事长，硬件工程高级副总裁约翰·特努斯将从 2026 年 9 月 1 日起担任新任 CEO。董事会已一致批准该安排，库克将在整个夏天继续担任 CEO，以完成交接。 这是自 2011 年蒂姆·库克接任 CEO 以来，苹果首次进行 CEO 交接，标志着这家全球最具价值公司之一进入新时代。特努斯作为长期主管硬件的高管，表明苹果将延续以产品为核心的领导风格，但此次任命仍对苹果未来的产品方向和公司战略具有重大影响。 约翰·特努斯于 2001 年加入苹果，2013 年升任硬件工程副总裁，2021 年进入高管团队，近年来负责 iPhone、Mac、iPad 和 AirPods 等硬件产品。现任董事长 Arthur Levinson 将于 9 月 1 日转任首席独立董事，特努斯也将于同一天加入董事会。

telegram · zaihuapd · 8月31日 10:21

**背景**: 在苹果历史上，CEO 一职仅更换过几次；蒂姆·库克在 2011 年接替史蒂夫·乔布斯，此前他担任首席运营官，领导苹果完成了多款重要产品发布和服务扩展。在公司董事会结构中，执行董事长通常负责统筹董事会工作，同时继续参与公司领导，而 CEO 负责日常运营。约翰·特努斯多年来一直是苹果硬件开发的核心人物，此次任命使他成为苹果历史上第四位 CEO。

**标签**: `#Apple`, `#Leadership`, `#CEO`, `#Tech Industry`

---

<a id="item-5"></a>
## [DeepSeek 上线视觉语言模型 deepseek-v4-flash-vision-exp API](https://t.me/zaihuapd/43518) ⭐️ 8.0/10

DeepSeek 已于 2026 年 8 月 21 日在 API 上发布了实验性视觉语言模型 deepseek-v4-flash-vision-exp，官网文档和定价均已更新。该模型支持图像与文本混合输入，可完成图像描述、截图文字提取和图表分析等任务。 此次发布标志着 DeepSeek 进入多模态 AI 服务领域，开发者无需依赖 GPT-4V、Gemini 或 Claude 等专有模型，就能构建具备视觉能力的应用。通过提供带 API 访问的实验性视觉模型，DeepSeek 在竞争日益激烈的 AI 基础设施市场中巩固了自身地位。 该模型可通过 Chat Completions、Responses 以及兼容 Anthropic 的 Messages API 访问，图像支持通过 URL、Base64 或文件上传提供。据 DeepSeek 介绍，与 DeepSeek-V4-Flash-0731 相比，deepseek-v4-flash-vision-exp 在多模态智能体任务上取得了显著提升，同时在纯文本智能体任务上保持了相当的性能。

telegram · zaihuapd · 8月31日 11:41

**背景**: 视觉语言模型（VLM）是一种能同时解读并生成图像与文本信息的人工智能系统，扩展了仅能处理文本的大语言模型（LLM）的能力。OpenAI 通过 GPT-4V 为 ChatGPT 引入了视觉能力，随后谷歌 Gemini、Anthropic Claude 和微软 Copilot 也加入了类似功能。DeepSeek 作为领先的 AI 实验室，一直在发布开放权重模型和 API 服务，这款新的实验性视觉模型为其产品线补充了多模态能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://api-docs.deepseek.com/guides/vision/?ref=upstract.com">Vision | DeepSeek API Docs</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash-Vision-Exp">deepseek-ai/ DeepSeek - V 4 - Flash - Vision - Exp · Hugging Face</a></li>
<li><a href="https://en.wikipedia.org/wiki/Vision-language_model">Vision-language model</a></li>

</ul>
</details>

**标签**: `#deepseek`, `#api`, `#vision`, `#language-model`, `#ai`

---