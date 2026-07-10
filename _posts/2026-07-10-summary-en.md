---
layout: default
title: "Horizon Summary: 2026-07-10 (EN)"
date: 2026-07-10
lang: en
---

> From 38 items, 10 important content pieces were selected

---

1. [OpenAI Releases GPT-5.6, Sets New SOTA on ARC-AGI-3](#item-1) ⭐️ 10.0/10
2. [EU Parliament Approves Chat Control 1.0 via Loophole](#item-2) ⭐️ 9.0/10
3. [TypeScript 7.0 Released: Go Rewrite Delivers Up to 12x Speed Boost](#item-3) ⭐️ 9.0/10
4. [Ant Open-Sources LingBot-Video: First MoE Embodied Video Model](#item-4) ⭐️ 9.0/10
5. [Rust Rewrite of PostgreSQL Passes All Regression Tests](#item-5) ⭐️ 8.0/10
6. [Meta Launches Muse Spark 1.1 Agentic AI Model](#item-6) ⭐️ 8.0/10
7. [Meta Superintelligence Update: RL Startup, Compute Ramp, Advice](#item-7) ⭐️ 8.0/10
8. [DJI EV50 VTOL Drone Surmounts Everest at 8,861m](#item-8) ⭐️ 8.0/10
9. [National Supercomputing Internet Core Node Launches in Zhengzhou with 100K+ Domestic AI Cards](#item-9) ⭐️ 8.0/10
10. [OpenAI and US War Dept Plan to Ban AI Surveillance of Citizens](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI Releases GPT-5.6, Sets New SOTA on ARC-AGI-3](https://openai.com/index/gpt-5-6/) ⭐️ 10.0/10

OpenAI released GPT-5.6, its latest frontier model, which achieves a new state-of-the-art score of 7.8% on the ARC-AGI-3 benchmark and introduces features like intent understanding and original image detail preservation. The model comes in three sizes: Luna, Terra, and Sol. This release advances the frontier of AI reasoning and agentic capabilities, as GPT-5.6 is the first verified frontier model to beat an ARC-AGI-3 game. The improved intent understanding reduces the need for explicit step-by-step instructions, potentially lowering the barrier for complex task automation. The three model sizes are priced at Luna $1/$6, Terra $2.50/$15, and Sol $5/$30 per 1M input/output tokens. GPT-5.6 also scores highly on BenchCAD, suggesting specific training on programmatic CAD data.

hackernews · logickkk1 · Jul 9, 17:04 · [Discussion](https://news.ycombinator.com/item?id=48849066)

**Background**: ARC-AGI-3 is an interactive reasoning benchmark that challenges AI agents to explore novel environments, infer goals, and plan actions through abstract turn-based games. It is designed to measure human-like intelligence and agentic capabilities. Frontier models like GPT-5.6 represent the most advanced AI systems, typically combining large-scale pre-training with reasoning techniques.

<details><summary>References</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>
<li><a href="https://arxiv.org/abs/2603.24621">[2603.24621] ARC-AGI-3: A New Challenge for Frontier Agentic Intelligence</a></li>

</ul>
</details>

**Discussion**: Community reactions are broadly positive, with praise for the intent understanding and image preservation features, as well as the new SOTA on ARC-AGI-3. Some users note that OpenAI omitted comparisons with Fable 5 on biology benchmarks because Fable 5 refused to answer advanced biology questions. Developers also debate whether to switch from Claude Code to OpenAI's codex model.

**Tags**: `#GPT-5.6`, `#OpenAI`, `#AI`, `#frontier model`, `#ARC-AGI-3`

---

<a id="item-2"></a>
## [EU Parliament Approves Chat Control 1.0 via Loophole](https://www.patrick-breyer.de/en/eu-parliament-greenlights-chat-control-1-0-breyer-our-children-lose-out/) ⭐️ 9.0/10

The European Parliament approved the extension of Chat Control 1.0, a regulation allowing US tech companies to scan private messages without a warrant until 2028, despite a majority of MEPs voting against it (314 against, 276 in favor, 17 abstentions). The measure passed because a motion to reject it failed to secure the required absolute majority of 361 votes. This decision sets a concerning precedent for digital privacy and encryption in the EU, potentially undermining end-to-end encryption and enabling mass surveillance. It affects millions of users on platforms like Instagram, Discord, Snapchat, Gmail, and iCloud, and may embolden similar measures elsewhere. The regulation, known as Chat Control 1.0, was initially a temporary measure in 2021 and was set to expire, but its extension was fast-tracked and passed on July 9, 2026, using an urgency procedure that required an absolute majority to reject. The law allows client-side scanning of private messages for child sexual abuse material, but critics argue it effectively mandates mass surveillance and breaks encryption.

hackernews · rapnie · Jul 9, 11:03 · [Discussion](https://news.ycombinator.com/item?id=48843923)

**Background**: Chat Control is an EU regulation aimed at combating child sexual abuse online by requiring digital platforms to detect and report such material. Civil society groups argue that the proposal undermines end-to-end encryption and violates fundamental privacy rights. The first version (Chat Control 1.0) was a temporary measure that ended in March 2026, but it has now been revived until 2028. A more comprehensive Chat Control 2.0 is still under discussion.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control_1.0">Chat Control 1.0</a></li>
<li><a href="https://www.techtimes.com/articles/320010/20260709/eu-parliament-passes-chat-control-default-314-meps-couldnt-block-scanning-law.htm">EU Parliament Passes Chat Control by Default: 314 MEPs Couldn ...</a></li>
<li><a href="https://samsungmagazine.eu/en/2026/07/09/chat-control/">The end of privacy on the internet. Chat Control passed the ...</a></li>

</ul>
</details>

**Discussion**: Community comments strongly criticize the parliamentary procedure as an undemocratic trick, noting that the vote was held before the summer break and required an absolute majority to reject, allowing a minority to pass the law. Commenters express concern that this sets a dangerous precedent for a 'totalitarian' EU and undermines the legitimacy of the EU project.

**Tags**: `#privacy`, `#EU regulation`, `#mass surveillance`, `#encryption`, `#digital rights`

---

<a id="item-3"></a>
## [TypeScript 7.0 Released: Go Rewrite Delivers Up to 12x Speed Boost](https://devblogs.microsoft.com/typescript/announcing-typescript-7-0/) ⭐️ 9.0/10

Microsoft has officially released TypeScript 7.0, a native version rewritten in Go that achieves 8-12x faster complete builds and supports shared-memory multi-threading. The new language server can be used via LSP in mainstream editors. This is a paradigm shift in TypeScript tooling, dramatically improving developer productivity by reducing build times and enabling parallel project builds. The Go rewrite signals a major architectural move that could influence other compiler projects. TypeScript 7.0 introduces --checkers and --builders parameters to customize parallelism, but embedded language toolchains for Vue and Svelte are not yet supported and must continue using TypeScript 6. A compatibility package allows side-by-side installation with TypeScript 6.

telegram · zaihuapd · Jul 9, 04:01

**Background**: TypeScript is a typed superset of JavaScript that compiles to plain JavaScript, widely used for large-scale web development. The Language Server Protocol (LSP) standardizes communication between editors and language servers, enabling features like autocomplete and diagnostics. Previous TypeScript versions were written in TypeScript itself, leading to performance bottlenecks in large projects.

<details><summary>References</summary>
<ul>
<li><a href="https://devblogs.microsoft.com/typescript/announcing-typescript-7-0/">Announcing TypeScript 7.0 - TypeScript</a></li>
<li><a href="https://en.wikipedia.org/wiki/Language_Server_Protocol">Language Server Protocol - Wikipedia</a></li>
<li><a href="https://devblogs.microsoft.com/typescript/announcing-typescript-7-0-rc/">Announcing TypeScript 7.0 RC - TypeScript</a></li>

</ul>
</details>

**Tags**: `#TypeScript`, `#Microsoft`, `#Performance`, `#Compiler`

---

<a id="item-4"></a>
## [Ant Open-Sources LingBot-Video: First MoE Embodied Video Model](https://www.qbitai.com/2026/07/446458.html) ⭐️ 9.0/10

Ant Group's Lingbot has open-sourced LingBot-Video, the world's first Mixture-of-Experts (MoE) based embodied intelligence video generation foundation model. It has 30 billion total parameters but activates only about 3 billion during generation, achieving roughly 3x inference efficiency compared to dense architectures of similar scale. This represents a significant breakthrough in embodied AI, offering a more efficient and capable foundation model for robot action prediction, simulation data generation, and world model research. By open-sourcing, Ant Group may accelerate progress in the robotics and embodied intelligence field. The model adopts a DiT+MoE architecture, uses a 70,000-hour embodied data engine covering dexterous manipulation, robot movement, and first-person interaction, and introduces a multi-dimensional reinforcement learning reward system focusing on physical plausibility and task completion. It is released under the Apache 2.0 license on GitHub.

telegram · zaihuapd · Jul 9, 04:30

**Background**: The Mixture of Experts (MoE) architecture uses multiple specialized sub-networks (experts) with a router to activate only relevant experts per input, enabling larger models with lower computational cost. DiT (Diffusion Transformer) combines diffusion models with Transformer architecture for high-quality video generation. Embodied intelligence refers to AI systems that can perceive and act in the physical world, such as robots.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/mixture-of-experts/">What Is Mixture of Experts (MoE) and How It Works?</a></li>
<li><a href="https://huggingface.co/docs/diffusers/api/pipelines/dit">DiT · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#MoE`, `#具身智能`, `#视频生成`, `#机器人`, `#开源`

---

<a id="item-5"></a>
## [Rust Rewrite of PostgreSQL Passes All Regression Tests](https://github.com/malisper/pgrust) ⭐️ 8.0/10

A developer successfully rewrote PostgreSQL in Rust, achieving 100% pass rate on the official PostgreSQL regression test suite using LLM-generated code. This demonstrates the feasibility of rewriting a mature, complex database system in a memory-safe language, potentially improving safety and performance while maintaining full compatibility. The project, pgrust, uses LLMs to generate 7101 commits in under a month, sparking debate about code review and long-term maintainability.

hackernews · SweetSoftPillow · Jul 9, 06:18 · [Discussion](https://news.ycombinator.com/item?id=48841676)

**Background**: PostgreSQL is a 30-year-old relational database written in C. The regression test suite is a comprehensive set of SQL tests ensuring correctness. Rust is a systems programming language known for memory safety without garbage collection.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/malisper/pgrust">GitHub - malisper/pgrust: Postgres rewritten in Rust, now ...</a></li>
<li><a href="https://malisper.me/pgrust-rebuilding-postgres-in-rust-with-ai/">pgrust: Rebuilding Postgres in Rust with AI - malisper.me</a></li>
<li><a href="https://www.postgresql.org/docs/current/regress.html">PostgreSQL: Documentation: 18: Chapter 31. Regression Tests</a></li>

</ul>
</details>

**Discussion**: Community members expressed concerns about single-person rewrites, maintainability, and the use of AI-generated code, with suggestions for testing under real workloads and skepticism about long-term viability.

**Tags**: `#PostgreSQL`, `#Rust`, `#database`, `#rewrite`, `#LLM`

---

<a id="item-6"></a>
## [Meta Launches Muse Spark 1.1 Agentic AI Model](https://ai.meta.com/blog/introducing-muse-spark-meta-model-api/) ⭐️ 8.0/10

Meta announced Muse Spark 1.1, a new agentic AI model with API pricing, alongside an evaluation report and developer resources. The model supports text, image, and speech input and has a 262k context window. This release signals Meta's entry into the commercial agentic AI market, with pricing significantly lower than competitors like Anthropic and OpenAI. It could commoditize coding agents and pressure other providers to lower prices. Pricing is set at $1.25 per million tokens for input and $4.5 for output, with cached input at $0.15. The model features tool-use, visual chain-of-thought, and multi-agent orchestration, but is not open-source.

hackernews · ot · Jul 9, 14:10 · [Discussion](https://news.ycombinator.com/item?id=48846184)

**Background**: Agentic AI refers to systems that can use tools, plan, and act autonomously to achieve goals. Meta's previous AI models were often open-weight, but Muse Spark is closed-source and accessed via API, reflecting a strategic shift toward monetization.

<details><summary>References</summary>
<ul>
<li><a href="https://ai.meta.com/blog/introducing-muse-spark-meta-model-api/">Introducing Muse Spark 1.1</a></li>
<li><a href="https://artificialanalysis.ai/models/muse-spark">Muse Spark - Intelligence, Performance & Price Analysis</a></li>
<li><a href="https://agentic.ai/what-is-agentic-ai">What Is Agentic AI? Definition, 6 Levels & Examples (2026)</a></li>

</ul>
</details>

**Discussion**: Developers raised concerns about benchmark validity, noting that evaluation tasks exceeded resource limits. Others praised the low pricing and practical usability, while some criticized the closed-source approach, arguing only Anthropic and OpenAI matter in closed-source AI.

**Tags**: `#AI`, `#Meta`, `#Muse Spark`, `#agentic model`, `#open source`

---

<a id="item-7"></a>
## [Meta Superintelligence Update: RL Startup, Compute Ramp, Advice](https://newsletter.semianalysis.com/p/the-future-of-meta-superintelligence) ⭐️ 8.0/10

A new top-tier reinforcement learning environment startup has emerged from Meta's superintelligence efforts, alongside the most aggressive compute ramp to date, scaling across more than 2000 km, and direct advice for Google DeepMind. This update signals Meta's intensified push toward superintelligence, potentially reshaping the competitive landscape among AI labs and driving unprecedented infrastructure investments. The compute ramp includes a new 'Tent' datacenter design enabling expedited scaling, and the RL environment startup is described as spawning 'out of thin air,' likely indicating talent acquisitions or internal spin-offs.

rss · Semianalysis · Jul 9, 19:16

**Background**: Reinforcement learning (RL) environments are virtual sandboxes where AI models learn by taking actions and receiving scores. Scale-across networking interconnects data centers across hundreds of kilometers to form a single supercomputer. Meta's superintelligence initiative aims to achieve artificial general intelligence (AGI) or beyond, requiring massive compute and specialized infrastructure.

<details><summary>References</summary>
<ul>
<li><a href="https://benanderson.work/blog/dont-build-rl-env-startup/">Don't Build an RL Environment Startup</a></li>
<li><a href="https://www.broadcom.com/topics/what-is-scale-across-networking-for-ai-clusters">Scale-across Networking | AI Clusters | AI Infrastructure</a></li>
<li><a href="https://www.keysight.com/blogs/en/inds/ai/ai-infrastructure-scaling-domains">AI Infrastructure Scaling Domains</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Meta`, `#superintelligence`, `#reinforcement learning`, `#compute infrastructure`

---

<a id="item-8"></a>
## [DJI EV50 VTOL Drone Surmounts Everest at 8,861m](https://www.163.com/dy/article/L1CUCV940514R9OJ.html) ⭐️ 8.0/10

DJI's unreleased EV50 VTOL cargo drone flew over Mount Everest at 8,861 meters, setting a record for high-altitude drone flight and collecting atmospheric data at above 8,000m. This achievement demonstrates DJI's engineering capability for extreme environments and showcases the potential of VTOL drones for high-altitude logistics and scientific research. The EV50 is a composite-wing drone that takes off and lands vertically and switches to fixed-wing cruise. During a 12-day mission, it completed 32 sorties, climbed 3,730m continuously, and returned with 30% battery remaining.

telegram · zaihuapd · Jul 9, 06:00

**Background**: VTOL (Vertical Take-Off and Landing) drones combine the flexibility of multirotors with the efficiency of fixed-wing aircraft. High-altitude flight above 8,000m presents challenges like thin air and extreme cold, requiring robust propulsion and battery systems. DJI is known for consumer drones but is now entering the cargo drone market.

<details><summary>References</summary>
<ul>
<li><a href="https://dronexl.co/2026/07/09/dji-ev50-evtol-delivery-drone-everest/">DJI EV50 Debuts As Company's First EVTOL Delivery Drone With ...</a></li>
<li><a href="https://pandaily.com/dji-ev50-everest-vtol-cargo-drone-jul2026">DJI Unreleased EV50 VTOL Cargo Drone Flies Above Everest ...</a></li>
<li><a href="https://aviationweek.com/business-aviation/aircraft-propulsion/dji-enters-fixed-wing-evtol-cargo-drone-market">DJI Enters Fixed-Wing eVTOL Cargo Drone Market</a></li>

</ul>
</details>

**Tags**: `#drone`, `#VTOL`, `#high-altitude`, `#logistics`, `#DJI`

---

<a id="item-9"></a>
## [National Supercomputing Internet Core Node Launches in Zhengzhou with 100K+ Domestic AI Cards](https://36kr.com/newsflashes/3887797387344387) ⭐️ 8.0/10

On July 9, 2026, the core node of China's National Supercomputing Internet officially went live in Zhengzhou, offering over 100,000 domestic AI computing cards. This marks the largest single domestic AI computing resource pool ever connected to the platform. This milestone significantly strengthens China's self-reliance in AI computing infrastructure, providing a unified scheduling system for computational resources nationwide. It accelerates AI research, industrial simulation, and scientific computing by offering massive domestic computing power. The core node integrates over 100,000 domestic AI accelerators (e.g., Cambricon, Huawei Ascend) and serves as the operations management and resource dispatch hub for the National Supercomputing Internet platform. It also provides services for supply-demand matching and industry incubation.

telegram · zaihuapd · Jul 9, 07:00

**Background**: The National Supercomputing Internet is a national initiative led by the Ministry of Science and Technology, launched in April 2023, to connect supercomputing centers across China into a unified service network. Its goal is to break down silos between individual computing centers and enable efficient allocation of computing resources for scientific research, AI training, and industrial applications.

<details><summary>References</summary>
<ul>
<li><a href="https://local.cctv.com/2026/07/09/ARTIGxl4CPHCEclGCTrNzq34260709.shtml">国内首个十万卡级超智融合算力资源池在郑上线_地方频道_央视网 (cct...</a></li>
<li><a href="https://baike.baidu.com/item/国家超算互联网/62902938">国家超算互联网 - 百度百科 国家超算互联网 - 高性能计算服务与 AI 服务平台 - AIHub 国家超算互联网平台上线 - 中国政府网 超算互联网 - 百度百科 国家超算互联网用户规模破百万 - 中国政府网 国家超算互联网正式上线 DeepSeek，全民可用！国家队强势助力！</a></li>
<li><a href="https://www.scnet.cn/home/internet/index.html">超算互联网 - scnet.cn</a></li>

</ul>
</details>

**Tags**: `#supercomputing`, `#AI infrastructure`, `#domestic chips`, `#China`, `#national computing network`

---

<a id="item-10"></a>
## [OpenAI and US War Dept Plan to Ban AI Surveillance of Citizens](https://t.me/zaihuapd/42459) ⭐️ 8.0/10

OpenAI and the US War Department (formerly the Department of Defense) have agreed to amend their AI collaboration contract to prohibit the use of AI for deliberate surveillance of US citizens, a proposal initiated by OpenAI CEO Sam Altman. This move addresses growing public concern over AI being used for mass surveillance by the military, setting a precedent for ethical boundaries in government AI contracts. It also contrasts with a similar stalled agreement between competitor Anthropic and the War Department. The revised clauses explicitly forbid using AI systems for intentional surveillance of US citizens and prohibit tracking or monitoring using personally identifiable information obtained commercially. The amendment has not yet been formally signed.

telegram · zaihuapd · Jul 9, 13:22

**Background**: The US War Department is the former name of the Department of Defense; it is involved in AI partnerships for national security. Concerns about AI-powered surveillance have intensified after reports of other AI companies, such as Anthropic, facing controversy over similar military contracts. OpenAI's proposal aims to ensure AI is used responsibly without infringing on civil liberties.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>
<li><a href="https://www.anthropic.com/">Home \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#AI ethics`, `#OpenAI`, `#US government`, `#surveillance`, `#policy`

---