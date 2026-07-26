---
layout: default
title: "Horizon Summary: 2026-07-26 (EN)"
date: 2026-07-26
lang: en
---

> From 25 items, 9 important content pieces were selected

---

1. [vLLM v0.26.0 Adds Inkling Support and DeepSeek-V4 Optimizations](#item-1) ⭐️ 8.0/10
2. [Claude 5's New Context Engineering Rules Ignite Debate on Lock-In](#item-2) ⭐️ 8.0/10
3. [Open-weight AI’s Kubernetes-like rise](#item-3) ⭐️ 8.0/10
4. [Android May Restrict On-Device ADB Access](#item-4) ⭐️ 8.0/10
5. [Ruff v0.16.0 Expands Default Rules from 59 to 413](#item-5) ⭐️ 8.0/10
6. [China Fines Ctrip $800 Million for Monopoly Abuse](#item-6) ⭐️ 8.0/10
7. [Microsoft to Use TPM Chips to Block Pirated Windows Activation](#item-7) ⭐️ 8.0/10
8. [DeepSeek Halts New Funding Round Over Leaked Comments](#item-8) ⭐️ 8.0/10
9. [Silicon Valley Coalition Opposes Ban on Chinese Open-Weight AI](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.26.0 Adds Inkling Support and DeepSeek-V4 Optimizations](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 8.0/10

vLLM v0.26.0 introduces full support for the Inkling 975B-parameter MoE model family, including piecewise CUDA graphs and Hopper FA4 relative attention, and achieves substantial performance improvements for DeepSeek-V4 with specialized routing kernels and fused operations. This release strengthens vLLM as a production-ready inference engine for the latest open-weight models, enabling efficient serving of large-scale MoE architectures like Inkling and further optimizing DeepSeek-V4, which drives down latency and cost for real-world LLM deployments. The release includes 411 commits from 212 contributors, flexible attention backends selectable per KV-cache group, fp32 lm_head for improved generation accuracy, and Rust frontend support for multimodal video and audio.

github · khluu · Jul 25, 10:38

**Background**: vLLM is an open-source high-throughput LLM serving engine that uses PagedAttention and efficient CUDA kernels to reduce memory overhead. The Inkling model from Thinking Machines Lab is a 975B-parameter Mixture-of-Experts transformer with 41B active parameters, supporting up to 1M token context. Hopper FA4 is the latest FlashAttention algorithm optimized for NVIDIA Hopper GPUs via asynchronous pipelining. NVFP4 quantization from NVIDIA ModelOpt enables 4-bit floating-point weight storage for reduced memory usage.

<details><summary>References</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/introducing-inkling/">Inkling: Our Open-Weights Model - Thinking Machines Lab</a></li>
<li><a href="https://arxiv.org/html/2603.05451v1">FlashAttention-4: Algorithm and Kernel Pipelining Co-Design for Asymmetric Hardware Scaling</a></li>
<li><a href="https://arunksingh16.medium.com/nvidia-nvfp4-quantization-blackwell-and-the-path-to-production-inference-12407e14e084">NVIDIA NVFP4: Quantization, Blackwell, and the Path to Production Inference | by Arun Kumar Singh | Jul, 2026 | Medium</a></li>

</ul>
</details>

**Tags**: `#vllm`, `#LLM inference`, `#release`, `#performance optimization`, `#GPU computing`

---

<a id="item-2"></a>
## [Claude 5's New Context Engineering Rules Ignite Debate on Lock-In](https://claude.com/blog/the-new-rules-of-context-engineering-for-claude-5-generation-models) ⭐️ 8.0/10

Anthropic has released a new set of context engineering rules for its Claude 5 model, aiming to optimize how the model uses context during inference, but the community has raised concerns about vendor lock-in and the reliability of the automemory feature. These rules could fundamentally change how developers interact with Claude 5, potentially increasing dependence on Anthropic-specific tooling, while automemory issues may undermine trust in the model's decision-making process. The new rules emphasize structured instructions and leverage Claude's automemory feature, which stores and retrieves context across sessions, but users report that automemory can make unreliable leaps and increase token consumption due to failed initial attempts.

hackernews · mellosouls · Jul 25, 20:42 · [Discussion](https://news.ycombinator.com/item?id=49051361)

**Background**: Context engineering is the discipline of designing and optimizing the information provided to an LLM during inference, extending beyond prompts to include structured instructions and external data. Automemory is a feature that allows the model to store and recall information across sessions, but its reliability is questioned. Anthropic's new rules aim to standardize these practices for Claude 5.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents">Effective context engineering for AI agents \ Anthropic</a></li>
<li><a href="https://www.philschmid.de/context-engineering">The New Skill in AI is Not Prompting, It's Context Engineering</a></li>
<li><a href="https://www.linkedin.com/posts/koujala_claudecode-ai-developertools-activity-7432311920109596672-FgaD">Unlock Claude Code's AutoMemory Feature for Efficient... | LinkedIn</a></li>

</ul>
</details>

**Discussion**: The community is sharply divided: some criticize the new rules as a move to increase lock-in to Anthropic's platform, citing Claude 5's accidental deletions and vague reasoning traces. Others worry that reliance on automemory introduces unpredictable behavior and liability risks, while a few see potential for more concise context engineering without verbose instructions.

**Tags**: `#Claude 5`, `#context engineering`, `#AI`, `#lock-in`, `#community discussion`

---

<a id="item-3"></a>
## [Open-weight AI’s Kubernetes-like rise](https://tobi.knaup.me/2026-07-25-open-weight-ai-is-having-its-kubernetes-moment/) ⭐️ 8.0/10

Open-weight AI models are rapidly becoming the standard for AI development, mirroring how Kubernetes standardized cloud infrastructure, driven by cost efficiency and community collaboration. This shift could democratize AI access, reduce dependency on proprietary models, and foster collaborative development, potentially transforming the AI industry as Kubernetes did for cloud computing. Open-weight models release the trained parameters (weights) publicly, allowing customization and local deployment, but they are not fully open-source as the training data and code may not be included. The analogy with Kubernetes highlights the role of community-driven standardization.

hackernews · tknaup · Jul 25, 14:49 · [Discussion](https://news.ycombinator.com/item?id=49048034)

**Background**: Model weights are numerical parameters in neural networks that determine how the model processes information; they store the 'knowledge' learned during training. Open-weight AI models make these weights publicly available, enabling developers to fine-tune or run the model on their own hardware. This is similar to how Kubernetes, an open-source container orchestration platform, became the standard for managing cloud infrastructure through community collaboration and cost savings.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/thought-vector/open-weight-llms-a-strategic-advantage-for-enterprise-ai-1c4859ea6885">Open - Weight LLMs: A Strategic Advantage for Enterprise AI | Medium</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-are-weights">What are Weights? | Stanford HAI</a></li>
<li><a href="https://www.linkedin.com/pulse/open-weight-ai-what-we-finally-opened-bonnet-nicolas-pistorio-n3ulf">Open - weight AI : what if we finally opened the bonnet ?</a></li>

</ul>
</details>

**Discussion**: Commenters debate the feasibility of banning Chinese models by origin since weights are just numbers, criticize the opaque pricing 'tokenomics' of proprietary models, and advocate for truly open collaborative models akin to Linux. Some note that American labs like OpenAI have released open-weight models but wish for more frequent updates.

**Tags**: `#AI`, `#open-source`, `#Kubernetes`, `#model weights`, `#industry trend`

---

<a id="item-4"></a>
## [Android May Restrict On-Device ADB Access](https://kitsumed.github.io/blog/posts/android-may-soon-restrict-on-device-adb/) ⭐️ 8.0/10

Android is reportedly planning to restrict on-device ADB (Android Debug Bridge) access in a future update, potentially limiting how developers and advanced users interact with their devices. This change could significantly impact Android developers who rely on ADB for debugging and sideloading, while also raising concerns about the balance between security and user freedom. It signals a broader trend of Android becoming less open, akin to iOS. The attack vector that this restriction targets requires both developer options and remote ADB to be enabled, which is realistic for only a small fraction of users. Google has also discussed restricting access to specific interfaces or IP addresses as an alternative.

hackernews · shscs911 · Jul 25, 06:57 · [Discussion](https://news.ycombinator.com/item?id=49045159)

**Background**: Android Debug Bridge (ADB) is a command-line tool that allows developers to communicate with Android devices for debugging, installing apps, and running shell commands. It can be used over USB or wirelessly via TCP. On-device ADB access refers to using ADB locally on the device itself, often via terminal emulators.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Android_Debug_Bridge">Android Debug Bridge - Wikipedia</a></li>
<li><a href="https://developer.android.com/tools/adb">Android Debug Bridge (adb) | Android Studio | Android Developers</a></li>
<li><a href="https://medium.com/@EazSoftware/a-comprehensive-guide-to-adb-android-debug-bridge-the-unsung-hero-for-android-developers-28b349037436">A Comprehensive Guide to ADB (Android Debug Bridge): The Unsung Hero for Android Developers | by Eaz Software | Medium</a></li>

</ul>
</details>

**Discussion**: Community comments are mixed: some argue the restriction targets a non-existent threat (requires developer options enabled), while others see it as part of Google's ongoing push to lock down Android, predicting further restrictions on sideloading and customizability. There is skepticism about Google's motives, with some users expecting eventual paid access or identity surrender.

**Tags**: `#Android`, `#ADB`, `#security`, `#developer tools`, `#privacy`

---

<a id="item-5"></a>
## [Ruff v0.16.0 Expands Default Rules from 59 to 413](https://simonwillison.net/2026/Jul/25/ruff/#atom-everything) ⭐️ 8.0/10

Ruff v0.16.0, released on July 23, 2026, increased the default rule set from 59 to 413 rules, dramatically expanding the number of potential issues detected without any configuration. This change significantly improves Python code quality by catching severe errors like syntax errors and runtime bugs that were previously only detected with explicit rule configuration, potentially breaking CI jobs but ultimately making codebases safer. Ruff now has 968 total rules, with the new defaults automatically enabling checks for issues like timezone-naive datetime usage and blind exception catching. Users can auto-fix most violations using `ruff check --fix --unsafe-fixes`.

rss · Simon Willison · Jul 25, 22:44

**Background**: Ruff is an extremely fast Python linter and code formatter written in Rust, designed to replace tools like Flake8 and Black. It is developed by Astral, which was recently acquired by OpenAI, and is known for its performance and comprehensive rule set.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.astral.sh/ruff/">An extremely fast Python linter and code formatter, written in Rust.</a></li>
<li><a href="https://astral.sh/ruff">Ruff , an extremely fast Python linter | Astral</a></li>

</ul>
</details>

**Tags**: `#ruff`, `#python`, `#linting`, `#astral`

---

<a id="item-6"></a>
## [China Fines Ctrip $800 Million for Monopoly Abuse](https://t.me/zaihuapd/42767) ⭐️ 8.0/10

On July 25, China's State Administration for Market Regulation (SAMR) fined Ctrip Group 5.179 billion yuan ($717 million) for abusing its market dominance, confiscating 1.658 billion yuan in illegal gains and imposing a 3.521 billion yuan penalty. SAMR also ordered Ctrip to cease violations, refund 122 million yuan in order reserves to hotel operators, and implement comprehensive rectifications. This fine is among the largest antitrust penalties in China's tech sector, signaling the government's intensified enforcement against platform monopolies. It will reshape competition in China's online travel market and serve as a warning to other dominant digital platforms. The penalty includes both confiscation of illegal gains and a separate fine, totaling 5.179 billion yuan. Ctrip is required to refund 122 million yuan in order reserves that were forcibly deducted from hotel operators, and must publicly disclose its corrective measures.

telegram · zaihuapd · Jul 25, 11:56

**Background**: Ctrip (now Trip.com Group) is the dominant online travel agency in China, controlling a large share of hotel and flight bookings. China's Anti-Monopoly Law prohibits abuse of market dominance, and since 2020, regulators have increasingly targeted large tech platforms for anticompetitive practices, following earlier actions against Alibaba and Tencent.

**Tags**: `#antitrust`, `#regulation`, `#China`, `#travel technology`, `#monopoly`

---

<a id="item-7"></a>
## [Microsoft to Use TPM Chips to Block Pirated Windows Activation](https://www.techspot.com/news/113232-microsoft-using-tpm-chips-crack-down-pirated-windows.html) ⭐️ 8.0/10

Microsoft announced a new TPM attestation mechanism for its enterprise KMS (Key Management Service) tools, which verifies the hardware identity of KMS servers before allowing bulk activation requests, effectively blocking long-exploited KMS-based activation exploits. This feature will become mandatory starting from the next version of Windows Server, with preparation prompts rolling out from August 2026 on Windows Server 2025. This move directly targets the most common method of software piracy for enterprise Windows versions, potentially shutting down many activation tools that rely on fake KMS servers. It also raises the bar for hardware-based security in software licensing, though the emergence of bypass methods like Massgrave's TSforge suggests an ongoing arms race. The TPM attestation will verify that the KMS server's hardware identity has been certified by Microsoft and not tampered with, before processing any activation requests. Microsoft has already shut down the KMS38 vulnerability in 2025, and the Online KMS method from the Massgrave group (which requires reconnection every six months) may be rendered ineffective; however, Massgrave recently introduced TSforge, which claims to bypass the entire Windows DRM activation architecture.

telegram · zaihuapd · Jul 25, 15:55

**Background**: KMS (Key Management Service) is a legitimate enterprise volume activation method designed to allow organizations to activate multiple Windows or Office machines using a local KMS host. Over the years, attackers have set up fake KMS servers that mimic the real ones to activate software without valid licenses. TPM (Trusted Platform Module) is a hardware security chip that stores encryption keys and verifies system integrity; it has been required for Windows 11 but is now being leveraged for activation security.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.pingcode.com/ask/241653.html">TPM 芯 片 的工作原理是什么 – PingCode</a></li>
<li><a href="https://www.laoliang.net/jsjh/technology/13891.html">Windows系统下 KMS （ 批 量 授权）和HWID...</a></li>
<li><a href="https://massgrave.dev/blog/tsforge">TSforge | MAS</a></li>

</ul>
</details>

**Tags**: `#微软`, `#TPM`, `#Windows激活`, `#安全`, `#反盗版`

---

<a id="item-8"></a>
## [DeepSeek Halts New Funding Round Over Leaked Comments](https://www.bloomberg.com/news/articles/2026-07-25/deepseek-said-to-tell-backers-of-funding-pause-after-viral-posts) ⭐️ 8.0/10

DeepSeek has orally informed some second-round investors that it is pausing the signing of investment agreements, partly due to founder Liang Wenfeng's anger over leaked internal discussions. The company still plans to proceed with an IPO. This suspension highlights the sensitivity of internal communications in high-profile AI startups and could affect investor confidence. It also delays a major funding round that was expected to raise at least 10 billion yuan at a valuation of 480 billion yuan, impacting the AI funding landscape. The company raised $7 billion in its first funding round in June 2026, with investors including Tencent, CATL, and a national AI industry fund. The paused round was expected to value the company at no less than 480 billion yuan pre-money.

telegram · zaihuapd · Jul 26, 01:17

**Background**: DeepSeek is a Chinese AI startup that has gained prominence for developing competitive large language models. The company's rapid growth and high-profile funding rounds have drawn significant attention in the AI industry. The founder Liang Wenfeng is known for his aggressive vision and has been vocal about the company's direction.

**Tags**: `#DeepSeek`, `#funding`, `#AI`, `#IPO`, `#business news`

---

<a id="item-9"></a>
## [Silicon Valley Coalition Opposes Ban on Chinese Open-Weight AI](https://t.me/zaihuapd/42772) ⭐️ 8.0/10

Nearly 200 Silicon Valley companies, including Y Combinator and Proton, have sent a letter to the Trump administration opposing any ban on Chinese open-weight AI models, arguing it would harm U.S. startups and proposing targeted security measures instead. This coalition represents a significant industry pushback against potential U.S. policy that could restrict access to cost-effective AI models, impacting the competitive landscape for AI startups and US-China tech relations. The letter was organized by the Little Tech Association. They argue that a blanket ban would cripple next-generation U.S. startups that rely on affordable Chinese open-weight models, and that more targeted security measures would be preferable.

telegram · zaihuapd · Jul 26, 02:00

**Background**: An open-weight AI model refers to a model whose trained parameters (weights) are publicly released, allowing developers to download, fine-tune, and deploy the model. Unlike open-source, which includes the full training code and data, open-weight models provide the final weights. Chinese open-weight models, such as those from DeepSeek, have become popular in the startup community for their affordability and competitive performance.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/openais-open-weight-model-what-means-developers-ai-industry-tsi9f">OpenAI’s Open - Weight Model : What It Means for Developers and the...</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#US-China tech relations`, `#open-source AI`, `#startups`, `#regulation`

---