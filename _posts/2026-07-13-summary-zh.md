---
layout: default
title: "Horizon Summary: 2026-07-13 (ZH)"
date: 2026-07-13
lang: zh
---

> 从 31 条内容中筛选出 6 条重要资讯。

---

1. [GPT-5.6 一小时攻克 50 年图论猜想](#item-1) ⭐️ 10.0/10
2. [xAI Grok CLI 默认上传整个代码库及密钥文件](#item-2) ⭐️ 9.0/10
3. [中国批准全球首款侵入式脑机接口医疗器械](#item-3) ⭐️ 9.0/10
4. [Chromium 148 的 Math.tanh 可实现操作系统指纹识别](#item-4) ⭐️ 8.0/10
5. [陶哲轩用 LLM 编码代理构建应用](#item-5) ⭐️ 8.0/10
6. [我爱大模型，我恨炒作](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [GPT-5.6 一小时攻克 50 年图论猜想](https://www.qbitai.com/2026/07/447873.html) ⭐️ 10.0/10

GPT-5.6 Sol Ultra 在不到一小时内自主证明了图论中悬而未决 50 年之久的循环双覆盖猜想，并生成了一份 3 页的 PDF 证明文件。 这一成就标志着人工智能驱动数学研究的重大里程碑，表明大型语言模型能够自主解决复杂的长期悬而未决的猜想。它可能加速数学领域的进展，并激发新的 AI 辅助发现方法。 该模型使用了 64 个子 agent 并行工作，将问题转化为有限域上的边标号和线性方程组问题。OpenAI 还公布了完整的提示词（约 700 个字符），其中明确了验收标准、定义、边界条件和失败情形，但没有规定固定的解题步骤。

telegram · zaihuapd · 7月12日 03:49

**背景**: 循环双覆盖猜想由 W. T. Tutte 等人提出，询问是否每个无桥图都存在一组圈，使得每条边恰好出现两次。这是图论中的一个核心问题，与图嵌入和多面体理论有关。过去五十年的尝试未能给出证明。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cycle_double_cover_conjecture">Cycle double cover conjecture</a></li>

</ul>
</details>

**标签**: `#AI`, `#Mathematics`, `#Graph Theory`, `#GPT`, `#Breakthrough`

---

<a id="item-2"></a>
## [xAI Grok CLI 默认上传整个代码库及密钥文件](https://gist.github.com/cereblab/dc9a40bc26120f4540e4e09b75ffb547) ⭐️ 9.0/10

此隐私漏洞会暴露开发者的完整代码库和密钥，可能导致数据泄露和知识产权盗窃，影响尤为严重的是，该工具被许多 AI 开发社区广泛使用。 该工具会将文件内容嵌入模型对话请求发送，并独立创建一个完整仓库的 git bundle 进行上传，与提示词无关。测试中，12 GB 的仓库有超过 5 GiB 数据被成功上传且无存储端拒绝，一个被明确指令“不要打开”的文件仍可在上传包中完整恢复。

telegram · zaihuapd · 7月12日 04:19

**背景**: Git bundle 是 Git 的一个命令，可将整个仓库打包成一个文件以便离线传输。Google Cloud Storage 是一个可扩展的对象存储服务。xAI 的 Grok CLI 是一个与 Grok AI 模型交互的命令行工具，常被开发者用于编码辅助。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://git-scm.com/docs/git-bundle">Git - git-bundle Documentation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Google_Cloud_Storage">Google Cloud Storage</a></li>

</ul>
</details>

**标签**: `#security`, `#privacy`, `#xAI`, `#Grok CLI`, `#data leakage`

---

<a id="item-3"></a>
## [中国批准全球首款侵入式脑机接口医疗器械](https://t.me/zaihuapd/42515) ⭐️ 9.0/10

国家药监局批准了博睿康医疗科技（上海）有限公司的‘植入式脑机接口手部运动功能代偿系统’，这是全球首个获得监管批准进入临床应用的侵入式脑机接口医疗器械。 这一里程碑标志着脑机接口技术从研究走向临床，为颈段脊髓损伤所致四肢瘫痪患者提供了恢复手部抓握功能的新治疗方案，有望显著改善其生活质量。 该设备采用硬脑膜外微创植入与无线供能通信技术，配合气动手套辅助 18 至 60 岁颈段脊髓损伤患者实现手部抓握动作。临床试验结果显示受试者手部抓握能力提高，生活质量改善。

telegram · zaihuapd · 7月12日 14:39

**背景**: 脑机接口（BCI）实现了大脑与外部设备之间的直接通信。侵入式脑机接口将电极植入大脑表面或内部，以高精度记录神经信号。该设备针对因脊髓损伤而失去手部功能的四肢瘫痪患者，通过从脑信号解码其运动意图来控制气动手套，从而恢复抓握能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.163.com/dy/article/KQ5H8KUB0530RMN7.html">163.com/dy/article/KQ5H8KUB0530RMN7.html</a></li>
<li><a href="https://health.people.com.cn/n1/2026/0414/c14739-40700851.html">人机交互新形态走向临床（深度观察） --健康·生活--人民网</a></li>

</ul>
</details>

**标签**: `#brain-computer interface`, `#medical device`, `#neural engineering`, `#spinal cord injury`, `#regulatory approval`

---

<a id="item-4"></a>
## [Chromium 148 的 Math.tanh 可实现操作系统指纹识别](https://scrapfly.dev/posts/browser-math-os-fingerprint/) ⭐️ 8.0/10

自 Chromium 148 起，不同操作系统上 Math.tanh 实现的细微差异使得网站只需一次 tanh 调用就能推断出底层操作系统。 这一新的指纹识别向量使用户隐私受损，即使篡改用户代理字符串也能进行持久的操作系统检测，影响所有基于 Chromium 的浏览器。 该漏洞源于不同操作系统上超越函数实现的非一致性，对同一输入产生的 Math.tanh 结果不同。

hackernews · joahnn_s · 7月12日 21:12 · [社区讨论](https://news.ycombinator.com/item?id=48884853)

**背景**: 浏览器指纹识别通过收集设备特征来识别用户，无需使用 Cookie。Math.tanh 是一种双曲正切函数，其精度可能因硬件和操作系统数学库而异，因此成为潜在的指纹识别向量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pappp.net/?p=108314">Since Chromium 148, Math.tanh is now fingerprintable to link ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Transcendental_function">Transcendental function - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者反应不一：有人指出该技术还可用于指纹识别浏览器版本范围，也有人质疑发布该信息的抓取公司的动机。有人担心 Linux 用户会被误标记为爬虫，并指出 Tor 浏览器已放弃隐藏操作系统。

**标签**: `#fingerprinting`, `#browser security`, `#privacy`, `#Math.tanh`, `#Chromium`

---

<a id="item-5"></a>
## [陶哲轩用 LLM 编码代理构建应用](https://terrytao.wordpress.com/2026/07/11/old-and-new-apps-via-modern-coding-agents/) ⭐️ 8.0/10

著名数学家陶哲轩记录了他使用现代 LLM 编码代理构建交互式可视化应用的过程，展示了非专业人士通过引导式 AI 交互创建软件的工作流程。 这表明 AI 可以民主化软件创建，使没有传统编程技能的人也能构建定制工具，并凸显了技术核心领域之外巨大的潜在软件需求。 陶哲轩强调，对于非关键性辅助内容（如学术论文的可视化），使用 LLM 代理的下行风险是可接受的，他的方法涉及引导式交互而非完全自主的代码生成。

hackernews · subset · 7月12日 11:09 · [社区讨论](https://news.ycombinator.com/item?id=48880170)

**背景**: LLM 编码代理是利用大型语言模型辅助软件开发任务的 AI 系统，包括代码生成、调试和 UI 设计。这些代理可以在终端、IDE 甚至独立桌面应用等多种环境中运行，属于更广泛的 AI 辅助软件开发领域的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI-assisted_software_development">AI-assisted software development</a></li>
<li><a href="https://opencode.ai/">OpenCode | The open source AI coding agent</a></li>

</ul>
</details>

**社区讨论**: 社区评论普遍对软件创建的民主化表示兴奋，一些人幽默地指出看到菲尔兹奖得主像普通人一样依赖 AI。一位评论者强调了非软件领域的价值，另一位则赞赏陶哲轩对该工具局限性的平衡观点。

**标签**: `#LLM`, `#coding agents`, `#AI-assisted development`, `#software engineering`, `#Hacker News`

---

<a id="item-6"></a>
## [我爱大模型，我恨炒作](https://geohot.github.io//blog/jekyll/update/2026/07/12/i-love-llms.html) ⭐️ 8.0/10

George Hotz 认为，前沿 AI 实验室可能无法捕获 LLM 创造的经济价值，因为真正的生产力提升发生在私有、定制化应用中，而非通过付费 token 实现。 这一批评通过指出价值捕获问题，挑战了前沿实验室的高估值，暗示 LLM 最大的受益者可能是个人用户和小企业，而非模型提供商。 Hotz 指出，虽然前沿模型的订阅价格（每月 100–200 美元）很有吸引力，但由此带来的生产力提升往往隐藏在私人部署（如家庭实验室）中，而非面向公众的产品。

hackernews · therepanic · 7月12日 18:31 · [社区讨论](https://news.ycombinator.com/item?id=48883343)

**背景**: 像 GPT-4 和 Claude 这样的大语言模型（LLM）引发了大量投资和炒作，许多人相信它们将改变各行业。然而，谁最终能从这项技术中获利——是构建模型的公司，还是将其应用于特定任务的用户——仍存疑问。Hotz 的论点呼应了一个经典的经济学难题：创新可能创造巨大价值，但捕获这一价值却并非必然。

**社区讨论**: 评论者基本同意 Hotz 的观点，指出当前价格下订阅前沿模型是不需要犹豫的选择，真正的生产力提升出现在私有的、一次性软件项目中。一些人还表达了对开源未来担忧，因为借助 LLM 维护分支变得更容易，可能减少向上游贡献的意愿。

**标签**: `#LLM`, `#AI hype`, `#valuation`, `#open source`, `#productivity`

---