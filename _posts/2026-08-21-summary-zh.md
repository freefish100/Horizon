---
layout: default
title: "Horizon Summary: 2026-08-21 (ZH)"
date: 2026-08-21
lang: zh
---

> 从 37 条内容中筛选出 11 条重要资讯。

---

1. [恶意 arrayref crate 在构建时执行载荷，供应链攻击](#item-1) ⭐️ 9.0/10
2. [GitHub 8 月 17 日故障：重试风暴与规模性失败](#item-2) ⭐️ 8.0/10
3. [斯沃茨因抓取获罪，Meta 却毫发无损？](#item-3) ⭐️ 8.0/10
4. [速卖通网页利用无声 WebAudio 指纹识别破坏蓝牙多点连接](#item-4) ⭐️ 8.0/10
5. [学校教育如何扼杀对生物学的热爱，以及如何重新发现它](#item-5) ⭐️ 8.0/10
6. [125M Transformer 在设备端实时自动补全钢琴演奏](#item-6) ⭐️ 8.0/10
7. [ChatGPT 搜索大规模使用 site: 操作符](#item-7) ⭐️ 8.0/10
8. [OpenAI 预览前沿模型零数据留存与私密安全处理](#item-8) ⭐️ 8.0/10
9. [Stripe 拟逾 70 亿美元收购 AI 模型聚合平台 OpenRouter](#item-9) ⭐️ 8.0/10
10. [陶哲轩警告：AI 或引发数学界自哥德尔以来最大危机](#item-10) ⭐️ 8.0/10
11. [反向图像搜索服务泄露数百万张人脸照片](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [恶意 arrayref crate 在构建时执行载荷，供应链攻击](https://safedep.io/arrayref-proc-macro1-rust-build-time-malware/) ⭐️ 9.0/10

流行的 Rust crate 'arrayref' 发布了一个恶意版本，在构建时执行载荷。crates.io 直接删除了该问题版本，而没有标记为 yanked，也未发布任何安全公告。 这是 Rust 生态系统中的一次关键供应链安全事件，影响了所有依赖受影响版本 arrayref 的项目。它暴露了 crates.io 在事件处理上的不足，以及构建脚本所承载的固有信任风险。 该载荷通过构建脚本（build.rs）在编译期间执行，这是 Rust 中已知的攻击向量。问题版本被直接移除，没有 yank 通知或安全公告，增加了用户发现和应对的难度。

hackernews · abhisek · 8月20日 13:23 · [社区讨论](https://news.ycombinator.com/item?id=49374269)

**背景**: crate 是 Rust 编译器一次处理的最小代码单元，本质上相当于库或包。Rust 构建脚本在编译前执行任意代码，而过程宏在编译器内部运行，因此恶意 crate 可以在开发者执行简单的'cargo build'时就在其机器上运行代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://doc.rust-lang.org/book/ch07-01-packages-and-crates.html">Packages and Crates - The Rust Programming Language</a></li>
<li><a href="https://github.com/rust-secure-code/wg/issues/29">Build-time sandboxing · Issue #29 · rust-secure-code/wg</a></li>

</ul>
</details>

**社区讨论**: 评论者批评 crates.io 对事件准备不足，指出问题 crate 版本被直接删除而没有 yank 标记或安全公告。有人呼吁 Cargo 为 build.rs 脚本增加沙箱机制，也有人认为 Rust 庞大的依赖树使其与 JavaScript 生态系统一样脆弱。

**标签**: `#security`, `#rust`, `#supply-chain`, `#malware`, `#crates.io`

---

<a id="item-2"></a>
## [GitHub 8 月 17 日故障：重试风暴与规模性失败](https://github.blog/news-insights/company-news/the-august-17-outage-and-the-work-ahead/) ⭐️ 8.0/10

GitHub 发布了 8 月 17 日故障的事后分析，指出重试风暴和与规模相关的故障是根本原因。公司还概述了未来提高服务韧性的工作计划。 这一点很重要，因为 GitHub 承载着数百万团队和开发者的代码与开发工作流，一次重大故障会扰乱全球软件生态。它还突显了在平台使用量以前所未有的速度增长时维持可靠性的困难。 事后分析指出，自 4 月以来，月度提交量从 14 亿增长到 29 亿。某次事件中，内部端点的延迟响应触发了 VS Code 中一个潜在的重试缺陷，使流量放大约 10 倍，并延误了 Copilot Token Service 的恢复。

hackernews · 0xedb · 8月20日 19:22 · [社区讨论](https://news.ycombinator.com/item?id=49378957)

**背景**: 重试风暴是指许多客户端自动且激进地重试失败的请求，从而产生大量流量，即使在原始问题解决后也可能压垮系统。这与级联故障不同，级联故障是问题通过依赖关系传播。在大规模分布式系统中，重试风暴会严重延迟恢复，因为额外的流量使系统无法跟上。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@Rajjj/retry-storm-how-a-single-user-crashed-30-ecs-tasks-at-production-98c84c17331c">Retry Storm : How A Single User Crashed 30 ECS Tasks At... | Medium</a></li>
<li><a href="https://dash.fi/blog/retry-storm">The Operational Waste Created by Retry Storms - Dash.fi...</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍对故障处理持批评态度，不少人指出增长规模惊人且可能难以持续。一些人对 GitHub 是否能在不收费的情况下跟上步伐表示怀疑，而另一些人则指出，微软的人工智能业务利益可能使其愿意承担这些成本。

**标签**: `#outage`, `#postmortem`, `#github`, `#reliability`, `#scaling`

---

<a id="item-3"></a>
## [斯沃茨因抓取获罪，Meta 却毫发无损？](https://blog.curiousquail.com/im-upset-again-about-a-co-creator-of-rss-being-prosecuted-for-something-meta-is-doing-with-little-consequence/) ⭐️ 8.0/10

一篇评论文章指出，RSS 共同创造者亚伦·斯沃茨当年因抓取学术论文被依据《计算机欺诈与滥用法案》严厉起诉，而 Meta 如今大规模抓取数据用于 AI 训练却没有面临类似的法律后果。文章认为这暴露了数据抓取法律执法中的系统性不公。 这篇文章将一桩具有标志性意义的悲剧案件与当下 AI 训练数据的争议联系起来，质疑大型科技公司是否享有执法上的优待。它可能影响公众舆论以及围绕抓取、版权和 AI 发展问责制的政策讨论。 文章的核心是美国政府对斯沃茨的起诉：他通过麻省理工学院的网络下载 JSTOR 论文，面临数十年刑期，而 JSTOR 本身未提起民事诉讼。相比之下，Meta 为 AI 训练进行的大规模抓取并未招致类似的联邦打击，作者认为这种差异源于企业权力。

hackernews · speckx · 8月20日 20:07 · [社区讨论](https://news.ycombinator.com/item?id=49379550)

**背景**: 网页抓取（web scraping）是从网站自动提取数据的技术，常用于价格监控、研究和 AI 训练。《计算机欺诈与滥用法案》（CFAA）是美国 1986 年颁布的法律，将某些未经授权的计算机访问定为犯罪，但近年法院已缩小了其适用范围。亚伦·斯沃茨是互联网活动家、RSS 共同创造者，他 2011 年被捕、2013 年自杀，成为反对过度刑事化人士的著名案例。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Web_scraping">Web scraping</a></li>
<li><a href="https://en.wikipedia.org/wiki/Computer_Fraud_and_Abuse_Act">Computer Fraud and Abuse Act</a></li>

</ul>
</details>

**社区讨论**: 评论者观点不一：有人认为法律体系执行本就参差不齐，金钱和权力能让大公司免受追究；也有人指出斯沃茨案涉及物理入侵和绕过网络禁令，与普通的开放网页抓取不同。还有评论者提醒不要把斯沃茨简化为一个隐喻，强调他个人的脆弱性和案件背后真实的人生故事。整体讨论既表达了对斯沃茨的同情，也呼吁更准确的比较。

**标签**: `#scraping`, `#legal`, `#AaronSwartz`, `#Meta`, `#AI ethics`

---

<a id="item-4"></a>
## [速卖通网页利用无声 WebAudio 指纹识别破坏蓝牙多点连接](https://blog.laserphile.com/2026/08/aliexpress-webpage-keeping-multipoint.html) ⭐️ 8.0/10

速卖通首页通过高度混淆的阿里巴巴安全脚本，静默创建两个运行中的 WebAudio 音频图，用于指纹识别。这一行为不仅可实现用户追踪，还会无意中让蓝牙多点连接耳机持续处于活动状态。 与 Cookie 不同，WebAudio 指纹识别是隐形的，即使在开启“不追踪”的情况下也能生效，因此构成严重的隐私威胁。它还能干扰蓝牙多点连接，说明激进的指纹识别会对用户的现实硬件使用产生实际影响。 客户端代码会收集并传输大量类似指纹的测量数据，但服务端的数据保留和身份关联行为在浏览器中不可见。Firefox 和 WebKit 等浏览器已着手修复静音 AudioContext 指纹识别问题，但这类做法依然普遍存在。

hackernews · emctech · 8月20日 10:08 · [社区讨论](https://news.ycombinator.com/item?id=49372583)

**背景**: 指纹识别是网站不依赖 Cookie，而是通过采集设备和浏览器特征来识别用户的一种技术。WebAudio 指纹识别利用 AudioContext 接口生成细微的音频信号，其输出可反映硬件和软件细节；所谓“无声”是指输出不被用户听到，从而避免被发现。蓝牙多点连接允许一副耳机同时连接两个设备，而网页持续占用音频流会让耳机误以为有活跃连接，从而切换离开其他设备。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.laserphile.com/2026/08/aliexpress-webpage-keeping-multipoint.html">laserphile: AliExpress webpage keeping multipoint Bluetooth headphones active with WebAudio fingerprinting</a></li>
<li><a href="https://news.ycombinator.com/item?id=49372583">AliExpress runs silent WebAudio fingerprinting that breaks Bluetooth multipoint | Hacker News</a></li>
<li><a href="https://bugzilla.mozilla.org/show_bug.cgi?id=1358149">1358149 - Address fingerprinting issues with AudioContext</a></li>

</ul>
</details>

**社区讨论**: 评论区用户分享了各自的现实遭遇，例如 iPhone 上助听器环境噪音放大变化，以及速卖通 iOS 应用在后台触发汽车语音命令。还有人提到 Firefox 已对 WebAudio 指纹识别采取缓解措施，也有人质疑苹果是否会以封闭生态的隐私承诺为由，将速卖通从 App Store 下架。

**标签**: `#privacy`, `#fingerprinting`, `#websecurity`, `#bluetooth`, `#webaudio`

---

<a id="item-5"></a>
## [学校教育如何扼杀对生物学的热爱，以及如何重新发现它](https://jsomers.net/i-should-have-loved-biology/) ⭐️ 8.0/10

在这篇 2020 年的反思文章中，作者在 jsomers.net 指出，传统的生物学教育常常用死记硬背取代好奇心，并描述了他后来通过独立阅读和思考重新发现生物学之美与复杂性的过程。这篇文章广受关注，并多次出现在 Hacker News 上。 这篇文章引起了许多读者的共鸣，他们认为学校里的科学教育扼杀了好奇心，同时也为关于教学法和如何在 STEM 教育中培养内在动机的持续讨论提供了素材。它的走红表明，人们普遍渴望一种更强调发现而非记忆的科学教育。 这篇文章是一篇个人叙事而非学术论文，文中着重描述了若干具体的生物学机制，体现了作者重新燃起的敬畏感。评论者指出其真正主题是教学法，引用了皮亚杰和帕佩特等思想家；还有人提供了 Hacker News 搜索链接，显示这篇文章是‘常青热门’。

hackernews · tyre · 8月20日 17:50 · [社区讨论](https://news.ycombinator.com/item?id=49377853)

**背景**: 传统的生物学教育往往侧重于记忆术语、代谢通路和分类，而忽视对生命系统的探索，这可能会抑制好奇心。这篇随笔属于更广泛的 STEM 教育反思类文本，最初于 2020 年发表在 jsomers.net 上，并在 Hacker News 上引发了程序员和科学家之间长时间的讨论。

**社区讨论**: 评论区总体持赞赏态度，但也不乏补充与修正：一位转行生命科学研究的评论者称这种看法‘浪漫化’，并指出现实中没有光环的‘螺丝钉’角色；其他人同意文章真正谈的是教学法，并联系到皮亚杰和帕佩特。还有读者分享了自己对生物学的热爱，或表示在物理、化学中也有类似感受。

**标签**: `#biology`, `#education`, `#pedagogy`, `#science`, `#curiosity`

---

<a id="item-6"></a>
## [125M Transformer 在设备端实时自动补全钢琴演奏](https://simedw.com/2026/08/20/midi-autocomplete/) ⭐️ 8.0/10

一位开发者训练了一个 1.25 亿参数的 Transformer 模型，可在 iPhone 15 上以每秒约 108 个音符的速度实时自动补全 MIDI 钢琴演奏。该模型通过 Core ML 完全在设备端运行，配套应用免费提供试用。 它将常见的代码自动补全范式应用到音乐创作中，证明能力较强的 Transformer 模型可以在消费级硬件上实现富有表现力的实时交互。这也为设备端生成式音乐工具开辟了新可能，并引发关于创造力、品味和音乐传统的更广泛讨论。 该模型参数量为 1.25 亿，采用 Transformer 架构，将音符视为类似代码补全的离散 token。用户弹奏几个 MIDI 音符即可作为提示词，开发者愿意解答关于训练、Core ML 以及过程中许多失败尝试的问题。

hackernews · simedw · 8月20日 12:04 · [社区讨论](https://news.ycombinator.com/item?id=49373456)

**背景**: 自动补全系统（如 GitHub Copilot）会根据输入上下文预测后续内容。这个项目将同样的思路应用于 MIDI 形式的符号音乐，把音符视为离散 token。通过 Core ML 在设备端部署可降低延迟并避免隐私问题，从而支持实时的交互式演奏。有趣的是，基于套式(formula)的续写也是古典作曲家训练的一部分，因此这一概念与长期存在的音乐实践相呼应。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Core_ML">Core ML</a></li>
<li><a href="https://github.com/apple/coremltools">GitHub - apple/coremltools: Core ML tools contain supporting tools for Core ML model conversion, editing, and validation. · GitHub</a></li>
<li><a href="https://developer.apple.com/machine-learning/models/">Core ML models - Machine Learning</a></li>

</ul>
</details>

**社区讨论**: 评论区整体反应积极，多位评论者将其与古典作曲家的训练和基于模式的生成传统联系起来。一位古典钢琴家兼产品设计师指出它与 AI 驱动的 UX 设计工具相似，认为当生成成本趋近于零时，品味成为关键的差异点。还有评论者询问训练数据规模，分享相关的算法旋律生成项目，并有人表示听到《致爱丽丝》向完全意想不到的方向发展时，会感到一种令人不安的奇异感。

**标签**: `#machine-learning`, `#music`, `#MIDI`, `#on-device`, `#transformer`

---

<a id="item-7"></a>
## [ChatGPT 搜索大规模使用 site: 操作符](https://simonwillison.net/2026/Aug/20/chatgpt-search-now-uses-the-siteoperator-at-scale/) ⭐️ 8.0/10

Promptwatch 的聚合数据显示，ChatGPT 搜索的 fanout 查询中包含 site: 操作符的比例从大约 0.3%–0.5% 跃升至 8 月 8 日的 16%–17%，与 OpenAI 的 GPT-5.6 发布相吻合。Simon Willison 认为这标志着 ChatGPT 底层搜索工具设计发生了显著变化。 这件事很重要，因为 ChatGPT 庞大的用户群如今更加依赖限定域名的搜索，这会改变哪些网站能在 AI 回答中出现。对内容发布者和 SEO/GEO 从业者而言，这预示着被 AI 引擎引用将更多地取决于站点级权威和信任，而非单页优化。 Promptwatch 的数据仅反映其自动化跟踪覆盖的提示词，并非全部 ChatGPT 流量。OpenAI 8 月 6 日的公告只提到 GPT-5.6 Sol 将“更可靠地处理事实”，Willison 认为新工具的形态更可能是 search(query, recency, domains)，而非直接使用 site: 操作符。

rss · Simon Willison · 8月20日 23:57

**背景**: site: 操作符是一种搜索查询指令，可将搜索结果限制在特定域名或 URL 前缀，长期以来被 Google 等传统搜索引擎使用。所谓“fanout 查询”（fan-out queries），是 AI 搜索平台为获取更全面信息而从用户原始提示词扩展出的子查询。生成式引擎优化（GEO）是一种新兴实践，旨在优化内容，使 ChatGPT、Claude 和 Gemini 等 AI 引擎在回答中引用该内容。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developers.google.com/search/docs/monitor-debug/search-operators/all-search-site">How To Use the Site Search Operator | Google Search Central | Documentation | Google for Developers</a></li>
<li><a href="https://ahrefs.com/blog/query-fan-out/">What is Query Fan-Out? Understanding the Hidden Queries Driving AI Search</a></li>
<li><a href="https://www.shopify.com/pk/enterprise/blog/generative-engine-optimization">The GEO Playbook: How (& Why) to Optimize for AI... - Shopify Pakistan</a></li>

</ul>
</details>

**标签**: `#ChatGPT`, `#search`, `#GEO`, `#AI`, `#SEO`

---

<a id="item-8"></a>
## [OpenAI 预览前沿模型零数据留存与私密安全处理](https://openai.com/index/offering-zero-data-retention-for-frontier-models/) ⭐️ 8.0/10

OpenAI 宣布将向符合条件的 API 客户提供零数据留存（ZDR）承诺，请求处理完毕后不保留提示词与回复。同时预览了「私密安全处理」机制，可在不向 OpenAI 人员暴露原始内容的情况下识别滥用行为，计划于 9 月逐步上线。 这对 API 客户，尤其是处理敏感或受监管数据的企业来说，是一项重大的隐私与安全增强。通过提供零数据留存和私密滥用检测，OpenAI 可能为可信 AI 服务树立新的行业标准，并促使 Anthropic、Google 等竞争对手跟进。 客户内容使用客户控制的密钥加密存储，即使被标记，OpenAI 人员也无法读取原文。该功能正在与早期客户测试，计划于 9 月逐步上线，并同步发布技术白皮书。

telegram · zaihuapd · 8月20日 02:33

**背景**: 零数据留存（ZDR）是一种隐私模式，AI API 提供商不存储提示词、回复或元数据，也不用于训练或滥用监测。传统上，滥用检测需要审查原始内容，这与隐私相冲突；新的私密安全处理技术通过安全计算仅回传有限的安全信号。客户托管加密密钥（CMEK）允许组织自行管理加密密钥，这通常是受监管行业的要求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://decagon.ai/glossary/what-is-zero-data-retention-ai">What is Zero Data Retention AI? Definition & Vendor Guide | Decagon</a></li>
<li><a href="https://inria.hal.science/hal-01355951v3/document">Privacy - Preserving Abuse Detection in Future Decentralised Online...</a></li>
<li><a href="https://docs.databricks.com/aws/en/security/keys/customer-managed-keys">Customer - managed keys for encryption | Databricks on AWS</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#Zero Data Retention`, `#Privacy`, `#AI Security`, `#API`

---

<a id="item-9"></a>
## [Stripe 拟逾 70 亿美元收购 AI 模型聚合平台 OpenRouter](https://t.me/zaihuapd/43290) ⭐️ 8.0/10

据知情人士透露，Stripe 已就收购 AI 模型聚合平台 OpenRouter 达成协议，交易金额超过 70 亿美元。最终价格仍可能变动，双方均未官方确认。 这将是 AI 开发者服务领域的重大整合，Stripe 将获得一个服务 800 万开发者、接入 400 多个 AI 模型的入口。这可能改变 AI 开发者购买和访问模型推理的方式，并巩固 Stripe 在 AI 经济中的地位。 OpenRouter 成立于 2023 年初，通过单一 API 聚合了 60 多家提供商的模型。据报道交易金额超过 70 亿美元，但消息人士称最终价格仍可能变动，Stripe 拒绝置评。

telegram · zaihuapd · 8月20日 07:00

**背景**: OpenRouter 是一个多模型 LLM API 市场和基础设施平台，通过统一接口接入众多模型，解决大语言模型碎片化的问题。Stripe 是一家主要在线支付公司，并日益关注 AI 相关支付基础设施，如 AI 代理支付和模型市场。如此规模的收购将成为 AI 基础设施领域最大的收购之一。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openrouter.ai/">OpenRouter</a></li>
<li><a href="https://www.zenml.io/llmops-database/building-a-multi-model-llm-api-marketplace-and-infrastructure-platform">OpenRouter: Building a Multi-Model LLM API Marketplace and Infrastructure Platform - ZenML LLMOps Database</a></li>

</ul>
</details>

**标签**: `#Stripe`, `#OpenRouter`, `#收购`, `#AI模型`, `#开发者服务`

---

<a id="item-10"></a>
## [陶哲轩警告：AI 或引发数学界自哥德尔以来最大危机](https://the-decoder.com/terence-tao-says-ai-could-trigger-maths-biggest-crisis-since-godel/) ⭐️ 8.0/10

陶哲轩在为 2026 年国际数学家大会撰写的文章中表示，数学界应停止争论 AI 能做什么，转而直面研究目标这一被回避的问题。他援引 First-Proof 项目第二轮结果警告，AI 可能让数学从“证明稀缺”转向“证明过剩”，产生大量无人能讲清的证明。 作为全球最知名的数学家之一，陶哲轩的警告为“AI 生成的证明可能削弱数学界的信任与验证体系”这一担忧增加了分量。如果证明的产生速度超过人类理解能力，数学可能面临堪比 20 世纪初的基础性危机，影响研究人员、期刊和形式化验证工作。 First-Proof 项目第二轮用 4 个 AI 系统测试了 10 道未发表的研究题，其中 7 道至少被一个系统判定为合格，每题成本从数十到数百美元不等。陶哲轩认为，一个无人能清晰讲解的证明即使通过形式化验证，也应被视为不完整。

telegram · zaihuapd · 8月20日 13:19

**背景**: 罗素悖论由伯特兰·罗素于 1901 年发表，它揭示了朴素集合论中的无限制概括公理会导出矛盾，动摇了将数学化归为逻辑的尝试。哥德尔不完备定理于 1931 年发表，证明任何能表达算术的一致形式系统都无法证明关于自然数的全部真命题。这两个结果共同引发了 20 世纪初的数学基础危机，陶哲轩正是将当下与之类比。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://1stproof.org/">First Proof Project</a></li>
<li><a href="https://arxiv.org/html/2606.18119v1">First Proof Second Batch</a></li>

</ul>
</details>

**标签**: `#AI`, `#mathematics`, `#Terence Tao`, `#proof verification`, `#research crisis`

---

<a id="item-11"></a>
## [反向图像搜索服务泄露数百万张人脸照片](https://arstechnica.com/gadgets/2026/08/reverse-lookup-service-exposed-millions-of-photos-of-peoples-faces/) ⭐️ 8.0/10

一家反向图像搜索服务发生数据泄露，数百万张人脸照片及相关个人信息被公开。泄露的数据库约 450GB，包含超过 900 万张图像，并涉及邮箱、电话和 IP 地址。 人脸属于难以更换的生物识别信息，一旦泄露可能引发严重的身份盗用和隐私风险。攻击者可能利用泄露的数据对受害者进行未授权的身份识别、个人追踪或诈骗。 涉事服务方已限制数据库访问，但事件影响范围和后续补救措施尚待确认。专家提醒，人脸图像一旦与其他个人数据关联，滥用风险会进一步放大。

telegram · zaihuapd · 8月20日 15:14

**背景**: 反向图像搜索通过提取上传图片的视觉特征，与网络上的索引图片进行比对，而不是依赖文字关键词。人脸识别类搜索服务则利用面部识别算法，在不同照片中匹配出同一个人。人脸等生物特征属于人体固有的物理属性，无法像密码或信用卡号那样重置或更换，因此此类数据一旦泄露，影响将长期存在。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pimeyes.com/en/blog/how-does-reverse-image-search-work">How does reverse image search work ? | PimEyes</a></li>
<li><a href="https://recfaces.com/articles/biometric-security">[:en] Biometric Security: Importance and Future | RecFaces</a></li>

</ul>
</details>

**标签**: `#security`, `#privacy`, `#data breach`, `#biometrics`, `#reverse image search`

---