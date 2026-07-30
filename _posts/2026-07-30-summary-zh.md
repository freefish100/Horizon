---
layout: default
title: "Horizon Summary: 2026-07-30 (ZH)"
date: 2026-07-30
lang: zh
---

> 从 40 条内容中筛选出 12 条重要资讯。

---

1. [开源引擎在 M 系列 Mac 上仅用 2GB 内存运行 Gemma 4 26B 模型](#item-1) ⭐️ 9.0/10
2. [俄联邦安全局指控 Telegram 创始人杜罗夫协助恐怖活动](#item-2) ⭐️ 9.0/10
3. [AI 初创公司减少论文发表，透明度堪忧](#item-3) ⭐️ 8.0/10
4. [米切尔·桥本创立 Superlogical](#item-4) ⭐️ 8.0/10
5. [AI 蠕虫利用提示注入攻击微软 Copilot for Word](#item-5) ⭐️ 8.0/10
6. [长政策文件无法可靠地管理 AI 代理](#item-6) ⭐️ 8.0/10
7. [Matthew Green 称后量子密码转型正需 AI](#item-7) ⭐️ 8.0/10
8. [使用 ncnn 和 Vulkan 实现边缘设备上供应商无关的 ML 推理](#item-8) ⭐️ 8.0/10
9. [Hugging Face 被大量用于生成深度伪造裸照](#item-9) ⭐️ 8.0/10
10. [月之暗面寻求 20 亿美元融资，估值达 300 亿美元](#item-10) ⭐️ 8.0/10
11. [中国起草反网络暴力法，针对 AI 生成网暴](#item-11) ⭐️ 8.0/10
12. [OpenAI 向 10 万学者免费开放 GPT-5.6 模型](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [开源引擎在 M 系列 Mac 上仅用 2GB 内存运行 Gemma 4 26B 模型](https://github.com/drumih/turbo-fieldfare) ⭐️ 9.0/10

TurboFieldfare 是一个用 Swift 和 Metal 编写的全新开源推理引擎，通过仅从 SSD 流式传输路由专家，在任意 M 系列 Mac 上以约 2GB 内存运行 4 位量化后的 Gemma 4 26B MoE 模型。在 8GB M2 MacBook Air 上达到 5-6 token/秒，在 M5 MacBook Pro 上达到 31-35 token/秒。 这一突破使得大型混合专家模型能在内存有限的设备上运行，将此前需要高端硬件的设备端 AI 普及化。它可能激发更多内存高效推理技术的研究，并扩大本地 AI 在笔记本电脑和边缘设备上的实际应用。 模型的 4 位权重约占用 14GB，但引擎将共享层和 KV 缓存保留在 RAM 中，同时通过有界并行 pread 和专家缓存仅从 SSD 流式传输所需专家。它还包含一个实验性的 OpenAI 兼容本地服务器，支持流式输出和工具调用。

hackernews · gitpusher42 · 7月29日 15:05 · [社区讨论](https://news.ycombinator.com/item?id=49098510)

**背景**: 混合专家（MoE）模型使用多个专门的子网络（专家）和一个门控网络，仅为每个输入激活相关专家，从而减少计算量。KV 缓存存储先前 token 的键值对，避免生成过程中重复计算。4 位量化将模型权重压缩为每个参数 4 位，大幅降低内存占用且准确性损失极小。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>
<li><a href="https://medium.com/@minh.hoque/understanding-kv-caching-in-transformers-729271c9b74a">Understanding KV Caching in Transformers - Medium</a></li>
<li><a href="https://www.emergentmind.com/topics/4-bit-model-quantization">4-Bit Model Quantization</a></li>

</ul>
</details>

**社区讨论**: 社区表达了兴奋并指出其实际影响，有用户报告在 64GB M4 Max 上达到 48 token/秒。有人将其与 llama.cpp 的 mmap 方法进行技术比较，开发者进行了回应。一位贡献者还提供了针对较旧 macOS 版本的构建修复。

**标签**: `#inference`, `#on-device AI`, `#Gemma`, `#Mac`, `#SSD streaming`

---

<a id="item-2"></a>
## [俄联邦安全局指控 Telegram 创始人杜罗夫协助恐怖活动](https://www.interfax.ru/russia/1106228) ⭐️ 9.0/10

7 月 29 日，俄罗斯联邦安全局（FSB）依据《刑法》第 205.1 条指控 Telegram 创始人帕维尔·杜罗夫协助恐怖活动，并将其列入国际通缉名单。 这一指控加剧了俄罗斯当局与这款流行通讯平台之间的冲突，可能开创将科技公司高管对用户生成内容承担刑事责任的先例，对平台责任和言论自由产生全球影响。 FSB 指控 Telegram 管理层拒绝删除被乌克兰情报机构及恐怖组织用于协调破坏、袭击、大规模杀戮和诈骗的频道、群组和机器人，造成人员伤亡和数十亿卢布损失。

telegram · zaihuapd · 7月29日 05:56

**背景**: Telegram 是一款以强大加密和隐私功能闻名的广泛使用的通讯应用。它曾因内容审核问题受到多国政府审视，包括此前俄罗斯因拒绝提供解密密钥而对其处以罚款。本次指控针对创始人个人发出国际通缉，标志着事态的严重升级。

**标签**: `#Telegram`, `#Pavel Durov`, `#Security`, `#Legal`, `#Geopolitics`

---

<a id="item-3"></a>
## [AI 初创公司减少论文发表，透明度堪忧](https://www.science.org/content/article/ai-s-top-startups-are-barely-publishing-their-research) ⭐️ 8.0/10

最新报告显示，领先的 AI 初创公司发表的论文数量大幅减少，标志着开放科学的转变。 这种下降威胁到 AI 研究的透明度和可重复性，可能减缓科学进步并阻碍同行评审。 尽管出版物减少，OpenAI 在初创公司中的累计引用量仍居首位。该论文还指出，谷歌等公司因非独角兽而被排除在外。

hackernews · YeGoblynQueenne · 7月29日 21:25 · [社区讨论](https://news.ycombinator.com/item?id=49103285)

**背景**: AI 研究历史上是开放的，像 NeurIPS 这样的会议和 arXiv 上的预印本促进了快速传播。然而，随着 AI 初创公司面临商业压力，许多选择将工作保密以保持竞争优势。这一趋势引发了对该领域验证发现和基于先前工作建立能力的担忧。

**社区讨论**: 评论者分享了不同的经历：一位指出发表论文导致被顶级期刊拒绝，另一位为避免被 OpenAI 和 Anthropic 抄袭而选择不发表。有人担心 AI 研究的“博客化”使得未经支持的声明得以传播。

**标签**: `#AI`, `#research`, `#startups`, `#publishing`, `#transparency`

---

<a id="item-4"></a>
## [米切尔·桥本创立 Superlogical](https://www.superlogical.com/) ⭐️ 8.0/10

米切尔·桥本宣布成立新公司 Superlogical，该公司将基于开源库 libghostty 构建终端应用，而 Ghostty 本身已移交给非营利组织。 此举验证了一种新颖的商业模式：公司在社区维护的开源核心之上构建专有产品，可能影响开源项目的自我维持方式。 Superlogical 将使用与其他消费者相同的 MIT 许可组件，并继续向上游贡献共享终端工作。首个 libghostty 组件 libghostty-vt 提供了一个零依赖 API，用于终端序列解析和状态管理。

hackernews · yan · 7月29日 15:41 · [社区讨论](https://news.ycombinator.com/item?id=49098965)

**背景**: Ghostty 是一个用 Zig 编写的现代终端模拟器，libghostty 是其 C 兼容库，可嵌入其他应用中实现终端仿真。通过将 libghostty 独立为 MIT 许可库，桥本让其他人无需重新发明轮子即可构建终端工具。Superlogical 旨在成为 libghostty 的一个消费者，专注于终端产品。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mitchellh.com/writing/libghostty-is-coming">Libghostty Is Coming – Mitchell Hashimoto</a></li>
<li><a href="https://github.com/Uzaaft/awesome-libghostty">GitHub - Uzaaft/awesome-libghostty</a></li>
<li><a href="https://docsmith.aigne.io/docs/ghostty/en/libghostty-ed730d">libghostty API - docsmith.aigne.io</a></li>

</ul>
</details>

**社区讨论**: 评论者大多称赞开源治理模式，simonw 强调了将 Ghostty 移交给非营利组织。一些人将其与 OLE/COM 相提并论，少数人批评标题晦涩有标题党之嫌。总体情绪积极，对该商业模式感兴趣。

**标签**: `#announcement`, `#open source`, `#terminal`, `#company`, `#Mitchell Hashimoto`

---

<a id="item-5"></a>
## [AI 蠕虫利用提示注入攻击微软 Copilot for Word](https://enklypesalt.com/posts/context-collapse-part3-ai-worming-through-word/) ⭐️ 8.0/10

研究者 Håkon Måløy 开发了一个概念验证 AI 蠕虫，通过将恶意提示以白色隐藏文字嵌入文档，利用 Microsoft Copilot for Word 自我复制传播，首次在主流办公软件中展示了文档型 AI 蠕虫。 这一漏洞揭示了 AI 代理在混合指令与数据时存在的严重安全问题，蠕虫可能自主窃取数据、篡改文档并在组织间传播，对企业采用 AI 构成重大威胁。 攻击使用白色文本结合超链接或嵌入提示，对人眼不可见但 Copilot 可读，并通过指示 Copilot 将相同提示写入新文档实现传播。

hackernews · Canopy9560 · 7月29日 11:44 · [社区讨论](https://news.ycombinator.com/item?id=49096188)

**背景**: 提示注入攻击利用了大型语言模型无法区分系统指令和用户提供数据的缺陷。当 Copilot 等 AI 代理拥有文档写入权限时，嵌入的指令可导致代理执行未授权操作。本研究基于已知的间接提示注入技术，但首次在商业 LLM 应用中展示了自我复制蠕虫。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://enklypesalt.com/posts/context-collapse-part3-ai-worming-through-word/">Context Collapse, Part 3 - AI Worming through Word | En Klype Salt</a></li>
<li><a href="https://windowsnews.ai/article/after-144-days-microsoft-still-cant-fully-fix-copilot-vulnerability-that-lets-hidden-text-manipulate.440856">After 144 Days, Microsoft Still Can't Fully Fix Copilot Vulnerability That Lets Hidden Text Manipulate Reports - Windows News</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了震惊与怀疑，rwmj 指出指令与数据混合是不可修复的缺陷，boothby 预测情况会进一步恶化。simonw 表示担忧，averagjoe 称已卸载 Copilot 避免此类攻击。piker 指出白色隐藏文字方法仍然有效并分享了相关链接。

**标签**: `#security`, `#AI`, `#worms`, `#prompt injection`, `#Microsoft Copilot`

---

<a id="item-6"></a>
## [长政策文件无法可靠地管理 AI 代理](https://arxiv.org/abs/2607.25398) ⭐️ 8.0/10

一篇名为'Handbook.md'的新论文表明，由于上下文窗口限制和模型量化问题，长政策文档无法可靠地指导 AI 代理。 这一发现挑战了详细书面政策能确保 AI 行为负责任的假设，引发了在现实应用中部署 AI 代理的担忧。 研究强调，即使声称拥有 100 万 token 上下文窗口的模型，在极端量化和不佳采样下也会失败，导致代理在几分钟交互后忽略早期指令。

hackernews · spIrr · 7月29日 13:01 · [社区讨论](https://news.ycombinator.com/item?id=49096969)

**背景**: 语言模型具有有限的上下文窗口，类似于工作记忆，限制了它们一次能处理的文本量。模型量化通过降低精度来提高效率，但可能会降低性能。这些因素共同削弱了代理遵循长政策的能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Context_window">Context window - Wikipedia</a></li>
<li><a href="https://developer.nvidia.com/blog/model-quantization-concepts-methods-and-why-it-matters/">Model Quantization: Concepts, Methods, and Why It Matters</a></li>

</ul>
</details>

**社区讨论**: 评论者大多同意论文的发现，有人指出本地推理可以缓解问题，而另一人指出人类也难以遵循长政策。一位有 Claude 经验的用户报告称，CLAUDE.md 文件中的指令很快被绕过，表明该问题很普遍。

**标签**: `#AI`, `#LLM`, `#long context`, `#agents`, `#policy compliance`

---

<a id="item-7"></a>
## [Matthew Green 称后量子密码转型正需 AI](https://simonwillison.net/2026/Jul/29/matthew-green/#atom-everything) ⭐️ 8.0/10

著名密码学家 Matthew Green 指出，从传统公钥算法向后量子算法的历史性转型为 AI 参与密码分析创造了绝佳时机。他认为这既能验证新标准，也可能暴露根本性缺陷，从而使密码分析文献更加充实。 这一见解凸显了抗量子密码学与先进 AI 的交汇，可能增强对新密码学问题的信心，也可能彻底颠覆它们。其结果将影响未来数字基础设施的安全以及加密技术对抗量子威胁的韧性。 Green 特别提到了 HAWK 方案——NIST 附加后量子签名竞赛中的格基候选方案，并引用了 Impagliazzo 的五个世界理论，尤其是公钥密码可能不存在的 Minicrypt 世界。他还提及了 Anthropic 近期在 AI 驱动密码分析方面的工作。

rss · Simon Willison · 7月29日 18:18

**背景**: 公钥密码学是安全在线通信的基础，但量子计算机威胁着 RSA 和 ECC 等算法。NIST 正主导为期多年的后量子算法标准化工作，HAWK 是数字签名候选之一。Impagliazzo 的五个世界理论是基于计算困难假设对可能密码学现实的分类。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://csrc.nist.gov/csrc/media/Projects/pqc-dig-sig/documents/round-1/spec-files/hawk-spec-web.pdf">HAWK Specification Document - NIST Computer Security Resource ...</a></li>
<li><a href="https://fanpu.io/blog/2022/impagliazzos-five-worlds/">Impagliazzo 's Five Worlds , or The Computational... | Fan Pu Zeng</a></li>
<li><a href="https://thehackernews.com/2026/07/claude-ai-just-cracked-post-quantum.html">Claude AI Just Cracked a Post-Quantum Test Scheme and Found a ...</a></li>

</ul>
</details>

**标签**: `#post-quantum cryptography`, `#AI cryptanalysis`, `#cryptography transition`, `#Matthew Green`

---

<a id="item-8"></a>
## [使用 ncnn 和 Vulkan 实现边缘设备上供应商无关的 ML 推理](https://www.reddit.com/r/MachineLearning/comments/1v9s4mz/vendoragnostic_ml_inference_on_production_edge/) ⭐️ 8.0/10

视频编辑工具 PostSlate 使用 ncnn 及其 Vulkan 后端在生产级边缘设备上运行 ML 模型，相比 ONNX CPU 推理实现了高达 10 倍的加速，同时避免了 CUDA 等供应商特定的运行时。 这种方法实现了跨平台的 ML 推理，无需用户安装特定供应商的驱动或运行时，简化了在生产环境中跨多种 GPU 硬件（NVIDIA、AMD、Intel、Apple Silicon）的部署。 在 NVIDIA 4070 上使用 fp16，ArcFace R50 人脸嵌入耗时 3 毫秒（ONNX CPU 为 30 毫秒），SCRFD 人脸检测耗时 2.5 毫秒（ONNX CPU 为 25 毫秒）。模型大小也从 174 MB（ONNX fp32）减少到 87 MB（ncnn fp16）。

reddit · r/MachineLearning · /u/ppchaos · 7月29日 10:22

**背景**: ncnn 是腾讯开发的高性能神经网络推理框架，专为移动和边缘平台设计。它支持 CPU 和 Vulkan GPU 后端，无需第三方运行时依赖。Vulkan API 是一个跨平台的图形和计算标准，提供底层 GPU 访问，使其适合供应商无关的 ML 加速。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/Tencent/ncnn">Tencent/ ncnn : ncnn is a high-performance neural network inference ...</a></li>
<li><a href="https://www.phoronix.com/news/NVIDIA-Vulkan-AI-ML-Success">NVIDIA Is Finding Great Success With Vulkan Machine Learning ...</a></li>

</ul>
</details>

**标签**: `#ML inference`, `#Vulkan`, `#edge devices`, `#ncnn`, `#cross-platform`

---

<a id="item-9"></a>
## [Hugging Face 被大量用于生成深度伪造裸照](https://www.theverge.com/ai-artificial-intelligence/971723/hugging-face-nudify-deepfake-undress-women-children) ⭐️ 8.0/10

这突显了开源 AI 平台在伦理和安全方面的严重漏洞，可能导致广泛的滥用和伤害，尤其是对弱势群体，并呼吁加强内容审核和平台责任。 该报告使用蜜罐在 7 天内收到超过 1000 条请求，并发现排名前九的图像编辑模型中有七个能通过简单提示轻松为女性“脱衣”，无需精心构造绕过话术。

telegram · zaihuapd · 7月29日 08:20

**背景**: Hugging Face 是一个流行的开源平台，用于托管和共享机器学习模型，被开发者广泛使用。深度伪造指利用 AI 生成的合成媒体，用于操纵图像或视频，常被恶意用于制作非自愿的色情内容。该报告强调了此类平台缺乏足够的安全防护措施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hugging_Face">Hugging Face</a></li>
<li><a href="https://en.wikipedia.org/wiki/Deepfake">Deepfake</a></li>

</ul>
</details>

**标签**: `#AI Ethics`, `#Deepfake`, `#Hugging Face`, `#Content Moderation`, `#AI Safety`

---

<a id="item-10"></a>
## [月之暗面寻求 20 亿美元融资，估值达 300 亿美元](https://t.me/zaihuapd/42845) ⭐️ 8.0/10

月之暗面（Moonshot AI），Kimi 聊天机器人的开发商，正寻求至多 20 亿美元的新融资，目标估值 300 亿美元，这已是其六个月内第三轮融资。 这种快速的估值增长和强劲收入表明，中国 AI 初创公司正在获得显著市场动力，挑战全球竞争对手并吸引大量投资。 该公司 4 月份的年度经常性收入（ARR）突破 2 亿美元，同时推出了通用 AI 代理 Kimi Work，并正在筹备香港上市。

telegram · zaihuapd · 7月29日 10:12

**背景**: 年度经常性收入（ARR）是订阅制业务的关键指标，代表每年可预期的经常性收入。通用 AI 代理是指能够自主执行多种任务的 AI 系统，与专门的聊天机器人有所区别。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.lightercapital.com/blog/what-is-arr-annual-recurring-revenue-definition-formula">What is Annual Recurring Revenue ( ARR ) in SaaS ?</a></li>
<li><a href="https://www.ibm.com/think/topics/ai-agents">What Are AI Agents ? | IBM</a></li>

</ul>
</details>

**标签**: `#AI startup`, `#funding`, `#Moonshot AI`, `#Kimi chatbot`, `#valuation`

---

<a id="item-11"></a>
## [中国起草反网络暴力法，针对 AI 生成网暴](https://mp.weixin.qq.com/s/PrzKFhbwjgFEGBPADvFD6Q) ⭐️ 8.0/10

2026 年 7 月 29 日，国家互联网信息办公室公布反网络暴力法征求意见稿，其中专门规制利用 AI 技术制作、传播网络暴力信息的行为。 这标志着全球首批明确规制 AI 生成网络暴力的主要法律框架之一，为网络治理和 AI 监管树立先例。可能影响平台部署 AI 工具的方式以及受害者寻求法律救济的途径。 草案共七章六十条，明确网络暴力为侵害名誉权、隐私权、肖像权、个人信息等的行为。草案压实平台监测和防护责任，并引入人格权侵害禁令和精神损害赔偿等司法保护措施。

telegram · zaihuapd · 7月29日 10:59

**背景**: 网络暴力在中国社交媒体上日益普遍，而 deepfake 等 AI 工具可能加剧危害。中国当局一直在加强网络内容监管，此次草案将现有保护扩展至专门覆盖 AI 生成的侵害行为。机器学习、deepfake 检测等技术手段对于法律执行具有相关性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.igi-global.com/chapter/ai-based-cyberbullying-detection-techniques-and-strategies/369055">AI -Based Cyberbullying Detection Techniques and Strategies</a></li>
<li><a href="https://journal.ut.ac.ir/article_99050_7cf51958e1c400d52e8a8e52372bee45.pdf">Artificial Intelligence-Driven Cyberbullying Detection : A Survey of</a></li>
<li><a href="https://danaya.tech/seo/deepfake-detection/social-media">Deepfake Detection for Social Media | Danaya</a></li>

</ul>
</details>

**标签**: `#AI regulation`, `#cyberbullying`, `#China law`, `#online governance`

---

<a id="item-12"></a>
## [OpenAI 向 10 万学者免费开放 GPT-5.6 模型](https://openai.com/index/chatgpt-for-academic-researchers/) ⭐️ 8.0/10

OpenAI 于 2026 年 7 月 29 日宣布推出 ChatGPT for Academic Researchers 项目，计划在 2027 年前向全球 10 万名学术研究人员免费提供其前沿的 GPT-5.6 模型，首批 1 万个名额于今年夏天开放。 这一举措可能通过消除成本障碍，大幅加速多个学科的科学发现，使研究人员能够利用前沿 AI 进行基因组分析、蛋白质建模和文献综述等任务，总投资达 2.5 亿美元。 符合条件的学位授予机构的研究人员可邀请最多 4 位机构合作者，工作区默认不将数据用于模型训练；申请人需验证机构身份并提交研究计划。

telegram · zaihuapd · 7月30日 00:17

**背景**: GPT-5.6 于 2026 年 7 月发布，是 OpenAI 最强大的网络安全和科学推理模型，在编程、知识工作和科学领域取得了最先进的结果，同时效率更高。该项目是 OpenAI 到 2027 年投入超 2.5 亿美元支持外部科研的承诺的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/chatgpt-for-academic-researchers/">Accelerating scientific discovery with ChatGPT for Academic ...</a></li>
<li><a href="https://www.axios.com/2026/07/29/openai-academics-research-chatgpt-sol">OpenAI launches free AI access program for academic researchers</a></li>
<li><a href="https://openai.com/index/gpt-5-6/">GPT‑5.6: Frontier intelligence that scales with your ambition</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#AI for Science`, `#Academic Research`, `#GPT-5`, `#Funding`

---