---
layout: default
title: "Horizon Summary: 2026-08-15 (EN)"
date: 2026-08-15
lang: en
---

> From 34 items, 12 important content pieces were selected

---

1. [Qwen 3.8 27B Reveals Impressive Local Reasoning and Efficiency Trade-offs](#item-1) ⭐️ 9.0/10
2. [GLM-5.3: Frontier coding with emergent cyber capabilities](#item-2) ⭐️ 9.0/10
3. [Apple Announces CEO Transition: Tim Cook to Step Down, Ternus to Take Over](#item-3) ⭐️ 9.0/10
4. [Going Dark and the Rise of Law Enforcement Hacking](#item-4) ⭐️ 8.0/10
5. [Claude Opus 5 Faces Backlash Over Exhausting, Abstract Communication](#item-5) ⭐️ 8.0/10
6. [Firefox becomes last major browser to fully support uBlock Origin](#item-6) ⭐️ 8.0/10
7. [Compiling Doom's Renderer Into a 21B-Parameter Transformer Without Training](#item-7) ⭐️ 8.0/10
8. [AI Human-Tissue Lab Tests 3.1 Million Samples a Year, May End Animal Testing](#item-8) ⭐️ 8.0/10
9. [Xiaohongshu Open-Sources dots3-note: 280B MoE with 16B Active Params](#item-9) ⭐️ 8.0/10
10. [Judge Orders Google to Remove Third-Party App Store Installation Barriers](#item-10) ⭐️ 8.0/10
11. [PostgreSQL Patches Critical to_char Heap Buffer Overflow Allowing Code Execution](#item-11) ⭐️ 8.0/10
12. [Apple Develops China-Specific AI Model with Alibaba, Could Be First Foreign Firm Approved](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Qwen 3.8 27B Reveals Impressive Local Reasoning and Efficiency Trade-offs](https://huggingface.co/Qwen/Qwen3.8-27B-FP8) ⭐️ 9.0/10

Alibaba's Qwen team released Qwen3.8-27B-FP8, a new 27-billion-parameter local LLM, on Hugging Face. Early community tests highlight strong reasoning performance, with one user calling it the best 'pelican' (image-reasoning) model that runs on a laptop. This release strengthens the open-source local LLM ecosystem, offering a capable alternative to models from major US AI companies. It also shows that non-US players like Alibaba are closing the gap in reasoning performance, which could accelerate on-device and private AI deployments. The FP8 quantized model runs efficiently on consumer hardware: one RTX 5090 user reported ~138 tokens/second with the ninfer engine, roughly double a naive llama.cpp setup. However, a commenter noted VRAM usage appears less efficient than Gemma 4 or Muse Glimmer, and the model's unique 'caveman-style' thinking trace may hinder MTP (multi-token prediction) efficiency.

hackernews · erdaltoprak · Aug 14, 15:00 · [Discussion](https://news.ycombinator.com/item?id=49299605)

**Background**: Qwen is a family of large language and multimodal models developed by Alibaba Cloud, first released as Tongyi Qianwen in 2023. Its architecture is based on Meta's Llama design. Local LLMs like Qwen are designed to run on personal devices, enabling private, offline AI use without cloud dependency.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>
<li><a href="https://huggingface.co/Qwen">Qwen (Qwen)</a></li>

</ul>
</details>

**Discussion**: Community reactions are highly positive but mixed on efficiency. Users praised its rare ability to solve private reasoning benchmarks, noted distinct changes in thinking-trace writing compared to previous versions, and excitedly predicted that non-US models like Qwen and GLM could soon rival big US labs. Some concerns were raised about VRAM usage and MTP limitations.

**Tags**: `#Qwen`, `#Local LLM`, `#AI`, `#Reasoning`, `#Open Source`

---

<a id="item-2"></a>
## [GLM-5.3: Frontier coding with emergent cyber capabilities](https://z.ai/blog/glm-5.3) ⭐️ 9.0/10

GLM-5.3 is a frontier coding model demonstrating emergent cyber capabilities, including autonomous security research and large-scale vulnerability scanning, sparking significant community debate.

hackernews · pella · Aug 14, 05:19 · [Discussion](https://news.ycombinator.com/item?id=49294997)

**Tags**: `#AI`, `#LLM`, `#cybersecurity`, `#coding`, `#GLM`

---

<a id="item-3"></a>
## [Apple Announces CEO Transition: Tim Cook to Step Down, Ternus to Take Over](https://t.me/zaihuapd/43191) ⭐️ 9.0/10

Apple has announced a leadership transition in which Tim Cook will step down as CEO and hardware engineering chief John Ternus will become the new CEO effective September 1, 2026. Cook will move to the role of executive chairman of Apple's board, and the board has unanimously approved the arrangement. This marks the first CEO change at Apple in over a decade and a major shift in leadership at one of the world's most influential technology companies. Ternus's hardware engineering background signals a continued focus on Apple's core product lines such as iPhone, Mac, iPad, and AirPods. Ternus joined Apple in 2001, became vice president of hardware engineering in 2013, and joined the executive team in 2021. Current chairman Arthur Levinson will become lead independent director on September 1, 2026, and Ternus will join the board the same day; Cook will remain CEO through the summer to complete the transition.

telegram · zaihuapd · Aug 14, 11:00

**Background**: Apple is one of the world's largest technology companies, and its CEO is responsible for overall company strategy and operations. The executive chairman position is a board leadership role focused on governance and strategic oversight, distinct from the day-to-day management duties of the CEO. Ternus, who joined Apple in 2001, has led hardware engineering across iPhone, Mac, iPad, and AirPods since joining the executive team in 2021.

**Tags**: `#Apple`, `#CEO transition`, `#Tim Cook`, `#John Ternus`, `#Tech Industry`

---

<a id="item-4"></a>
## [Going Dark and the Rise of Law Enforcement Hacking](https://blog.cryptographyengineering.com/2026/08/14/everything-is-about-to-go-dark/) ⭐️ 8.0/10

A widely-discussed August 2026 blog post on Cryptography Engineering examines the 'going dark' problem and argues that law enforcement hacking has become the primary surveillance method as encryption blocks traditional wiretapping. The article analyzes the policy and security trade-offs of this shift. This matters because it signals a broader shift in law enforcement from passive wiretapping to offensive hacking, affecting encryption policy, privacy protections, and the legal limits of government surveillance. The debate will influence how companies design secure products and how courts treat remote searches. Key examples include Network Investigative Techniques (NITs), the FBI's warrant-authorized malware used since at least 2002 to defeat Tor anonymity, and the 2016 amendment to Rule 41 that expanded remote-access authority. The article also touches on whether the supply of software bugs is hitting a ceiling, a claim some commenters dispute.

hackernews · vslira · Aug 14, 20:52 · [Discussion](https://news.ycombinator.com/item?id=49304447)

**Background**: The 'going dark' problem refers to law enforcement's difficulty in accessing encrypted communications even with a legal warrant, a concern raised publicly by FBI Director James Comey and others in the 2010s. In response, agencies have increasingly turned to hacking techniques such as NITs, which are delivered as drive-by downloads to extract identifying information from suspects' devices. This approach raises Fourth Amendment questions about whether remote access should be treated like a physical search.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Network_Investigative_Technique">Network Investigative Technique - Wikipedia</a></li>
<li><a href="https://www.congress.gov/crs_external_products/R/PDF/R44481/R44481.7.pdf">Encryption and the “Going Dark” Debate - Congress.gov</a></li>
<li><a href="https://assets.carnegieendowment.org/static/files/Wilde_Landi_Law_Enforcement_Cyber_final_1-1.pdf">Exploring Law Enforcement Hacking as a Tool Against ...</a></li>

</ul>
</details>

**Discussion**: Commenters offered a spectrum of views: one recalled the pre-digital era when wiretaps required expensive physical phone lines, while another rejected the article's suggestion that useful software bugs are nearing a ceiling, arguing AI-assisted development is creating more bugs. A third critic found the 'going dark' label absurd given the ubiquity of security cameras and metadata collection by tech companies.

**Tags**: `#cryptography`, `#law enforcement`, `#surveillance`, `#security`, `#hacking`

---

<a id="item-5"></a>
## [Claude Opus 5 Faces Backlash Over Exhausting, Abstract Communication](https://mun-logadan.github.io/why-does-opus-5-feel-worse/) ⭐️ 8.0/10

A widely shared blog post criticizes Claude Opus 5's communication style as exhausting and overly abstract, with 705 comments and strong engagement on Hacker News. Commenters speculate that post-training now optimizes for agent-to-agent communication rather than human users, and some have switched to other models like OpenAI's Sol. This critique suggests that even as models become more capable, a shift in optimization targets—from human satisfaction to agentic performance—can degrade the actual user experience. It raises important questions about the direction of post-training for frontier LLMs and how companies like Anthropic balance capability with usability. Commenters describe Opus 5's writing as elliptical and abstract, with sentences that orbit a point, and note a tendency to 'be honest' and 'confess mistakes' at length. Some users report reverting to Claude 4.8 or moving to OpenAI's solutions, and one commenter suspects the model is smaller or more economical, suggesting 'benchmaxxing' is marketing-driven.

hackernews · numeri · Aug 14, 10:12 · [Discussion](https://news.ycombinator.com/item?id=49296740)

**Background**: Claude is Anthropic's family of large language models, with Opus historically serving as the most-capable tier alongside Sonnet and Haiku. Anthropic described Claude Opus 5 as a 'thoughtful and proactive' model that approaches the frontier intelligence of Claude Fable 5 at about half the price. In recent years the field has increasingly emphasized agentic AI, including protocols and structured reasoning for AI-to-AI communication, making human readability a potential afterthought. This context helps explain why some users now feel a disconnect between technical performance and pleasant interaction.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Opus">Claude Opus</a></li>
<li><a href="https://www.anthropic.com/news/claude-opus-5">Introducing Claude Opus 5 \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Agent_Communications_Language">Agent Communications Language</a></li>

</ul>
</details>

**Discussion**: Commenters broadly agree that Opus 5 feels more capable yet harder to converse with, citing verbose, abstract phrasing and a tendency to over-apologize. Several speculate that post-training now targets other agents rather than humans, and one user suggests the model may be more economical or smaller, with 'benchmaxxing' as mere marketing. The thread reflects a shared preference for readable, human-friendly output even as frontier models become more powerful.

**Tags**: `#AI`, `#LLM`, `#Claude Opus 5`, `#user experience`, `#agent communication`

---

<a id="item-6"></a>
## [Firefox becomes last major browser to fully support uBlock Origin](https://www.pcworld.com/article/3212428/firefox-is-now-the-last-major-browser-that-still-supports-ublock-origin.html) ⭐️ 8.0/10

Firefox is now the only major browser that fully supports the original uBlock Origin extension. This comes as Chromium-based browsers, led by Chrome, have transitioned to Manifest V3, which severely limits the capabilities of ad-blocking extensions. uBlock Origin is one of the most popular and effective ad blockers, so losing full support in Chrome weakens ad-blocking and privacy protection for millions of users. This shift also highlights the growing divergence between Google and Mozilla over user choice and content-filtering approaches. Manifest V3 replaces the blocking webRequest API with declarativeNetRequest, which restricts ad-blockers to a smaller set of static rules. Google's recommended alternative, uBlock Origin Lite, has fewer features, and an unofficial MV3 port exists but is limited because the webRequestBlocking permission is only available to enterprise sideloaded extensions.

hackernews · DemiGuru · Aug 14, 19:03 · [Discussion](https://news.ycombinator.com/item?id=49303202)

**Background**: uBlock Origin is a free, open-source, cross-platform browser extension for content filtering, primarily aimed at blocking ads and protecting privacy. Chrome first announced Manifest V3 in 2018 as a security and privacy improvement, but it also reduces the effectiveness of ad blockers. Firefox continues to support Manifest V2, allowing uBlock Origin to run with its full feature set.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/UBlock_Origin">uBlock Origin - Wikipedia</a></li>
<li><a href="https://developer.chrome.com/docs/extensions/develop/migrate/what-is-mv3">Extensions / Manifest V3 | Chrome for Developers</a></li>
<li><a href="https://arstechnica.com/gadgets/2024/08/chromes-manifest-v3-and-its-changes-for-ad-blocking-are-coming-real-soon/">Chrome’s Manifest V3, and its changes for ad blocking, are coming real soon - Ars Technica</a></li>

</ul>
</details>

**Discussion**: Commenters largely criticized Google's Manifest V3 rollout, with some noting that Firefox also curates and reviews popular extensions for security. Others highlighted an unofficial MV3 port of uBlock Origin, while a few users said they had not noticed any deficiencies with uBlock Origin Lite. Overall sentiment was a mix of concern, resignation, and practical workarounds.

**Tags**: `#browsers`, `#ad-blocking`, `#uBlock Origin`, `#Manifest V3`, `#privacy`

---

<a id="item-7"></a>
## [Compiling Doom's Renderer Into a 21B-Parameter Transformer Without Training](https://www.reddit.com/r/MachineLearning/comments/1voazhm/i_compiled_dooms_renderer_into_a_21bparameter/) ⭐️ 8.0/10

A developer compiled Doom's rendering algorithm into a 21B-parameter transformer using a custom compiler that converts computation graphs into transformer weights, with no training involved. The resulting standard Hugging Face checkpoint generates pixel-drawing commands that reproduce the game's iconic E1M1 frame. This demonstrates that computation can be embedded into transformer weights through compilation rather than training, opening new possibilities for interpretability, model editing, and neural network analysis. It also showcases a creative use of transformers for algorithmic execution beyond natural language tasks. Rendering one frame requires a 3,614-token prompt and generates 53,747 tokens, taking about 40 minutes on an NVIDIA B200 — roughly 35 frames per day, compared to the original Doom's 35 FPS on a 486-era machine. The host program to load the checkpoint and parse the output is just 43 lines of Python.

reddit · r/MachineLearning · /u/notforrob · Aug 14, 15:50

**Background**: Transformers are typically trained on massive datasets to learn patterns, but this project takes a different route: a compiler converts explicit computation graphs into transformer weights. The Doom engine uses binary space partitioning (BSP) to determine visible walls and draws the scene from near to far, a deterministic algorithm that can be represented as a graph. This work builds on earlier attempts to embed small programs or computers inside neural networks by analytically constructing weights rather than learning them.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Doom_engine">Doom engine - Wikipedia</a></li>
<li><a href="https://doom.fandom.com/wiki/Doom_rendering_engine">Doom rendering engine</a></li>
<li><a href="https://data-today.net/transformer-compiler-no-training/">A compiler that skips training and writes transformer weights</a></li>

</ul>
</details>

**Tags**: `#transformer`, `#compiler`, `#neural-networks`, `#doom`, `#computation-graph`

---

<a id="item-8"></a>
## [AI Human-Tissue Lab Tests 3.1 Million Samples a Year, May End Animal Testing](https://www.fastcompany.com/91589344/the-worlds-largest-biological-datacenter-could-help-make-animal-testing-obsolete) ⭐️ 8.0/10

Vivodyne has launched what it calls the world's largest human biological datacenter, a network of 12 robotic HIVE laboratories that can run controlled trials on 3.1 million living human tissue samples per year. The AI-driven system designs experiments to better predict how new drugs will work in humans. This could make animal testing obsolete by giving drug developers a faster, more human-relevant way to screen therapies. It addresses the long-standing problem that about 90% of clinical trials fail even after drugs pass animal tests. The annual testing capacity is estimated to be roughly twice the scale of all clinical trials in the United States combined. Vivodyne was built out of University of Pennsylvania bioengineering research, and the HIVE labs work with large human tissues rather than traditional 2D cell cultures.

telegram · zaihuapd · Aug 14, 01:48

**Background**: Pharmaceutical testing has long relied on animal models, but those results often fail to predict human responses. Advances in stem-cell and organoid technology allow scientists to grow miniature, functioning human tissues in the lab, and combining those tissues with robotic automation and AI makes it possible to run large-scale controlled experiments on human biology. Vivodyne's launch represents an early attempt to industrialize this approach as a commercial drug-testing platform.

<details><summary>References</summary>
<ul>
<li><a href="https://www.laboratorynetwork.com/doc/vivodyne-launches-the-world-largest-human-biological-datacenter-train-first-world-model-human-biology-0001">Vivodyne Launches The World's Largest Human Biological ...</a></li>
<li><a href="https://biobuzz.io/news/penn-born-vivodyne-launches-what-it-calls-the-worlds-largest-human-biological-datacenter/">Penn-Born Vivodyne Launches What It Calls the World's Largest ...</a></li>
<li><a href="https://www.intechopen.com/chapters/81045">Introductory Chapter: Organoid Technology and... | IntechOpen</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Biotech`, `#Drug Discovery`, `#Lab Automation`, `#Animal Testing`

---

<a id="item-9"></a>
## [Xiaohongshu Open-Sources dots3-note: 280B MoE with 16B Active Params](https://x.com/dotsstudioai/status/2088083314855018521) ⭐️ 8.0/10

Xiaohongshu's dots lab has open-sourced dots3-note preview, the first open-weight model in the dots3 series, with 280B total parameters and 16B active parameters. The model supports a 512K context length and handles text, images, video, and audio. This release makes a very large but efficient MoE model openly available, lowering the barrier for researchers and developers to work with frontier-scale architectures. The accompanying TEMPO reinforcement learning method and two new agent benchmarks also contribute to advancing long-horizon agent research. The model introduces TEMPO, a reinforcement learning approach that trains long-horizon agents using self-critique and test-time value estimation. Weights are available on Hugging Face, alongside the new VibeSearchBench and VibeLifeBench real-world agent benchmarks.

telegram · zaihuapd · Aug 14, 08:27

**Background**: Mixture of Experts (MoE) is a machine learning technique that divides a model into multiple specialized sub-models, or experts, and activates only a subset for each input. This allows scaling up total parameter count while keeping inference compute low, as measured by active parameters. VibeSearchBench, one of the new benchmarks, evaluates agents on long-horizon proactive search tasks with vague, multi-turn queries.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/mixture-of-experts">What is mixture of experts? | IBM</a></li>
<li><a href="https://arxiv.org/abs/2605.27882">[2605.27882] VibeSearchBench: Benchmarking Long-horizon ...</a></li>

</ul>
</details>

**Tags**: `#MoE`, `#Open Source`, `#AI Model`, `#Reinforcement Learning`, `#Benchmark`

---

<a id="item-10"></a>
## [Judge Orders Google to Remove Third-Party App Store Installation Barriers](https://www.androidauthority.com/google-play-store-remove-third-party-app-store-friction-3698697/) ⭐️ 8.0/10

U.S. District Judge James Donato ordered Google to simplify the installation process for rival Android app stores, removing extra steps and warning pop-ups from the Play Store. The court found that the multi-step prompts, such as showing a 'view' button before 'install', were intentionally designed as anticompetitive friction. This ruling forces Google to alter its Play Store policies, potentially opening Android app distribution to greater competition from third-party stores. It directly affects how users install alternative app markets and could reshape the developer ecosystem's access to Android devices. Google must comply within one week, making the installation of third-party stores as direct as installing a regular Android app. The order stems from the Epic v. Google antitrust verdict, where a jury found Google held an illegal monopoly in Android app distribution.

telegram · zaihuapd · Aug 14, 09:55

**Background**: The Play Store is Android's default app marketplace, and Google has historically shown warning pop-ups and multi-step processes when users sideload apps from outside it. This friction has long been a point of contention, and in 2023 a jury concluded that Google's control over Android app distribution was an illegal monopoly in the Epic v. Google case. Separately, Google has been introducing new sideloading verification rules, such as a mandatory 24-hour lock for apps from unverified developers, which continue to affect third-party app installation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.androidauthority.com/how-android-sideloading-restrictions-may-work-3595355/">Google's plan to restrict sideloading on Android has a ...</a></li>
<li><a href="https://www.androidauthority.com/google-android-sideloading-unverified-apps-new-rules-3650343/">Android's new sideloading rules are here, and they come with ...</a></li>
<li><a href="https://www.digitaltrends.com/phones/google-will-still-let-you-sideload-apps-but-theres-a-catch-now/">Google will still let you sideload apps, but there's a catch ...</a></li>

</ul>
</details>

**Tags**: `#antitrust`, `#Google`, `#Android`, `#Play Store`, `#app distribution`

---

<a id="item-11"></a>
## [PostgreSQL Patches Critical to_char Heap Buffer Overflow Allowing Code Execution](https://www.postgresql.org/support/security/CVE-2026-14669/) ⭐️ 8.0/10

PostgreSQL disclosed CVE-2026-14669, a high-severity heap buffer overflow in the to_char(timestamptz) function caused by overly long POSIX time zone abbreviations. Fixes are available in minor releases 18.6, 17.11, 16.15, 15.19, and 14.24; 18.x users should upgrade directly to 18.6 because 18.5 was not released due to a regression. This vulnerability can let a low-privileged database user execute arbitrary code with the operating system privileges of the PostgreSQL server process, posing a serious risk to affected installations. With a CVSS score of 8.8, administrators should prioritize upgrading their minor releases to prevent potential server compromise. The flaw is triggered when to_char(timestamptz) processes a very long POSIX time zone abbreviation; exploitation requires an attacker to have a low-privileged database account and the ability to set a time zone, so it is not unauthenticated. The minor releases do not require a dump or pg_upgrade; users only need to replace program files and restart the service.

telegram · zaihuapd · Aug 14, 14:35

**Background**: PostgreSQL's to_char function converts timestamps, intervals, numbers, and other values into formatted strings, and timestamptz stores a date and time together with a UTC offset. POSIX time zone strings can include abbreviations and offsets, and an excessively long abbreviation can overflow a fixed-size buffer in the server's C code. Heap buffer overflows are memory-safety bugs that can often be exploited to execute arbitrary code, which is why the project treats this issue as high severity. Users should apply the latest minor release for their major version to fix the flaw.

<details><summary>References</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/functions-formatting.html">PostgreSQL: Documentation: 18: 9.8. Data Type Formatting Functions</a></li>
<li><a href="https://www.postgresql.org/docs/current/datatype-datetime.html">PostgreSQL: Documentation: 18: 8.5. Date/Time Types</a></li>

</ul>
</details>

**Tags**: `#PostgreSQL`, `#CVE`, `#Security`, `#Vulnerability`, `#to_char`

---

<a id="item-12"></a>
## [Apple Develops China-Specific AI Model with Alibaba, Could Be First Foreign Firm Approved](https://www.reuters.com/business/retail-consumer/apple-trains-its-own-ai-model-china-market-with-alibabas-support-sources-say-2026-08-14/) ⭐️ 8.0/10

Apple is training a dedicated large language model for the Chinese market with support from Alibaba, shifting from its previous reliance on third-party models. Apple Intelligence is expected to launch in China in the coming months via an iOS update, and the Cyberspace Administration of China has already filed the company's generative AI service. If approved, Apple would become the first foreign company allowed to offer its own AI model in China, a milestone with major implications for AI regulation and the competitive landscape. It also gives Apple greater control over the AI experience on its devices in one of its most important markets. Apple's proprietary model is being trained specifically for China, with Alibaba providing support, according to people familiar with the matter. The Chinese cybersecurity regulator has already filed or registered Apple's generative AI service, a key step under China's Interim Measures for the Management of Generative AI Services, which took effect in August 2023.

telegram · zaihuapd · Aug 14, 14:47

**Background**: Apple Intelligence is Apple's personal intelligent system integrated into iOS 18, iPadOS 18, and macOS Sequoia, combining on-device and server-side processing. In China, all generative AI services must be filed or registered with the Cyberspace Administration of China before offering services to the public, which is why Apple needs to comply with local regulations.

<details><summary>References</summary>
<ul>
<li><a href="https://zh.wikipedia.org/wiki/Apple_Intelligence">Apple Intelligence - 维基百科，自由的百科全书</a></li>
<li><a href="https://www.gov.cn/zhengce/zhengceku/202307/content_6891752.htm">生成式人工智能服务管理暂行办法_国务院部门文件_中国政府网</a></li>
<li><a href="https://www.cac.gov.cn/2024-04/02/c_1713729983803145.htm">国家互联网信息办公室关于发布生成式人工智能服务已备案信息的公告_中...</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#AI`, `#China`, `#Alibaba`, `#Large Language Model`

---