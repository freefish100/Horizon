---
layout: default
title: "Horizon Summary: 2026-07-17 (EN)"
date: 2026-07-17
lang: en
---

> From 41 items, 14 important content pieces were selected

---

1. [Firefox Runs Inside Chrome via WebAssembly](#item-1) ⭐️ 9.0/10
2. [Inkling: Open-Weights Multimodal Model from Mira Murati's Lab](#item-2) ⭐️ 9.0/10
3. [Japan to Buy 27,500 Nvidia Rubin Chips for Robot Sovereign AI](#item-3) ⭐️ 9.0/10
4. [Kimi Releases K3: 2.8 Trillion Parameter Open-Source MoE Model](#item-4) ⭐️ 9.0/10
5. [LM Studio Launches Bionic AI Agent for Open Models](#item-5) ⭐️ 8.0/10
6. [Classical ML for LLM Text Detection: Feasibility and Challenges](#item-6) ⭐️ 8.0/10
7. [Rust-to-Zig Rewrite: A Compiler's Tale](#item-7) ⭐️ 8.0/10
8. [Codex Bug Can Delete Home Directory in Full Access Mode](#item-8) ⭐️ 8.0/10
9. [Linus Torvalds Declares Linux Not Anti-AI](#item-9) ⭐️ 8.0/10
10. [QLoRA 2e-4 default causes overfitting on small datasets](#item-10) ⭐️ 8.0/10
11. [ExTernD: Ternary Decomposition for Accurate LLM Quantization](#item-11) ⭐️ 8.0/10
12. [TSMC announces additional $100B US investment, Q2 profit jumps 77%](#item-12) ⭐️ 8.0/10
13. [1Password Launches Claude Integration for AI Login Without Exposing Passwords](#item-13) ⭐️ 8.0/10
14. [Truth Social to sell API for Trump posts to Wall Street](#item-14) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Firefox Runs Inside Chrome via WebAssembly](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 9.0/10

Puter successfully compiled the Firefox browser to WebAssembly, enabling it to run as a full browser within another browser like Chrome. The demo uses Claude Opus and Fable to assist with the compilation, costing an estimated $25,000 in tokens but less due to a subscription plan. This breakthrough proves that complex native applications like full browsers can be ported to WebAssembly, opening up possibilities for sandboxed, portable computing environments. It could lead to new ways of isolating browser tabs, legacy software access, or even running multiple operating system instances in the browser. The team chose Firefox/Gecko for its strong single-process support, which simplifies the port. All network traffic is proxied through Puter's server using the Wisp WebSocket protocol, and the system supports end-to-end encryption. The compiled WebAssembly file (gecko.wasm) is 233 MB, with additional assets totaling 18 MB.

rss · Simon Willison · Jul 16, 23:34

**Background**: WebAssembly (WASM) is a binary instruction format that allows code written in languages like C++ to run in web browsers at near-native speed. Traditionally, WASM has been used for smaller applications or libraries; compiling a full browser is a monumental task due to the complexity of handling graphics, networking, and DOM interactions. The Wisp protocol is a low-overhead method for proxying TCP and UDP sockets over a single WebSocket connection, which is necessary because browser code cannot open raw network connections.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Wire_protocol">Wire protocol</a></li>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/ wisp - protocol : Wisp is a low-overhead...</a></li>

</ul>
</details>

**Tags**: `#WebAssembly`, `#Firefox`, `#browser technology`, `#compilation`, `#demo`

---

<a id="item-2"></a>
## [Inkling: Open-Weights Multimodal Model from Mira Murati's Lab](https://simonwillison.net/2026/Jul/16/inkling/#atom-everything) ⭐️ 9.0/10

Thinking Machines Lab, led by Mira Murati, released Inkling, an open-weights Mixture-of-Experts multimodal model with 975B total parameters and 41B active parameters, under the Apache-2.0 license. This release strengthens the US open-weights ecosystem with a competitive model for fine-tuning, challenging Chinese open models and joining ranks with NVIDIA Nemotron and Gemma 4. Inkling is trained on 45 trillion tokens of text, images, audio, and video, but the model card and training data documentation are notably sparse. A smaller Inkling-Small variant (276B total, 12B active) is promised later.

rss · Simon Willison · Jul 16, 15:35

**Background**: A Mixture-of-Experts (MoE) model activates only a subset of parameters per input, enabling efficient inference despite large total size. Open-weights models release trained parameters, allowing anyone to download and fine-tune them, but do not typically include training data or code.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>

</ul>
</details>

**Tags**: `#open-weights`, `#multimodal`, `#AI`, `#Mixture-of-Experts`, `#Mira Murati`

---

<a id="item-3"></a>
## [Japan to Buy 27,500 Nvidia Rubin Chips for Robot Sovereign AI](https://www.bloomberg.com/news/articles/2026-07-16/japan-to-buy-nvidia-rubin-chips-to-build-sovereign-ai-for-robots) ⭐️ 9.0/10

Japan announced plans to purchase 27,500 of Nvidia's next-generation Rubin chips, led by newly formed company Noetra, to build a large-scale data center for developing a domestic foundational AI model tailored for robotics. The project is backed by 387.3 billion yen (approximately $24 billion) in government funding, with participation from SoftBank, Toyota-backed Preferred Networks, and NEC. This represents a major strategic push for Japan to achieve technological independence in AI and robotics, aiming to create a 'third option' beyond US and Chinese dominance. If successful, Japan could capture over 30% of the global robotics market by 2040, reshaping the competitive landscape of both AI hardware and robotics. Noetra plans to release its first AI model by March next year and a robot-specific version within a few years. The Rubin architecture is not just a GPU but an integrated 'AI factory' ecosystem combining GPUs, CPUs, networking, and storage, designed to handle massive compute clusters.

telegram · zaihuapd · Jul 16, 10:59

**Background**: The term 'sovereign AI' refers to national efforts to control AI capabilities and reduce dependence on foreign providers, encompassing infrastructure, data, and models. Nvidia's Rubin architecture represents its most ambitious platform yet, shifting from single-chip GPUs to integrated AI factory ecosystems. Japan's investment is part of a global trend where countries seek to build independent AI capabilities, though questions remain about cost, performance, and supply chain dependencies.

<details><summary>References</summary>
<ul>
<li><a href="https://www.thundercompute.com/blog/nvidia-rubin-architecture">Nvidia Rubin Architecture : Everything You Must... | Thunder Compute</a></li>
<li><a href="https://en.wikipedia.org/wiki/Sovereign_AI">Sovereign AI</a></li>
<li><a href="https://www.redhat.com/en/topics/ai/sovereign-ai">What is sovereign AI?</a></li>

</ul>
</details>

**Tags**: `#NVIDIA`, `#Rubin`, `#sovereign AI`, `#robotics`, `#Japan`

---

<a id="item-4"></a>
## [Kimi Releases K3: 2.8 Trillion Parameter Open-Source MoE Model](https://t.me/zaihuapd/42619) ⭐️ 9.0/10

Kimi released K3, a 2.8 trillion parameter open-source model using a sparse Mixture-of-Experts architecture with 896 experts and 16 activated per token, supporting up to 1M context tokens and native vision understanding. K3 represents one of the largest openly released models, potentially advancing the frontier of open-source AI and challenging proprietary models with its efficiency gains (2.5x over K2) and extreme scale. The model uses novel Kimi Delta Attention (linear scaling for long contexts) and Attention Residuals (replacing standard residuals with learned attention over depth). Full weights will be released within days, and pricing is $3/$15 per million tokens (cache $0.3).

telegram · zaihuapd · Jul 17, 00:02

**Background**: Sparse Mixture-of-Experts (MoE) is an architecture that divides a model into multiple specialized sub-networks (experts) and activates only a subset per input, improving efficiency. Kimi Delta Attention is a mechanism for efficient long-context processing with linear complexity, while Attention Residuals allow each layer to selectively aggregate earlier representations via learned attention, replacing fixed residual connections. These innovations enable the 2.8 trillion parameter model to remain computationally feasible.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sparse_mixture-of-experts">Sparse mixture-of-experts</a></li>
<li><a href="https://arxiv.org/abs/2603.15031">[2603.15031] Attention Residuals</a></li>
<li><a href="https://jianyuh.github.io/attention/2025/12/13/KDA.html">Linear Attention : Kimi Delta Attention | Jianyu Huang’s Blog</a></li>

</ul>
</details>

**Discussion**: Community comments note the high pricing ($3/$15 per million tokens) as justified if K3 truly reaches frontier performance, with some questioning whether Chinese labs are commoditizing intelligence. Simulated benchmarks show K3 surpassing Opus 4.8 and trailing only Fable/Sol-tier models, but skepticism remains due to the Telegram source and fictional-sounding competitor names.

**Tags**: `#AI`, `#large language model`, `#Mixture of Experts`, `#open-source`, `#attention mechanism`

---

<a id="item-5"></a>
## [LM Studio Launches Bionic AI Agent for Open Models](https://lmstudio.ai/blog/introducing-lm-studio-bionic) ⭐️ 8.0/10

LM Studio has launched Bionic, a new AI agent application that enables users to perform complex tasks like coding, research, and document manipulation using open-source language models, with a familiar UI and enterprise features. Bionic brings practical agentic capabilities to local open models, making them more accessible for real work while maintaining data privacy and cost control, which could accelerate enterprise adoption of open models. Bionic supports both 'Code' projects for coding tasks and 'Work' projects for document creation with automatic checkpointing. Users can point it to their existing LM Studio model library and run models like Qwen3.6 35B locally.

hackernews · minimaxir · Jul 16, 20:18 · [Discussion](https://news.ycombinator.com/item?id=48939662)

**Background**: LM Studio is a desktop application that allows users to run open-source large language models locally without requiring internet access. Bionic expands LM Studio's functionality from simple chat to an AI agent that can autonomously perform multi-step tasks using those models.

<details><summary>References</summary>
<ul>
<li><a href="https://lmstudio.ai/blog/introducing-lm-studio-bionic">Introducing LM Studio Bionic : the AI agent for open models</a></li>
<li><a href="https://9to5mac.com/2026/07/16/lm-studio-expands-beyond-chat-with-bionic-a-new-ai-agent-app-for-open-models/">LM Studio launches Bionic , a new AI agent app for open... - 9to5Mac</a></li>

</ul>
</details>

**Discussion**: Early users report positive experiences with Bionic's ease of use and familiar interface, though some express concerns about the shift toward cloud-based features (LM Studio Secure Cloud). The founder has offered free credits for testing specific models.

**Tags**: `#AI agent`, `#open models`, `#LM Studio`, `#local LLM`, `#developer tools`

---

<a id="item-6"></a>
## [Classical ML for LLM Text Detection: Feasibility and Challenges](https://blog.lyc8503.net/en/post/llm-classifier/) ⭐️ 8.0/10

A blog post explores using classical machine learning (e.g., TF-IDF and logistic regression) to detect whether a text was generated by an LLM, achieving some success but highlighting fundamental limitations. As LLM-generated content proliferates, reliable detection is crucial for academic integrity, misinformation, and content moderation. This post contributes to the ongoing debate on whether such detection is even possible in the long run. The classifier is small enough that it could potentially run in a browser extension to flag LLM-generated paragraphs in real time. However, the author acknowledges that text lacks the information density of images, making detection inherently probabilistic.

hackernews · uneven9434 · Jul 16, 16:41 · [Discussion](https://news.ycombinator.com/item?id=48936880)

**Background**: Classical machine learning methods like TF-IDF and logistic regression are simpler and more interpretable than deep learning. They rely on handcrafted features such as word frequencies and n-gram patterns. The post compares this approach to detecting 'accent' patterns that LLMs tend to exhibit.

**Discussion**: Community comments express skepticism about the long-term viability of AI text detection, with some comparing it to 'tarot card reading' due to text's low information density. Others suggest focusing on measuring writing effort rather than authorship, and note that humans remain the best detectors for now.

**Tags**: `#LLM`, `#AI detection`, `#machine learning`, `#text classification`

---

<a id="item-7"></a>
## [Rust-to-Zig Rewrite: A Compiler's Tale](https://rtfeldman.com/rust-to-zig) ⭐️ 8.0/10

The blog post details the experience and rationale behind rewriting a compiler from Rust to Zig, highlighting trade-offs such as safety, performance, and incremental build speed. This discussion is significant because it sparks debate on memory safety and language choice in systems programming, particularly for compilers that emit machine code. The rewrite leverages Zig's incremental builds and manual memory management, while sacrificing Rust's compile-time safety guarantees; the post notes that memory-unsafe operations are common in compilers, but some community members dispute this claim.

hackernews · jorangreef · Jul 16, 11:39 · [Discussion](https://news.ycombinator.com/item?id=48933149)

**Background**: Rust is a systems programming language focused on safety and concurrency through its ownership model and borrow checker, preventing memory errors at compile time. Zig is a newer language that aims to be a simpler, pragmatic alternative to C, offering manual memory management and powerful compile-time features without a built-in safety checker. Both are used for low-level development, but they differ fundamentally in their approach to safety: Rust enforces it strictly, while Zig gives the programmer more control and responsibility.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>

</ul>
</details>

**Discussion**: Comments express varied opinions: Steve Klabnik questions the claim that memory-unsafe operations are a big part of compiler work, noting that emitting machine code doesn't inherently require unsafe code. Landr0id points out potential inaccuracies regarding Zig's runtime safety checks, specifically about use-after-free detection. ArthurBrown wonders why OCaml wasn't chosen despite its flexibility, and Onlyrealcuzzo praises Zig's incremental builds but hopes Rust will adopt similar features.

**Tags**: `#rust`, `#zig`, `#compiler`, `#systems programming`, `#rewrite`

---

<a id="item-8"></a>
## [Codex Bug Can Delete Home Directory in Full Access Mode](https://simonwillison.net/2026/Jul/16/bad-codex-bug/#atom-everything) ⭐️ 8.0/10

A bug in GPT-5.6 Codex, when run in full access mode without sandboxing or auto-review, can accidentally delete the user's home directory. This occurs when the model attempts to override the $HOME environment variable for a temporary directory but mistakenly deletes $HOME. This bug highlights critical safety risks in using AI coding agents with destructive capabilities, especially when proper safeguards are disabled. It underscores the need for robust sandboxing and automatic review mechanisms to prevent accidental data loss in production environments. The bug is triggered by a combination of full access mode, lack of sandboxing, and disabled auto-review. Thibault Sottiaux investigated the issue and found it stems from the model erroneously deleting $HOME instead of a temporary directory it intended to create.

rss · Simon Willison · Jul 16, 17:45

**Background**: AI coding agents like Codex can execute code on behalf of users. Full access mode gives the agent unfettered filesystem access, while sandboxing and auto-review are safety features that isolate the agent and review its actions before execution. When these protections are disabled, mistakes like accidental file deletion can have severe consequences.

<details><summary>References</summary>
<ul>
<li><a href="https://blaxel.ai/blog/sandbox-management-for-ai-coding-agents">Sandbox Management for AI Coding Agents | Blaxel Blog</a></li>
<li><a href="https://www.bunnyshell.com/guides/coding-agent-sandbox/">Coding Agent Sandbox: Secure Environments for AI-Generated Code | Bunnyshell</a></li>
<li><a href="https://developers.openai.com/codex/concepts/sandboxing/auto-review">Auto-review | ChatGPT Learn</a></li>

</ul>
</details>

**Tags**: `#codex`, `#coding-agents`, `#generative-ai`, `#ai-safety`, `#software-bugs`

---

<a id="item-9"></a>
## [Linus Torvalds Declares Linux Not Anti-AI](https://simonwillison.net/2026/Jul/16/linus-torvalds/#atom-everything) ⭐️ 8.0/10

Linus Torvalds, the creator of Linux, publicly stated on the Linux Media mailing list that Linux is not an anti-AI project and that AI is a clearly useful tool, asserting his authority as top-level maintainer. This clarifies the Linux project's stance on AI, potentially influencing the open-source community's direction and encouraging integration of AI tools, while also pushing back against anti-AI sentiments. Torvalds emphasized that AI is a tool like any other, that it is unquestionably useful now, and that anyone who disagrees may fork the project or leave.

rss · Simon Willison · Jul 16, 13:26

**Background**: Linus Torvalds is the creator and lead maintainer of the Linux kernel, one of the largest open-source projects. Recently, there has been debate within the open-source community about the role of AI, with some developers opposing its use due to ethical or technical concerns. This statement directly addresses those concerns from a position of authority.

**Tags**: `#Linux`, `#AI`, `#Linus Torvalds`, `#open source`

---

<a id="item-10"></a>
## [QLoRA 2e-4 default causes overfitting on small datasets](https://www.reddit.com/r/MachineLearning/comments/1uy1z8b/the_qlora_2e4_default_is_wrong_under_10k_samples/) ⭐️ 8.0/10

A practitioner reports that the widely-used QLoRA learning rate default of 2e-4 leads to overfitting on datasets with fewer than 10,000 samples, and that lowering it to 1e-4 while increasing epochs significantly improves evaluation performance. This challenges a common default in the LLM fine-tuning community, potentially saving many practitioners from wasted time and poor results when fine-tuning on small, custom datasets. The author spent three weeks debugging, including data cleaning and prompt engineering, before discovering that simply reducing the learning rate from 2e-4 to 1e-4 and increasing epochs from 3 to 5 produced the largest eval improvement. They suggest that for datasets above 30k samples, 2e-4 may still be fine, but below 10k samples, start at 1e-4 or lower.

reddit · r/MachineLearning · /u/Pretty-Ad774 · Jul 16, 12:50

**Background**: QLoRA (Quantized Low-Rank Adaptation) is a parameter-efficient fine-tuning method that reduces memory usage by quantizing the base model and applying low-rank updates via LoRA adapters. The default learning rate of 2e-4 originated from the Alpaca dataset (52k samples), but many practitioners fine-tune on much smaller custom datasets without adjusting this hyperparameter.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@levxn/lora-and-qlora-effective-methods-to-fine-tune-your-llms-in-detail-6e56a2a13f3c">LoRA and QLoRA - Effective methods to Fine - tune your... | Medium</a></li>
<li><a href="https://www.geeksforgeeks.org/nlp/fine-tuning-large-language-models-llms-using-qlora/">Fine - Tuning Large Language Models (LLMs) Using QLoRA</a></li>
<li><a href="https://vucense.com/dev-corner/qlora-unsloth-fine-tuning-2026/">Fine-Tune Llama 4 with QLoRA & Unsloth on a Consumer GPU 2026</a></li>

</ul>
</details>

**Tags**: `#QLoRA`, `#fine-tuning`, `#learning rate`, `#overfitting`, `#practical ML`

---

<a id="item-11"></a>
## [ExTernD: Ternary Decomposition for Accurate LLM Quantization](https://www.reddit.com/r/MachineLearning/comments/1uy2zb3/externd_expandedrank_ternary_decomposition/) ⭐️ 8.0/10

A new post-training quantization method called ExTernD decomposes weight matrices into two ternary matrices and a diagonal scaling matrix, allowing arbitrary rank and accuracy approaching full precision. This breakthrough addresses a fundamental limitation of ternary quantization—fixed matrix size—and enables high-accuracy LLM deployment with only a modest increase in VRAM, making efficient inference more practical. The inner rank can be arbitrarily large, so accuracy can be arbitrarily high, and the VRAM overhead is only slightly higher than current quantization methods, making the trade-off worthwhile when exploiting ternary arithmetic.

reddit · r/MachineLearning · /u/LMTLS5 · Jul 16, 13:31

**Background**: Ternary quantization reduces model size by mapping weights to ternary values {-α, 0, +α}. Post-training quantization (PTQ) applies quantization without retraining, but standard ternary PTQ suffers from limited representational power due to fixed matrix size. ExTernD overcomes this by expanding the rank through matrix decomposition into two ternary matrices and a diagonal scaling matrix, similar to low-rank factorization techniques.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/ternary-quantization">Ternary Quantization in Neural Networks</a></li>
<li><a href="https://arxiv.org/abs/2303.01505">[2303.01505] Ternary Quantization: A Survey</a></li>

</ul>
</details>

**Tags**: `#quantization`, `#LLM`, `#ternary`, `#PTQ`, `#efficient inference`

---

<a id="item-12"></a>
## [TSMC announces additional $100B US investment, Q2 profit jumps 77%](https://www.reuters.com/world/asia-pacific/tsmcs-second-quarter-profit-seen-hitting-record-ai-boom-2026-07-15/) ⭐️ 8.0/10

TSMC announced an additional $100 billion investment in its Arizona fabs and reported a 77% surge in Q2 net profit to a record NT$706.6 billion ($22 billion), far exceeding market expectations. This massive investment and record profit underscore TSMC's dominant role in AI chip manufacturing, strengthening the US semiconductor supply chain and signaling sustained AI demand growth. TSMC also raised its 2026 capital expenditure forecast to $60-$64 billion and expects full-year US dollar revenue growth of slightly over 40%. Arizona now has eight fabs under construction or planning, with four more possible.

telegram · zaihuapd · Jul 16, 12:29

**Background**: TSMC is the world's largest contract semiconductor manufacturer, producing chips for companies like Apple and Nvidia. The surge in AI demand has driven record profits and expansion, with US investment aimed at diversifying chip production away from Taiwan amid geopolitical tensions.

**Tags**: `#TSMC`, `#semiconductor`, `#AI`, `#investment`, `#manufacturing`

---

<a id="item-13"></a>
## [1Password Launches Claude Integration for AI Login Without Exposing Passwords](https://9to5mac.com/2026/07/16/1password-now-lets-claude-sign-in-to-websites-without-seeing-your-passwords/) ⭐️ 8.0/10

1Password has launched a browser extension integration with Anthropic's Claude AI that lets Claude log into websites using stored credentials, without the passwords or 2FA codes ever being exposed to Claude's context, memory, or Anthropic's systems. This addresses a major security concern with AI agents accessing sensitive accounts, enabling automation without compromising credential privacy. It could pave the way for broader adoption of AI assistants in enterprise and personal productivity. Credentials are injected directly into the target webpage via a secure channel; users must biometrically approve each login request, and permissions are session-specific. The feature is available on Mac for business, family, and personal plans, requiring both 1Password and Claude desktop and browser extensions.

telegram · zaihuapd · Jul 16, 15:54

**Background**: Password managers like 1Password securely store and autofill credentials across websites. AI agents such as Claude can perform tasks on behalf of users, but granting them direct access to passwords poses privacy risks. Credential injection is a technique that inserts vaulted credentials directly into a login session without revealing them to the agent, preserving both automation and security.

<details><summary>References</summary>
<ul>
<li><a href="https://1password.com/blog/1password-for-claude">1Password for Claude: Give Claude access without giving up your credentials | 1Password</a></li>
<li><a href="https://www.theverge.com/tech/966442/1password-anthropic-claude-browser-integration">Claude can now use your 1Password credentials for you | The Verge</a></li>
<li><a href="https://www.engadget.com/2216405/1password-anthropic-claude-integration/">You can now grant Claude access to your 1Password credentials - Engadget</a></li>

</ul>
</details>

**Tags**: `#password management`, `#AI integration`, `#security`, `#Claude`, `#1Password`

---

<a id="item-14"></a>
## [Truth Social to sell API for Trump posts to Wall Street](https://www.cnn.com/2026/07/16/business/truth-social-data-wall-street) ⭐️ 8.0/10

Trump Media & Technology Group announced on July 16, 2026, that it will launch Truth API on August 1, providing institutional clients with real-time access to posts from the top 10 accounts on Truth Social, including President Trump, in milliseconds for high-frequency trading. This move directly monetizes Trump's social media influence for financial markets, potentially giving algorithmic traders an edge on market-moving political announcements, but it raises serious ethical concerns about blurring lines between presidential duties and private business interests. The API delivers posts in milliseconds from the top 10 Truth Social accounts; pricing has not been disclosed. CNN previously reported that Trump used Truth Social to promote stocks he had just bought.

telegram · zaihuapd · Jul 17, 01:02

**Background**: Truth Social has become Trump's primary platform for announcing policy decisions, and his posts on tariffs, Iran, and the Strait of Hormuz have previously caused significant volatility in stock and oil markets. High-frequency trading firms use real-time data feeds to execute trades within microseconds, and access to non-public or faster data can provide an unfair advantage. The launch of Truth API raises questions about whether Trump is leveraging his official position for private financial gain.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnn.com/2026/07/16/business/truth-social-data-wall-street">Truth Social will sell Wall Street quicker access to posts | CNN Business</a></li>
<li><a href="https://www.cnbc.com/2026/07/16/trump-truth-social-wall-street-traders-api.html">Trump Media launches paid data service to help Wall Street track Trump’s posts</a></li>

</ul>
</details>

**Tags**: `#Truth Social`, `#API`, `#High-Frequency Trading`, `#Market Data`, `#Ethical Concerns`

---