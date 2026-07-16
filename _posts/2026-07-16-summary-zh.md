---
layout: default
title: "Horizon Summary: 2026-07-16 (ZH)"
date: 2026-07-16
lang: zh
---

> 从 33 条内容中筛选出 13 条重要资讯。

---

1. [Claude web_fetch 工具绕过漏洞导致记忆数据泄露](#item-1) ⭐️ 9.0/10
2. [马斯克：X 将无条件开源全部代码，接受第三方审查](#item-2) ⭐️ 9.0/10
3. [支持音频的开放权重模型 Inkling](#item-3) ⭐️ 8.0/10
4. [xAI 在隐私丑闻后开源 Grok Build](#item-4) ⭐️ 8.0/10
5. [Stripe 与 Advent 联合出价 530 亿美元收购 PayPal](#item-5) ⭐️ 8.0/10
6. [在 13 年历史的 Xeon 上无 GPU 跑 Gemma 4 26B，速度 5 tokens/秒](#item-6) ⭐️ 8.0/10
7. [在编码中优先考虑心理健康和沟通](#item-7) ⭐️ 8.0/10
8. [Telegram 数据中心调查揭示潜在 FSB 关联](#item-8) ⭐️ 8.0/10
9. [通过哈达玛积聚类解耦卷积神经元](#item-9) ⭐️ 8.0/10
10. [美国法官质疑 Epic 与谷歌反垄断和解交易](#item-10) ⭐️ 8.0/10
11. [DeepSeek 首轮融资超 500 亿元，采用特殊架构维持控制权](#item-11) ⭐️ 8.0/10
12. [开发者利用沙盒逃逸，用 Filza 读取 iOS 27 备忘录数据库](#item-12) ⭐️ 8.0/10
13. [xAI 起诉用户利用 Grok 生成儿童性虐待深度伪造](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Claude web_fetch 工具绕过漏洞导致记忆数据泄露](https://simonwillison.net/2026/Jul/15/claude-web-fetch-exfiltration/#atom-everything) ⭐️ 9.0/10

安全研究员 Ayush Paul 发现 Claude 的 web_fetch 工具存在一个绕过漏洞，允许攻击者通过提示注入攻击窃取用户的私人记忆数据。该漏洞利用创建一个蜜罐网站，诱使 AI 按照嵌套生成的链接泄露数据。 该漏洞破坏了 Anthropic 为 Claude 设计的关键数据防泄露保护，凸显了 AI 系统中提示注入攻击的持续挑战。它表明即使精心设计的安全措施也可能被绕过，对用户隐私和 AI 助手的信任构成重大风险。 该攻击利用了一个漏洞：web_fetch 被允许访问先前获取页面中嵌入的 URL，从而可以通过嵌套链接链泄露数据。Anthropic 声称已内部发现该问题，并通过移除 web_fetch 从获取内容中导航到其他链接的能力来修复该漏洞。

rss · Simon Willison · 7月15日 14:21

**背景**: 提示注入攻击是指攻击者向语言模型输入恶意指令，导致其执行非预期操作。Simon Willison 提出的'致命三重奏'概念描述了 AI 代理易受攻击的三种能力组合：访问私人数据、摄取不可信内容和具备外部通信能力。Claude 的 web_fetch 工具设计时有限制以防止数据泄露，但嵌套链接的漏洞绕过了这些限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/">The lethal trifecta for AI agents: private data, untrusted content, and external communication</a></li>
<li><a href="https://simonwillison.net/2025/Sep/10/claude-web-fetch-tool/">Claude API: Web fetch tool</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#prompt injection`, `#security vulnerability`, `#LLM`, `#Claude`

---

<a id="item-2"></a>
## [马斯克：X 将无条件开源全部代码，接受第三方审查](https://x.com/elonmusk/status/2077361679034118271) ⭐️ 9.0/10

埃隆·马斯克宣布，X 平台在完成安全漏洞审查后，将无条件开源其全部代码库，并邀请第三方审查者检查正在运行的系统，以确认开源代码与实际运行的代码一致。 此举可能大幅提升 X 平台的透明度和信任度，为大型社交媒体平台的可问责性树立新标准，并可能影响其他科技公司效仿。 开源的前提是先完成安全漏洞审查，第三方审查者将确认运行的二进制文件与发布的源代码一致，这种做法类似于二进制透明度和可重现构建。

telegram · zaihuapd · 7月15日 13:32

**背景**: 开源软件允许任何人查看、修改和分发源代码，促进透明度和社区协作。然而，确保编译后的二进制文件与发布的源代码一致（可重现构建）以及维护可验证的发布日志（二进制透明度）对于防止篡改和建立信任至关重要。马斯克的声明表明 X 将采用这些实践，以确保声称开源的代码确实是在其服务器上运行的代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Reproducible_builds">Reproducible builds</a></li>
<li><a href="https://reproducible-builds.org/">Reproducible Builds — a set of software development practices that create an independently-verifiable path from source to binary code</a></li>
<li><a href="https://binary.transparency.dev/">Binary Transparency</a></li>

</ul>
</details>

**标签**: `#open source`, `#transparency`, `#Elon Musk`, `#X`, `#social media`

---

<a id="item-3"></a>
## [支持音频的开放权重模型 Inkling](https://thinkingmachines.ai/news/introducing-inkling/) ⭐️ 8.0/10

Thinking Machines Lab 发布了 Inkling，一个支持音频的开放权重多模态模型，旨在以更低成本进行微调。 该模型为定制化提供了一个强大的开放权重替代方案，尤其在音频相关任务中，可能使前沿微调模型的获取更加民主化。 Inkling 并非整体最强模型，但结合了多模态能力、高效推理以及可在 Tinker 平台上微调的特点；它是计划中的模型系列的首个版本。

hackernews · vimarsh6739 · 7月15日 18:12 · [社区讨论](https://news.ycombinator.com/item?id=48924912)

**背景**: 开放权重模型允许任何人下载、运行、研究和修改模型，比闭源模型更透明。多模态 AI 处理文本、音频和图像等多种数据类型。Inkling 在开放权重模型中因支持音频而突出。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/introducing-inkling/">Inkling: Our open-weights model - Thinking Machines Lab</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Multimodal_model">Multimodal model</a></li>

</ul>
</details>

**社区讨论**: 评论者对 Inkling 的音频能力和作为可定制开放模型的潜力表示热情。有人将其与其他中国开放模型比较，并指出在 Tinker 上提供微调的商业模式。还有人对现代模型设计的复杂性表示赞赏。

**标签**: `#open-weights model`, `#multimodal AI`, `#audio AI`, `#fine-tuning`, `#AI business model`

---

<a id="item-4"></a>
## [xAI 在隐私丑闻后开源 Grok Build](https://github.com/xai-org/grok-build) ⭐️ 8.0/10

xAI 已在 GitHub 上开源其 Grok Build CLI 工具，将代码库以开源许可证形式公开。 此举允许开发者检查、修改和复刻代码，但在此之前，该工具曾因会上传整个目录（包括 SSH 密钥和密码数据库）而引发重大隐私争议。许多人认为开源是一种恢复信任和社区参与的战术性回应。 代码库包含一个自包含的终端渲染器，使用 Unicode 框绘图渲染部分 Mermaid 图表。已出现多个社区复刻版本，例如去除供应商遥测并阻止自动更新的 'gork-build'，以及从源代码构建的 'dgrok'。

hackernews · skp1995 · 7月15日 20:24 · [社区讨论](https://news.ycombinator.com/item?id=48926590)

**背景**: Grok Build 是 xAI（SpaceXAI）于 2026 年 5 月推出的早期测试版编程代理和 CLI 工具，用于专业软件工程。它可运行最多 8 个 AI 代理，经过规划、搜索和构建三个阶段，在 SWE-bench verified 上得分为 70.8%。该工具最近因用户发现其在目录中运行时会将该目录整体上传至 xAI 云存储而受到严厉批评。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Grok_Build">Grok Build</a></li>
<li><a href="https://x.ai/news/grok-build-cli">Introducing Grok Build | SpaceXAI</a></li>
<li><a href="https://grok.com/build">Grok Build</a></li>

</ul>
</details>

**社区讨论**: 社区情绪复杂：有人赞扬开源举动，但许多人因之前的数据泄露和埃隆·马斯克的关联而表示不信任。像 'gork-build' 这样的复刻版本被视为注重隐私的替代方案而受到欢迎；一些评论者指出此次发布更多是战术性操作而非真正致力于开放。

**标签**: `#open-source`, `#AI`, `#xAI`, `#Grok`, `#build-system`

---

<a id="item-5"></a>
## [Stripe 与 Advent 联合出价 530 亿美元收购 PayPal](https://www.reuters.com/business/finance/stripe-advent-offer-buy-paypal-more-than-53-billion-sources-say-2026-07-15/) ⭐️ 8.0/10

据消息人士透露，Stripe 与私募股权公司 Advent International 联合出价超过 530 亿美元收购 PayPal。 这笔潜在收购将打造在线支付领域的霸主，融合 Stripe 的现代支付基础设施与 PayPal 庞大的用户群及 Venmo、Braintree 等品牌，引发重大反垄断担忧。 该出价对 PayPal 估值超过 530 亿美元，反垄断监管机构可能因市场集中度问题要求剥离 Venmo 和 Braintree。

hackernews · rvz · 7月15日 03:32 · [社区讨论](https://news.ycombinator.com/item?id=48915953)

**背景**: PayPal 是最古老且规模最大的在线支付平台之一，而 Stripe 是互联网企业领先的支付处理商。赫芬达尔-赫希曼指数（HHI）是衡量市场集中度的指标，如果这些公司合并，该指数可能会非常高，表明存在潜在的反垄断问题。

**社区讨论**: 社区成员对反垄断影响及合并后可能涨价表示强烈担忧。一些人指出，Stripe 对特定行业（如大麻、成人内容）的限制性政策可能会伤害目前由 PayPal 更宽松政策服务的商家。

**标签**: `#fintech`, `#acquisition`, `#payments`, `#antitrust`

---

<a id="item-6"></a>
## [在 13 年历史的 Xeon 上无 GPU 跑 Gemma 4 26B，速度 5 tokens/秒](https://www.neomindlabs.com/2026/06/08/running-gemma-4-26b-at-5-tokens-sec-on-a-13-year-old-xeon-with-no-gpu/) ⭐️ 8.0/10

一篇博文展示了在没有 GPU 的情况下，在一台双路 13 年历史的 Xeon 服务器上以每秒 5 个 token 的速度运行 Google 的 Gemma 4 26B 混合专家模型。 这表明在非常老旧、低成本的硬件上运行大型语言模型是可行的，挑战了本地推理需要昂贵 GPU 的假设。同时引发了社区关于本地推理与云端 API 相比在电费和硬件成本上是否划算的讨论。 使用的服务器是双路 Xeon E5-2670（Sandy Bridge 架构，约 2013 年），配备 256 GB DDR3 内存，通过 llama.cpp 使用 4 比特量化版 Gemma 4 26B 达到 5 tokens/秒。社区成员指出，在这样的速度下，使用推理提供商的费用可能比本地电费更便宜，也有人报告在同等硬件上获得了相似或更快的速度。

hackernews · neomindryan · 7月15日 15:34 · [社区讨论](https://news.ycombinator.com/item?id=48922434)

**背景**: Gemma 4 是 Google 推出的开源模型系列，其中包括一个 260 亿参数的混合专家（MoE）变体，每个 token 仅激活约 40 亿参数，使其更适合 CPU 推理。通过量化和使用 llama.cpp 等优化推理引擎，可以在没有 GPU 的 CPU 上运行大模型，但 token 生成速度通常比现代 GPU 慢数个数量级。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/google/gemma-4-26B-A4B">google/gemma-4-26B-A4B · Hugging Face</a></li>
<li><a href="https://ai.google.dev/gemma/docs/core">Gemma 4 model overview | Google AI for Developers</a></li>
<li><a href="https://ollama.com/library/gemma4:26b">gemma4:26b</a></li>

</ul>
</details>

**社区讨论**: 评论者在成本问题上意见不一：有人认为使用推理提供商比本地电费更便宜，而另一些人反驳说摊销硬件成本和提示处理会降低本地成本。有用户预测到 2027 年消费级硬件可运行超过 200B 的 MoE 模型，并举例自己在 16GB Mac 上以 7-9 t/s 运行 Qwen3.6-35B。另一位用户分享了在双路 Xeon 与 256 GB DDR4 上运行模型的报告，获得了类似速度。

**标签**: `#LLM`, `#inference`, `#hardware optimization`, `#cost analysis`, `#community discussion`

---

<a id="item-7"></a>
## [在编码中优先考虑心理健康和沟通](https://ramones.dev/posts/mental-health/) ⭐️ 8.0/10

一位软件开发者发表了关于心理健康的个人反思，倡导更好的沟通和自我管理，并设定了 2027 年的具体目标以减少错误。这篇文章引发了关于神经多样性和职场福祉的丰富讨论。 这场讨论凸显了软件行业对心理健康日益增长的认识——高认知需求常导致倦怠。它验证了许多开发者（尤其是神经多样性人群）的经历，并鼓励更开放的对话。 评论串揭示了许多开发者对管理注意力和避免错误的挣扎感同身受，而另一些人则强调神经多样性并非可以“突然摆脱”，需要量身定制的策略。帖子本身设定了具体目标，例如为每项任务制定计划并只做那件事。

hackernews · ramon156 · 7月15日 11:27 · [社区讨论](https://news.ycombinator.com/item?id=48919198)

**背景**: 神经多样性指人类大脑功能的自然变异，包括自闭症、ADHD、阅读障碍等，影响注意力、社交舒适度和认知。在软件开发这种要求持续细节关注的工作中，神经多样性个体常面临完成任务和沟通方面的独特挑战。神经多样性运动视这些差异为正常变异而非障碍，倡导职场合理便利。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Neurodivergence">Neurodivergence</a></li>
<li><a href="https://en.wikipedia.org/wiki/Neurodiversity">Neurodiversity - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了强烈的共鸣，许多人分享了自己类似挣扎的个人经历。一些人警告说，神经多样性的模式无法通过简单的计划系统来修复，而另一些人则强调自我接纳和发挥自身独特优势的重要性，而不是试图成为别人。

**标签**: `#mental health`, `#software development`, `#communication`, `#neurodivergence`, `#workplace well-being`

---

<a id="item-8"></a>
## [Telegram 数据中心调查揭示潜在 FSB 关联](https://dev.moe/en/3025) ⭐️ 8.0/10

一项对 Telegram 数据中心架构的调查揭示了异常模式，例如缺少 DC3，以及有报道称管理 Telegram 基础设施的人也在管理俄罗斯 FSB 的基础设施。 这些发现对数亿 Telegram 用户的隐私和安全提出了严重关切，尤其是俄罗斯和乌克兰的用户，因为它们暗示可能存在政府影响或监控能力。 Telegram 的数据中心（DC1 至 DC5）分布不均，其中 DC2 服务于俄罗斯和乌克兰用户，而 DC3 在编号方案中缺失；调查还声称，Telegram 的基础设施由一位同时管理 FSB 基础设施的人管理，且 Telegram 员工不知情。

hackernews · theanonymousone · 7月15日 13:22 · [社区讨论](https://news.ycombinator.com/item?id=48920475)

**背景**: Telegram 为其云消息服务使用分布式数据中心架构，每个用户根据地理位置被分配到特定的数据中心。MTProto 协议处理客户端-服务器通信。IStories 的最新报道称，同一个人同时管理 Telegram 和 FSB 的基础设施，这可能允许监控或干预。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Telegram_(software)">Telegram (software) - Wikipedia</a></li>
<li><a href="https://core.telegram.org/api/datacenter">Working with Different Data Centers</a></li>
<li><a href="https://core.telegram.org/mtproto">MTProto Mobile Protocol</a></li>

</ul>
</details>

**社区讨论**: 评论者提供了额外证据：有人链接了一篇 IStories 文章确认 FSB 基础设施关联，另一人指出 DC2 在俄语社区中经常宕机，还有一人推测缺失的 DC3 可能用于“特殊”账户数据。另一位评论者批评 Telegram 的自定义基础设施是技术债务。

**标签**: `#telegram`, `#data centers`, `#infrastructure`, `#privacy`, `#security`

---

<a id="item-9"></a>
## [通过哈达玛积聚类解耦卷积神经元](https://www.reddit.com/r/MachineLearning/comments/1uwya70/mechanistic_interpretability_a_first_paper_on/) ⭐️ 8.0/10

作者提出了一种新方法，利用神经元的感受野与其权重的哈达玛积，结合聚类分析，解耦并揭示了 InceptionV1 中单个神经元内的单语义和多语义聚类。 这项工作通过提供更细粒度的方法来理解单个卷积神经元检测的内容，推进了机制可解释性，可能有助于更好地理解神经网络并构建更安全的 AI 系统。 该技术应用于 InceptionV1 的 mixed4e 层中的一个 1x1 卷积神经元，得到了汽车、猫等物体的干净单语义聚类，以及字母、人脸等噪声聚类，并发现梯度下降通过均匀分布正负权重来抑制不需要的模式。

reddit · r/MachineLearning · /u/narang_27 · 7月15日 06:59

**背景**: 机制可解释性旨在通过理解神经网络内部组件和计算来对其进行逆向工程。单语义性是一个关键概念，指神经元或特征只对单一概念做出响应。哈达玛积（Hadamard product）是逐元素乘法，在此用于隔离神经元在其感受野中“看到”的内容。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mechanistic_interpretability">Mechanistic interpretability</a></li>
<li><a href="https://arize.com/blog/towards-monosemanticity/">Towards Monosemanticity : Decomposing Language Models... - Arize AI</a></li>

</ul>
</details>

**标签**: `#mechanistic interpretability`, `#disentangling neurons`, `#convolutional neural networks`, `#InceptionV1`, `#monosemanticity`

---

<a id="item-10"></a>
## [美国法官质疑 Epic 与谷歌反垄断和解交易](https://t.me/zaihuapd/42588) ⭐️ 8.0/10

在听证会上，美国地区法官 James Donato 披露，Epic Games 与谷歌已达成一项新的商业合作，涉及 Epic 在六年内向谷歌支付约 8 亿美元，以及联合产品开发、营销和合作伙伴关系。 法官质疑该合作是否削弱了 Epic 在反垄断诉讼中推动 Android 生态改革的立场，可能影响诉讼结果及未来的移动平台政策。 该合作涉及 Unreal Engine、《堡垒之夜》及 Android 相关业务，Epic CEO Tim Sweeney 表示协议未包含为 Epic Games Store 提供 Google Play 商店的特殊访问权限。

telegram · zaihuapd · 7月15日 11:15

**背景**: Epic Games 于 2020 年起诉谷歌，指控其通过 Google Play 在 Android 应用分发市场实施垄断行为。反垄断审判于 2023 年 12 月以陪审团裁决支持 Epic 告终，目前案件处于补救阶段。这一新的商业交易引发了对 Epic 开放 Android 生态系统承诺的质疑。

**标签**: `#antitrust`, `#Epic Games`, `#Google`, `#Android`, `#app store`

---

<a id="item-11"></a>
## [DeepSeek 首轮融资超 500 亿元，采用特殊架构维持控制权](https://t.me/zaihuapd/42589) ⭐️ 8.0/10

DeepSeek 完成了首轮融资，筹集超过 500 亿元人民币（约合 740 亿美元），估值超过 500 亿美元，并采用特殊架构维持创始人控制权。 本轮巨额融资吸引了腾讯和宁德时代等主要投资者，表明市场对 DeepSeek 人工智能技术的强烈信心，其独特的治理架构可能为中国大型科技公司创始人控制权树立先例。 投资者需将资金注入由 CEO 梁文锋管理的有限合伙企业，接受五年锁定期且不享有表决权。梁文锋在本轮融资中个人投资 2000 亿元。

telegram · zaihuapd · 7月15日 12:56

**背景**: DeepSeek 是中国领先的人工智能公司。本轮融资采用“特殊架构”，投资者不直接持有 DeepSeek 股份，而是投资于有限合伙企业，从而使创始人梁文锋保持控制权。这种结构在大规模融资中并不常见，可能引发治理方面的疑问。

**标签**: `#DeepSeek`, `#Funding`, `#AI`, `#Venture Capital`, `#China`

---

<a id="item-12"></a>
## [开发者利用沙盒逃逸，用 Filza 读取 iOS 27 备忘录数据库](https://x.com/0xjohnny/status/2077216973256274272) ⭐️ 8.0/10

开发者@0xjohnny 修改了 iOS 文件管理器 Filza，利用沙盒逃逸漏洞，在运行 iOS 27 beta 3 的 iPhone 17 Pro Max 上访问了备忘录数据库。 这展示了一个高风险沙盒逃逸漏洞，可用于访问敏感用户数据，凸显了 iOS 持续面临的安全挑战。同时也表明第三方工具如何能在测试版软件上绕过苹果的安全边界。 该漏洞绕过了应用自身的容器限制，以读取外部数据，具体是备忘录数据库。用户修改了 Filza（一款流行的越狱 iOS 设备文件管理器），并在预发布版本 iOS 27 beta 3 上进行了测试。

telegram · zaihuapd · 7月15日 14:35

**背景**: 沙盒逃逸是一种安全漏洞，允许应用突破其受限环境，访问其他应用或系统的数据。Filza 是一款常用于越狱 iOS 设备的文件管理器，可浏览整个文件系统。沙盒逃逸是关键漏洞，因为它们可能导致未经授权的数据访问，过去的研究和黑客竞赛中已有先例。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ios-repo-updates.com/repository/tigisoftware/package/com.tigisoftware.filza/">Package: Filza File Manager • com.tigisoftware....</a></li>
<li><a href="https://www.tigisoftware.com/default/?page_id=78">Filza – TIGI Software</a></li>
<li><a href="https://www.idownloadblog.com/2025/03/27/banking-apps-using-0-day-sandbox-escape-to-detect-trollstore/">Are certain banking apps using a 0-day sandbox escape to detect...</a></li>

</ul>
</details>

**标签**: `#iOS安全`, `#沙盒逃逸`, `#漏洞利用`, `#Filza`

---

<a id="item-13"></a>
## [xAI 起诉用户利用 Grok 生成儿童性虐待深度伪造](https://www.reuters.com/legal/litigation/musks-xai-sues-grok-user-over-sexualized-deepfakes-2026-07-15/) ⭐️ 8.0/10

xAI 对南卡罗来纳州男子 Terry Harwood 提起诉讼，指控其利用 Grok 聊天机器人生成儿童性虐待材料和非自愿成人深度伪造，这是 AI 公司因用户此类滥用行为而起诉用户的首批案件之一。 此案为追究用户滥用 AI 工具生成有害深度伪造的法律责任树立了先例，并凸显了 AI 公司为打击儿童剥削和非自愿内容而加强执法力度的趋势。 xAI 报告称，今年已暂停 52,222 个账户，向国家失踪与受虐儿童中心举报 73,604 次，并促成至少 244 人被捕。该诉讼要求赔偿并申请法院永久禁止 Harwood 使用 Grok。

telegram · zaihuapd · 7月16日 01:45

**背景**: Grok 是由 xAI 开发的生成式 AI 聊天机器人，于 2023 年 11 月推出，以其与 X（原 Twitter）的集成以及生成露骨内容的争议性倾向而闻名。深度伪造技术利用生成对抗网络（GAN）等深度学习模型创建逼真但虚假的图像或视频；若被滥用，可产生非自愿的色情化内容。此案反映了对 AI 安全的持续担忧，以及监管大型平台上用户生成的滥用内容的挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Grok_(chatbot)">Grok (chatbot)</a></li>
<li><a href="https://grok.com/">Grok</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#deepfakes`, `#legal`, `#child safety`, `#ethics`

---