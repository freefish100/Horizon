---
layout: default
title: "Horizon Summary: 2026-08-04 (EN)"
date: 2026-08-04
lang: en
---

> From 45 items, 13 important content pieces were selected

---

1. [LLMs Amplify Expertise Rather Than Replace It](#item-1) ⭐️ 8.0/10
2. [OpenAI Highlights Ten Advances in Mathematics and Theoretical Computer Science](#item-2) ⭐️ 8.0/10
3. [MiniMax H3 Gets Day-0 ComfyUI Support: Open Weights, Native Audio, 2K Video](#item-3) ⭐️ 8.0/10
4. [Andy Pavlo Joins ClickHouse to Launch ClickHouse Labs](#item-4) ⭐️ 8.0/10
5. [Bonsai: Jane Street's OCaml UI Library](#item-5) ⭐️ 8.0/10
6. [LLMs Make Open Source Software More Accessible for Modification](#item-6) ⭐️ 8.0/10
7. [Kimi K3 Analysis: Compressed Memory, Depth Attention, Latent Routing](#item-7) ⭐️ 8.0/10
8. [Time to Desk Reject ML Papers Without Reproducible Code](#item-8) ⭐️ 8.0/10
9. [Qwen3.8-Max open-weight model matches Kimi K3 and DeepSeek V4 Flash](#item-9) ⭐️ 8.0/10
10. [DeepSeek V4-Flash 284B MoE runs at 33 tok/s on used dual-Xeon and 2× RTX 3090](#item-10) ⭐️ 8.0/10
11. [Security Flaw in DNA Analyzers Puts 30 Years of Crime Evidence at Risk](#item-11) ⭐️ 8.0/10
12. [Cracked Nvidia CMP 170HX unlocks 80GB VRAM, 94 TFLOPS; used prices soar](#item-12) ⭐️ 8.0/10
13. [Telegram Removed from App Store Across 175 Regions](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [LLMs Amplify Expertise Rather Than Replace It](https://www.seangoedecke.com/llms-reward-expertise/) ⭐️ 8.0/10

The article argues that LLMs reward expertise by amplifying the existing skills of experienced software engineers, rather than allowing novices to bypass learning. It has drawn substantial engagement, with 461 points and 199 comments on Hacker News. This counters the popular narrative that LLMs will democratize software development for everyone. It suggests that deep expertise and codebase familiarity remain crucial, guiding how developers and companies should adopt AI-assisted tools. The essay argues that LLM output quality depends on the user's domain knowledge, codebase familiarity, and ability to evaluate the generated code. It also highlights that knowing what to ask and how to integrate the code is more valuable than merely generating code.

hackernews · MaxMussio · Aug 3, 21:13 · [Discussion](https://news.ycombinator.com/item?id=49161518)

**Background**: Large language models (LLMs) like GPT-4 can generate code, leading to widespread claims that anyone can build software with AI. However, this essay argues that successful use of LLMs still requires engineering expertise, because users must formulate prompts, judge outputs, and fit them into a larger system. This piece is part of a broader industry debate about whether AI-assisted development democratizes programming or simply amplifies existing skills.

**Discussion**: The comments largely match the article's thesis, sharing real-world experiments where LLMs failed without sufficient user expertise. One commenter likened LLMs to an 'amplifying mirror' that reflects the user's own interaction quality, while another noted that codebase familiarity is often a bottleneck. A few commenters cautioned about confirmation bias and called for formal study.

**Tags**: `#LLMs`, `#AI-assisted development`, `#software engineering`, `#expertise`, `#developer tools`

---

<a id="item-2"></a>
## [OpenAI Highlights Ten Advances in Mathematics and Theoretical Computer Science](https://openai.com/index/ten-advances-in-mathematics/) ⭐️ 8.0/10

OpenAI published a post titled 'Ten advances in mathematics and theoretical computer science,' highlighting a series of AI-driven breakthroughs in these fields. The announcement has generated widespread discussion about the accelerating impact of AI on mathematical research. This matters because it signals that AI is moving beyond routine automation into core mathematical discovery, potentially reshaping how research is done. It also fuels debate about the pace of progress and its implications for areas like post-quantum cryptography. The post does not appear to list specific results in the provided content, but commenters reference the nearest vector problem and post-quantum cryptography, suggesting some advances relate to lattice-based problems. The original article is hosted on OpenAI's website.

hackernews · milkshakes · Aug 3, 16:27 · [Discussion](https://news.ycombinator.com/item?id=49157930)

**Background**: OpenAI is an artificial intelligence research organization known for large language models and other AI systems. This announcement likely relates to using AI models to generate or verify mathematical proofs, a growing area of interest known as 'AI for math.' The mathematization of AI research may also enable faster discovery of new algorithms and theorems.

**Discussion**: Commenters express both excitement and concern. One notes that fast solutions to the nearest vector problem would impact post-quantum cryptography deployments, while another observes that progress seems to follow an exponential curve, with writing and politics being more stubborn to crack. Some users also question the promotion mechanics of the post on Hacker News.

**Tags**: `#AI`, `#mathematics`, `#theoretical computer science`, `#OpenAI`, `#research`

---

<a id="item-3"></a>
## [MiniMax H3 Gets Day-0 ComfyUI Support: Open Weights, Native Audio, 2K Video](https://blog.comfy.org/p/minimax-h3-day-0-support-in-comfyui) ⭐️ 8.0/10

ComfyUI has released day-0 support for MiniMax H3, an open-weight omni-modal model that generates up to 2K video with native stereo audio and accepts combined text, image, video, and audio inputs. The integration lets users run the model locally via ComfyUI's node-based interface. Because MiniMax H3 is open-weight and ComfyUI is the de facto node-based workflow tool for AI generation, this integration lowers the barrier for creators to experiment with state-of-the-art multimodal video generation, including native audio, without relying on closed APIs. It also signals a trend toward day-0 support for major new models across the diffusion ecosystem. The model can generate up to 15 seconds of 2K video with native stereo audio, and MiniMax reports that pruning a large portion of modulation weights into a lookup table plus dynamic VRAM offloading cuts memory use from 123.6 GB to 42.5 GB, enabling local runs on GPUs like the RTX 3060. Early users report long generation times on consumer hardware — about 10 minutes for a 10-second 480p video on a 16 GB RTX 4070 Ti Super.

hackernews · vblanco · Aug 3, 13:34 · [Discussion](https://news.ycombinator.com/item?id=49155629)

**Background**: MiniMax (稀宇科技) is a Shanghai-based AI company known for multimodal models, consumer apps like Talkie and Xingye, and the video-generation service Hailuo AI. ComfyUI is an open-source, node-based interface for building diffusion-model workflows, widely used in the AI art and video community. 'Day-0 support' means a tool is ready to run a newly released model on the same day it launches, as seen recently with vLLM's Kimi K3 support and AMD's Qwen 3.5 support. MiniMax H3 itself is positioned as a general-purpose omni-modal generation model that jointly understands text, images, video, and audio.

<details><summary>References</summary>
<ul>
<li><a href="https://www.minimax.io/blog/minimax-h3">MiniMax H3: An Open Model Breaking the Boundaries Between Tasks and Modalities - MiniMax Research | MiniMax</a></li>
<li><a href="https://fal.ai/minimax-h3">MiniMax H3 - Open-Weights General-Purpose Multimodal Video Model | fal</a></li>
<li><a href="https://en.wikipedia.org/wiki/MiniMax_Group">MiniMax Group</a></li>

</ul>
</details>

**Discussion**: Community reaction is largely positive: users call the output 'spectacular' and note a 'pretty big leap' over current state-of-the-art models, while also cautioning that unusual or surreal prompts still produce janky results and some clips retain an 'AI smoothening' artifact. One commenter questions the claimed lossless weight-pruning technique and asks whether it could apply to LLMs, while another shares concrete performance numbers on consumer hardware, noting both the long render time and the impressive quality.

**Tags**: `#ComfyUI`, `#MiniMax`, `#video generation`, `#open source`, `#AI`

---

<a id="item-4"></a>
## [Andy Pavlo Joins ClickHouse to Launch ClickHouse Labs](https://clickhouse.com/blog/andy-pavlo-joins-clickhouse) ⭐️ 8.0/10

Andy Pavlo, a prominent database researcher, has joined ClickHouse to establish ClickHouse Labs, a new research lab focused on database systems research and OLAP architecture. This marks a notable industry-academia collaboration and reflects a broader trend of corporate research labs in non-AI infrastructure. It could influence the future direction of OLAP database innovation and open-source database development. ClickHouse is an open-source column-oriented DBMS for online analytical processing (OLAP). Andy Pavlo is well known for his CMU database lecture series, and community members hope those lectures will continue in a sponsored format.

hackernews · nikolay_sivko · Aug 3, 14:09 · [Discussion](https://news.ycombinator.com/item?id=49156011)

**Background**: ClickHouse is a column-oriented SQL database management system designed for OLAP, enabling real-time analytical reports from large datasets. OLAP databases are typically optimized for complex analytical queries and often use denormalized schemas or star schemas to improve query performance.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ClickHouse">ClickHouse - Wikipedia</a></li>
<li><a href="https://clickhouse.com/docs/intro">What is ClickHouse? - ClickHouse Documentation</a></li>

</ul>
</details>

**Discussion**: The community response is largely positive, with commenters praising the industry-academia collaboration and Andy Pavlo's lectures. Some urged ClickHouse to fund academic database research amid shrinking government and AI-focused funding, while others discussed the convergence of OLAP architectures like StarRocks, ClickHouse, and Trino around decoupled compute and storage.

**Tags**: `#database`, `#clickhouse`, `#research`, `#olap`, `#industry-academia`

---

<a id="item-5"></a>
## [Bonsai: Jane Street's OCaml UI Library](https://github.com/janestreet/bonsai) ⭐️ 8.0/10

Jane Street has released Bonsai, a UI library for building dynamic, reactive web applications in OCaml. The library enables developers to use OCaml on both the frontend and backend, allowing shared types and functional programming patterns across the full stack. This matters because it allows teams to write both client and server code in one language, increasing type safety and code reuse. It also highlights Jane Street's investment in functional programming and open-sourcing internal tools, which could strengthen the OCaml ecosystem. Bonsai is partly inspired by Elm and is used internally at Jane Street for almost all web applications, from the corporate directory to tools that monitor trading systems. Adopting Bonsai may mean moving away from the JavaScript ecosystem, such as React and GraphQL.

hackernews · KolmogorovComp · Aug 3, 08:29 · [Discussion](https://news.ycombinator.com/item?id=49152842)

**Background**: OCaml is a general-purpose, high-level, multi-paradigm programming language created in 1996, known for expressiveness and safety. Bonsai is a UI library for building reactive web applications in OCaml, and Jane Street uses it to build nearly all of its internal web apps. The library's design emphasizes type safety and functional programming, drawing inspiration from the Elm architecture.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/janestreet/bonsai">GitHub - janestreet/bonsai: A library for building dynamic webapps ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/OCaml_programming_language">OCaml programming language</a></li>
<li><a href="https://ocaml.org/">Welcome to a World of OCaml</a></li>

</ul>
</details>

**Discussion**: Commenters were generally enthusiastic about using OCaml across the stack, with one saying they were waiting for this possibility. Some compared Bonsai to Melange, questioning whether it means giving up the JS ecosystem, while others raised concerns about the aesthetics of the UI and practical adoption compared to tools like Tailwind CSS.

**Tags**: `#OCaml`, `#UI library`, `#functional programming`, `#web development`, `#Jane Street`

---

<a id="item-6"></a>
## [LLMs Make Open Source Software More Accessible for Modification](https://simonwillison.net/2026/Aug/3/devtools-must-be-open-source-exedev/#atom-everything) ⭐️ 8.0/10

Simon Willison argues that large language models (LLMs) now reduce the friction of reading, building, and modifying open source code, making the original promise of open source more feasible for ordinary users. He describes daily use of AI assistants like Claude and Codex to clone repositories, explain internals, and compile projects. This matters because it suggests AI tools could dramatically lower the barrier to user participation in open source, potentially reviving its core ideals of transparency and modifiability. If more people can engage with source code, the open source ecosystem could see broader contributions and deeper trust. Willison notes that getting software to compile used to be enough friction that he often skipped the effort, but now he treats it as a zero-time-investment challenge for coding agents. He says he is not yet habitually modifying software, but he can see a path to doing so that did not exist a year ago.

rss · Simon Willison · Aug 3, 15:30

**Background**: Open source software grants users the freedom to examine, modify, and redistribute code. However, for most people, even expert programmers, reading and modifying the source of tools they use is too time-consuming. LLMs like Claude and coding agents like Codex or Claude Code are AI systems that can interpret, explain, and edit code, reducing that time investment drastically.

**Tags**: `#open source`, `#LLM`, `#developer tools`, `#AI`, `#software engineering`

---

<a id="item-7"></a>
## [Kimi K3 Analysis: Compressed Memory, Depth Attention, Latent Routing](https://newsletter.semianalysis.com/p/kimi-k3-the-manos-the-mythos-the) ⭐️ 8.0/10

SemiAnalysis published a detailed technical analysis of Kimi K3's architecture, highlighting its use of compressed memory, attention across depth, and latent expert routing to achieve strong inference performance. This analysis is significant because it reveals novel architectural mechanisms that could influence future LLM design, especially in memory efficiency and routing. These techniques may help reduce inference costs while maintaining quality, impacting the broader AI systems field. The article covers three specific mechanisms: compressed memory to reduce context footprint, attention across depth to allow layers to selectively reuse earlier representations, and latent expert routing to improve MoE efficiency. The analysis also benchmarks inference performance, suggesting practical gains in speed and memory usage.

rss · Semianalysis · Aug 3, 19:42

**Background**: Transformers typically add each layer's output to a residual stream, limiting selective reuse of earlier representations; depth-attention methods seek to change this. Mixture-of-experts (MoE) models rely on routing to select experts, and latent routing methods aim to improve load balancing and expert utilization. Memory compression techniques help manage long context windows by reducing the memory footprint of conversational history or key-value caches.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2606.05014">Depth-Attention: Cross-Layer Value Mixing for Language Models</a></li>
<li><a href="https://arxiv.org/html/2506.21328">Latent Prototype Routing: Achieving Near-Perfect Load Balancing in Mixture-of-Experts Preprint - Work in Progress. Code: Here</a></li>
<li><a href="https://arxiv.org/abs/2601.00756">[2601.00756] Memory Bank Compression for Continual Adaptation of Large Language Models</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#Model Architecture`, `#Inference`, `#Memory`, `#AI Systems`

---

<a id="item-8"></a>
## [Time to Desk Reject ML Papers Without Reproducible Code](https://www.reddit.com/r/MachineLearning/comments/1vei12v/its_time_to_desk_reject_papers_that_dont_include/) ⭐️ 8.0/10

A machine learning reviewer reports that out of 12 papers reviewed for NeurIPS and two other major conferences this year, only 1 provided full runnable code, 4 gave partial code, and 7 provided no code at all. They argue for desk rejecting papers that do not include code to reproduce results. This proposal directly addresses the reproducibility crisis in machine learning research. If adopted, it could fundamentally change author incentives, improve the reliability of published results, and set a precedent for mandatory code sharing across AI conferences. The reviewer noted that of the 5 papers with at least some code, 3 contained obvious bugs that invalidated the results. They suggest that hiding code is incentivized because releasing it only increases the risk of rejection when reviewers find bugs.

reddit · r/MachineLearning · /u/Flaky-Ambition5900 · Aug 3, 16:17

**Background**: In machine learning research, reproducible results require sharing the code that trains the model and produces metrics like AUROC (Area Under the Receiver Operating Characteristic curve), which measures a model's ability to discriminate between classes. Desk rejection is when editors or chairs reject a paper without sending it to review, often due to missing essential elements. Many researchers still omit code, partly because there are few penalties and a fear that bugs will be discovered. Standards for reproducibility, such as publishing data, model, and code, are being proposed in various fields.

<details><summary>References</summary>
<ul>
<li><a href="https://glassboxmedicine.com/2019/02/23/measuring-performance-auc-auroc/">Measuring Performance: AUC ( AUROC ) – Glass Box Medicine</a></li>
<li><a href="https://www.researchgate.net/publication/354228851_Reproducibility_standards_for_machine_learning_in_the_life_sciences">Reproducibility standards for machine learning in the life sciences</a></li>

</ul>
</details>

**Tags**: `#reproducibility`, `#machine learning`, `#peer review`, `#research practices`, `#open science`

---

<a id="item-9"></a>
## [Qwen3.8-Max open-weight model matches Kimi K3 and DeepSeek V4 Flash](https://www.reddit.com/r/LocalLLaMA/comments/1vellf2/qwen38max_matches_kimi_k3_and_deepseek_v4_flash/) ⭐️ 8.0/10

Alibaba's Qwen team announced Qwen3.8-Max, a 2.4-trillion-parameter open-weight model that matches Kimi K3 and DeepSeek V4 Flash on benchmarks and is stronger at coding and software tasks. The weights will be released next week, and a smaller open-weight Qwen3.8-27B is also confirmed. This shows that frontier-scale open-weight models can now compete directly with top models from Kimi and DeepSeek. Its strong coding performance and low API pricing could push broader adoption of open-source LLMs and intensify competition among Chinese AI labs. In benchmarks, Qwen3.8-Max performs on par with Kimi K3 and DeepSeek V4 Flash across all categories while showing better coding and software-engineering results. Its API pricing is $2.0 per million input tokens, $6.0 per million output tokens, and $0.25 per million tokens for implicit caching, with open weights coming next week.

reddit · r/LocalLLaMA · /u/davidthesong · Aug 3, 18:25

**Background**: Qwen is Alibaba's family of large language models. Kimi K3, from Moonshot AI, is the world's first open 3-trillion-parameter model with native multimodality and a 1M-token context window, while DeepSeek V4 Flash is an efficiency-optimized mixture-of-experts model with 284B total parameters and about 13B active parameters. Open-weight models are increasingly compared on coding, reasoning, and knowledge benchmarks, and per-million-token pricing is a key factor for developer adoption. Implicit caching automatically reuses previously processed prompt segments to reduce API costs.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kimi_(AI)">Kimi (AI) - Wikipedia</a></li>
<li><a href="https://openrouter.ai/deepseek/deepseek-v4-flash">DeepSeek V 4 Flash - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://www.linkedin.com/pulse/google-finally-fixing-ai-api-costs-lets-talk-implicit-r-pillai-esbse">Is Google Finally Fixing AI API Costs? Let’s Talk Implicit Caching</a></li>

</ul>
</details>

**Tags**: `#AI/ML`, `#Open Source Models`, `#Qwen`, `#LLM Benchmarks`

---

<a id="item-10"></a>
## [DeepSeek V4-Flash 284B MoE runs at 33 tok/s on used dual-Xeon and 2× RTX 3090](https://www.reddit.com/r/LocalLLaMA/comments/1veow4b/deepseek_v4flash_284b_moe_at_33_toks_single_68/) ⭐️ 8.0/10

A user published detailed benchmarks for running the full DeepSeek V4-Flash-0731 official checkpoint (284B total / 13B active MoE) on commodity used hardware: a quad-Xeon Dell R940 with 768 GB DDR4 and two RTX 3090s. The setup reached 33 tok/s single-stream decode and 53–68 tok/s aggregate with four concurrent users, and the author added prefill measurements after a commenter requested them. This shows that a 284B-parameter model can run at usable speed on roughly $6K of used hardware, without a requantized version or expensive unified-memory workstations. It also provides rare Ampere (sm_86) performance data for DeepSeek's V4-Flash engine, which is useful for budget-minded local LLM enthusiasts and small teams. The model is 156 GB with experts stored natively in MXFP4 and activations in BF16, and the 2× RTX 3090 cards are TP=2 with about 21.6 GB VRAM used per card. Each instance needs about 170 GB of system RAM pinned to one NUMA node, so roughly 512 GB of RAM (~$6K all-in) is the practical entry point; power draw is about 1,000 W under decode and 435 W idle, while the 250 W power cap on the GPUs never engages.

reddit · r/LocalLLaMA · /u/AbbreviationsSad5582 · Aug 3, 20:25

**Background**: DeepSeek V4-Flash is a preview of the DeepSeek V4 series, a mixture-of-experts (MoE) model with 284B total parameters and only 13B activated per token, supporting a 1M-token context window. In MoE models, a router selects only a subset of experts per token, so memory capacity matters more than raw bandwidth and a large CPU-side expert pool can be streamed into the GPU. LLM inference has two phases: prefill (prompt tokens processed in parallel) and decode (tokens generated one by one), and Ampere GPUs lack native FP8/FP4 compute, so the fork uses weight-only Marlin kernels instead.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash">deepseek -ai/ DeepSeek - V 4 - Flash · Hugging Face</a></li>
<li><a href="https://www.datacamp.com/blog/mixture-of-experts-moe">What Is Mixture of Experts ( MoE )? How It Works, Use... | DataCamp</a></li>
<li><a href="https://developer.nvidia.com/blog/mastering-llm-techniques-inference-optimization/">Mastering LLM Techniques: Inference Optimization | NVIDIA Technical...</a></li>

</ul>
</details>

**Discussion**: A commenter pointed out that CPU-GPU hybrid benchmark posts usually show decode speed but never prefill, calling it a 'fair hit'; the author acknowledged this, added a new prefill section, and said that number determines what the system is actually good for. The exchange appears substantive and positive, with no major disagreements.

**Tags**: `#LocalLLaMA`, `#DeepSeek`, `#hardware`, `#MoE`, `#benchmark`

---

<a id="item-11"></a>
## [Security Flaw in DNA Analyzers Puts 30 Years of Crime Evidence at Risk](https://www.wsj.com/tech/cybersecurity/security-flaw-placed-30-years-of-dna-evidence-at-risk-of-hacking-1932775a) ⭐️ 8.0/10

Researchers discovered security vulnerabilities in Thermo Fisher DNA analysis instruments used by most U.S. crime labs and, using code generated by Anthropic's Claude AI, modified DNA scan files without detection in about 45 minutes. Thermo Fisher issued a high-severity advisory on Friday and released a software update that adds digital signatures. Forensic DNA evidence has been used in criminal cases for decades, so an undetectable tampering method could undermine convictions, appeals, and ongoing investigations. The findings also highlight how AI can lower the barrier to attacking critical laboratory infrastructure, especially given inconsistent security across more than 200 U.S. labs. The vulnerable data files date back to around 1995, and the modified files did not trigger alerts in commonly used analysis software. Thermo Fisher acknowledged the issue privately in July, is coordinating with CISA, and said there are no known cases of the vulnerability being exploited in the wild.

telegram · zaihuapd · Aug 3, 05:15

**Background**: DNA profiling identifies individuals by analyzing specific genetic markers, and forensic labs typically use capillary electrophoresis instruments, such as Thermo Fisher's genetic analyzers, to produce DNA profiles from crime-scene samples. These instruments generate data files containing the raw scan results, which are then interpreted by software; if the files are not cryptographically signed or authenticated, an attacker with access to the instrument or network could alter them without detection.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DNA_profiling">DNA profiling - Wikipedia</a></li>
<li><a href="https://www.thermofisher.com/us/en/home/life-science/sequencing/sanger-sequencing/sanger-sequencing-technology-accessories.html">Applied Biosystems Genetic Analysis ... | Thermo Fisher Scientific - US</a></li>
<li><a href="https://en.wikipedia.org/wiki/Anthropic_Claude">Anthropic Claude</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#DNA forensics`, `#vulnerability`, `#critical infrastructure`, `#AI`

---

<a id="item-12"></a>
## [Cracked Nvidia CMP 170HX unlocks 80GB VRAM, 94 TFLOPS; used prices soar](https://finance.sina.com.cn/tech/roll/2026-08-03/doc-inikzqsf4659769.shtml) ⭐️ 8.0/10

Researchers at Arizona State University publicly detailed a method to bypass Nvidia's physical OTP fuse locks on the CMP 170HX mining card, expanding its VRAM from 8GB to up to 80GB and boosting FP32 performance from 0.39 to 94 TFLOPS. The exploit pushed second-hand prices from 300–500 yuan to 3000–4000 yuan, with overseas listings reaching $1,500. This matters because it converts a cheap, previously crippled mining card into a capable AI inference accelerator with A100-class GA100 silicon, enabling budget-friendly local LLM and image-generation workloads. It also highlights that Nvidia's OTP fuse-based hardware locks are not irreversible, which could affect resale economics and the wider GPU market. The attack exploits a stack overflow in the Falcon security coprocessor to achieve unauthorized DMA access, hijack privileges, and rewrite registers that control compute, memory, and PCIe limits. Community tests confirm unlocked cards work on Windows and Linux for AI workloads, but long-term stability and maximum unlocked VRAM vary by card batch.

telegram · zaihuapd · Aug 3, 11:29

**Background**: The CMP 170HX is a dedicated cryptocurrency mining card Nvidia released in 2021, built on the same GA100 die as the A100 accelerator but with heavy hardware restrictions—cut-down CUDA cores and only 8GB of HBM2e VRAM—imposed via one-time-programmable (OTP) fuses that were widely assumed to be irreversible. Because the card lacks display outputs and was designed for mining, it became cheap on the second-hand market after the mining boom faded. OTP fuses are physical one-time programmable elements that permanently store configuration settings, and bypassing them normally requires silicon- or firmware-level exploits.

<details><summary>References</summary>
<ul>
<li><a href="https://www.techpowerup.com/289310/nvidia-cmp-170hx-mining-card-tested-based-on-ga100-gpu-sku">NVIDIA CMP 170HX Mining Card Tested, Based on GA100 GPU SKU | TechPowerUp</a></li>
<li><a href="https://www.newegg.com/p/2NS-009N-00014">Refurbished: Nvidia Cmp 170Hx 8Gb Mining Card Gpu 164Mh/S - Newegg.com</a></li>
<li><a href="https://electronics.stackexchange.com/questions/455756/how-are-otp-fuses-in-ics-implemented">integrated circuit - How are OTP fuses in ICs implemented? - Electrical...</a></li>

</ul>
</details>

**Tags**: `#hardware`, `#AI/ML`, `#security exploit`, `#GPU`, `#Nvidia`

---

<a id="item-13"></a>
## [Telegram Removed from App Store Across 175 Regions](https://applecensorship.com/app-store-monitor/app/686449807) ⭐️ 8.0/10

As of the latest update, Telegram is no longer available on the Apple App Store in 175 regions, including the United States, and TestFlight downloads have also stopped working. Users who previously purchased or downloaded the app can still re-install it via the 'Previously Purchased' section. This development impacts Telegram's global user base and highlights the influence Apple's App Store policies have on the availability of major apps. It raises concerns about content moderation and the centralization of app distribution on Apple platforms. The removal spans 175 App Store regions, starting with the United States. Apple's TestFlight beta testing channel has also stopped providing the app, but the 'Previously Purchased' section still allows existing owners to download it.

telegram · zaihuapd · Aug 4, 01:10

**Background**: The Apple App Store is the sole official way to install apps on iPhone and iPad, and apps removed from it become unavailable to new users. TestFlight is Apple's service for developers to distribute beta versions of their apps to testers; its unavailability suggests the removal extends beyond the public store. The 'Previously Purchased' feature lets users re-download apps they have acquired before, even if they are no longer listed.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/TestFlight">TestFlight - Wikipedia</a></li>
<li><a href="https://developer.apple.com/testflight/">TestFlight - Apple Developer</a></li>

</ul>
</details>

**Tags**: `#Telegram`, `#App Store`, `#Apple`, `#Censorship`, `#Tech News`

---