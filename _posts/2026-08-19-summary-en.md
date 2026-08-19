---
layout: default
title: "Horizon Summary: 2026-08-19 (EN)"
date: 2026-08-19
lang: en
---

> From 31 items, 7 important content pieces were selected

---

1. [Mojo programming language goes open source under Apache 2 license](#item-1) ⭐️ 9.0/10
2. [Amazon's Ad Model Taxes Consumer Trust, Godin Argues](#item-2) ⭐️ 8.0/10
3. [Train Movement Turns Railway into a Flatbed Scanner](#item-3) ⭐️ 8.0/10
4. [Recovering a bricked AMD 7040 Framework 13 with $20 tools](#item-4) ⭐️ 8.0/10
5. [China Orders Some Agencies to Uninstall Custom Windows 10 Early](#item-5) ⭐️ 8.0/10
6. [Chinese Domestic AI Chips to Supply ~90% of Market by 2026](#item-6) ⭐️ 8.0/10
7. [Long March 10B Achieves World's First Net-Based Sea Recovery](#item-7) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Mojo programming language goes open source under Apache 2 license](https://simonwillison.net/2026/Aug/18/mojo-is-now-open-source/) ⭐️ 9.0/10

Modular released the Mojo compiler and toolchain under an Apache 2 license on August 18, 2026, following the Mojo 1.0 release last week. This fulfills the open-source commitment first made when Mojo was announced in May 2023. Open-sourcing Mojo is a major milestone that allows developers to inspect, modify, and contribute to the compiler, boosting trust and adoption for AI and GPU programming. It also marks a strategic shift from a proprietary tool to a community-driven language in a competitive landscape. Mojo was originally intended to be a superset of Python, but around August 2025 Modular revised that goal, allowing the language to evolve independently while remaining Python-inspired. The compiler is built on the MLIR compiler framework rather than directly on LLVM, which helps it target CPUs, GPUs, TPUs, and other accelerators.

rss · Simon Willison · Aug 18, 21:39

**Background**: Mojo is a systems programming language developed by Modular for high-performance AI infrastructure, combining Python-like syntax with low-level features such as static typing and a borrow checker. It uses MLIR, a modern compiler framework, to generate efficient code across heterogeneous hardware. The language has been proprietary since its May 2023 announcement, and the open-source release has been a key community demand.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_(programming_language)">Mojo (programming language)</a></li>
<li><a href="https://mojolang.org/">Mojo - Modular</a></li>

</ul>
</details>

**Tags**: `#mojo`, `#open-source`, `#programming-language`, `#compiler`, `#modular`

---

<a id="item-2"></a>
## [Amazon's Ad Model Taxes Consumer Trust, Godin Argues](https://seths.blog/2026/08/the-amazon-tax/) ⭐️ 8.0/10

Seth Godin published an essay titled 'The Amazon tax' arguing that Amazon's advertising model functions as a tax on consumer trust. The piece ignited a Hacker News discussion with 903 points and 526 comments. This matters because it highlights the broader industry trend of ad-driven platform decay, where platforms increasingly prioritize advertising revenue over user experience. It affects consumers, sellers, and the long-term trustworthiness of e-commerce marketplaces. Commenters raised potential legal avenues such as trademark infringement and fraud when Amazon shows competitor ads for branded search queries. The debate also contrasts Amazon's model with other ad-supported environments like subways, television, and restaurant menus.

hackernews · herbertl · Aug 18, 13:22 · [Discussion](https://news.ycombinator.com/item?id=49345263)

**Background**: Amazon is a dominant e-commerce platform where product search results now include sponsored ads. Godin's 'tax' metaphor suggests that consumers pay a hidden cost in attention and trust when ads distract from their intended purchases. This is part of a wider conversation about how platforms monetize user attention and whether that undermines their core value proposition.

**Discussion**: Commenters were divided: some suggested legal action against Amazon for serving competitor ads on trademarked searches, while others argued such ads could be relevant and beneficial to consumers. A recurring theme was that advertising ruining platforms is a familiar pattern seen in subways, TV, and elsewhere, not unique to Amazon.

**Tags**: `#Amazon`, `#Advertising`, `#E-commerce`, `#Platform Economics`, `#Consumer Trust`

---

<a id="item-3"></a>
## [Train Movement Turns Railway into a Flatbed Scanner](https://philo.gay/linecam/) ⭐️ 8.0/10

The project Linecam uses a train's movement and a stationary camera to create slit-scan images, effectively turning the railway network into a massive flatbed scanner. It is a novel creative-coding experiment that combines photography, computer vision, and hardware. This experiment demonstrates how everyday infrastructure can be repurposed as an imaging device, offering a fresh artistic perspective on train travel. It may inspire further motion-based imaging techniques and creative coding projects. The technique relies on slit-scan photography: a stationary camera captures consecutive narrow strips of the passing scene while the train's forward motion provides the scanning movement. The resulting images compress time and space along the track's axis.

hackernews · otherayden · Aug 18, 12:43 · [Discussion](https://news.ycombinator.com/item?id=49344825)

**Background**: Slit-scan photography is a photographic process where a slit is used to expose only a narrow line of the image at a time, often used in panoramic and photo-finish cameras. In this project, the train's motion acts as the scan mechanism, and the fixed camera on board records the scene line by line. The result is a flattened, elongated view of the railway corridor.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Slit-scan_photography">Slit-scan photography</a></li>
<li><a href="https://thelawlers.com/Blognosticator/?p=2519">Spinning time into gold with slit - scan images | thelawlers.com</a></li>

</ul>
</details>

**Discussion**: Community members shared related experiments, including a similar 2008 setup with an iSight camera, manually spliced animations, and a web-based slit-scan tool. Some commented that the unexpected 'error' shots are subjectively more interesting than the standard captures.

**Tags**: `#slit-scan`, `#photography`, `#creative-coding`, `#computer-vision`, `#hardware`

---

<a id="item-4"></a>
## [Recovering a bricked AMD 7040 Framework 13 with $20 tools](https://quantum5.ca/2026/08/16/fixing-bricked-amd-7040-series-framework-13-laptop-with-20-tools/) ⭐️ 8.0/10

A new technical guide details how the author recovered an AMD 7040-series Framework Laptop 13 that had been bricked by a faulty BIOS update, using roughly $20 worth of tools. The write-up walks through the recovery step by step, including the use of pogo pins to reach the BIOS flash chip because the model lacks a populated flashing header. This matters because a failed firmware update can turn an otherwise working laptop into e-waste, and this guide offers a low-cost recovery path that individual owners and repair shops can follow. It also fuels the ongoing debate over firmware update risks, right to repair, and whether manufacturers should be held liable for faulty updates. The recovery required pogo pins and an external programmer rather than a simple connector, because Framework does not populate a dedicated BIOS flashing header on this model. The guide stands out for documenting a common but often underdocumented repair; commenters also note that Framework's own open-source debugger tooling exists but its connector is left unpopulated on production boards to cut costs.

hackernews · jp_sc · Aug 18, 13:18 · [Discussion](https://news.ycombinator.com/item?id=49345220)

**Background**: Framework Computer is an American laptop maker known for modular, repairable designs and a strong right-to-repair stance; its Framework Laptop 13 launched in 2021. A 'bricked' device is one that has become as useful as a brick, often because a failed BIOS or firmware update corrupted the low-level code needed to boot. Recovering such a device usually requires an external programmer to rewrite the flash chip outside the normal update path.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Framework_Computer">Framework Computer - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Framework_Laptop">Framework Laptop</a></li>
<li><a href="https://timvsaedlex.wordpress.com/2012/10/16/what-does-bricking-a-device-mean/">What Does “ Bricking ” a Device Mean ? | timvsaedlex</a></li>

</ul>
</details>

**Discussion**: Commenters are broadly critical of manufacturer practices: one user argues Framework should be legally liable for faulty BIOS updates and suggests taking the case to small-claims court, while another shares a similar bricking experience with a ThinkPad and says PC makers "really don't care." Others call for official updates to extend warranties and criticize Framework's cost-cutting omission of a flashing header. At least one user says the article makes them regret buying a Framework laptop.

**Tags**: `#hardware`, `#firmware`, `#BIOS`, `#laptop repair`, `#Framework`

---

<a id="item-5"></a>
## [China Orders Some Agencies to Uninstall Custom Windows 10 Early](https://www.bloomberg.com/news/articles/2026-08-18/china-axing-microsoft-windows-from-state-agencies-ahead-of-plan) ⭐️ 8.0/10

China's Ministry of State Security has ordered some government agencies to uninstall the customized Windows 10 ahead of the original February 2027 cutoff, moving the deadline up by several months. The move is driven by data security concerns, though no specific vulnerability was cited. The accelerated phase-out signals a deepening push by Beijing to reduce reliance on foreign technology in government IT. It could affect Microsoft's government business in China and boost domestic operating system vendors. The directive applies to the Windows 10 China Government Edition, a custom version developed with China Electronics Technology Group. Microsoft said it has found no security incidents affecting the product and that the OS continues to receive regular security updates.

telegram · zaihuapd · Aug 18, 06:22

**Background**: Windows 10 China Government Edition was announced in 2017, built by Microsoft and CETC through their joint venture CMIT for Chinese government customers. The Chinese government has been steadily moving toward domestic software alternatives amid broader U.S.-China tech tensions and data sovereignty concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://blogs.windows.com/windowsexperience/2017/05/23/announcing-windows-10-china-government-edition-new-surface-pro/">Announcing Windows 10 China Government Edition and the new...</a></li>
<li><a href="https://www.partitionwizard.com/news/windows-10-china-government-edition.html">Windows 10 China Government Edition : An Impactful Version</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#government policy`, `#Microsoft Windows`, `#China`

---

<a id="item-6"></a>
## [Chinese Domestic AI Chips to Supply ~90% of Market by 2026](https://www.tomshardware.com/tech-industry/artificial-intelligence/chinas-homegrown-ai-accelerators-to-supply-90-percent-of-the-countrys-domestic-market-analysts-suggest-cambricon-and-huawei-expected-to-be-the-biggest-winners-in-the-shift-away-from-nvidia-and-amd) ⭐️ 8.0/10

TrendForce projects that Chinese domestic AI accelerators will supply nearly 90% of China's market by 2026, up from 45% last year. Cambricon and Huawei are expected to be the biggest beneficiaries of this shift away from Nvidia and AMD. This projected market shift reflects China's drive for semiconductor self-sufficiency amid US export controls, and could reshape the global AI chip competitive landscape. Huawei and Cambricon stand to gain significant market share and revenue, while Nvidia and AMD face shrinking access to China. In 2025, Nvidia held 55% of the Chinese market with 2.2 million units shipped, while Huawei shipped 812,000 units for a 20.3% share. To achieve the projection, China must increase high-end AI chip production by 2.2 times to roughly 1.96 million units within a year, raising questions about manufacturing capacity.

telegram · zaihuapd · Aug 18, 13:03

**Background**: AI accelerators are specialized hardware designed to speed up AI and machine learning workloads, such as neural networks and matrix operations. Cambricon is a Beijing-based, partially state-owned company that designs AI processors and general-purpose GPUs, often compared to Nvidia. Huawei's Ascend AI chips are also key domestic alternatives. US export controls restricting Nvidia and AMD from selling their most advanced chips to China have accelerated Chinese efforts to develop homegrown solutions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_accelerator">AI accelerator</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cambricon_Technologies">Cambricon Technologies</a></li>

</ul>
</details>

**Tags**: `#AI chips`, `#Huawei`, `#Cambricon`, `#semiconductor`, `#china-tech`

---

<a id="item-7"></a>
## [Long March 10B Achieves World's First Net-Based Sea Recovery](https://t.me/zaihuapd/43264) ⭐️ 8.0/10

On July 10, 2026, the Long March 10B rocket lifted off from the Hainan Commercial Space Launch Site. About six minutes after stage separation, its first stage made a controlled vertical return and was successfully captured by a net-based recovery system on an offshore platform, marking China's first controlled recovery of a rocket first stage and the world's first net-based recovery. This milestone makes China the second country after the United States to master large-thrust reusable rocket technology. The net-based recovery approach eliminates heavy landing legs, reducing structural mass and launch costs, which could significantly benefit commercial satellite constellation deployment. The Long March 10B is a 5-meter-diameter two-stage liquid rocket with a liftoff thrust of about 890 tons and liftoff mass of about 760 tons. Its core first stage uses liquid oxygen/kerosene propellants, the second stage uses liquid oxygen/methane, and in reusable mode it delivers 16 tons to low Earth orbit. The net-based recovery expands the capture window and improves buffering success without adding landing gear.

telegram · zaihuapd · Aug 19, 00:16

**Background**: Reusable rockets cut launch costs by recovering and reflying the most expensive stage. SpaceX's Falcon 9 pioneered propulsive landing on droneships, while China's Long March 10B uses a novel net capture on an offshore platform that avoids landing legs and trims dry mass. The rocket was developed by the China Academy of Launch Vehicle Technology, and the first flight verified technologies such as propellant management with baffled tanks, multiple engine restarts, high-altitude ignition, and high-precision navigation. The team plans to complete a first-stage reuse flight by the end of 2026.

<details><summary>References</summary>
<ul>
<li><a href="https://news.qq.com/rain/a/20260710A05V3Y00">成功！我国首次实现火箭一子级可控回收，预计年底前完成复用飞行_腾讯新闻</a></li>
<li><a href="https://www.dw.com/zh/中国首次实现运载火箭一子级可控回收/a-77909061">中国首次实现运载火箭一子级可控回收</a></li>
<li><a href="https://sputniknews.cn/20260710/1072272257.html">中国首次成功实施运载火箭一子级可控回收 - 2026年7月10日, 俄罗斯卫星通讯社</a></li>

</ul>
</details>

**Tags**: `#aerospace`, `#rocketry`, `#space exploration`, `#reusable rocket`, `#China`

---