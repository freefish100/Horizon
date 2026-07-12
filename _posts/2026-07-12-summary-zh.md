---
layout: default
title: "Horizon Summary: 2026-07-12 (ZH)"
date: 2026-07-12
lang: zh
---

> 从 28 条内容中筛选出 8 条重要资讯。

---

1. [苹果起诉 OpenAI 系统性窃取商业机密](#item-1) ⭐️ 10.0/10
2. [vLLM v0.25.0：Model Runner V2 成为默认，PagedAttention 被移除](#item-2) ⭐️ 9.0/10
3. [全球首次：人形机器人远程完成活猪手术](#item-3) ⭐️ 9.0/10
4. [英伟达、CoreWeave、Nebius：GPU 热潮中的循环融资剖析](#item-4) ⭐️ 8.0/10
5. [推荐在 SQLite 中使用严格表](#item-5) ⭐️ 8.0/10
6. [VultronRetriever 系列模型登顶 MTEB，可在边缘设备离线运行](#item-6) ⭐️ 8.0/10
7. [U-Boot 引导程序漏洞可在操作系统启动前执行代码](#item-7) ⭐️ 8.0/10
8. [上海设定 2027 年高质量脑机接口目标](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [苹果起诉 OpenAI 系统性窃取商业机密](https://www.cnbc.com/2026/07/10/apple-openai-lawsuit-trade-secrets.html) ⭐️ 10.0/10

2026 年 7 月 10 日，苹果在美国加州北区联邦法院起诉 OpenAI、两名前员工及 io Products，指控其系统性窃取商业机密以加快消费级硬件研发。 此诉讼突显了两大科技巨头在知识产权和人才争夺上的紧张关系升级，可能为 AI 公司如何利用泄露的硬件专业知识设立先例。 苹果指控前员工 Chang Liu 离职后仍访问内部网络并下载数十份硬件文件；硬件负责人 Tang Yew Tan 被指在离职前将供应商资料发至个人邮箱，并曾要求求职者携带苹果零部件参加面试。

telegram · zaihuapd · 7月11日 03:14

**背景**: 苹果和 OpenAI 都是人工智能和消费电子领域的主要参与者。商业机密盗窃诉讼在科技行业很常见，通常涉及员工将专有信息带到竞争对手处。此案涉及超过 400 名现任 OpenAI 的前苹果员工。

**标签**: `#Apple`, `#OpenAI`, `#Trade Secrets`, `#Lawsuit`, `#AI Hardware`

---

<a id="item-2"></a>
## [vLLM v0.25.0：Model Runner V2 成为默认，PagedAttention 被移除](https://github.com/vllm-project/vllm/releases/tag/v0.25.0) ⭐️ 9.0/10

vLLM v0.25.0 将 Model Runner V2 设为所有稠密模型的默认执行路径，移除了传统的 PagedAttention 注意力实现，并实现了与 Transformers 建模后端的性能等价。该版本还新增了 LLaVA-OneVision-2 等模型以及流式解析引擎。 此版本巩固了 vLLM 的架构改进，简化了代码库并加速了稠密模型的推理。PagedAttention 的移除标志着一个重要的里程碑，它是 vLLM 最初的创新，其被淘汰意味着更新、更好的后端已经成熟。 Model Runner V2 (MRv2) 现在支持 EVS、实时嵌入、Mamba 混合模型的前缀缓存以及完整的 CUDA 图动态投机解码。Transformers 后端获得了 FP8 MoE 支持，并迁移了 GPTBigCode、Starcoder2 和 RoBERTa。

github · khluu · 7月11日 20:06

**背景**: vLLM 是一个面向大语言模型的高性能推理引擎，最初基于 PagedAttention 构建，这是一种通过分页高效管理 KV 缓存内存的注意力算法。Model Runner V2 是一个重新设计的执行流水线，旨在取代原始更复杂的系统，以获得更好的性能和可维护性。此版本标志着 MRv2 成为默认配置，同时原始 PagedAttention 实现退役。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/vllm-project/vllm/releases">Releases · vllm -project/ vllm</a></li>
<li><a href="https://docs.vllm.ai/en/latest/design/paged_attention/">Paged Attention - vLLM</a></li>
<li><a href="https://en.wikipedia.org/wiki/PagedAttention">PagedAttention - Wikipedia</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM Inference`, `#Model Runner`, `#Release Notes`, `#Performance`

---

<a id="item-3"></a>
## [全球首次：人形机器人远程完成活猪手术](https://arstechnica.com/ai/2026/07/humanoid-robots-controlled-by-surgeons-did-world-first-operation-on-live-pigs/) ⭐️ 9.0/10

外科医生通过远程操控宇树 G1 人形机器人，成功在活猪身上完成两例微创胆囊切除手术，这是全球首次将通用人形机器人用于活体手术，成果发表在《自然》期刊。 这一突破展示了低成本人形机器人将手术能力带到偏远和资源有限场景（如农村、战场或太空任务）的潜力。与达芬奇等专用手术机器人相比，它可能大幅降低费用门槛。 宇树 G1 基础款起售价 13500 美元，配备灵巧手后约 67000 美元，远低于现有手术机器人。该机器人高约 1.5 米、重约 27 公斤，占用空间小。

telegram · zaihuapd · 7月11日 02:29

**背景**: 机器人手术已发展多年，但达芬奇等专用系统造价数十万到数百万美元。通用人形机器人通常用于仓库作业或娱乐等任务。这项研究显示，通过远程操作，低成本人形机器人可以执行精细的手术操作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://m.dzplus.dzng.com/share/general/0/NEWS2139618WUMBNTSKAWAFL">半岛聚焦丨65...</a></li>
<li><a href="https://www.jinantimes.com.cn/news-243-5048472.html">jinantimes.com.cn/news-243-5048472.html</a></li>

</ul>
</details>

**标签**: `#humanoid robots`, `#robotic surgery`, `#medical robotics`, `#Nature publication`, `#low-cost healthcare`

---

<a id="item-4"></a>
## [英伟达、CoreWeave、Nebius：GPU 热潮中的循环融资剖析](https://io-fund.com/ai-stocks/nvidia-coreweave-nebius-circular-financing-gpu-boom) ⭐️ 8.0/10

一篇分析文章探讨了循环融资实践，即英伟达投资于 CoreWeave 和 Nebius 等 GPU 云提供商，而后者又大量采购英伟达硬件，引发了关于 AI 基础设施需求可持续性的质疑。 这种动态可能虚增 GPU 需求，如果投资循环崩溃，将产生财务风险，影响整个 AI 基础设施生态系统和投资者信心。 英伟达对 CoreWeave 的 20 亿美元投资仅占其 2026 年 350 亿美元资本支出的约 5.7%，表明循环性可能被夸大了。社区评论者认为，关注经济盈利能力——例如每代币的 ROI 和企业代币预算——比融资结构更重要。

hackernews · adletbalzhanov · 7月11日 17:21 · [社区讨论](https://news.ycombinator.com/item?id=48873836)

**背景**: 循环融资是指公司相互投资，并用所得资金购买对方产品，造成需求假象。在 AI 热潮中，英伟达主导 GPU 供应，而 CoreWeave 和 Nebius 等云提供商依赖英伟达芯片。担忧在于，如果没有真正的终端用户需求，这种循环可能导致泡沫。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.buildthisnow.com/blog/guide/mechanics/is-ai-a-bubble">Is AI a Bubble? ' Circular Financing ' in Plain English | Build This Now</a></li>
<li><a href="https://en.wikipedia.org/wiki/CoreWeave">CoreWeave - Wikipedia</a></li>
<li><a href="https://nebius.com/about">About Nebius</a></li>

</ul>
</details>

**社区讨论**: 社区评论观点不一：有人认为循环融资的说法被夸大了，因为英伟达的投资比例很小；另一些人则转而关注 AI 基础设施建设能否实现经济盈利，引用每代币 ROI 等指标；少数人警告说，如果需求疲软，系统可能崩溃。

**标签**: `#GPU boom`, `#circular financing`, `#Nvidia`, `#CoreWeave`, `#AI infrastructure`

---

<a id="item-5"></a>
## [推荐在 SQLite 中使用严格表](https://evanhahn.com/prefer-strict-tables-in-sqlite/) ⭐️ 8.0/10

该文章推荐在 SQLite 中使用严格表以改善类型强制，社区工具如 sqlite-utils 现已支持将非严格表转换为严格表。 严格表通过强制列类型提高数据完整性，对多应用程序数据库至关重要，并解决了习惯于传统 SQL 数据库的开发者的常见抱怨。 严格表自 SQLite 3.37.0（2021-11-27）引入，通过 STRICT 关键字按表启用；但不能直接 ALTER 表使其变为严格，必须重建表，而 sqlite-utils 等工具有助于自动化这一过程。

hackernews · ingve · 7月11日 17:33 · [社区讨论](https://news.ycombinator.com/item?id=48873940)

**背景**: SQLite 传统上使用动态类型，列数据类型仅为提示而非严格规则，提供了灵活性但面临数据损坏风险。严格表在列级别强制类型约束，拒绝不兼容的数据。该功能旨在满足那些希望在不放弃 SQLite 轻量特性的前提下获得更强类型安全性的用户。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sqlite.org/stricttables.html">STRICT Tables</a></li>
<li><a href="https://news.ycombinator.com/item?id=48873940">Prefer strict tables in SQLite - Hacker News</a></li>

</ul>
</details>

**社区讨论**: 社区评论意见不一：simonw 为 sqlite-utils 添加了转换功能；dfabulich 引用 SQLite 文档，认为不应将严格设为默认，因为修复错误较困难；而 jll29 和 petilon 等人则强烈主张将严格设为默认。

**标签**: `#SQLite`, `#database`, `#strict tables`, `#data integrity`, `#tools`

---

<a id="item-6"></a>
## [VultronRetriever 系列模型登顶 MTEB，可在边缘设备离线运行](https://www.reddit.com/r/MachineLearning/comments/1utmxq8/vultronretriever_family_of_models_released_on/) ⭐️ 8.0/10

VultronRetriever 系列（包括 Prime-8B、Core-4.5B、Flash-0.8B 三款模型）已在 HuggingFace 上发布，在 MTEB 排行榜上各自类别中排名第一，其中 8B 模型位居全球榜首。相比之前的领先模型，该系列实现了 16 倍的索引存储缩小和 12 倍的吞吐量提升，并且能够在 iPhone 等边缘设备上完全离线运行。 这一进展显著提升了检索模型的效率，使得最先进的检索技术能够在资源受限且无需联网的边缘设备上实现。这对于移动搜索、离线文档问答以及注重低延迟和数据本地化的隐私保护 AI 等应用具有广泛影响。 这些模型利用 Hydra 架构实现后期交互检索，在内存消耗仅为同类模型一半的情况下实现了高精度。所有训练数据集均具有 0% 的跨数据集重复和 0% 的评估污染，并且在私有 MTEB 评估中未观察到过拟合现象。

reddit · r/MachineLearning · /u/madkimchi · 7月11日 15:22

**背景**: MTEB（大规模文本嵌入基准）排行榜是评估嵌入和检索模型在多种任务上表现的标准基准。后期交互检索（如 ColBERT 等模型采用的方法）允许查询和文档之间进行细粒度的词元级匹配，从而提高检索精度。边缘 AI 部署使模型能够直接在本地设备上运行，从而降低延迟并增强隐私保护。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/spaces/mteb/leaderboard">MTEB Leaderboard - a Hugging Face Space by mteb</a></li>
<li><a href="https://modal.com/blog/mteb-leaderboard-article">Top embedding models on the MTEB leaderboard</a></li>
<li><a href="https://weaviate.io/blog/late-interaction-overview">An Overview of Late Interaction Retrieval Models: ColBERT, ColPali, and ColQwen | Weaviate</a></li>

</ul>
</details>

**标签**: `#retrieval`, `#MTEB`, `#edge AI`, `#embedding`, `#HuggingFace`

---

<a id="item-7"></a>
## [U-Boot 引导程序漏洞可在操作系统启动前执行代码](https://www.bleepingcomputer.com/news/security/new-u-boot-flaws-could-enable-stealthy-firmware-attacks/) ⭐️ 8.0/10

安全公司 Binarly 披露了 U-Boot 的 FIT 签名验证代码中的 6 个漏洞，其中两个可导致任意代码执行，四个可造成拒绝服务。这些漏洞自 U-Boot 2013.07 版本起存在，影响超过 50 个稳定版本。 这些漏洞允许攻击者在操作系统和安全软件启动之前执行恶意代码，可能禁用固件安全功能或植入持久性恶意软件。对于支持远程固件更新的 BMC 系统，攻击者无需物理接触即可利用这些漏洞。 Binarly 已提交补丁并被 U-Boot 维护者接受，但修复需要硬件厂商集成到固件更新中才能分发。已停止支持的老旧设备可能永远无法获得修复。

telegram · zaihuapd · 7月11日 08:32

**背景**: U-Boot 是嵌入式系统中广泛使用的开源引导程序，FIT（扁平化映像树）是一种将内核、设备树和其他数据与加密签名捆绑在一起的格式。FIT 签名验证确保只启动受信任的映像。这些漏洞存在于验证代码中，允许攻击者绕过完整性检查。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.u-boot-project.org/en/latest/usage/fit/signature.html">U - Boot FIT Signature Verification — Das U - Boot unknown version...</a></li>
<li><a href="https://cybersecuritynews.com/u-boot-fit-signature-verification/">Six U - Boot FIT Signature Verification Flaws Enable Code Execution...</a></li>

</ul>
</details>

**标签**: `#security`, `#U-Boot`, `#firmware`, `#vulnerabilities`, `#bootloader`

---

<a id="item-8"></a>
## [上海设定 2027 年高质量脑机接口目标](https://t.me/zaihuapd/42501) ⭐️ 8.0/10

上海市科学技术委员会印发《上海市脑机接口未来产业培育行动方案（2025-2030 年）》，目标是在 2027 年前实现高质量脑控，半侵入式脑机接口产品在国内率先实现临床应用，侵入式脑机接口研发取得突破。 该政策为重要科技中心的脑机接口发展设定了明确里程碑，可能加速临床转化，并使中国在全球神经技术领域具有竞争力。它有望帮助瘫痪或失语患者恢复部分功能。 该方案还计划到 2027 年，推动 5 款以上侵入式、半侵入式脑机接口产品完成医疗器械型式检验和临床试验，面向失语、瘫痪等患者实现部分语言和运动功能恢复。

telegram · zaihuapd · 7月11日 15:49

**背景**: 脑机接口（BCI）能够实现大脑与外部设备之间的直接通信。侵入式 BCI 需要通过手术植入大脑内部，而半侵入式 BCI（如 ECoG）将电极放置在颅骨下的脑表面但硬脑膜上方，平衡了信号质量与风险。非侵入式 BCI 使用头皮电极，但信号分辨率较低。

<details><summary>参考链接</summary>
<ul>
<li><a href="http://learn.neurotechedu.com/introtobci/">Intro to Brain Computer Interface - NeurotechEDU</a></li>
<li><a href="https://www.cell.com/the-innovation/fulltext/S2666-6758(24)00033-X">Fully implantable wireless brain-computer interface for humans: Advancing toward the future: The Innovation</a></li>

</ul>
</details>

**标签**: `#brain-computer interface`, `#neural engineering`, `#China policy`, `#medical technology`, `#neurotechnology`

---