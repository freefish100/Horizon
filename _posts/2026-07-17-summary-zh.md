---
layout: default
title: "Horizon Summary: 2026-07-17 (ZH)"
date: 2026-07-17
lang: zh
---

> 从 41 条内容中筛选出 14 条重要资讯。

---

1. [Firefox 通过 WebAssembly 在 Chrome 内运行](#item-1) ⭐️ 9.0/10
2. [Inkling：Mira Murati 实验室发布开放权重多模态模型](#item-2) ⭐️ 9.0/10
3. [日本拟购 2.75 万块英伟达 Rubin 芯片建设机器人主权 AI](#item-3) ⭐️ 9.0/10
4. [Kimi 发布 K3：2.8 万亿参数开源 MoE 模型](#item-4) ⭐️ 9.0/10
5. [LM Studio 推出面向开放模型的 Bionic AI 代理](#item-5) ⭐️ 8.0/10
6. [用传统机器学习检测 LLM 文本：可行性与挑战](#item-6) ⭐️ 8.0/10
7. [从 Rust 到 Zig 的重写：编译器开发之经验谈](#item-7) ⭐️ 8.0/10
8. [Codex 漏洞可在完全访问模式下删除用户主目录](#item-8) ⭐️ 8.0/10
9. [Linus Torvalds 表示 Linux 不反 AI](#item-9) ⭐️ 8.0/10
10. [QLoRA 的 2e-4 默认学习率在小数据集上导致过拟合](#item-10) ⭐️ 8.0/10
11. [ExTernD：用于 LLM 精确量化的扩展秩三元分解](#item-11) ⭐️ 8.0/10
12. [台积电再投千亿美元赴美，Q2 利润飙升 77%创新高](#item-12) ⭐️ 8.0/10
13. [1Password 推出 Claude 集成：AI 代登录但不接触密码](#item-13) ⭐️ 8.0/10
14. [Truth Social 将向华尔街出售特朗普帖子的 API](#item-14) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Firefox 通过 WebAssembly 在 Chrome 内运行](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 9.0/10

Puter 成功将 Firefox 浏览器编译为 WebAssembly，使其能像完整浏览器一样在 Chrome 等浏览器内部运行。该演示借助 Claude Opus 和 Fable 协助编译，预计花费约 25,000 美元的 tokens，但因订阅计划实际成本更低。 这一突破证明了像完整浏览器这样的复杂原生应用可以移植到 WebAssembly，为沙箱化、可移植的计算环境开辟了可能性。它可能带来隔离浏览器标签、访问遗留软件，甚至在浏览器中运行多个操作系统实例的新方式。 团队选择了 Firefox/Gecko，因为它具有强大的单进程支持，简化了移植。所有网络流量通过 Wisp WebSocket 协议经过 Puter 的服务器进行代理，并且系统支持端到端加密。编译后的 WebAssembly 文件 (gecko.wasm) 为 233 MB，附加资源共 18 MB。

rss · Simon Willison · 7月16日 23:34

**背景**: WebAssembly (WASM) 是一种二进制指令格式，允许用 C++ 等语言编写的代码以接近原生的速度在浏览器中运行。传统上，WASM 用于较小的应用或库；编译完整浏览器是一项艰巨的任务，因为需要处理图形、网络和 DOM 交互的复杂性。Wisp 协议是一种低开销的方法，用于通过单个 WebSocket 连接代理多个 TCP 和 UDP 套接字，这对于浏览器代码无法打开原始网络连接的情况是必要的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Wire_protocol">Wire protocol</a></li>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/ wisp - protocol : Wisp is a low-overhead...</a></li>

</ul>
</details>

**标签**: `#WebAssembly`, `#Firefox`, `#browser technology`, `#compilation`, `#demo`

---

<a id="item-2"></a>
## [Inkling：Mira Murati 实验室发布开放权重多模态模型](https://simonwillison.net/2026/Jul/16/inkling/#atom-everything) ⭐️ 9.0/10

Mira Murati 领导的 Thinking Machines Lab 发布了开放权重 MoE 多模态模型 Inkling，总参数 975B，激活参数 41B，采用 Apache-2.0 许可证。 此次发布增强了美国开放权重生态系统，提供了一个可用于微调的竞争性模型，挑战了中国开源模型，并与 NVIDIA Nemotron 和 Gemma 4 看齐。 Inkling 在 45 万亿 token 的文本、图像、音频和视频上训练，但模型卡和训练数据文档明显不详细。后续将发布更小的 Inkling-Small 变体（总参数 276B，激活 12B）。

rss · Simon Willison · 7月16日 15:35

**背景**: 混合专家模型（MoE）每个输入仅激活部分参数，从而在总参数量大的情况下实现高效推理。开放权重模型发布训练后的参数，允许任何人下载和微调，但通常不包含训练数据或代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>

</ul>
</details>

**标签**: `#open-weights`, `#multimodal`, `#AI`, `#Mixture-of-Experts`, `#Mira Murati`

---

<a id="item-3"></a>
## [日本拟购 2.75 万块英伟达 Rubin 芯片建设机器人主权 AI](https://www.bloomberg.com/news/articles/2026-07-16/japan-to-buy-nvidia-rubin-chips-to-build-sovereign-ai-for-robots) ⭐️ 9.0/10

日本宣布计划购买 27,500 块英伟达下一代 Rubin 芯片，由新成立的 Noetra 公司牵头建设大型数据中心，开发面向机器人的本土基础 AI 模型。该项目获得日本政府 3873 亿日元（约 240 亿美元）拨款，软银、丰田支持的 Preferred Networks 以及 NEC 等企业参与其中。 这标志着日本在 AI 和机器人领域追求技术独立的重大战略举措，旨在打造中美之外的'第三种选择'。如果成功，日本有望到 2040 年占据全球机器人市场 30%以上的份额，从而重塑 AI 硬件和机器人产业的竞争格局。 Noetra 计划明年 3 月发布首个 AI 模型，并在数年内推出机器人专用版本。Rubin 架构不仅仅是一块 GPU，而是一个集成了 GPU、CPU、网络和存储的'AI 工厂'生态系统，旨在处理大规模计算集群。

telegram · zaihuapd · 7月16日 10:59

**背景**: “主权 AI”一词指的是国家为控制 AI 能力并减少对外国供应商依赖所做的努力，涵盖基础设施、数据和模型。英伟达的 Rubin 架构是其迄今为止最雄心勃勃的平台，从单一 GPU 芯片转向集成的 AI 工厂生态系统。日本的投资是全球各国寻求建立独立 AI 能力趋势的一部分，但成本、性能和供应链依赖等问题仍存争议。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.thundercompute.com/blog/nvidia-rubin-architecture">Nvidia Rubin Architecture : Everything You Must... | Thunder Compute</a></li>
<li><a href="https://en.wikipedia.org/wiki/Sovereign_AI">Sovereign AI</a></li>
<li><a href="https://www.redhat.com/en/topics/ai/sovereign-ai">What is sovereign AI?</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#Rubin`, `#sovereign AI`, `#robotics`, `#Japan`

---

<a id="item-4"></a>
## [Kimi 发布 K3：2.8 万亿参数开源 MoE 模型](https://t.me/zaihuapd/42619) ⭐️ 9.0/10

Kimi 发布了 K3，这是一个 2.8 万亿参数的开源模型，采用稀疏混合专家架构，包含 896 个专家，每个 token 激活 16 个专家，支持高达 100 万上下文 token 和原生视觉理解。 K3 是迄今最大规模的开源模型之一，其 2.5 倍于 K2 的效率提升和极端规模可能推动开源 AI 前沿，对专有模型构成挑战。 该模型采用了新颖的 Kimi Delta Attention（线性缩放以支持长上下文）和 Attention Residuals（用学到的深度注意力替代标准残差连接）。完整权重将在几天内发布，定价为每百万 token 3 美元/15 美元（缓存 0.3 美元）。

telegram · zaihuapd · 7月17日 00:02

**背景**: 稀疏混合专家架构将模型划分为多个专门化的子网络（专家），每个输入仅激活部分专家，从而提高效率。Kimi Delta Attention 是一种线性复杂度的长上下文高效处理机制，而 Attention Residuals 允许每层通过学到的注意力有选择地聚合早期表示，取代固定的残差连接。这些创新使得 2.8 万亿参数模型在计算上成为可能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sparse_mixture-of-experts">Sparse mixture-of-experts</a></li>
<li><a href="https://arxiv.org/abs/2603.15031">[2603.15031] Attention Residuals</a></li>
<li><a href="https://jianyuh.github.io/attention/2025/12/13/KDA.html">Linear Attention : Kimi Delta Attention | Jianyu Huang’s Blog</a></li>

</ul>
</details>

**社区讨论**: 社区评论指出，如果 K3 确实达到前沿性能，其高昂定价（每百万 token 3/15 美元）是合理的，同时有人质疑这是否是中国实验室在将智能商品化。模拟基准显示 K3 超越 Opus 4.8，仅次于 Fable/Sol 级别模型，但由于 Telegram 来源和虚构的竞品名称，仍然存在怀疑。

**标签**: `#AI`, `#large language model`, `#Mixture of Experts`, `#open-source`, `#attention mechanism`

---

<a id="item-5"></a>
## [LM Studio 推出面向开放模型的 Bionic AI 代理](https://lmstudio.ai/blog/introducing-lm-studio-bionic) ⭐️ 8.0/10

LM Studio 发布了 Bionic，这是一款新的 AI 代理应用，允许用户使用开源语言模型执行编码、研究和文档处理等复杂任务，提供熟悉的用户界面和企业级功能。 Bionic 为本地开放模型带来了实用的代理能力，使它们在保持数据隐私和成本控制的同时更适用于实际工作，这可能加速企业对开放模型的采用。 Bionic 支持用于编码任务的“代码”项目和用于文档创建且带有自动检查点的“工作”项目。用户可将其指向现有的 LM Studio 模型库，本地运行如 Qwen3.6 35B 等模型。

hackernews · minimaxir · 7月16日 20:18 · [社区讨论](https://news.ycombinator.com/item?id=48939662)

**背景**: LM Studio 是一款桌面应用，允许用户在本地运行开源大语言模型，无需联网。Bionic 将 LM Studio 的功能从简单聊天扩展到 AI 代理，能够自主使用这些模型执行多步骤任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lmstudio.ai/blog/introducing-lm-studio-bionic">Introducing LM Studio Bionic : the AI agent for open models</a></li>
<li><a href="https://9to5mac.com/2026/07/16/lm-studio-expands-beyond-chat-with-bionic-a-new-ai-agent-app-for-open-models/">LM Studio launches Bionic , a new AI agent app for open... - 9to5Mac</a></li>

</ul>
</details>

**社区讨论**: 早期用户对 Bionic 的易用性和熟悉界面给予积极评价，但也有用户对转向云端功能（LM Studio Secure Cloud）表示担忧。创始人已提供免费额度用于测试特定模型。

**标签**: `#AI agent`, `#open models`, `#LM Studio`, `#local LLM`, `#developer tools`

---

<a id="item-6"></a>
## [用传统机器学习检测 LLM 文本：可行性与挑战](https://blog.lyc8503.net/en/post/llm-classifier/) ⭐️ 8.0/10

一篇博客文章探讨了使用传统机器学习（如 TF-IDF 和逻辑回归）来检测文本是否由 LLM 生成，取得了一定成功，但也指出了根本性的局限。 随着 LLM 生成内容的激增，可靠的检测对于学术诚信、虚假信息防范和内容审核至关重要。这篇文章为关于这种检测是否长期可行的持续辩论做出了贡献。 该分类器足够小，可能可以在浏览器扩展中运行，实时标记 LLM 生成的段落。但作者承认文本缺乏图像的信息密度，使得检测本质上是概率性的。

hackernews · uneven9434 · 7月16日 16:41 · [社区讨论](https://news.ycombinator.com/item?id=48936880)

**背景**: 传统机器学习方法如 TF-IDF 和逻辑回归比深度学习更简单、更可解释。它们依赖于手工特征，如词频和 n-gram 模式。文章将此方法比作检测 LLM 倾向于表现的“口音”模式。

**社区讨论**: 社区评论对 AI 文本检测的长期可行性表示怀疑，有用户将其比作‘塔罗牌占卜’，因为文本的信息密度低。另一些人建议专注于衡量写作努力而非作者身份，并指出目前人类仍然是最好的检测者。

**标签**: `#LLM`, `#AI detection`, `#machine learning`, `#text classification`

---

<a id="item-7"></a>
## [从 Rust 到 Zig 的重写：编译器开发之经验谈](https://rtfeldman.com/rust-to-zig) ⭐️ 8.0/10

这篇博文详细描述了将编译器从 Rust 重写为 Zig 的经验和理由，重点讨论了安全性、性能和增量构建速度等方面的权衡。 这场讨论意义重大，因为它引发了关于系统编程中内存安全与语言选择的辩论，尤其是对于生成机器码的编译器而言。 重写利用了 Zig 的增量构建和手动内存管理，但牺牲了 Rust 的编译时安全保证；文章指出在编译器中不安全的内存操作很常见，但部分社区成员对此提出了异议。

hackernews · jorangreef · 7月16日 11:39 · [社区讨论](https://news.ycombinator.com/item?id=48933149)

**背景**: Rust 是一种专注于安全和并发的系统编程语言，通过其所有权模型和借用检查器在编译时防止内存错误。Zig 是一种较新的语言，旨在成为 C 语言的简单实用替代品，提供手动内存管理和强大的编译时特性，但没有内置的安全检查器。两者都用于底层开发，但在安全方法上根本不同：Rust 严格执行安全，而 Zig 给予程序员更多控制和责任。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>

</ul>
</details>

**社区讨论**: 评论意见各异：Steve Klabnik 质疑“不安全操作是编译器工作重要部分”的说法，指出生成机器码本身不必然需要不安全代码。Landr0id 指出关于 Zig 运行时安全检查（尤其是释放后使用检测）的描述可能不准确。ArthurBrown 质疑为何未选择更灵活的 OCaml，而 Onlyrealcuzzo 称赞 Zig 的增量构建，但希望 Rust 能引入类似特性。

**标签**: `#rust`, `#zig`, `#compiler`, `#systems programming`, `#rewrite`

---

<a id="item-8"></a>
## [Codex 漏洞可在完全访问模式下删除用户主目录](https://simonwillison.net/2026/Jul/16/bad-codex-bug/#atom-everything) ⭐️ 8.0/10

GPT-5.6 Codex 的一个漏洞在完全访问模式下且未启用沙箱或自动审查时，可能意外删除用户的主目录。该问题源于模型试图覆盖 $HOME 环境变量以定义临时目录，但错误地删除了 $HOME。 此漏洞凸显了在使用具有破坏性能力的 AI 编码代理时，尤其是在禁用适当保护措施的情况下，存在的严重安全风险。它强调了需要强大的沙箱和自动审查机制，以防止在生产环境中意外丢失数据。 该漏洞由完全访问模式、缺乏沙箱保护以及禁用自动审查共同触发。Thibault Sottiaux 调查后发现，问题源于模型错误地删除了 $HOME，而非它本想创建的临时目录。

rss · Simon Willison · 7月16日 17:45

**背景**: 像 Codex 这样的 AI 编码代理可以代表用户执行代码。完全访问模式赋予代理无限制的文件系统访问权限，而沙箱和自动审查是安全功能，用于隔离代理并在执行前审查其操作。当这些保护措施被禁用时，像意外删除文件这样的错误可能造成严重后果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blaxel.ai/blog/sandbox-management-for-ai-coding-agents">Sandbox Management for AI Coding Agents | Blaxel Blog</a></li>
<li><a href="https://www.bunnyshell.com/guides/coding-agent-sandbox/">Coding Agent Sandbox: Secure Environments for AI-Generated Code | Bunnyshell</a></li>
<li><a href="https://developers.openai.com/codex/concepts/sandboxing/auto-review">Auto-review | ChatGPT Learn</a></li>

</ul>
</details>

**标签**: `#codex`, `#coding-agents`, `#generative-ai`, `#ai-safety`, `#software-bugs`

---

<a id="item-9"></a>
## [Linus Torvalds 表示 Linux 不反 AI](https://simonwillison.net/2026/Jul/16/linus-torvalds/#atom-everything) ⭐️ 8.0/10

Linux 创始人 Linus Torvalds 在 Linux 媒体邮件列表中公开表示，Linux 不是一个反 AI 的项目，并且 AI 是一个明确有用的工具，他作为顶级维护者行使了决策权。 这明确了 Linux 项目对 AI 的立场，可能影响开源社区的方向，鼓励整合 AI 工具，同时反对反 AI 的情绪。 Torvalds 强调 AI 是一种与其他工具无异的工具，当前无疑是有用的，并表示不认同的人可以分叉项目或离开。

rss · Simon Willison · 7月16日 13:26

**背景**: Linus Torvalds 是 Linux 内核的创建者和首席维护者，Linux 是最大的开源项目之一。近期，开源社区内部就 AI 的角色存在争议，一些开发者因伦理或技术原因反对使用 AI。这份声明从权威立场直接回应了这些担忧。

**标签**: `#Linux`, `#AI`, `#Linus Torvalds`, `#open source`

---

<a id="item-10"></a>
## [QLoRA 的 2e-4 默认学习率在小数据集上导致过拟合](https://www.reddit.com/r/MachineLearning/comments/1uy1z8b/the_qlora_2e4_default_is_wrong_under_10k_samples/) ⭐️ 8.0/10

一位从业者报告，广泛使用的 QLoRA 默认学习率 2e-4 在样本少于 1 万的数据集上会导致过拟合，将其降低至 1e-4 并增加训练轮数后，评估性能显著提升。 这一发现挑战了 LLM 微调社区中的一个常见默认设置，可能帮助众多从业者在小型定制数据集上进行微调时避免浪费时间和获得糟糕结果。 作者花了三周时间调试，包括数据清洗和提示工程，最终发现将学习率从 2e-4 降至 1e-4 并将训练轮数从 3 增加到 5，带来了最大的评估提升。他们建议，对于超过 3 万样本的数据集，2e-4 可能仍然适用，但低于 1 万样本时，应从 1e-4 或更低的学习率开始。

reddit · r/MachineLearning · /u/Pretty-Ad774 · 7月16日 12:50

**背景**: QLoRA（量化低秩适配）是一种参数高效的微调方法，通过量化基础模型并利用 LoRA 适配器应用低秩更新来减少内存占用。默认学习率 2e-4 源自 Alpaca 数据集（5.2 万样本），但许多从业者在远小于此的自定义数据集上微调时并未调整这一超参数。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@levxn/lora-and-qlora-effective-methods-to-fine-tune-your-llms-in-detail-6e56a2a13f3c">LoRA and QLoRA - Effective methods to Fine - tune your... | Medium</a></li>
<li><a href="https://www.geeksforgeeks.org/nlp/fine-tuning-large-language-models-llms-using-qlora/">Fine - Tuning Large Language Models (LLMs) Using QLoRA</a></li>
<li><a href="https://vucense.com/dev-corner/qlora-unsloth-fine-tuning-2026/">Fine-Tune Llama 4 with QLoRA & Unsloth on a Consumer GPU 2026</a></li>

</ul>
</details>

**标签**: `#QLoRA`, `#fine-tuning`, `#learning rate`, `#overfitting`, `#practical ML`

---

<a id="item-11"></a>
## [ExTernD：用于 LLM 精确量化的扩展秩三元分解](https://www.reddit.com/r/MachineLearning/comments/1uy2zb3/externd_expandedrank_ternary_decomposition/) ⭐️ 8.0/10

一种名为 ExTernD 的新型训练后量化方法将权重矩阵分解为两个三元矩阵和一个对角缩放矩阵，从而允许任意秩，精度接近全精度。 这一突破解决了三元量化的一个基本限制——固定矩阵大小——并且只需适度增加 VRAM 即可实现高精度 LLM 部署，使高效推理更加实用。 内部秩可以任意大，因此精度可以任意高，而 VRAM 开销仅略高于当前量化方法，在利用三元算术时这一权衡是值得的。

reddit · r/MachineLearning · /u/LMTLS5 · 7月16日 13:31

**背景**: 三元量化通过将权重映射到三元值{-α, 0, +α}来缩小模型尺寸。训练后量化(PTQ)无需重新训练即可应用量化，但标准的三元 PTQ 由于固定矩阵大小而受到表示能力限制。ExTernD 通过将矩阵分解为两个三元矩阵和一个对角缩放矩阵来扩展秩，从而克服了这一限制，类似于低秩分解技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/ternary-quantization">Ternary Quantization in Neural Networks</a></li>
<li><a href="https://arxiv.org/abs/2303.01505">[2303.01505] Ternary Quantization: A Survey</a></li>

</ul>
</details>

**标签**: `#quantization`, `#LLM`, `#ternary`, `#PTQ`, `#efficient inference`

---

<a id="item-12"></a>
## [台积电再投千亿美元赴美，Q2 利润飙升 77%创新高](https://www.reuters.com/world/asia-pacific/tsmcs-second-quarter-profit-seen-hitting-record-ai-boom-2026-07-15/) ⭐️ 8.0/10

台积电宣布在亚利桑那州追加 1000 亿美元投资，并公布第二季度净利润同比飙升 77%至 7066 亿新台币（约 220 亿美元），创历史新高，远超市场预期。 这一巨额投资和创纪录的利润凸显了台积电在 AI 芯片制造中的主导地位，增强了美国半导体供应链，并预示着 AI 需求的持续增长。 台积电还将 2026 年资本支出预测上调至 600 亿至 640 亿美元，并预计全年美元营收增长略超 40%。亚利桑那州目前有 8 座工厂在建或规划中，未来可能再增 4 座。

telegram · zaihuapd · 7月16日 12:29

**背景**: 台积电是全球最大的半导体代工厂，为苹果、英伟达等公司生产芯片。AI 需求的激增推动了创纪录的利润和扩张，而美国投资旨在在地缘政治紧张局势下实现芯片生产从台湾的多元化。

**标签**: `#TSMC`, `#semiconductor`, `#AI`, `#investment`, `#manufacturing`

---

<a id="item-13"></a>
## [1Password 推出 Claude 集成：AI 代登录但不接触密码](https://9to5mac.com/2026/07/16/1password-now-lets-claude-sign-in-to-websites-without-seeing-your-passwords/) ⭐️ 8.0/10

1Password 推出了与 Anthropic Claude 的浏览器扩展集成，允许 Claude 使用存储的凭证登录网站，但密码和二次验证码不会进入 Claude 的上下文、记忆或 Anthropic 的系统。 这解决了 AI 代理访问敏感账户时的重大安全问题，可在不泄露凭证隐私的情况下实现自动化，有望推动 AI 助手在企业与个人生产力中的更广泛应用。 凭证通过安全通道直接注入目标网页；用户需通过生物识别逐条审批登录请求，权限仅限当前会话。该功能面向 Mac 端的商业、家庭及个人版用户开放，需同时安装 1Password 和 Claude 的桌面及浏览器扩展。

telegram · zaihuapd · 7月16日 15:54

**背景**: 像 1Password 这样的密码管理器能够安全地存储并在各网站自动填充凭证。Claude 等 AI 代理可代表用户执行任务，但直接授予其密码访问权限会带来隐私风险。凭证注入技术可将保管库中的凭证直接插入登录会话，而不向 AI 代理暴露凭证内容，从而兼顾自动化与安全性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://1password.com/blog/1password-for-claude">1Password for Claude: Give Claude access without giving up your credentials | 1Password</a></li>
<li><a href="https://www.theverge.com/tech/966442/1password-anthropic-claude-browser-integration">Claude can now use your 1Password credentials for you | The Verge</a></li>
<li><a href="https://www.engadget.com/2216405/1password-anthropic-claude-integration/">You can now grant Claude access to your 1Password credentials - Engadget</a></li>

</ul>
</details>

**标签**: `#password management`, `#AI integration`, `#security`, `#Claude`, `#1Password`

---

<a id="item-14"></a>
## [Truth Social 将向华尔街出售特朗普帖子的 API](https://www.cnn.com/2026/07/16/business/truth-social-data-wall-street) ⭐️ 8.0/10

特朗普媒体科技集团于 2026 年 7 月 16 日宣布，将于 8 月 1 日推出 Truth API，为机构客户提供 Truth Social 上排名前 10 账号（包括特朗普本人）的毫秒级实时帖子访问，用于高频交易。 此举将特朗普的社交媒体影响力直接货币化用于金融市场，可能使算法交易员在影响市场的政治声明中获得优势，但也引发了关于模糊总统职责与私人商业利益界限的严重伦理担忧。 该 API 以毫秒级速度提供 Truth Social 排名前 10 账号的帖子；定价尚未公布。CNN 此前报道称，特朗普曾利用 Truth Social 宣传自己刚买入的股票。

telegram · zaihuapd · 7月17日 01:02

**背景**: Truth Social 已成为特朗普宣布政策决定的主要平台，他关于关税、伊朗和霍尔木兹海峡的帖子此前曾引发股市和油市剧烈波动。高频交易公司使用实时数据源在微秒内执行交易，获取非公开或更快的数据可能带来不公平优势。Truth API 的推出引发了关于特朗普是否利用公职谋取私利的质疑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnn.com/2026/07/16/business/truth-social-data-wall-street">Truth Social will sell Wall Street quicker access to posts | CNN Business</a></li>
<li><a href="https://www.cnbc.com/2026/07/16/trump-truth-social-wall-street-traders-api.html">Trump Media launches paid data service to help Wall Street track Trump’s posts</a></li>

</ul>
</details>

**标签**: `#Truth Social`, `#API`, `#High-Frequency Trading`, `#Market Data`, `#Ethical Concerns`

---