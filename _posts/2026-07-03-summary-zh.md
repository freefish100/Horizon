---
layout: default
title: "Horizon Summary: 2026-07-03 (ZH)"
date: 2026-07-03
lang: zh
---

> 从 36 条内容中筛选出 12 条重要资讯。

---

1. [Cloudflare 9 月起默认拦截 AI 爬虫，点名批评 Google](#item-1) ⭐️ 9.0/10
2. [弗吉尼亚州禁止出售地理定位数据](#item-2) ⭐️ 8.0/10
3. [美国隐私危机：Aaronson 呼吁行动](#item-3) ⭐️ 8.0/10
4. [Linux 6.9 回归：LUKS 暂停不再清除内存中的密钥](#item-4) ⭐️ 8.0/10
5. [Podman v6.0.0 发布，增强网络和 Quadlet 支持](#item-5) ⭐️ 8.0/10
6. [Immich 3.0 发布引发端到端加密争议](#item-6) ⭐️ 8.0/10
7. [理解才能参与：与 AI 协作的原则](#item-7) ⭐️ 8.0/10
8. [Meta 的 NeoCloud 雄心：扩展推荐系统与自研芯片](#item-8) ⭐️ 8.0/10
9. [ECTC 2026：EMIB-T、定制 HBM、HBM4、微流体冷却、光子互连](#item-9) ⭐️ 8.0/10
10. [OpenAI 提议美国政府持股 5%，或扩展至谷歌 Meta](#item-10) ⭐️ 8.0/10
11. [多公司因 AI 成本飙升限制员工使用](#item-11) ⭐️ 8.0/10
12. [Anthropic 自研 AI 芯片，与三星洽谈代工](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Cloudflare 9 月起默认拦截 AI 爬虫，点名批评 Google](https://techcrunch.com/2026/07/01/cloudflares-new-policy-pushes-ai-companies-to-pay-for-publishers-content/) ⭐️ 9.0/10

Cloudflare 宣布自 9 月 15 日起，默认阻止同时用于搜索索引和 AI 训练的'混合用途'爬虫，并点名批评 Google 利用搜索收录漏洞训练其 AI 模型。 这标志着网络政策的重大转变，可能迫使 AI 公司为使用网站内容向发布商付费，并可能重塑开放网络索引与专有 AI 训练之间的平衡。 新政策适用于使用 Cloudflare 服务且开启广告页面的发布商；允许搜索引擎收录的网站不再自动允许其内容用于 AI 训练。

telegram · zaihuapd · 7月2日 05:37

**背景**: Cloudflare 是一家领先的内容分发网络和安全服务提供商，保护网站免受恶意流量攻击。包括 Google 在内的一些 AI 公司使用网络爬虫收集数据来训练大型语言模型。此前，许多网站阻止了 AI 爬虫，但允许 Google 的搜索爬虫，无意中导致 Google 通过其搜索收录漏洞将网站内容用于 AI 训练。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/1982210831434412370">爬虫如何绕过Cloudflare？2025最实用的网页抓取解决方案 - 知乎</a></li>
<li><a href="https://developers.google.com/search/docs/fundamentals/ai-optimization-guide">Google's Guide to Optimizing for Generative AI Features on Google Search | Google Search Central | Documentation | Google for Developers</a></li>
<li><a href="https://www.bright.cn/blog/ai/scrape-google-ai-mode">如何抓取 Google AI 模式：完整指南与 API 方法</a></li>

</ul>
</details>

**标签**: `#Cloudflare`, `#AI爬虫`, `#Google`, `#内容付费`, `#网络政策`

---

<a id="item-2"></a>
## [弗吉尼亚州禁止出售地理定位数据](https://www.hunton.com/privacy-and-cybersecurity-law-blog/virginia-bans-sale-of-geolocation-data) ⭐️ 8.0/10

弗吉尼亚州通过了一项法律，禁止出售地理定位数据，这标志着州级隐私监管的重要一步。 这项法律可能为其他州树立先例，并解决了人们对位置数据被滥用的日益担忧，尤其是在堕胎广告和保险定价等背景下。 该禁令适用于地理定位数据的出售，但执法挑战依然存在，例如对州外公司的管辖权以及在弗吉尼亚云服务器上收集的数据。

hackernews · toomuchtodo · 7月2日 21:03 · [社区讨论](https://news.ycombinator.com/item?id=48767347)

**背景**: 来自移动设备的地理定位数据经常被数据经纪人未经明确用户同意而收集并出售用于各种目的。这些担忧促使监管加强，弗吉尼亚州是首批专门禁止出售此类数据的州之一。

**社区讨论**: 评论者表达了不同观点：一些人称赞该法律是一个良好的开端，但指出了执法困难；另一些人则强调了现实中的滥用行为，如追踪前往 Planned Parenthood 的访问。有人质疑车牌自动识别（ALPR）等公司如何遵守该法律。

**标签**: `#privacy`, `#geolocation`, `#data regulation`, `#legislation`

---

<a id="item-3"></a>
## [美国隐私危机：Aaronson 呼吁行动](https://scottaaronson.blog/?p=9902) ⭐️ 8.0/10

Scott Aaronson 认为，由于缺乏联邦隐私立法以及企业过度影响，美国面临隐私危机，他呼吁采用差分隐私等措施。 这一论点凸显了美国在隐私保护方面与其他国家的关键差距，可能激发公众讨论和立法行动，从而重塑数据隐私法律和企业实践。 Aaronson 特别强调差分隐私——一种通过向数据添加噪声来保护个人隐私同时保留统计效用的数学框架——应被强制采用。

hackernews · flowercalled · 7月3日 00:01 · [社区讨论](https://news.ycombinator.com/item?id=48768992)

**背景**: 美国目前缺乏全面的联邦隐私法律，不像欧盟的 GDPR 或中国的个人信息保护法。差分隐私是一种严格的数学定义，确保算法的输出不会透露任何个人的数据是否被包含在内，已被一些政府机构和科技公司使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Differential_privacy">Differential privacy</a></li>
<li><a href="https://medium.com/georgian-impact-blog/a-brief-introduction-to-differential-privacy-eacf8722283b">A Brief Introduction to Differential Privacy | by Georgian | Medium</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论了相关问题：有人指出企业影响力阻碍了育儿假等受欢迎的政策，其他人则辩论了 2020 年人口普查中差分隐私的有效性，还有人提供了联系立法者的链接，或评论了资本与国家的关系。

**标签**: `#privacy`, `#differential privacy`, `#United States`, `#technology policy`, `#legislation`

---

<a id="item-4"></a>
## [Linux 6.9 回归：LUKS 暂停不再清除内存中的密钥](https://mathstodon.xyz/@iblech/116769502749142438) ⭐️ 8.0/10

自 Linux 内核 6.9 起，`cryptsetup luksSuspend` 命令在系统暂停期间不再从内核内存中清除磁盘加密密钥，可能导致主密钥可被访问。 这一回归削弱了 LUKS 磁盘加密的核心安全功能，在暂停期间将加密数据暴露给具有物理访问权限的攻击者。依赖 `luksSuspend` 在休眠前擦除密钥的用户现在面临风险。 该漏洞通过 NixOS 测试发现，影响用于临时暂停 LUKS 设备并从内存中移除加密密钥的 `luksSuspend` 命令。暂停后密钥仍留在内存中，与预期行为相反。

hackernews · IngoBlechschmid · 7月2日 15:25 · [社区讨论](https://news.ycombinator.com/item?id=48763035)

**背景**: LUKS（Linux 统一密钥设置）是 Linux 上的磁盘加密标准。`luksSuspend` 命令会阻塞对加密设备的 I/O 并从内核内存中清除加密密钥，这在暂停至 RAM 时对于防止密钥暴露至关重要。该命令是 cryptsetup 的一部分，可通过系统脚本或 systemd 钩子触发。此回归仅影响启用此扩展的发行版，因为它不属于上游内核。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48763035">Since Linux 6.9, LUKS suspend stopped wiping disk-encryption keys from memory | Hacker News</a></li>
<li><a href="https://github.com/vianney/arch-luks-suspend">GitHub - vianney/arch-luks-suspend: Lock encrypted root volume on suspend in Arch Linux · GitHub</a></li>

</ul>
</details>

**社区讨论**: Hacker News 的评论者讨论了严重性：有人指出 `luksSuspend` 是 Debian 扩展而非上游官方支持，因此回归可能范围有限。其他人澄清了暂停至 RAM（密钥通常保留在内存中）与休眠至磁盘（密钥被加密）的区别。总体而言，社区赞赏发现该漏洞的 NixOS 测试，但质疑标题是否危言耸听。

**标签**: `#security`, `#linux kernel`, `#disk encryption`, `#LUKS`, `#regression`

---

<a id="item-5"></a>
## [Podman v6.0.0 发布，增强网络和 Quadlet 支持](https://blog.podman.io/2026/07/introducing-podman-v6-0-0/) ⭐️ 8.0/10

Podman v6.0.0 是一个主要版本发布，改进了网络功能，并增强了 Quadlet 集成，可通过 systemd 单元文件进行声明式容器管理。 此版本巩固了 Podman 作为领先的 Docker 替代品的地位，尤其对于寻求无根容器管理和与 systemd 集成的用户而言，可能推动其在 DevOps 环境中的更广泛采用。 关键改进包括更好的网络支持（可能通过 netavark 或 CNI），以及 Quadlet 使容器能够以声明式单元文件作为 systemd 服务运行。由于支持 compose 文件，用户可以从 Docker 迁移而无需做太多更改。

hackernews · soheilpro · 7月2日 14:23 · [社区讨论](https://news.ycombinator.com/item?id=48762098)

**背景**: Podman 是一个无守护进程的容器引擎，可以无根运行容器，是 Docker 的直接替代品。Quadlet 是一项功能，允许将容器作为 systemd 单元进行声明式管理，简化了 Linux 系统上的部署，无需像 Kubernetes 那样的完整编排工具。此版本在这些能力基础上改进了网络和易用性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.podman.io/en/latest/markdown/podman-systemd.unit.5.html">podman-systemd.unit — Podman documentation</a></li>
<li><a href="https://www.redhat.com/en/blog/quadlet-podman">Make systemd better for Podman with Quadlet</a></li>
<li><a href="https://docs.podman.io/en/latest/markdown/podman-quadlet.1.html">podman-quadlet — Podman documentation</a></li>

</ul>
</details>

**社区讨论**: 社区评论大致正面，用户 cdmckay 报告从 Docker 迁移无缝。其他人称赞 Quadlet 简化了无根容器托管。但 rsyring 批评缺乏对 Ubuntu 的官方安装包，认为这是采用的障碍。

**标签**: `#containerization`, `#Podman`, `#DevOps`, `#open-source`, `#docker-alternative`

---

<a id="item-6"></a>
## [Immich 3.0 发布引发端到端加密争议](https://github.com/immich-app/immich/discussions/29439) ⭐️ 8.0/10

自托管照片管理工具 Immich 发布了 3.0 重大更新，被赞为 Apple Photos 和 Google Photos 的即插即用替代品，但因缺乏端到端加密（E2EE）而受到批评。社区正在积极讨论这种权衡是否可接受。 此版本凸显了自托管社区在便利性与隐私之间的持续矛盾。Immich 作为自托管解决方案的流行地位使其设计选择对更广泛的生态系统具有影响力，尤其是在用户将其与专注于 E2EE 的替代方案（如 Ente）进行比较时。 Immich 3.0 不包含端到端加密，这是出于性能和功能权衡（例如服务器端机器学习功能）而故意做出的决定。一些社区成员认为，只要服务器处于个人控制之下，缺乏 E2EE 是可以接受的，而另一些人则指出像 Ente 这样的替代方案提供了 E2EE。

hackernews · hashier · 7月2日 14:13 · [社区讨论](https://news.ycombinator.com/item?id=48761944)

**背景**: Immich 是一个开源、自托管的照片和视频管理解决方案，允许用户在自己的服务器上备份、整理和分享媒体。它常被比作 Google Photos 和 Apple Photos 等云服务，但让用户完全掌控数据。端到端加密确保只有用户才能解密数据，但可能限制服务器端功能，如 AI 驱动的搜索和对象识别。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://immich.app/">Immich</a></li>
<li><a href="https://grokipedia.com/page/Immich">Immich</a></li>

</ul>
</details>

**社区讨论**: 社区意见分歧：一些用户（如 AussieWog93）认为，对于自托管设置而言，E2EE 并非必要，因为物理安全威胁很小，且加密会使数据恢复复杂化。而其他用户（如 Cider9986）则专门因为 E2EE 选择了 Ente 等替代方案。总体而言，讨论反映了自托管软件中隐私与功能优先级的更广泛辩论。

**标签**: `#self-hosting`, `#photo management`, `#open-source`, `#encryption`, `#privacy`

---

<a id="item-7"></a>
## [理解才能参与：与 AI 协作的原则](https://simonwillison.net/2026/Jul/2/understand-to-participate/#atom-everything) ⭐️ 8.0/10

Simon Willison 强调了 Geoffrey Litt 提出的'理解才能参与'原则，该原则认为与编码代理协作的开发者必须保持对代码的深入理解，以避免认知债务并在过程中保持积极创造力。 随着 AI 编码代理能力的增强，开发者面临着积累认知债务的风险——即自身对代码库的心智模型逐渐退化。这一原则提供了一种主动保持参与、防止对软件演进失去控制的方法。 Geoffrey Litt 在 2026 年 AIE World's Fair 上提出了这一概念，Simon Willison 随后发布博客文章呼应了这一观点。该原则强调，对代码达到足够深度的理解是进一步与 AI 代理进行高效协作的必要条件。

rss · Simon Willison · 7月2日 17:07

**背景**: 认知债务指的是随着时间推移，软件系统中共享理解的侵蚀，类似于技术债务但存在于开发者的头脑中。随着 AI 代理生成越来越多的代码，开发者可能对代码库逐渐陌生，导致难以推理和安全修改系统。'理解才能参与'原则倡导持续学习和参与，以抵消这种偏差。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://margaretstorey.com/blog/2026/02/09/cognitive-debt/">How Generative and Agentic AI Shift Concern from Technical Debt to Cognitive Debt</a></li>
<li><a href="https://getdx.com/blog/cognitive-debt-the-hidden-risk-in-ai-driven-software-development/">Cognitive debt: The hidden risk in AI-driven software development</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#cognitive debt`, `#code collaboration`, `#software engineering`

---

<a id="item-8"></a>
## [Meta 的 NeoCloud 雄心：扩展推荐系统与自研芯片](https://newsletter.semianalysis.com/p/meta-compute-everyone-wants-to-be) ⭐️ 8.0/10

SemiAnalysis 的分析表明，Meta 正在推进 NeoCloud 战略，将其推荐系统规模扩大 10 倍，并通过“Bedrock 2.0”等项目开发自研芯片，同时参与 GPU 云市场竞争，发布 ClusterMAX 排名。 这一转变使 Meta 成为 AI 基础设施领域的潜在重要参与者，挑战传统超大规模云和 NeoCloud 提供商，并可能重塑 AI 训练与推理的经济性。 内容提到“推荐系统扩展 10 倍”，表明推荐系统工作负载大幅增长；“Bedrock 2.0”可能指 Meta 的下一代计算平台；ClusterMAX 是 SemiAnalysis 发布的 GPU 云评级系统，按性能、网络等标准对提供商进行排名。

rss · Semianalysis · 7月2日 22:18

**背景**: NeoCloud 指专注于 AI 工作负载、使用 GPU 加速器的专业云提供商，与传统超大规模云不同。Meta 传统上是超大规模云服务商，现在正大力投资自研芯片和类似 NeoCloud 的能力，以减少对外部供应商的依赖，并优化其推荐系统等 AI 服务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cisco.com/site/us/en/learn/topics/computing/what-is-neocloud.html">What Is Neocloud? - Cisco</a></li>
<li><a href="https://blog.equinix.com/blog/2025/10/14/what-is-a-neocloud/">What Is a Neocloud? - Interconnections - The Equinix Blog</a></li>
<li><a href="https://www.clustermax.ai/">GPU Cloud ClusterMAX ™ Rating & Ranking System | SemiAnalysis</a></li>

</ul>
</details>

**标签**: `#cloud computing`, `#meta`, `#AI infrastructure`, `#recommender systems`

---

<a id="item-9"></a>
## [ECTC 2026：EMIB-T、定制 HBM、HBM4、微流体冷却、光子互连](https://newsletter.semianalysis.com/p/ectc2026) ⭐️ 8.0/10

在 ECTC 2026 上，英特尔推出了支持 HBM4 和 UCIe 的 EMIB-T 封装技术，微软则展示了用于 3D 异构集成的微流体冷却方案。其他亮点包括 SK 海力士的定制 HBM 解决方案以及 Lightmatter 在光子互连方面的进展。 这些公告解决了 AI 芯片性能中的关键瓶颈，包括内存带宽、热管理和芯片间互连。这些进展为更强大、更高效的数据中心加速器和高性能计算系统铺平了道路。 EMIB-T 降低了缺陷敏感性，并扩展到超越光罩尺寸限制的更大外形，英特尔报告良率达到 90%。微流体冷却将冷却液循环流过直接蚀刻在硅衬底中的微观通道，从而在靠近活动核心的位置实现高效散热。

rss · Semianalysis · 7月2日 17:25

**背景**: 英特尔的 EMIB 和台积电的 CoWoS 等先进封装技术将多个芯片集成在小面积内以克服晶体管缩放限制。然而，它们面临散热和互连密度的挑战。微流体冷却和光子互连是解决这些问题的新兴方案，光子互连利用光而非电传输数据，功耗更低、带宽更高。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/ammhasib_driving-the-future-of-multi-chip-compute-activity-7408764535257317376-dVkb">Intel EMIB - T : Revolutionizing AI and HPC Packaging with... | LinkedIn</a></li>
<li><a href="https://abit.ee/en/hard/intel-introduces-emib-t-revolutionary-multi-die-packaging-technology-with-hbm4-support">Intel Introduces EMIB - T — Revolutionary Multi-Die Packaging...</a></li>
<li><a href="https://www.datacenterdynamics.com/en/analysis/microfluidics-cooling-inside-the-chip/">Microfluidics: Cooling inside the chip - DCD</a></li>
<li><a href="https://lightmatter.co/knowledge-hub/how-do-photonic-interconnects-work/">How Do Photonic Interconnects Work?</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#advanced packaging`, `#HBM`, `#photonic interconnects`, `#cooling`

---

<a id="item-10"></a>
## [OpenAI 提议美国政府持股 5%，或扩展至谷歌 Meta](https://www.bloomberg.com/news/articles/2026-07-02/openai-proposes-giving-the-us-government-a-5-stake-ft-says) ⭐️ 8.0/10

OpenAI 提议让美国政府持有公司 5% 的股份，并讨论将类似 5% 的股份扩展至 Google、Meta 和 Anthropic 等其他主要 AI 公司，让公众直接分享 AI 热潮带来的收益。 这一提议标志着 AI 治理模式的转变，可能为政府参与私营 AI 公司开创先例，并引发关于控制权、监管以及 AI 利润公平分配的关键问题。 该提议包括由一个政府载体统一持有 OpenAI、Anthropic、Google 和 Meta 各 5% 的股份；然而，这些公司是否接受该安排尚不明确，并且已引发关于监管冲突和公司控制权的担忧。

telegram · zaihuapd · 7月2日 06:02

**背景**: AI 行业经历了快速增长，引发了关于如何确保其收益广泛共享的讨论。在美国，政府持有科技公司股份并不常见，通常更倾向于私营企业。该提议将在公众与 AI 利润之间建立直接的财务联系。

**标签**: `#AI`, `#Government Stake`, `#Regulation`, `#OpenAI`, `#Tech Policy`

---

<a id="item-11"></a>
## [多公司因 AI 成本飙升限制员工使用](https://www.404media.co/companies-are-throttling-employees-ai-use-because-its-too-expensive/) ⭐️ 8.0/10

花旗银行、Atlassian 和 Adobe 等公司因按用量计费模式下成本急剧飙升，限制员工使用 GPT-5.5、Claude Opus 4.7 等先进 AI 模型。 这一趋势表明企业 AI 应用面临成本管理挑战，可能减缓部署速度，迫使公司重新思考定价模式和使用政策。 花旗银行于 6 月 24 日完全禁用 Claude Opus 4.6、4.7 和 GPT-5.5。Atlassian 的 AI 月支出从 2025 年 8 月的 500 万美元飙升至 2026 年 5 月的逾 1500 万美元，导致设置使用上限。

telegram · zaihuapd · 7月2日 13:59

**背景**: 许多 AI 工具按 token 或 API 调用计费，称为按用量计费。企业通常批量购买 AI 积分并制定内部政策控制成本。随着模型更强大，每个任务消耗更多 token，推高费用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.5">GPT-5.5</a></li>
<li><a href="https://c-ai.chat/model-guides/">Models - Claude AI</a></li>
<li><a href="https://ordwaylabs.com/blog/ai-credits/">AI Credits : What They Are and How They Work</a></li>

</ul>
</details>

**标签**: `#AI cost`, `#enterprise AI`, `#AI regulation`, `#technology news`

---

<a id="item-12"></a>
## [Anthropic 自研 AI 芯片，与三星洽谈代工](https://www.theinformation.com/articles/anthropic-talks-samsung-manufacture-custom-ai-chip) ⭐️ 8.0/10

Anthropic 已开始自研 AI 芯片，并与三星电子洽谈潜在代工合作，旨在加强对支撑 Claude 模型的计算系统的控制。 此举反映了领先 AI 公司垂直整合的日益增长趋势，使 Anthropic 能够优化硬件-软件协同设计以提高效率，并减少对外部芯片供应商的依赖。 该项目仍处于早期阶段，且 Anthropic 相比其他已推进自研服务器芯片的公司入场较晚。三星将担任该芯片的代工厂商。

telegram · zaihuapd · 7月2日 15:57

**背景**: OpenAI 和谷歌等主要 AI 公司一直在开发定制芯片以加速 AI 工作负载并降低成本。三星是全球最大的存储芯片制造商和重要的代工厂商。代工制造允许芯片设计者在无需自建工厂的情况下生产其设计。

**标签**: `#AI chips`, `#Anthropic`, `#Samsung`, `#hardware`, `#custom silicon`

---