---
layout: default
title: "Horizon Summary: 2026-09-04 (EN)"
date: 2026-09-04
lang: en
---

> From 33 items, 6 important content pieces were selected

---

1. [OpenAI Launches GPT-6 Astra with Near-Perfect ARC-AGI-3 Score](#item-1) ⭐️ 10.0/10
2. [Verisign Proposes Ending Existing .name Third-Level Registrations](#item-2) ⭐️ 8.0/10
3. [Developer Ports 1993 Amiga Game to Godot Using LLM to Read 68000 Assembly](#item-3) ⭐️ 8.0/10
4. [Audacity 4.0 Launches Qt6-Based UI, Sparks Community Debate](#item-4) ⭐️ 8.0/10
5. [GPT-6 Astra Shows Notable Yet Limited Results on ARC-AGI-3 and Erdős Problems](#item-5) ⭐️ 8.0/10
6. [Microsoft to Enable Memory Integrity by Default on Windows 11 in October 2026](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI Launches GPT-6 Astra with Near-Perfect ARC-AGI-3 Score](https://openai.com/index/gpt-6-astra/) ⭐️ 10.0/10

OpenAI has announced GPT-6 Astra, a new flagship AI model, claiming a 99.9% score on the ARC-AGI-3 benchmark and strong gains on the Artificial Analysis Coding Agent Index. The announcement includes a system card and has quickly drawn an extensive Hacker News discussion. This is a major landmark in frontier-model releases, with implications for AI agents, coding assistants, and benchmark standards. The intense community debate also shows that how OpenAI reports benchmark scores is becoming as important as the model itself. OpenAI linked to a deployment-safety system card at deploymentsafety.openai.com/gpt-6-astra. Community commenters noted that the ARC-AGI-3 scorecard appears to use different harness conditions for GPT-5.6 Sol (showing 7.8% while estimating roughly 30% with the responses API harness), and saw relatively modest gains on most other benchmarks.

hackernews · kibae · Sep 3, 18:41 · [Discussion](https://news.ycombinator.com/item?id=49554643)

**Background**: ARC-AGI is a benchmark introduced by François Chollet in 2019 to measure fluid intelligence through visual grid puzzles that resist memorization, and near-perfect scores are considered a major milestone. A system card is a transparency document that OpenAI and Anthropic publish to describe model capabilities, safety evaluations, and limitations. Artificial Analysis is an independent benchmarking platform whose Coding Agent Index and Intelligence Index evaluate models on real software-engineering and knowledge tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi">ARC Prize - What is ARC-AGI?</a></li>
<li><a href="https://airiskaware.com/what-is/system-card">What Is System Card ? | AI Governance Glossary | AIRiskAware</a></li>
<li><a href="https://artificialanalysis.ai/">AI Model & API Providers Analysis | Artificial Analysis</a></li>

</ul>
</details>

**Discussion**: The Hacker News thread mixes curation and skepticism: one moderator asked users to keep rollout discussion separate, while technical commenters questioned the ARC-AGI-3 methodology and argued that most other benchmarks improved only modestly. Others criticized demos where models autonomously buy items, and some suggested that frontier progress still looks like skill acquisition rather than general intelligence.

**Tags**: `#GPT-6`, `#OpenAI`, `#AI`, `#LLM`, `#Benchmark`

---

<a id="item-2"></a>
## [Verisign Proposes Ending Existing .name Third-Level Registrations](https://neil.fraser.name/news/2026/09/03/) ⭐️ 8.0/10

Verisign has proposed terminating existing third-level registrations under the .name top-level domain rather than merely halting new ones. The plan would also release the underlying second-level domains, affecting addresses of the form x.y.name. If adopted, the proposal would cancel registrations that individuals and organizations may have held for years, which critics say contradicts ICANN's mission to ensure stable and secure operation of the Internet's unique identifier systems. Releasing the second-level domains could also enable domain squatting when short, desirable names go on sale. The policy targets only third-level .name registrations, so second-level domains directly owned by registrants, such as dvt.name, are not affected. It is unclear from the proposal whether Verisign will reserve the corresponding second-level domains for a period after the third-level registrations end, leaving a potential squatting window.

hackernews · pavel_lishin · Sep 3, 14:54 · [Discussion](https://news.ycombinator.com/item?id=49550772)

**Background**: The news concerns the .name top-level domain, a gTLD intended for individuals. In a domain like x.y.name, .name is the first level, y is the second level, and x is the third level, often called a subdomain. The proposal would retire the special class of registered third-level domains and release the corresponding second-level names for general availability. Domain squatting is the bad-faith practice of registering names identical or similar to trademarks, businesses, or individuals in order to profit from them.

<details><summary>References</summary>
<ul>
<li><a href="https://www.artera.net/en/hosting/domain-difference-between-first-second-and-third-level/">Domain: Difference between First, Second and Third Level - Artera</a></li>
<li><a href="https://www.dynadot.com/help/question/what-is-third-level-domain">What is a third-level domain? | Dynadot</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cybersquatting">Cybersquatting - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Many commenters say Verisign should stop accepting new third-level registrations while honoring existing ones and reserving affected second-level domains to prevent squatting. Some argue the move directly contradicts ICANN's stability-focused mission. Others clarify that .name itself is not ending and that only third-level registrations are at risk, while a few note that domain names are leased assets and can disappear when the registry changes course.

**Tags**: `#domain names`, `#ICANN`, `#internet governance`, `#policy`, `#.name TLD`

---

<a id="item-3"></a>
## [Developer Ports 1993 Amiga Game to Godot Using LLM to Read 68000 Assembly](https://babyloniantwins.com/blog/porting-a-1993-amiga-game-to-godot/) ⭐️ 8.0/10

The author documents how they ported their 1993 Amiga game, originally written in MC68000 assembly in Baghdad, to the Godot engine over an evening, using an LLM to read and translate the original assembly code. They also released the original game for free. This is a compelling demonstration of using LLMs for retro-game preservation and porting, potentially lowering the barrier for bringing decades-old assembly code to modern engines. It also validates that AI can assist with highly specialized, low-level code understanding rather than only high-level languages. The LLM first assembled the code using vasm on a Mac, iterating until the binary matched the original game's files byte-for-byte. Because the original files were snapshots of memory saved by the AsmOne assembler after the game had been running, there was a persistent 108-byte mismatch that the author never fully verified.

hackernews · rabahs · Sep 3, 14:28 · [Discussion](https://news.ycombinator.com/item?id=49550375)

**Background**: MC68000 assembly is the native instruction set of the Motorola 68000 processor used in the Amiga and other late-1980s/early-1990s computers; games were often written in assembly to maximize performance. On the Amiga, AsmOne was a popular assembler/IDE that assembled code directly into memory, and developers sometimes saved a memory snapshot as the binary for distribution. vasm is a portable, retargetable assembler often used today to recreate such binaries from original assembly source. Godot is a modern open-source game engine, and the author used an LLM to translate the 68000 assembly into engine-readable logic.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Amiga_programming_languages">Amiga programming languages - Wikipedia</a></li>
<li><a href="http://sun.hasenbraten.de/vasm/">vasm portable and retargetable assembler</a></li>

</ul>
</details>

**Discussion**: Commenters were enthusiastic and shared similar experiments: one person used Claude to convert a ZX81 memory dump to Go, another has built reusable console porting frameworks and extracted a 68k decoder for other systems. Others expressed nostalgia for the Amiga era, praised the original 1993 assembly work, and asked about debugging stories.

**Tags**: `#LLM`, `#Godot`, `#Assembly`, `#RetroGaming`, `#Porting`

---

<a id="item-4"></a>
## [Audacity 4.0 Launches Qt6-Based UI, Sparks Community Debate](https://github.com/audacity/audacity/releases/tag/Audacity-4.0.0) ⭐️ 8.0/10

Audacity 4.0 (tagged Audacity-4.0.0) has been released on GitHub, introducing a new Qt6-based user interface and broad improvements. The release has generated substantial discussion on Hacker News. As a major version of one of the most widely used open-source audio editors, this Qt6-based overhaul signals a significant modernization effort. The mixed community reception could shape future development priorities and affect both casual and advanced users across Windows, macOS, and Linux. The release tag is Audacity-4.0.0 on GitHub, and the new UI is based on the Qt6 cross-platform application framework. Comments indicate that while some users praised the cleaner interface, others point out that long-standing technical issues with JACK/PipeWire audio integration remain unaddressed.

hackernews · ClydeN · Sep 3, 10:53 · [Discussion](https://news.ycombinator.com/item?id=49548395)

**Background**: Audacity is a free, open-source audio editor widely used for recording and editing sound. Qt6 is a major version of the Qt framework, which provides cross-platform graphical user interface tools and supports C++17 and a modern graphics architecture. Moving Audacity's UI to Qt6 is central to this release's interface improvements and long-term maintainability.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Qt_(software)">Qt (software) - Wikipedia</a></li>
<li><a href="https://extenly.com/2024/12/20/from-qtwidgets-to-qt6-and-beyond-what-is-qt-capable-of/">From QtWidgets to Qt6 and Beyond: What Is Qt Capable Of? – Extenly</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters are divided: some praise the overhaul and recommend developer videos, while others express frustration that technical concerns such as intermittent JACK client behavior were not fixed. There are also reminders of past telemetry controversies, worries about 'audio.com' integration, and questions about what happened to fork projects like Tenacity.

**Tags**: `#Audacity`, `#open-source`, `#audio-editing`, `#release`, `#Qt6`

---

<a id="item-5"></a>
## [GPT-6 Astra Shows Notable Yet Limited Results on ARC-AGI-3 and Erdős Problems](https://arcprize.org/blog/astra) ⭐️ 8.0/10

A new ARC Prize blog post reports that OpenAI's latest model, GPT-6 Astra, has been evaluated on ARC-AGI-3 and Erdős problems, showing notable yet limited reasoning performance. On Epoch AI's FrontierMath Erdős benchmark, the model solved 5 of 68 problems across all attempts, with two direct successes: a counterexample disproving problem 74 and a proof of problem 126. This result matters because it empirically tests whether frontier AI scaling translates into genuine progress on hard, open-ended reasoning benchmarks. The high per-problem compute cost also fuels an ongoing debate about the economic viability of using such models for research-grade mathematics and problem-solving. ARC-AGI-3 is an interactive benchmark that requires AI agents to explore novel abstract environments, infer goals on the fly, and build internal models of environment dynamics, rather than simply pattern-match on static grids. In the Erdős tests, the two successful solves took roughly 15–16 hours and cost $218–$247 each; by comparison, human participants in controlled tests were paid about $12.78 per attempted game before bonuses.

hackernews · vignesh_warar · Sep 3, 19:45 · [Discussion](https://news.ycombinator.com/item?id=49555691)

**Background**: ARC-AGI-3 is the first interactive reasoning benchmark designed to measure human-like intelligence in AI agents by presenting them with novel, turn-based environments where they must explore, identify goals, and plan effective actions. The Erdős problems are a collection of open mathematical conjectures proposed by the prolific Hungarian mathematician Paul Erdős; Epoch AI's FrontierMath Erdős set adapts them as a hard benchmark for AI mathematical reasoning. GPT-6 Astra is OpenAI's most capable model, built for complex reasoning, coding, and research, and it supports multiple reasoning-effort levels and a 1,050,000-token context window.

<details><summary>References</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>
<li><a href="https://developers.openai.com/api/docs/models/gpt-6-astra">GPT-6 Astra Model | OpenAI API</a></li>
<li><a href="https://en.wikipedia.org/wiki/Erdős_problems">Erdős problems</a></li>

</ul>
</details>

**Discussion**: Commenters generally liked the Erdős benchmark but described GPT-6 Astra's progress as "tepid" now that the easy problems have been solved, with only two direct solves in 68 problems. Several debated whether such puzzle-solving truly defines intelligence and whether the roughly $360-per-puzzle cost will fall below minimum wage within two years, while another commenter questioned whether OpenAI had prior access to the ARC-AGI-3 tests and built a custom harness for them.

**Tags**: `#OpenAI`, `#GPT-6`, `#ARC-AGI`, `#AI benchmarks`, `#reasoning`

---

<a id="item-6"></a>
## [Microsoft to Enable Memory Integrity by Default on Windows 11 in October 2026](https://techcommunity.microsoft.com/blog/windows-itpro-blog/expanding-memory-integrity-protection-across-windows-devices/4551984) ⭐️ 8.0/10

Microsoft announced it will automatically enable memory integrity (HVCI) on eligible Windows 11 devices starting with the October 13, 2026 Patch Tuesday release. The change is designed to block malicious or vulnerable drivers from hijacking the operating system via kernel-mode vulnerabilities. Making memory integrity a default setting significantly raises the security baseline of Windows 11 against driver-based attacks, which are a common avenue for privilege escalation and ransomware. Enterprises and individuals with older or incompatible drivers will need to update their hardware or software to avoid blocked updates or blue-screen issues. Eligible devices must support hardware virtualization, UEFI, and Secure Boot; systems without these capabilities will not have the protection enabled. Incompatible legacy drivers can prevent memory integrity from turning on and, in rare cases, cause blue-screen errors, so Microsoft is limiting the rollout to devices whose drivers have been validated for compatibility.

telegram · zaihuapd · Sep 3, 06:09

**Background**: Memory integrity, also known as hypervisor-protected code integrity (HVCI), uses Virtualization-Based Security (VBS) to isolate kernel-mode code integrity checks in a secure hypervisor environment. The feature originally shipped as part of Device Guard and has been available as an opt-in setting in Windows 10 and Windows 11, but many users left it disabled due to performance overhead or compatibility concerns. By making it a default on eligible devices, Microsoft is extending this protection to a much larger population of Windows machines.

<details><summary>References</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/windows/security/hardware-security/enable-virtualization-based-protection-of-code-integrity">Enable virtualization-based protection of code integrity</a></li>
<li><a href="https://www.corsair.com/us/en/explorer/gamer/gaming-pcs/what-is-hvci/">What is HVCI? | CORSAIR</a></li>
<li><a href="https://medium.com/@boutnaru/the-windows-security-journey-hvci-hypervisor-protected-code-integrity-c13f98cac96f">The Windows Security Journey — HVCI (Hypervisor Protected Code Integrity) | by Shlomi Boutnaru, Ph.D. | Medium</a></li>

</ul>
</details>

**Tags**: `#Windows`, `#Security`, `#HVCI`, `#Microsoft`, `#Defense`

---