---
layout: default
title: "Horizon Summary: 2026-08-05 (ZH)"
date: 2026-08-05
lang: zh
---

> 从 39 条内容中筛选出 12 条重要资讯。

---

1. [Keyv 及其依赖包在 Shai-Hulud npm 供应链攻击中沦陷](#item-1) ⭐️ 9.0/10
2. [华为发表“韬定律”：以时间缩微替代几何缩微](#item-2) ⭐️ 9.0/10
3. [中国首部 L3/L4 自动驾驶强制性国标报批，2027 年实施](#item-3) ⭐️ 9.0/10
4. [Gwern 退出全职写作与匿名身份，启动 AI 安全项目 Guardian Angel](#item-4) ⭐️ 8.0/10
5. [Mistral 发布 Shieldstral：3B 开放权重多模态审核模型](#item-5) ⭐️ 8.0/10
6. [自定义色彩空间与算法生成多样化肤色](#item-6) ⭐️ 8.0/10
7. [Waymo 在达拉斯全面开放自动驾驶打车服务](#item-7) ⭐️ 8.0/10
8. [Oxide Computer 完成 4.45 亿美元 D 轮融资](#item-8) ⭐️ 8.0/10
9. [Xbox 宕机导致光盘游戏无法运行，暴露 DRM 脆弱性](#item-9) ⭐️ 8.0/10
10. [LLM 0.32 新增推理轨迹、服务端工具及 OpenAI Responses API 支持](#item-10) ⭐️ 8.0/10
11. [MiniMax-H3 全模态模型现可通过 MLX 在苹果芯片上本地运行](#item-11) ⭐️ 8.0/10
12. [谷歌为 Anthropic 搭建 2000 亿美元华尔街融资机器](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Keyv 及其依赖包在 Shai-Hulud npm 供应链攻击中沦陷](https://www.aikido.dev/blog/keyv-and-friends-compromised-in-npm-supply-chain-attack) ⭐️ 9.0/10

据 CISA 和安全厂商的警报，自复制的 Shai-Hulud 蠕虫已攻陷流行的 npm 包 Keyv 及其依赖包。该攻击正在持续，已波及 npm 注册表中的 500 多个包。 Keyv 是广泛使用的键值存储库，因此此次攻陷使大量 JavaScript 项目面临风险。它突显了 npm 依赖链的系统性脆弱性，并加强了限制自动安装脚本的呼声。 该蠕虫通过安装包时自动运行的 pre-install 钩子进行传播，并可窃取凭据、部署更多负载。Keyv 被攻陷尤其值得注意，因为它是许多其他包的依赖，放大了攻击影响范围。

hackernews · cimi_ · 8月4日 11:01 · [社区讨论](https://news.ycombinator.com/item?id=49166874)

**背景**: npm 是 JavaScript 的默认包注册表，项目依赖于成百上千个传递依赖。供应链攻击瞄准上游包，在开发者机器上植入恶意代码。pre-install 和 post-install 钩子是在安装时自动运行的 npm 生命周期脚本，当安装被攻陷的包版本时，它们为攻击者提供了入口点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cisa.gov/news-events/alerts/2025/09/23/widespread-supply-chain-compromise-impacting-npm-ecosystem">Widespread Supply Chain Compromise Impacting npm Ecosystem | CISA</a></li>
<li><a href="https://unit42.paloaltonetworks.com/npm-supply-chain-attack/">"Shai-Hulud" Worm Compromises npm Ecosystem in Supply Chain Attack (Updated November 26)</a></li>
<li><a href="https://www.trendmicro.com/en_us/research/25/i/npm-supply-chain-attack.html">What We Know About the NPM Supply Chain Attack | Trend Micro (US)</a></li>

</ul>
</details>

**社区讨论**: 评论者对此感到震惊，认为任何以前没有、现在突然出现的 pre-install 钩子都应受到极度怀疑，有人呼吁暂停新的钩子。其他人建议采用实际缓解措施，如一致使用 devcontainers 来隔离安装环境，或用 Packj 等工具扫描依赖项；还有人询问是否可以用 grep 命令在 node_modules 或 pnpm store 中检测受感染文件。

**标签**: `#supply chain`, `#security`, `#npm`, `#open source`, `#malware`

---

<a id="item-2"></a>
## [华为发表“韬定律”：以时间缩微替代几何缩微](https://t.me/zaihuapd/42966) ⭐️ 9.0/10

2026 年 5 月 25 日在上海举行的 2026 国际电路与系统研讨会上，华为正式发表“韬（τ）定律”，提出以“时间缩微”替代传统“几何缩微”。华为还宣布，今年秋季将发布完整采用逻辑折叠技术的新麒麟手机芯片。 这是中国在全球半导体领域首次提出指导产业发展的新原则，在摩尔定律逼近物理极限之际提供了一条潜在替代路径。该公告可能重塑半导体生态系统；消息公布后，A 股芯片产业链普遍走高，多只个股涨停。 华为表示，过去六年已基于韬（τ）定律设计并量产了 381 款芯片。预计到 2031 年，基于该定律的高端芯片晶体管密度有望达到 1.4 纳米制程的同等水平；逻辑折叠技术采用晶圆对晶圆混合键合与背面 TSV 技术，在不扩大封装尺寸的情况下提升有效晶体管密度。

telegram · zaihuapd · 8月4日 08:04

**背景**: 摩尔定律传统上预测晶体管密度大约每两年翻一番，其驱动力是特征尺寸的几何缩微。随着这一路径逼近物理极限，华为的韬（τ）定律转而定义器件、电路、芯片和系统各层级的特征时间常数，并以缩短这些时间常数作为统一优化目标。逻辑折叠是伴随该定律提出的设计方法论，通过在时间或空间维度复用硬件资源，在不依赖先进光刻的情况下协同优化性能、功耗与面积。

<details><summary>参考链接</summary>
<ul>
<li><a href="http://www.news.cn/tech/20260526/75603364bbae42bab67933d63d63e373/c.html">华为推出“韬定律” 改写全球半导体规则-新华网</a></li>
<li><a href="http://finance.people.com.cn/n1/2026/0525/c1004-40726802.html">华为正式发表半导体领域新定律--经济·科技--人民网</a></li>
<li><a href="https://www.eet-china.com/news/202605285809.html">华为麒麟首席架构师：“逻辑折叠”的四大挑战-电子工程专辑</a></li>

</ul>
</details>

**标签**: `#半导体`, `#芯片设计`, `#摩尔定律`, `#华为`, `#时间缩放`

---

<a id="item-3"></a>
## [中国首部 L3/L4 自动驾驶强制性国标报批，2027 年实施](https://t.me/zaihuapd/42972) ⭐️ 9.0/10

工信部已完成《智能网联汽车自动驾驶系统安全要求》强制性国家标准报批稿，并于 6 月 17 日起公示，建议 2027 年 7 月 1 日实施。这是中国首部针对 L3 和 L4 级自动驾驶的强制性国家标准。 该标准标志着监管从“概念松绑”转向“安全硬约束”，引入 Safety Case 安全档案机制，并对 L3 人机交接和 L4 系统自主风险处置分别提出要求。这将迫使车企以系统性安全论证取代过去的模糊宣传，对行业影响深远。 该标准适用于搭载 L3、L4 级系统的 M 类和 N 类车辆，但不适用于自动泊车系统。对于 L3 级系统，要求具备驾驶人接管能力监测功能，例如通过至少两种有效指标（眼部运动、头部运动、特定人机交互动作等）确认驾驶人在过去 30 秒内具备执行动态驾驶任务的能力。

telegram · zaihuapd · 8月4日 13:06

**背景**: L3 级自动驾驶允许系统在特定条件下接管驾驶，但当系统请求接管时仍需驾驶员接管，因此需要持续监测驾驶员状态以确认其具备接管能力。L4 级系统则需自主应对风险，无需驾驶员干预。Safety Case 是一种结构化的安全论证方法，通过“声明—论据—证据”体系来证明安全性，此前在航空航天、核工业等安全关键领域广泛应用，现在成为中国自动驾驶强制性国家标准的核心要求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.autohome.com.cn/news/202608/1316205.html">autohome.com.cn/news/202608/1316205.html</a></li>
<li><a href="https://www.163.com/dy/article/L01347E80547KOTE.html">163.com/dy/article/L01347E80547KOTE.html</a></li>

</ul>
</details>

**标签**: `#autonomous-driving`, `#L3/L4`, `#regulation`, `#China`, `#safety-standard`

---

<a id="item-4"></a>
## [Gwern 退出全职写作与匿名身份，启动 AI 安全项目 Guardian Angel](https://twitter.com/gwern/status/2084739205071343837) ⭐️ 8.0/10

Gwern 宣布退出全职写作和匿名身份，转而启动一项名为 Guardian Angel 的新 AI 安全计划，相关细节发布在他的网站上。这一公告发布在 Twitter 上，并引发了大量社区讨论。 Gwern 是一位受人尊敬的匿名 AI 研究者，早期曾预测了大语言模型（LLM）的扩展趋势，因此他的这一举动表明 AI 安全在社区中日益受到关注。它也凸显了独立研究者转向安全导向项目的趋势，尤其是在智能体 LLM 逐步成为现实之际。 gwern.net 上的 Guardian Angel 页面包含一篇详细文章，评论中引用了其中对聊天机器人角色‘与用户深度错位、与所有者一致’的批评。部分评论者认为该项目将 LLM 描绘成‘类神’的存在，另一些人则质疑其对‘生产力’这一指标的过度强调。

hackernews · mattsterett · 8月4日 20:48 · [社区讨论](https://news.ycombinator.com/item?id=49174900)

**背景**: Gwern Branwen 是一位匿名 AI 研究者和写作者，以其在 gwern.net 上的博客闻名，撰写了大量关于智能、缩放规律和技术的文章。他是最早预见大语言模型扩展趋势及其对 AGI 时间线影响的人之一。他决定放弃匿名身份，意味着此后他将以真实身份公开工作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://biztoc.com/x/9eb04436b0a8d12f">Q&A with pseudonymous AI researcher Gwern Branwen on...</a></li>
<li><a href="https://sleonproductions.com/qa-with-pseudonymous-ai-researcher-gwern-branwen-on-anonymity-the-grand-theory-of-intelligence-seeing-llm-scaling-early-agi-timelines-blogging-and-more/">Q&A with pseudonymous AI researcher Gwern Branwen on...</a></li>

</ul>
</details>

**社区讨论**: 社区反应褒贬不一：有人表示支持，并称赞 Gwern 的为人和正直；也有人持怀疑态度，称该项目是一种‘狂热’，并质疑其以生产力为中心的理念。批评点包括夸大 LLM 能力的风险，以及生产力与自我实现之间的紧张关系。

**标签**: `#AI safety`, `#AI alignment`, `#Gwern`, `#LLM`, `#Announcement`

---

<a id="item-5"></a>
## [Mistral 发布 Shieldstral：3B 开放权重多模态审核模型](https://mistral.ai/news/shieldstral/) ⭐️ 8.0/10

Mistral 发布了 Shieldstral，一个 3B 参数的开放权重多模态审核模型，可通过基于提示词的策略指令进行定制。该模型已上线 Hugging Face，旨在为内容过滤提供轻量且高性价比的选项。 内容审核是 UGC 平台面临的一大难题，而一个如此体量的开放权重模型允许开发者自托管审核功能，无需依赖昂贵的封闭 API。此次发布也体现了 Mistral 的战略：聚焦更小的专用微调模型，而非仅仅与前沿大模型竞争。 该模型在 Hugging Face 上以 mistralai/Shieldstral-1.0-3B 发布。'开放权重'意味着训练后的参数公开，但不一定包含训练数据和代码；基于提示词的策略无需重新训练即可定制，不过其在真实世界边界案例上的健壮性仍有待充分验证。

hackernews · riadsila · 8月4日 16:36 · [社区讨论](https://news.ycombinator.com/item?id=49171268)

**背景**: 多模态内容审核会自动分析文本、图片、音频和视频，以识别违反政策的内容。模型权重本质上是决定模型行为的学习参数；开放权重模型公开这些参数，使其他人可以在本地运行。Mistral 的 Shieldstral 基于紧凑的 3B 主干模型构建，旨在低成本处理审核任务，并通过提示词允许针对不同平台的策略调整。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.inc.com/ben-sherry/openais-new-open-weight-model-could-be-huge-for-governments-and-banks/91169920">OpenAI Has a New Open - Weight Model . Here's What That Means</a></li>
<li><a href="https://www.emergentmind.com/topics/multimodal-content-moderation">Multimodal Content Moderation</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍欢迎这种小模型策略，认为它是内容审核中现实且高性价比的解决方案。也有人质疑：基于提示词的策略能否超越简单的二元规则进行灵活调整；一位试用过演示的用户认为它在基本场景下可行，但对边界情况仍持怀疑态度。

**标签**: `#AI`, `#open-source`, `#content-moderation`, `#Mistral`, `#multimodal`

---

<a id="item-6"></a>
## [自定义色彩空间与算法生成多样化肤色](https://toneyalexander.github.io/inclusive-color-space/) ⭐️ 8.0/10

一位开发者创建了自定义色彩空间和程序化生成算法，让数字艺术和游戏开发中更容易选取多样化且逼真的肤色。该项目发布在 Hacker News，包含一个 JavaScript 取色器和 Python 示例算法。 这一项目意义重大，因为包容性的角色创建和数字艺术经常缺乏易用的工具来选取广泛的肤色。该项目实用的方法以及社区的热烈反响（468 分、88 条评论）可能会鼓励创意软件中出现更多包容性的色彩工具。 该色彩空间基于 PCA 得到的 U 空间向量和椭圆构建，并手工拟合了函数；作者承认方法偏向启发式而非严格科学。页面还提供 Python 版程序化生成算法（源码中有 JS 版），并包含“未来工作”部分。

hackernews · automatoney · 8月4日 15:16 · [社区讨论](https://news.ycombinator.com/item?id=49170165)

**背景**: 肤色建模众所周知地困难，因为它不仅是物理量，还涉及人类感知、光照及其他环境因素。程序化生成是一种通过算法（通常结合随机性与约束）而非手动方式创建数据的方法。该项目尝试定义一个专用的“够用”色彩空间，以简化生成逼真肤色的过程；讨论中还引用了 Pantone SkinTones、Oklab 色彩空间，以及“在最高饱和度下，任何种族的肤色都会呈现橙色”的观察。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://toneyalexander.github.io/inclusive-color-space/">What Colors Are We? Constructing A Color Space For Skin Tones</a></li>
<li><a href="https://en.wikipedia.org/wiki/Procedural_generation">Procedural generation - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 整体氛围积极：评论者称赞了这个想法、手工拟合函数的方法和视觉效果，还有人通过观察 Oklab 中肤色也呈相同月牙形分布来佐证其合理性。也有评论指出缺少对 Pantone SkinTones 等已有工作的引用，一位评论者还提到调色板中出现了绿色、蓝色和紫色。

**标签**: `#color space`, `#skin tones`, `#procedural generation`, `#digital art`, `#algorithm`

---

<a id="item-7"></a>
## [Waymo 在达拉斯全面开放自动驾驶打车服务](https://waymo.com/blog/shorts/dallas-open-to-all/) ⭐️ 8.0/10

Waymo 已向达拉斯所有用户开放其自动驾驶打车服务，使该市成为其最新的全面公开机器人出租车市场。此次扩张超越了等候名单和试点项目，服务区域内的任何人都可以呼叫无人驾驶车辆。 这标志着自动驾驶汽车在美国主要城市规模化落地的一个重要里程碑，对城市交通、安全监管和机器人出租车竞争格局都有影响。达拉斯独特的城市蔓延结构将考验无人驾驶技术在非“单中心辐射”城市布局中的适应能力。 达拉斯的大都市布局与 Waymo 其他得克萨斯州市场不同：奥斯汀、休斯顿和圣安东尼奥是“单中心辐射”型城市，而达拉斯则是围绕达拉斯-沃斯堡走廊发展的。评论者还提到，Waymo 此前在纽约市的试点项目据称显示其系统比人类驾驶员更危险，不过这属于轶事性信息。

hackernews · xnx · 8月4日 18:29 · [社区讨论](https://news.ycombinator.com/item?id=49172836)

**背景**: Waymo 前身为 Google 自动驾驶汽车项目，开发 L4 级自动驾驶技术，并在美国多个城市运营机器人出租车服务。L4 级自动化意味着车辆在限定的设计运行域内无需人工干预即可完成所有驾驶任务，但实现全场景完全自动驾驶（L5 级）尚未达成。公众对此类车辆的看法仍然复杂，安全、监管和城市规划方面的担忧持续影响着其部署。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://waymo.com/">Waymo - Self- Driving Cars - Autonomous Vehicles - Ride-Hail</a></li>
<li><a href="https://en.wikipedia.org/wiki/Self-driving_car">Self- driving car - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 讨论大体上是积极的，但也有不少保留意见：一些评论者称赞 Waymo 的驾驶行为和可预测性，另一些人则指出达拉斯独特的城市形态、扩大服务区域的需求，以及据报道 Waymo 在纽约试点中比人类驾驶员更危险的情况。一位评论者甚至认为无人驾驶汽车可以成为有效的经济适用房政策，引发了更广泛的城市规划视角。

**标签**: `#autonomous vehicles`, `#Waymo`, `#urban mobility`, `#safety`, `#policy`

---

<a id="item-8"></a>
## [Oxide Computer 完成 4.45 亿美元 D 轮融资](https://www.sec.gov/Archives/edgar/data/1795071/000179507126000002/xslFormDX01/primary_doc.xml) ⭐️ 8.0/10

根据美国证券交易委员会（SEC）的 Form D 文件，Oxide Computer 已完成 4.45 亿美元的 D 轮融资。此前该公司还完成了 1 亿美元的 B 轮和 2 亿美元的 C 轮融资。 这是基础设施创业公司规模最大的融资之一，表明投资者对机架规模系统作为传统云基础设施替代方案的信心很强。这笔资金可能帮助 Oxide 扩大市场推广和客户采用。 这笔融资通过 SEC Form D 文件披露，其中关于估值和投资者的信息有限。Oxide 构建的机架规模系统将计算、存储和网络集成到单一产品中，但一些社区成员质疑该公司是否已向客户交付硬件。

hackernews · depr · 8月4日 20:13 · [社区讨论](https://news.ycombinator.com/item?id=49174407)

**背景**: 机架规模系统是一种将整个数据中心机架作为单一集成产品出售的方案，通常配备机架内互联网络，并由单一操作系统管理整个机架。与分别组装服务器、存储和网络设备相比，这种方法简化了部署和管理。Oxide Computer 正是采用这种设计的初创公司之一，旨在提供具有云级敏捷性的本地基础设施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pantheon.run/learn/gpu-vs-server-vs-rack">GPU vs Server vs Rack : What You Actually Buy | Pantheon</a></li>
<li><a href="https://drops.dagstuhl.de/storage/04dagstuhl-reports/volume05/issue10/15421/DagRep.5.10.35/DagRep.5.10.35.pdf">Rack - scale Computing</a></li>

</ul>
</details>

**社区讨论**: 社区情绪总体积极，对 Oxide 的产品概念感到兴奋，有人对 Jessie Frazelle 等关键技术人物的能力表示信任。但也有批评声音指出销售响应不佳——一位工程副总裁表示其销售请求从未得到回复——以及缺乏实际向客户发货硬件的可见证据。

**标签**: `#Oxide Computer`, `#funding`, `#hardware`, `#cloud infrastructure`, `#systems`

---

<a id="item-9"></a>
## [Xbox 宕机导致光盘游戏无法运行，暴露 DRM 脆弱性](https://birchtree.me/blog/xbox-goes-down-you-cant-play-games-you-own-on-disc/) ⭐️ 8.0/10

在最近一次 Xbox 宕机中，玩家发现即使是拥有实体光盘的游戏也需要在线验证才能启动，导致游戏无法游玩。这一事件表明，所谓的“实体”游戏仍然依赖微软服务器来确认所有权。 此事关系重大，因为它触及了数字所有权争论的核心，表明在当前 DRM 实践下，消费者从未真正拥有自己购买的游戏。这会影响所有重视长期可玩性、二手交易和离线游戏的玩家，也可能促使监管机构或消费者要求更好的消费者权益保障。 此次宕机中断了即使插入光盘也需要的在线许可证验证，导致光盘在没有服务器批准的情况下沦为一把物理钥匙。Xbox Series S 是纯数字主机，但使用光盘游戏的 Series X 和 One 用户同样遇到了问题，这凸显了云端依赖凌驾于本地所有权的设计。

hackernews · surprisetalk · 8月4日 12:01 · [社区讨论](https://news.ycombinator.com/item?id=49167448)

**背景**: 数字版权管理（DRM）是指限制数字内容使用方式的访问控制技术，通常需要在线认证来确认购买行为。包括 Xbox 在内的许多现代主机甚至对实体光盘也强制实施 DRM，将光盘视为必须与服务器校验的许可证。这种做法把游戏从产品变成了服务，使其容易受到宕机和服务器关闭的影响。对此类政策的抵制加剧了关于消费者是否真正拥有所购媒体的广泛争论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Digital_rights_management">Digital rights management - Wikipedia</a></li>
<li><a href="https://www.pcgamingwiki.com/wiki/Digital_rights_management_(DRM)">Digital rights management ( DRM ) - PCGamingWiki PCGW - bugs...</a></li>
<li><a href="https://www.xbox.com/en-US/games/backward-compatibility">XBOX Backward Compatible Games | XBOX</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了沮丧和怀旧之情，一些人分享了个人 DRM 失败的经历，例如 Steam 版《光环》意外要求微软账号登录。有人认为核心问题是所有权，而非实体版与数字版之争，并列出了消费者应拥有的权利，包括永久访问、离线游玩、二手转售以及将游戏传给后代。还有人指出 PS3 等老主机支持局域网和离线游戏，认为现代在线强制要求是一种倒退。

**标签**: `#DRM`, `#digital ownership`, `#Xbox`, `#gaming`, `#cloud dependency`

---

<a id="item-10"></a>
## [LLM 0.32 新增推理轨迹、服务端工具及 OpenAI Responses API 支持](https://simonwillison.net/2026/Aug/4/new-release-of-llm/#atom-everything) ⭐️ 8.0/10

LLM 0.32 是自该工具发布以来最重要的版本，新增了可视化推理轨迹、服务端提供商工具、重新设计的 SQLite 日志，并支持 OpenAI Responses API。该版本还引入了 GPT-5.6 模型系列，以 GPT-5.6 Luna 作为新的默认模型，并新增了 llm openai endpoint 命令。 此版本通过让推理过程可见、支持直接从 CLI 使用代码执行和网页搜索等服务端工具，并扩展对 OpenAI 新 API 的兼容性，显著提升了开发者体验。这巩固了 LLM 在基于 CLI 的 AI 工作流和智能体应用生态中的重要地位。 推理轨迹输出到 stderr，可使用 -R/--hide-reasoning 标志隐藏。服务端工具包括 OpenAI 的 CodeInterpreter 和 WebSearch，而 llm-anthropic 插件新增了 WebSearch、WebFetch、CodeExecution 和 AnthropicMCP；新的 llm openai endpoint 命令可运行一次性提示词，且不会记录日志。

rss · Simon Willison · 8月4日 23:58

**背景**: LLM 是 Simon Willison 开发的一个命令行工具，允许用户对多种大语言模型运行提示词，并将提示词和响应存储在 SQLite 中。OpenAI Responses API 于 2025 年 3 月发布，是一个面向开发者的接口，旨在通过将聊天补全与高级工具调用能力相结合来构建智能体应用。推理轨迹是模型的中间推理步骤，常被称为“展示其思考过程”，之前是隐藏的，现在被显示出来以供调试和透明化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/simonw/llm">simonw/ llm : Access large language models from the command - line ...</a></li>
<li><a href="https://developers.openai.com/api/reference/responses/overview">Responses Overview | OpenAI API Reference</a></li>

</ul>
</details>

**标签**: `#LLM`, `#OpenAI`, `#release`, `#CLI`, `#SQLite`

---

<a id="item-11"></a>
## [MiniMax-H3 全模态模型现可通过 MLX 在苹果芯片上本地运行](https://simonwillison.net/2026/Aug/4/minimax-h3-mlx/#atom-everything) ⭐️ 8.0/10

Simon Willison 报道了他通过新的 PipeNetwork/minimax-h3-mlx 包，在 M5 Max MacBook Pro 上运行 MiniMax 的全模态生成模型 MiniMax-H3。该模型可以根据文本、图像、音频和视频输入，生成最长 15 秒、含音频的视频片段。 这表明最先进的全模态模型可以在消费级 Apple Silicon 硬件上本地运行，而不仅限于云端。这为研究人员和开发者打开了大门，让他们无需依赖 API 服务即可尝试视频生成和多模态理解。 模型文件总计约 115 GB，在 Willison 的机器上生成一个视频片段耗时不到 45 分钟。他指出，由于没有按照 MiniMax 的提示词指南操作，生成的音频是“类似语音的奇怪垃圾内容”，该指南提供了控制音频输出的建议。

rss · Simon Willison · 8月4日 19:10

**背景**: MiniMax-H3 是 MiniMax 发布的一个通用全模态生成系统，能够在统一模型中理解和生成文本、图像、音频和视频。MLX 是苹果的开源数组框架，专为在 Apple Silicon 上高效运行机器学习而设计，利用了统一内存架构。PipeNetwork/minimax-h3-mlx 包将 MiniMax-H3 移植到 MLX，使其能够在 Mac 上本地运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.minimax.io/blog/minimax-h3">MiniMax H3: An Open Model Breaking the Boundaries Between Tasks and Modalities - MiniMax Research | MiniMax</a></li>
<li><a href="https://huggingface.co/MiniMaxAI/MiniMax-H3">MiniMaxAI/MiniMax-H3 · Hugging Face</a></li>
<li><a href="https://www.marktechpost.com/2026/08/01/minimax-releases-minimax-h3-an-omni-modal-video-model-that-generates-15-second-2k-clips-with-native-stereo-audio/">MiniMax Releases MiniMax H3: An Omni-Modal Video Model That Generates 15-Second 2K Clips With Native Stereo Audio - MarkTechPost</a></li>

</ul>
</details>

**标签**: `#AI`, `#MLX`, `#MiniMax-H3`, `#video generation`, `#multimodal`

---

<a id="item-12"></a>
## [谷歌为 Anthropic 搭建 2000 亿美元华尔街融资机器](https://www.ft.com/content/549f2e23-5aa2-49c7-9ea6-a9784ab7087c) ⭐️ 8.0/10

《金融时报》8 月 4 日报道，谷歌已悄然搭建史上规模最大的基础设施融资架构之一，合同总额约 2000 亿美元，用于向 Anthropic 交付超 1500 亿美元 AI 芯片。名为 Compute SPV 的特殊目的载体已于 6 月完成首批交易，购入约 350 亿美元硬件，相当于约 1 吉瓦算力、100 万颗 TPU。 这标志着 AI 基础设施融资模式的范式转变，风险由谷歌、博通、阿波罗、黑石、摩根士丹利及加密矿企共同分担，避免任何一方单独承担数百亿美元 AI 硬件的资产负债表压力。该结构可能成为云厂商和 AI 初创公司为大规模芯片部署融资的模板，直接影响 AI 算力供应链与云经济。 由于 Anthropic 没有信用评级，该安排要求各方分担风险：谷歌为数据中心提供担保，博通购买并协助融资芯片，阿波罗与黑石购买硬件后回租给 Anthropic。该模式借鉴波音和 GE 推销飞机与发动机的厂商融资玩法，让各方都不必把数百亿美元 AI 硬件压在自家资产负债表上。

telegram · zaihuapd · 8月4日 10:52

**背景**: 张量处理单元（TPU）是谷歌自研的专用集成电路（ASIC），用于加速机器学习工作负载，是 Anthropic 云端算力的基础硬件。特殊目的载体（SPV）是为单一目标设立的独立法律实体，在基础设施融资中常见，用于汇集多方资本并隔离风险。厂商融资（vendor financing）是指设备供应商将技术与融资打包，通过租赁等结构帮助企业客户避免将大额采购直接计入资产负债表。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://jonathan-hui.medium.com/ai-chips-tpu-3fa0b2451a2d">AI Chips: Google TPU . Google ’s chip designers argue that the | Medium</a></li>
<li><a href="https://www.allocations.com/blog/special-purpose-vehicle-(spv)-what-it-is-and-why-investors-use-it">Special Purpose Vehicle ( SPV ): What It Is and Why... - Allocations</a></li>
<li><a href="https://www.lenovo.com/us/en/knowledgebase/business-it-financing-a-comprehensive-guide/">Business IT Financing : A Comprehensive Guide | Lenovo US</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#Google`, `#Anthropic`, `#Financing`, `#TPU`

---