---
layout: default
title: "Horizon Summary: 2026-08-30 (EN)"
date: 2026-08-30
lang: en
---

> From 24 items, 7 important content pieces were selected

---

1. [Tencent Open-Sources Hy4 Preview with Recursive Self-Improvement](#item-1) ⭐️ 8.0/10
2. [DHS uses obscure '1509 summons' to secretly get journalists' records](#item-2) ⭐️ 8.0/10
3. [Samsung Showcases Processing-in-Memory at Hot Chips to Slash AI Data Movement](#item-3) ⭐️ 8.0/10
4. [Simple 100-year-old SPC beats SOTA time series anomaly detection on TSB-AD](#item-4) ⭐️ 8.0/10
5. [LLM benchmark scores vary 3x more between days than within a day](#item-5) ⭐️ 8.0/10
6. [OpenAI cuts off Cursor after SpaceX acquisition, sets Nov 2026 shutdown](#item-6) ⭐️ 8.0/10
7. [Music Publishers Sue Anthropic Over Pirated Lyrics and Books in Claude Training](#item-7) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Tencent Open-Sources Hy4 Preview with Recursive Self-Improvement](https://www.tencent.com/tencent-releases-and-open-sources-tencent-hy4-preview/) ⭐️ 8.0/10

Tencent released and open-sourced Hy4 preview, a next-generation large language model with 770B total parameters, 49B active parameters, and a context window exceeding 1 million tokens. The model also contributed to its own development, participating in the automated optimization of training methods, data strategies, evaluation frameworks, and low-level operators, establishing an early-stage recursive self-improvement loop. This release marks a major open-source milestone from Tencent and demonstrates a concrete instance of recursive self-improvement, a capability that could dramatically accelerate AI development. With trillions of tokens processed on OpenRouter within days, Hy4 preview shows exceptionally strong early adoption, and its competitive pricing may pressure other providers. Hy4 preview is a Mixture-of-Experts model with a 1,024,000-token context window and 64,000-token output, priced at $0.83 per million input tokens and $2.50 per million output tokens across seven providers. Notably, the model's cache cost is only 5%, significantly cheaper than the typical 10–20% cache costs, which may help explain its rapid adoption.

hackernews · shenli3514 · Aug 29, 19:33 · [Discussion](https://news.ycombinator.com/item?id=49492632)

**Background**: Hy4 preview is Tencent's latest open-source large language model. Recursive self-improvement refers to an AI system that can improve its own capabilities — for example, by writing code, generating training data, or optimizing hardware — potentially leading to rapid, compounding progress. Tencent's announcement is notable because Hy4 preview applied this concept in a concrete early loop, proposing approaches, running experiments, and using the resulting logs and feedback in subsequent development rounds.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tencent.com/tencent-releases-and-open-sources-tencent-hy4-preview/">Tencent Releases and Open-Sources Tencent Hy 4 preview - Tencent</a></li>
<li><a href="https://models.dev/models/tencent/hy4-preview/">Hy 4 preview pricing, providers, and specs | Models .dev</a></li>
<li><a href="https://en.wikipedia.org/wiki/Recursive_self-improvement">Recursive self-improvement - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters had mixed reactions: minimaxir noted the model's 'ludicrous traction' on OpenRouter with trillions of tokens processed in days, while codethief connected the recursive self-improvement loop to broader predictions about AI progress. Jamie raised a genuine question about whether increased token density risks losing linguistic richness, and fastball criticized the benchmark charts used in Tencent's release materials.

**Tags**: `#AI`, `#Machine Learning`, `#LLM`, `#Tencent`, `#Open Source`

---

<a id="item-2"></a>
## [DHS uses obscure '1509 summons' to secretly get journalists' records](https://www.theguardian.com/us-news/2026/aug/29/trump-dhs-1509-summons-records-journalists-nonprofits) ⭐️ 8.0/10

The Guardian reported that the Department of Homeland Security (DHS) has been using obscure administrative subpoenas known as '1509 summonses' to secretly obtain phone records and other data from journalists, nonprofits, and unions. The DHS withdrew some summonses after court challenges but before a judge could rule on their legality. This raises serious civil-liberties and press-freedom concerns, because the power lets the government obtain records without a warrant or judicial oversight. The pattern of withdrawing summonses before judicial review may be a deliberate strategy to avoid a binding ruling on the law's constitutionality. The article reports that DHS obtained six months of phone records for a journalist from T-Mobile, including more than 10,000 calls and text messages, without notifying her until later; in contrast, Google reportedly did not comply. Since DHS must go to court to enforce a 1509 summons if it is ignored, companies that voluntarily comply bear substantial responsibility for the surveillance.

hackernews · firefax · Aug 29, 18:44 · [Discussion](https://news.ycombinator.com/item?id=49492219)

**Background**: A 1509 summons is an administrative subpoena that allows DHS agencies such as Customs and Border Protection and Immigration and Customs Enforcement to compel the production of records without a court order or grand jury subpoena. It has historically been associated with immigration enforcement, but civil-liberties groups say DHS has used it to target journalists and advocacy groups, often without notifying the subject. Concerns about the practice date back to at least 2018, when the DHS Office of Inspector General issued a management alert about its use by CBP.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theguardian.com/us-news/2026/aug/29/trump-dhs-1509-summons-records-journalists-nonprofits">Trump’s DHS is using an obscure law to secretly snoop... | The Guardian</a></li>
<li><a href="https://www.rcfp.org/doj-dhs-news-guidelines-alt-uscis/">DHS should follow DOJ's lead and adopt rules to protect journalists</a></li>
<li><a href="https://www.muckrock.com/foi/united-states-of-america-10/dhs-oig-1509-summonses-management-alert-materials-53593/">DHS OIG - 1509 summonses management alert materials • MuckRock</a></li>

</ul>
</details>

**Discussion**: Commenters largely condemned the surveillance, with several noting that DHS withdraws summonses precisely to avoid a judicial ruling and that companies which voluntarily comply are the real enablers. The T-Mobile vs. Google contrast was highlighted as an example of inconsistent corporate resistance. Some commenters also used the thread to share alternative infrastructure solutions for journalists, such as self-hosted email, while others cast the story as evidence of a broader authoritarian drift.

**Tags**: `#privacy`, `#surveillance`, `#law`, `#journalism`, `#civil-liberties`

---

<a id="item-3"></a>
## [Samsung Showcases Processing-in-Memory at Hot Chips to Slash AI Data Movement](https://chipsandcheese.com/p/hot-chips-2026-samsungs-processing) ⭐️ 8.0/10

At Hot Chips 2026, Samsung presented its Processing-in-Memory (PIM) technology, which places compute logic directly inside memory arrays to reduce data movement for AI workloads. The presentation highlighted PIM as a way to overcome the memory wall in modern accelerators. PIM directly targets the data-movement bottleneck between memory and compute, which dominates energy and performance costs in AI inference and training. If viable, it could reshape AI hardware designs and benefit memory-bound applications across the industry. In PIM, computation is integrated into the memory array itself, avoiding the von Neumann bottleneck of shuttling data back and forth. However, matrix multiplication still requires input and output elements to meet at the right multiplier, so significant data movement remains an open challenge.

hackernews · ingve · Aug 29, 06:06 · [Discussion](https://news.ycombinator.com/item?id=49487341)

**Background**: Conventional computers separate memory and processing, and moving data between them is slow and power-hungry — a problem known as the memory wall. Processing-in-Memory (PIM) is an emerging architectural paradigm that places computation near or inside memory to address this bottleneck. Samsung's presentation is part of a broader trend exploring non-von-Neumann designs for AI.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/processing-in-memory-pim-architectures-next-frontier-epbof">Processing - in - Memory ( PIM ) Architectures: The Next Frontier in...</a></li>
<li><a href="https://medium.com/@smkutukte58/processing-in-memory-revolutionizing-data-handling-45ed9c602d3c">Processing - in - Memory : Revolutionizing Data Handling | Medium</a></li>
<li><a href="https://safari.ethz.ch/projects_and_seminars/spring2022/doku.php?id=processing_in_memory">processing _ in _ memory [SAFARI Project & Seminars Courses...]</a></li>

</ul>
</details>

**Discussion**: Commenters noted historical precedents, including HPE Labs' similar work a decade ago and mention of commingling memory and processing in the 1980s Mead & Conway VLSI text. Sentiment was mixed: some called it a cool idea but pointed out that many exotic accelerator proposals at trade shows go nowhere, while others questioned the implementation, arguing that matrix multiplication still requires substantial data movement.

**Tags**: `#PIM`, `#AI hardware`, `#memory`, `#Samsung`, `#Hot Chips`

---

<a id="item-4"></a>
## [Simple 100-year-old SPC beats SOTA time series anomaly detection on TSB-AD](https://www.reddit.com/r/MachineLearning/comments/1w1wt1s/you_can_beat_sota_time_series_anomaly_detection/) ⭐️ 8.0/10

Eamonn Keogh demonstrated that a simple 100-year-old Statistical Process Control (SPC) method outperforms state-of-the-art time series anomaly detection methods on the TSB-AD-M benchmark. He argues that the benchmark is too trivial for meaningful comparisons and calls for community introspection. This challenges the validity of recent progress in time series anomaly detection, a prominent research area at NeurIPS, SIGKDD, and VLDB. If a century-old method can beat SOTA, the community may need to reconsider benchmark design and the credibility of many published claims. Keogh notes that TSB-AD contains many trivial traces, such as the 'TAO' examples and ECG traces, which SPC can solve perfectly. He also points to his own work on harder problems like sled dogs, Tuna, fuel cells, and smart manufacturing as a path forward for more challenging benchmarks.

reddit · r/MachineLearning · /u/eamonnkeogh · Aug 29, 20:16

**Background**: Time series anomaly detection aims to identify unusual patterns in temporal data, with applications in manufacturing, finance, and healthcare. TSB-AD is a widely used benchmark for evaluating such methods, ranking detectors by metrics like VUS-PR. Statistical process control is a quality-control technique using control charts to monitor process variation, originally developed for manufacturing and dating back to the 1920s.

<details><summary>References</summary>
<ul>
<li><a href="https://thedatumorg.github.io/TSB-AD/">TSB - AD</a></li>
<li><a href="https://github.com/TheDatumOrg/TSB-AD">GitHub - thedatumorg/ TSB - AD : Time-Series Anomaly Detection</a></li>
<li><a href="https://en.wikipedia.org/wiki/Statistical_process_control">Statistical process control</a></li>

</ul>
</details>

**Tags**: `#time series`, `#anomaly detection`, `#benchmarking`, `#research critique`, `#machine learning`

---

<a id="item-5"></a>
## [LLM benchmark scores vary 3x more between days than within a day](https://www.reddit.com/r/MachineLearning/comments/1w1jp1j/i_analyzed_31352_hourly_llm_benchmark_scores/) ⭐️ 8.0/10

An analysis of 31,352 hourly LLM benchmark scores found that between-day variation (8.4 points) is approximately three times larger than within-day variation (2.8 points). The author built a continuous evaluation pipeline and open-sourced it as AIStupidLevel, which also powers an OpenAI-compatible router. This matters because single-point LLM benchmarks can be misleading; production teams need to track model drift over time, not just one snapshot. The finding that between-day variation dominates suggests that daily evaluation windows provide a more reliable signal for detecting real performance degradation, which is crucial for model selection and monitoring. The evaluation pipeline executes coding tasks (not just model-based judging), tests tool-calling inside isolated Docker environments, and aggregates five repeated runs to reduce stochastic noise. Detection uses daily medians and sequential change-point detection, and it flagged a 32% sustained decline in Gemini 3.1 Flash Lite at the time of the screenshot.

reddit · r/MachineLearning · /u/ionutvi · Aug 29, 11:08

**Background**: Most LLM benchmarks measure models once, but LLMs are stochastic and their outputs vary even with the same inputs. Research has shown that benchmark scores carry uncertainty due to temperature, prompt phrasing, and repeated sampling. Canary tasks are small, self-contained tasks used for ongoing monitoring, and AIStupidLevel uses such tasks to continuously score models across coding, reasoning, tool use, reliability, latency, and cost.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2410.03492">[2410.03492] Towards Reproducible LLM Evaluation: Quantifying ... Towards Reproducible LLM Evaluation: Quantifying Uncertainty ... (PDF) Towards Reproducible LLM Evaluation: Quantifying ... LLM Benchmark Variance 2026: Why Your Benchmark Scores Are ... [PDF] Towards Reproducible LLM Evaluation: Quantifying ... (PDF) ReliableEval: A Recipe for Stochastic LLM Evaluation ... Breaking Down the Metrics: A Comparative Analysis of LLM ...</a></li>
<li><a href="https://dev.to/hackcpp_3619/free-coding-models-are-good-enough-for-some-of-your-tasks-heres-how-to-find-which-ones-ga">Free Coding Models Are Good Enough for Some of Your Tasks ...</a></li>
<li><a href="https://studioplatforms.eu/products/aistupidlevel">AI Training Data & Benchmarking Platform | AIStupidLevel .info</a></li>

</ul>
</details>

**Tags**: `#LLM evaluation`, `#benchmarking`, `#model drift`, `#continuous testing`, `#performance stability`

---

<a id="item-6"></a>
## [OpenAI cuts off Cursor after SpaceX acquisition, sets Nov 2026 shutdown](https://t.me/zaihuapd/43477) ⭐️ 8.0/10

OpenAI announced it will terminate its contract that provides OpenAI models through Cursor, recommending a service cutoff date of November 12, 2026. The decision follows SpaceX's acquisition of Cursor and cites concerns that SpaceX will not comply with service terms. This move affects the developer tools ecosystem, as Cursor is a widely used AI coding assistant and its users could lose access to OpenAI models. It also underscores growing friction between OpenAI and Elon Musk, whose xAI is a direct competitor and whose SpaceX now owns Cursor. OpenAI said it is giving the maximum notice period permitted by the contract. The company stated it cannot be confident SpaceX will adhere to the terms, citing Musk's companies' history of contract violations, including Twitter's post-acquisition breaches and xAI's admission earlier this year of violating OpenAI's service terms.

telegram · zaihuapd · Aug 29, 04:53

**Background**: Cursor is an AI-first code editor built on Visual Studio Code, designed to help developers write, debug, and understand code via natural-language instructions. Elon Musk co-founded OpenAI in 2015 but later left; he established xAI, which became a subsidiary of SpaceX in 2026. The acquisition of Cursor by SpaceX puts an OpenAI-powered tool under the control of a major OpenAI rival.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cursor_(code_editor)">Cursor (code editor)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Elon_Musk">Elon Musk - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#Cursor`, `#SpaceX`, `#AI tools`, `#Developer ecosystem`

---

<a id="item-7"></a>
## [Music Publishers Sue Anthropic Over Pirated Lyrics and Books in Claude Training](https://www.musicbusinessworldwide.com/files/2026/08/COMPLAINT-in-Sony_Music_Publishing_US_LLC_e.pdf) ⭐️ 8.0/10

Sony Music Publishing, Warner Chappell, and other publishers filed a lawsuit in California federal court against Anthropic and its founders, alleging the company illegally downloaded over 7 million books from pirate libraries such as LibGen and PiLiMi and scraped song lyrics without permission to train its Claude AI models. The plaintiffs are seeking up to $150,000 in damages per work and a permanent injunction against the use of their copyrighted material. This lawsuit is a major legal test for the AI industry, as it challenges the use of copyrighted training data by a leading AI company. A ruling against Anthropic could set a precedent with multi-billion dollar implications, reshaping how AI models are trained and forcing companies to secure proper licensing for training datasets. The complaint specifically alleges that Anthropic removed copyright management information (CMI) from downloaded lyrics, violating the Digital Millennium Copyright Act (DMCA). According to the lawsuit, this follows previous similar litigation in the music industry that has already resulted in $1.5 billion in settlements.

telegram · zaihuapd · Aug 30, 01:00

**Background**: LibGen, or Library Genesis, is a shadow library project that provides free access to pirated academic journals, books, and other works, and has long been accused of internet piracy by publishers. PiLiMi, short for Pirate Library Mirror, is a digitized library of pirated books that Anthropic reportedly used in its early AI training dataset and that courts have deemed infringing. Copyright management information (CMI) is identifying data attached to a work, such as the title, author, and copyright owner; the DMCA prohibits its removal or alteration to conceal infringement.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LibGen">LibGen</a></li>
<li><a href="https://en.wikipedia.org/wiki/PiLiMi">PiLiMi</a></li>
<li><a href="https://www.6pages.com/glossary/piratelibrarymirror(pilimi)/">Pirate Library Mirror (PiLiMi) | 6Pages</a></li>

</ul>
</details>

**Tags**: `#AI`, `#copyright`, `#lawsuit`, `#Anthropic`, `#training data`

---