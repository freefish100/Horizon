---
layout: default
title: "Horizon Summary: 2026-07-04 (ZH)"
date: 2026-07-04
lang: zh
---

> 从 47 条内容中筛选出 10 条重要资讯。

---

1. [欧洲议会间谍软件调查人员遭飞马间谍软件攻击](#item-1) ⭐️ 9.0/10
2. [CDD 仅从 Logits 恢复 LLM 微调数据](#item-2) ⭐️ 9.0/10
3. [腾讯玄武实验室阿图因 AI 在 CyberGym 测试中超越 Mythos](#item-3) ⭐️ 9.0/10
4. [本地运行顶级大模型指南揭示高昂成本](#item-4) ⭐️ 8.0/10
5. [PostgreSQL 严格内存过量使用避免 OOM 杀手](#item-5) ⭐️ 8.0/10
6. [Current AI 发布开源 AI 差距地图](#item-6) ⭐️ 8.0/10
7. [Anthropic 指控阿里巴巴对 Claude 发动大规模蒸馏攻击](#item-7) ⭐️ 8.0/10
8. [Claude Fable 5 重新上线，性能缩水安全误判令开发者不满](#item-8) ⭐️ 8.0/10
9. [华为 Mate 80 Pro 游戏能效超越骁龙 8 Gen3](#item-9) ⭐️ 8.0/10
10. [NASA 发射私人救援任务拯救老化的 Swift 望远镜](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [欧洲议会间谍软件调查人员遭飞马间谍软件攻击](https://citizenlab.ca/research/member-of-committee-investigating-spyware-hacked-with-pegasus/) ⭐️ 9.0/10

公民实验室确认，欧洲议会议员斯特利奥斯·库洛格卢的 iPhone 在 2022 年 10 月和 2023 年 3 月感染了飞马间谍软件，当时他正在调查非法间谍软件。感染被高度可信地检测到。 这是首次确认在任欧盟议员成为国家支持的间谍软件目标，破坏了民主监督，并引发了对欧盟成员国跨境监控的严重担忧。这凸显了监控工具被滥用于针对民选代表的情况。 首次感染与一起针对欧洲流亡记者的已知飞马行动重叠，表明一个获得授权在多个欧洲国家进行监控的单一飞马客户是幕后黑手。感染发生在 2022 年 10 月 21 日和 2023 年 3 月 6 日至 7 日。

hackernews · ledoge · 7月3日 20:38 · [社区讨论](https://news.ycombinator.com/item?id=48779683)

**背景**: 飞马是以色列 NSO 集团开发的一款强大间谍软件，能够远程零点击安装并从移动设备中大量提取数据。公民实验室是多伦多大学的一个研究小组，专门调查数字威胁，并揭露了政府针对记者、活动人士和政治对手的多次飞马滥用行为。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pegasus_(spyware)">Pegasus (spyware)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Citizen_Lab">Citizen Lab</a></li>

</ul>
</details>

**社区讨论**: 评论者对仅将攻击归咎于某个欧盟国家表示怀疑，理由是希腊和波兰已知的间谍软件滥用情况。一些人指出欧盟议员被成员国监控的讽刺之处，而另一些人则质疑欧盟官员缺乏设备分离政策。

**标签**: `#cybersecurity`, `#Pegasus`, `#surveillance`, `#espionage`, `#European Parliament`

---

<a id="item-2"></a>
## [CDD 仅从 Logits 恢复 LLM 微调数据](https://www.reddit.com/r/MachineLearning/comments/1umn2dk/contrastive_decoding_diffing_cdd_recovering/) ⭐️ 9.0/10

对比解码差分（CDD）是一种新的灰盒方法，仅使用 logit 输出即可从大型语言模型中恢复逐字微调数据，无需模型权重、激活或探测语料库。在 SDF 基准测试中，它在四个模型家族（1B 到 32B 参数）的 20 个生物×模型对中的 19 个上达到了 4+/5 的逐字恢复分数，优于白盒激活差异透镜（ADL），后者从未超过 3/5。 这项工作意义重大，因为它表明只需最低限度的访问权限即可从 LLM 中提取敏感的微调数据，从而引发了模型部署中的重要隐私和安全问题。它还提供了一个强大的可解释性工具，使研究人员无需完全访问模型即可审计通过微调注入了哪些知识。 CDD 是一种灰盒方法，它对比基础模型及其微调版本的 logits，使用单一默认配置，无需针对每个生物体进行校准或层选择。一个意外的发现是，CDD 在多个语义无关的微调领域中恢复了虚构角色“Elena Rodriguez 博士”，这揭示了这个名字是由 Claude Sonnet 3.6 在合成数据生成中一致生成的。

reddit · r/MachineLearning · /u/CebulkaZapiekana · 7月3日 19:01

**背景**: 对比解码是一种通过比较强模型和弱模型的输出来改进文本生成的技术。激活差异透镜（ADL）是一种先前的白盒方法，它利用基础模型和微调模型之间的激活差异来引导生成，但它需要完整的权重访问，并且只能恢复模糊的领域级描述。CDD 是 ADL 的输出级类比，直接作用于 logits。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aclanthology.org/2023.acl-long.687/">Contrastive Decoding : Open-ended Text Generation... - ACL Anthology</a></li>
<li><a href="https://arxiv.org/html/2510.13900">Narrow Finetuning Leaves Clearly Readable Traces in Activation ...</a></li>
<li><a href="https://www.lesswrong.com/posts/mXuqpJkJpaeTjyCgm/latent-reasoning-sprint-3-activation-difference-steering-and-1">Latent Reasoning Sprint #3: Activation Difference ... — LessWrong</a></li>

</ul>
</details>

**标签**: `#LLM`, `#interpretability`, `#model diffing`, `#finetuning`, `#logits`

---

<a id="item-3"></a>
## [腾讯玄武实验室阿图因 AI 在 CyberGym 测试中超越 Mythos](https://mp.weixin.qq.com/s/BzU7g-2iG7d6h4ViwMhxyg) ⭐️ 9.0/10

腾讯玄武实验室基于开源模型 GLM-5.1 构建的阿图因 AI 在 CyberGym 网络安全基准测试中获得 84.0% 的分数，超越了 Anthropic 的 Claude Mythos Preview。阿图因 AI 在 curl、OpenSSL 等项目中发现了多个 Mythos 未检出的高危逻辑漏洞，且消耗的预算不到 Mythos 的 0.1%。 这一突破表明，经济高效的开源模型能够在实际漏洞检测中超越主流商业系统，有望推动高级网络安全 AI 的普及。它凸显了开源大语言模型在专业技术领域中日益增强的效力。 阿图因 AI 在 curl、gnark、OpenSSL、Python cryptography 和 Java bc-java 等项目中发现了严重程度高达 9.3 的漏洞。在伯克利 BVI 真实世界漏洞榜单中，阿图因 AI 的严重漏洞严重程度排名第 1，总数排名第 5。

telegram · zaihuapd · 7月3日 16:12

**背景**: CyberGym 是由加州大学伯克利分校开发的大规模高质量网络安全评估框架，包含 188 个开源项目中的 1507 个真实世界漏洞，旨在严格评估 AI 代理在漏洞分析中的能力。GLM-5.1 是 Z.AI 的旗舰开源大语言模型，针对代理工作流和长序列推理任务进行了优化，能够自主处理单一任务长达 8 小时。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/sunblaze-ucb/cybergym">GitHub - sunblaze-ucb/cybergym: CyberGym is a large-scale, high-quality cybersecurity evaluation framework designed to rigorously assess the capabilities of AI agents on real-world vulnerability analysis tasks. · GitHub</a></li>
<li><a href="https://huggingface.co/zai-org/GLM-5.1">zai-org/GLM-5.1 · Hugging Face</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#AI`, `#benchmark`, `#vulnerability detection`, `#open-source model`

---

<a id="item-4"></a>
## [本地运行顶级大模型指南揭示高昂成本](https://github.com/jamesob/local-llm) ⭐️ 8.0/10

Jamesob 发布的本地运行顶级大模型指南显示，搭建所需硬件成本超过 5 万美元，引发社区对本地推理实用性和成本效益的讨论。 这突显了本地部署大模型的极端经济和技​​术门槛，降低了人们对在本地运行顶级模型的热情，并强化了云订阅服务对大多数用户的价值。 该指南中 4 万美元的预算实际需 5 万至 5.5 万美元，包含四块单价 1.2 万美元的 GPU，并依赖量化技术（如 REAP 剪枝的 GLM-5.2 配合 Int8-mix NVFP4 量化），可能影响实际性能。

hackernews · livestyle · 7月3日 15:03 · [社区讨论](https://news.ycombinator.com/item?id=48775921)

**背景**: 本地运行大语言模型需要高端 GPU，其显存需足够容纳模型权重。量化技术通过降低精度使模型适配内存，但可能影响输出质量。云订阅服务（如 ChatGPT 或 Claude）每月付费即可使用顶级模型，避免了高昂的硬件前期投入。

**社区讨论**: 评论者警告成本常被低估，有用户指出 4 万美元的配置实际需 5-5.5 万美元，相当于 16.8 年的 Claude Opus 订阅费。也有人提到 128GB 统一内存等替代方案可用于运行 DeepSeek V4，但总体观点是本地顶级模型仍然极其昂贵且质量低于云服务。

**标签**: `#local-LLM`, `#hardware`, `#cost-analysis`, `#AI-inference`

---

<a id="item-5"></a>
## [PostgreSQL 严格内存过量使用避免 OOM 杀手](https://www.ubicloud.com/blog/postgresql-and-the-oom-killer-why-we-use-strict-memory-overcommit) ⭐️ 8.0/10

Ubicloud 发布了一篇博客文章，解释了他们为何在 PostgreSQL 中使用严格内存过量使用模式（vm.overcommit_memory=2）来避免 Linux OOM 杀手终止数据库进程，这是基于大规模运营托管 Postgres 的经验。 这一点很重要，因为默认的 Linux 内存过量使用启发式策略可能在内存压力下触发 OOM 杀手杀死 PostgreSQL，导致停机。严格模式为数据库工作负载提供了更可预测的行为，但需要仔细调优以避免 fork 失败。 严格模式（vm.overcommit_memory=2）根据 swap + RAM * overcommit_ratio 设置 CommitLimit，并拒绝任何超出该限制的分配。这可以防止 OOM 杀手，但如果达到提交限制，可能会导致 fork() 等系统调用失败。

hackernews · furkansahin · 7月3日 13:00 · [社区讨论](https://news.ycombinator.com/item?id=48774509)

**背景**: Linux 默认允许内存过量使用，即进程可以分配超过物理 RAM 的虚拟内存。OOM 杀手是内核机制，在系统内存严重不足时终止进程。PostgreSQL 是内存密集型应用，在高负载或配置不当的情况下可能触发 OOM 杀手。可以通过 sysctl vm.overcommit_memory 更改过量使用策略：模式 0（启发式）、1（总是过量使用）或 2（严格）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ubicloud.com/blog/postgresql-and-the-oom-killer-why-we-use-strict-memory-overcommit">PostgreSQL and the OOM Killer: Why We Use Strict Memory Overcommit</a></li>
<li><a href="https://www.postgresql.org/docs/current/kernel-resources.html">PostgreSQL: Documentation: 18: 18.4. Managing Kernel Resources</a></li>
<li><a href="https://en.wikipedia.org/wiki/Out_of_memory">Out of memory - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区评论普遍赞同技术内容，但提醒注意副作用。一些用户报告严格模式在其环境中导致 fork 失败，尤其是结合过量使用比例时。博客作者 Ozgun 指出标题过于强烈，并承认严格模式可能不适合所有用例，例如与分配大量虚拟内存的应用程序混合工作负载的场景。

**标签**: `#postgresql`, `#linux`, `#memory-management`, `#database`, `#sysadmin`

---

<a id="item-6"></a>
## [Current AI 发布开源 AI 差距地图](https://simonwillison.net/2026/Jul/3/open-source-ai-gap-map/#atom-everything) ⭐️ 8.0/10

这份全面的地图提供了开源 AI 生态系统的结构化概览，帮助研究人员、开发者和资助者识别差距和机会，并可能影响该领域的战略投资和开发优先级。 该地图将产品划分为跨三个层（模型组件、产品/用户体验、基础设施）的 14 个类别，底层数据以 MIT 许可证在 GitHub 上发布，包含 1,184 个 YAML 文件和用于可重复性的脚本。

rss · Simon Willison · 7月3日 22:04

**背景**: Current AI 是一个旨在构建人工智能公共选项的全球合作伙伴关系，已承诺投入 4 亿美元。差距地图是系统化分类开源 AI 领域的努力，将其与专有 AI 开发区分开来。

**标签**: `#open source`, `#AI`, `#ecosystem map`, `#tools`, `#models`

---

<a id="item-7"></a>
## [Anthropic 指控阿里巴巴对 Claude 发动大规模蒸馏攻击](https://t.me/zaihuapd/42327) ⭐️ 8.0/10

Anthropic 正式指控阿里巴巴通过近 2.5 万个欺诈账户，在 2026 年 4 月 22 日至 6 月 5 日期间与 Claude AI 模型进行了超过 2880 万次交互，试图提取并复制其能力，发动了大规模“蒸馏攻击”。 这一事件凸显了人工智能领域工业间谍的新前沿，即竞争对手通过 API 访问窃取专有模型知识，威胁到投入巨资开发模型的前沿 AI 公司的商业模式。 Anthropic 通过其行为指纹和协调账户检测系统发现了此次攻击，并已与其他 AI 实验室、云服务提供商及当局共享技术指标。被指控方包括阿里巴巴及其 AI 实验室 Qwen。

telegram · zaihuapd · 7月3日 06:21

**背景**: 模型蒸馏是一种技术，通过 API 查询获取输入-输出对，让较弱的模型学习模仿较强模型的输出。当恶意使用时，就成为旨在未经授权克隆专有 AI 能力的“蒸馏攻击”。此类攻击对通过 API 访问实现商业化的 AI 公司构成生存威胁，可能削弱通过昂贵训练建立的竞争优势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/detecting-and-preventing-distillation-attacks">Detecting and preventing distillation attacks \ Anthropic</a></li>
<li><a href="https://medium.com/@tahirbalarabe2/understanding-llm-distillation-attacks-929306ca38cd">Understanding LLM Distillation Attacks | by Tahir | Medium</a></li>
<li><a href="https://cloud.google.com/blog/topics/threat-intelligence/distillation-experimentation-integration-ai-adversarial-use">GTIG AI Threat Tracker: Distillation, Experimentation, and (Continued) Integration of AI for Adversarial Use | Google Cloud Blog</a></li>

</ul>
</details>

**标签**: `#AI`, `#security`, `#distillation`, `#Anthropic`, `#Alibaba`

---

<a id="item-8"></a>
## [Claude Fable 5 重新上线，性能缩水安全误判令开发者不满](https://www.bleepingcomputer.com/news/artificial-intelligence/claude-fable-relaunch-disappoints-users-with-nerfed-performance/) ⭐️ 8.0/10

Anthropic 的 Claude Fable 5 模型在美国解除出口管制后重新上线，但用户报告性能大幅下降，安全误判频繁，尤其是在底层代码任务中。当遇到某些关键词时，模型会自动降级至 Opus 4.8。 这很重要，因为它影响了开发者对 Anthropic 旗舰模型的信任，并凸显了安全护栏与可用性之间的紧张关系。如果安全阈值过于激进，会阻碍生产力，并可能将用户推向其他模型。 Pro 和 Max 订阅用户对 Fable 5 的访问受限（7 月 7 日前仅 50%额度，之后按量付费）。安全护栏对“hook”或“vulnerability”等术语产生误判，触发回退至 Opus 4.8。模型底层性能未变，但护栏设置过于敏感。API 和企业按量付费版本仍可完整访问。

telegram · zaihuapd · 7月3日 07:20

**背景**: Anthropic 的 Claude 模型是先进的 AI 助手。安全护栏是防止有害输出的安全过滤器。Opus 4.8 是之前的模型。Fable 5 是旗舰模型。出口管制此前限制了其可用性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.implicator.ai/anthropics-965-billion-title-rests-on-a-model-built-to-flag-its-own-mistakes/">Anthropic Passes OpenAI at $965 Billion With Opus 4 . 8</a></li>
<li><a href="https://github.com/dialogoo/AI-Safety-Guardrails">GitHub - dialogoo/ AI - Safety - Guardrails : Production-ready, modular AI ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#Claude`, `#Model Performance`, `#Safety`, `#Developer Experience`

---

<a id="item-9"></a>
## [华为 Mate 80 Pro 游戏能效超越骁龙 8 Gen3](https://www.bilibili.com/video/BV1F7T46wEyT) ⭐️ 8.0/10

极客湾评测显示，搭载麒麟 9030 Pro 芯片并经过鸿蒙优化的华为 Mate 80 Pro 系列，在《原神》60 帧下整机功耗仅 4.9W，游戏能效优于骁龙 8 Gen3。 这表明华为的软硬芯云协同优化能够弥补理论性能差距，可能重塑移动芯片竞争格局，挑战高通在游戏能效方面的领先地位。 麒麟 9030 Pro 采用 9 核 14 线程 CPU 和 6 核马良 935 GPU，晶体管规模约 150 亿；其 CPU 多核能效介于骁龙 8 Gen2 与 8 Gen3 之间，但因鸿蒙原生应用优化，实际游戏表现超出纸面规格。

telegram · zaihuapd · 7月3日 13:27

**背景**: 麒麟 9030 是华为最新自研移动芯片，延续 Mate 系列集成先进 CPU 和 GPU 设计的传统。鸿蒙的“软硬芯云”协同优化利用原生应用和深度系统调优来提升效率。游戏能效衡量每瓦性能，对维持高帧率且不发热或耗电至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.mydrivers.com/1/1134/1134072.htm">华为Mate 80 Pro性能评测解禁！ 麒 麟 9030 Pro... | 快科技</a></li>
<li><a href="https://www.ithome.com/0/972/456.htm">华为 Mate 80 Pro 性能解禁：麒麟 9030 Pro GPU 相比 9020 提升 76...</a></li>
<li><a href="https://post.smzdm.com/p/a5rmxoex/">麒 麟 9030 Pro...</a></li>

</ul>
</details>

**标签**: `#Huawei`, `#Kirin 9030`, `#HarmonyOS`, `#mobile chipsets`, `#gaming efficiency`

---

<a id="item-10"></a>
## [NASA 发射私人救援任务拯救老化的 Swift 望远镜](https://apnews.com/article/swift-nasa-satellite-rescue-katalyst-a7ddd740ca099587c58865f583c7245a) ⭐️ 8.0/10

2026 年 7 月 3 日，NASA 发射了由 Katalyst Space Technologies 建造和运营的 LINK 航天器，旨在捕获并提升老化的 Swift 望远镜的轨道，防止其预计的失控再入。 此次任务标志着私人航天器首次尝试与未设计用于在轨服务的政府卫星对接并抬升其轨道，展示了减缓轨道碎片和延长卫星寿命的新能力。 LINK 将使用机械臂抓住 Swift 望远镜，然后通过推进器将其轨道抬升约 240 公里，Swift 可能最早在 9 月恢复观测。

telegram · zaihuapd · 7月3日 15:43

**背景**: Swift 望远镜于 2004 年发射，研究伽马射线暴及其他宇宙现象。由于太阳活动增加，其轨道持续下降。在轨卫星服务（OOS）此前仅限于政府任务；此次任务可能证明商业可行性。轨道高度降低时衰减加速，太阳活动使高层大气升温，增加阻力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LINK_spacecraft">LINK spacecraft</a></li>
<li><a href="https://en.wikipedia.org/wiki/Orbital_decay">Orbital decay - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/On-orbit_satellite_servicing">On-orbit satellite servicing</a></li>

</ul>
</details>

**标签**: `#space`, `#satellite rescue`, `#NASA`, `#orbital debris`

---