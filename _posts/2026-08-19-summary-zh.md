---
layout: default
title: "Horizon Summary: 2026-08-19 (ZH)"
date: 2026-08-19
lang: zh
---

> 从 31 条内容中筛选出 7 条重要资讯。

---

1. [Mojo 编程语言以 Apache 2 许可证开源](#item-1) ⭐️ 9.0/10
2. [戈丁：亚马逊广告模式是对消费者信任征税](#item-2) ⭐️ 8.0/10
3. [火车运动将铁路变成平板扫描仪](#item-3) ⭐️ 8.0/10
4. [用 20 美元工具救回变砖的 AMD 7040 Framework 13 笔记本](#item-4) ⭐️ 8.0/10
5. [中国下令部分机构提前移除定制版 Windows 10](#item-5) ⭐️ 8.0/10
6. [国产 AI 芯片 2026 年将占中国市场近 90%，寒武纪与华为成最大赢家](#item-6) ⭐️ 8.0/10
7. [长征十号乙完成全球首次网系海上回收](#item-7) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Mojo 编程语言以 Apache 2 许可证开源](https://simonwillison.net/2026/Aug/18/mojo-is-now-open-source/) ⭐️ 9.0/10

Modular 于 2026 年 8 月 18 日以 Apache 2 许可证发布了 Mojo 编译器和工具链，这在 1.0 版本发布一周之后。此举兑现了 Mojo 在 2023 年 5 月首次公布时作出的开源承诺。 Mojo 开源是一个重要里程碑，开发者可以查看、修改并为编译器做贡献，从而提升人们对这款 AI 和 GPU 编程语言的信任与采用。这也标志着它从一个专有工具转向社区驱动的语言，在竞争激烈的环境中具有战略意义。 Mojo 最初的目标是成为 Python 的超集，但 Modular 在 2025 年 8 月左右调整了这一目标，允许语言在保持 Python 风格的同时独立发展。编译器基于 MLIR 编译器框架而非直接基于 LLVM，因此能面向 CPU、GPU、TPU 和其他加速器生成代码。

rss · Simon Willison · 8月18日 21:39

**背景**: Mojo 是 Modular 为高性能 AI 基础设施开发的一门系统编程语言，它融合了类似 Python 的语法和静态类型、借用检查器等底层特性。Mojo 使用现代编译器框架 MLIR，可在异构硬件上生成高效代码。自 2023 年 5 月发布以来，这门语言一直是专有的，而开源是社区长期的关键诉求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_(programming_language)">Mojo (programming language)</a></li>
<li><a href="https://mojolang.org/">Mojo - Modular</a></li>

</ul>
</details>

**标签**: `#mojo`, `#open-source`, `#programming-language`, `#compiler`, `#modular`

---

<a id="item-2"></a>
## [戈丁：亚马逊广告模式是对消费者信任征税](https://seths.blog/2026/08/the-amazon-tax/) ⭐️ 8.0/10

赛斯·戈丁发表了一篇题为《亚马逊税》的文章，认为亚马逊的广告模式相当于对消费者信任征税。这篇文章在 Hacker News 上引发了热议，获得 903 分和 526 条评论。 这很重要，因为它揭示了广告驱动的平台衰退这一更广泛的行业趋势——平台日益优先考虑广告收入而非用户体验。这影响着消费者、卖家以及电商市场的长期信誉。 评论者提出了潜在的法律途径，例如当亚马逊在品牌搜索词下展示竞争对手广告时，可能构成商标侵权或欺诈。讨论还将亚马逊的模式与地铁、电视和餐厅菜单等其他广告支持环境进行对比。

hackernews · herbertl · 8月18日 13:22 · [社区讨论](https://news.ycombinator.com/item?id=49345263)

**背景**: 亚马逊是一个占主导地位的电商平台，其商品搜索结果中现在包含赞助广告。戈丁的“税”这一比喻意味着，当广告干扰消费者原本的购物意图时，消费者在注意力和信任上付出了隐性成本。这是关于平台如何将用户注意力变现以及这是否会削弱其核心价值主张的更广泛讨论的一部分。

**社区讨论**: 评论者意见不一：有人建议对亚马逊在商标搜索词下展示竞争对手广告的行为采取法律行动，也有人认为此类广告可能具有相关性，对消费者有益。一个反复出现的主题是，广告毁掉平台是一种常见模式，在地铁、电视等地方早已出现，并非亚马逊独有。

**标签**: `#Amazon`, `#Advertising`, `#E-commerce`, `#Platform Economics`, `#Consumer Trust`

---

<a id="item-3"></a>
## [火车运动将铁路变成平板扫描仪](https://philo.gay/linecam/) ⭐️ 8.0/10

Linecam 项目利用火车的运动和固定相机生成狭缝扫描图像，从而将铁路网络变成一个巨大的平板扫描仪。这是一项结合摄影、计算机视觉和硬件的新颖创意编码实验。 这项实验展示了如何将日常基础设施重新用作成像设备，为火车旅行提供了新的艺术视角。它可能激发更多基于运动的成像技术和创意编码项目。 该技术依赖于狭缝扫描摄影：固定相机在火车向前运动提供扫描移动时，连续捕捉经过场景的窄条。生成的图像沿轨道方向压缩了时间和空间。

hackernews · otherayden · 8月18日 12:43 · [社区讨论](https://news.ycombinator.com/item?id=49344825)

**背景**: 狭缝扫描摄影是一种利用狭缝每次仅曝光图像中一条窄线的摄影技术，常用于全景摄影和终点摄影相机。在该项目中，火车的运动充当扫描机制，车上的固定相机逐行记录场景。结果是铁路走廊被压平拉长的视图。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Slit-scan_photography">Slit-scan photography</a></li>
<li><a href="https://thelawlers.com/Blognosticator/?p=2519">Spinning time into gold with slit - scan images | thelawlers.com</a></li>

</ul>
</details>

**社区讨论**: 社区成员分享了相关实验，包括 2008 年使用 iSight 摄像头的类似设置、手动拼接动画以及一个基于 Web 的狭缝扫描工具。有人评论说，那些意外的“错误”镜头在主观上比正常拍摄更有趣。

**标签**: `#slit-scan`, `#photography`, `#creative-coding`, `#computer-vision`, `#hardware`

---

<a id="item-4"></a>
## [用 20 美元工具救回变砖的 AMD 7040 Framework 13 笔记本](https://quantum5.ca/2026/08/16/fixing-bricked-amd-7040-series-framework-13-laptop-with-20-tools/) ⭐️ 8.0/10

一篇新的技术指南详细记录了作者如何用约 20 美元的工具，救回一台因 BIOS 更新出错而变砖的 AMD 7040 系列 Framework Laptop 13。文章逐步展示了恢复过程，包括由于该型号没有焊接刷写排针，而使用 pogo pins（弹簧探针）接触 BIOS 闪存芯片。 这件事之所以重要，是因为固件更新失败可能让一台原本完好的笔记本变成电子垃圾，而这篇指南为个人用户和维修店提供了一条低成本的恢复途径。它也加剧了关于固件更新风险、维修权以及厂商是否应为问题更新负责的讨论。 恢复过程需要使用 pogo pins 和外部编程器，而不是简单地插上连接器，因为 Framework 在这款型号上没有焊接专用的 BIOS 刷写排针。这篇指南的特殊之处在于记录了一种常见却少有详细文档的维修方法；评论者还指出，Framework 其实有开源的调试工具，但出于成本考虑，量产主板上没有焊接相应的连接器。

hackernews · jp_sc · 8月18日 13:18 · [社区讨论](https://news.ycombinator.com/item?id=49345220)

**背景**: Framework Computer 是一家美国笔记本电脑制造商，以模块化、可维修的设计和积极支持“维修权”（right to repair）而闻名，其 Framework Laptop 13 于 2021 年发布。“变砖”（bricked）的设备指的是变得像砖头一样无用的设备，通常是因为 BIOS 或固件更新失败，破坏了启动所需的最底层代码。要恢复这类设备，通常需要使用外部编程器绕过正常更新流程重新写入闪存芯片。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Framework_Computer">Framework Computer - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Framework_Laptop">Framework Laptop</a></li>
<li><a href="https://timvsaedlex.wordpress.com/2012/10/16/what-does-bricking-a-device-mean/">What Does “ Bricking ” a Device Mean ? | timvsaedlex</a></li>

</ul>
</details>

**社区讨论**: 评论普遍对厂商的做法持批评态度：有用户认为 Framework 应为其有问题的 BIOS 更新承担法律责任，并建议将此事诉诸小额索赔法庭；另一用户则分享了 ThinkPad 变砖的类似经历，称 PC 厂商“根本不在乎”。还有人呼吁官方更新应延长保修期，并批评 Framework 为节省成本而不焊接刷写排针；至少有一位用户表示，这篇文章让他后悔购买了 Framework 笔记本。

**标签**: `#hardware`, `#firmware`, `#BIOS`, `#laptop repair`, `#Framework`

---

<a id="item-5"></a>
## [中国下令部分机构提前移除定制版 Windows 10](https://www.bloomberg.com/news/articles/2026-08-18/china-axing-microsoft-windows-from-state-agencies-ahead-of-plan) ⭐️ 8.0/10

中国国家安全部要求部分政府机构提前卸载定制版 Windows 10，使原定 2027 年 2 月的停用时间提前了数月。此举源于数据安全担忧，但未说明具体漏洞。 这一加速替换计划表明中国政府在政府 IT 领域进一步减少对外国技术的依赖。这可能影响微软在中国的政府业务，同时利好国产操作系统厂商。 该指令适用于与中国电子科技集团合作开发的 Windows 10 中国政府版。微软表示，未发现影响该产品的安全事件，该产品仍在定期获得安全更新。

telegram · zaihuapd · 8月18日 06:22

**背景**: Windows 10 中国政府版于 2017 年发布，由微软与中国电子科技集团通过合资公司 CMIT 为中国政府客户打造。在中美科技摩擦和数据主权担忧背景下，中国政府正逐步转向国产软件替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blogs.windows.com/windowsexperience/2017/05/23/announcing-windows-10-china-government-edition-new-surface-pro/">Announcing Windows 10 China Government Edition and the new...</a></li>
<li><a href="https://www.partitionwizard.com/news/windows-10-china-government-edition.html">Windows 10 China Government Edition : An Impactful Version</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#government policy`, `#Microsoft Windows`, `#China`

---

<a id="item-6"></a>
## [国产 AI 芯片 2026 年将占中国市场近 90%，寒武纪与华为成最大赢家](https://www.tomshardware.com/tech-industry/artificial-intelligence/chinas-homegrown-ai-accelerators-to-supply-90-percent-of-the-countrys-domestic-market-analysts-suggest-cambricon-and-huawei-expected-to-be-the-biggest-winners-in-the-shift-away-from-nvidia-and-amd) ⭐️ 8.0/10

TrendForce 预测，到 2026 年，中国本土 AI 加速器将占据国内市场近 90%的份额，而去年这一比例约为 45%。寒武纪和华为预计将成为这一从英伟达和 AMD 转向本土芯片趋势的最大受益者。 这一市场预测反映了中国在美国出口管制下推动半导体自给自足的努力，并可能重塑全球 AI 芯片竞争格局。华为和寒武纪有望获得显著的市场份额和收入增长，而英伟达和 AMD 对中国市场的获取将受到进一步限制。 2025 年，英伟达以 220 万颗出货量占中国市场份额 55%，华为则出货 81.2 万颗，占 20.3%。要实现上述预测，中国必须在一年内将高端 AI 芯片产量提升 2.2 倍至约 196 万颗，这使其制造产能面临考验。

telegram · zaihuapd · 8月18日 13:03

**背景**: AI 加速器是一种专用硬件，旨在加速人工智能和机器学习工作负载，如神经网络和矩阵运算。寒武纪是一家总部位于北京、部分国有控股的芯片设计公司，专注于开发 AI 处理器和通用 GPU，常被与英伟达类比。华为的昇腾 AI 芯片也是重要的国产替代方案。美国出口管制限制英伟达和 AMD 向中国出售最先进芯片，进一步加速了中国发展本土芯片替代方案的进程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_accelerator">AI accelerator</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cambricon_Technologies">Cambricon Technologies</a></li>

</ul>
</details>

**标签**: `#AI chips`, `#Huawei`, `#Cambricon`, `#semiconductor`, `#china-tech`

---

<a id="item-7"></a>
## [长征十号乙完成全球首次网系海上回收](https://t.me/zaihuapd/43264) ⭐️ 8.0/10

2026 年 7 月 10 日，长征十号乙运载火箭从海南商业航天发射场升空。一、二级分离约 6 分钟后，一子级垂直返回并成功被海上回收平台的网系捕获装置回收，这是中国首次成功实施运载火箭一子级可控回收，也是全球首次完成运载火箭网系回收。 这一里程碑使中国成为继美国之后全球第二个掌握大运力可回收火箭技术的国家。网系回收方式无需安装着陆腿，可减轻箭体重量并降低发射成本，有望为商业卫星星座部署带来显著效益。 长征十号乙为 5 米直径两级串联构型大型液体运载火箭，起飞推力约 890 吨，起飞重量约 760 吨。芯一级采用液氧煤油推进剂，芯二级采用液氧甲烷推进剂；重复使用状态下近地轨道运载能力为 16 吨。网系回收方案无需着陆腿，可扩大捕获窗口并提高缓冲成功率。

telegram · zaihuapd · 8月19日 00:16

**背景**: 可重复使用火箭通过回收并复用最昂贵的一子级来降低发射成本。SpaceX 的猎鹰 9 号率先实现了在海上无人船上的推进式垂直着陆，而中国长征十号乙则采用海上平台网系捕获这一新方案，无需着陆腿且降低结构重量。该火箭由中国运载火箭技术研究院抓总研制，首飞验证了隔板贮箱推进剂管理、发动机多次启动与高空点火、高精度导航控制等技术。研制团队计划在 2026 年底前完成一子级复用飞行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.qq.com/rain/a/20260710A05V3Y00">成功！我国首次实现火箭一子级可控回收，预计年底前完成复用飞行_腾讯新闻</a></li>
<li><a href="https://www.dw.com/zh/中国首次实现运载火箭一子级可控回收/a-77909061">中国首次实现运载火箭一子级可控回收</a></li>
<li><a href="https://sputniknews.cn/20260710/1072272257.html">中国首次成功实施运载火箭一子级可控回收 - 2026年7月10日, 俄罗斯卫星通讯社</a></li>

</ul>
</details>

**标签**: `#aerospace`, `#rocketry`, `#space exploration`, `#reusable rocket`, `#China`

---