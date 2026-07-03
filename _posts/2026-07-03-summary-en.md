---
layout: default
title: "Horizon Summary: 2026-07-03 (EN)"
date: 2026-07-03
lang: en
---

> From 36 items, 12 important content pieces were selected

---

1. [Cloudflare to Block AI Crawlers by Default, Calls Out Google](#item-1) ⭐️ 9.0/10
2. [Virginia Bans Sale of Geolocation Data](#item-2) ⭐️ 8.0/10
3. [US Privacy Emergency: Aaronson Calls for Action](#item-3) ⭐️ 8.0/10
4. [Linux 6.9 regression: LUKS suspend no longer wipes keys from memory](#item-4) ⭐️ 8.0/10
5. [Podman v6.0.0 Released with Enhanced Networking and Quadlet Support](#item-5) ⭐️ 8.0/10
6. [Immich 3.0 Release Sparks E2EE Debate](#item-6) ⭐️ 8.0/10
7. [Understand to Participate: A Principle for AI Collaboration](#item-7) ⭐️ 8.0/10
8. [Meta's Neocloud Ambitions: Scaling RecSys and Custom Silicon](#item-8) ⭐️ 8.0/10
9. [ECTC 2026: EMIB-T, Custom HBM, HBM4, Microfluidic Cooling, Photonic Interconnects](#item-9) ⭐️ 8.0/10
10. [OpenAI Proposes 5% US Government Stake, Could Extend to Google, Meta](#item-10) ⭐️ 8.0/10
11. [Companies Restrict AI Use Due to Soaring Costs](#item-11) ⭐️ 8.0/10
12. [Anthropic Develops AI Chip, Talks Samsung Manufacturing](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Cloudflare to Block AI Crawlers by Default, Calls Out Google](https://techcrunch.com/2026/07/01/cloudflares-new-policy-pushes-ai-companies-to-pay-for-publishers-content/) ⭐️ 9.0/10

Cloudflare announced that starting September 15, it will by default block 'hybrid' crawlers that simultaneously scrape content for search indexing and AI training, and specifically criticized Google for exploiting search indexing to train its AI models. This marks a major shift in web policy, potentially forcing AI companies to pay publishers for content usage, and could reshape the balance between open web indexing and proprietary AI training. The new policy applies to publishers using Cloudflare's services who have enabled ad-supported pages; websites that allow search indexing will no longer automatically allow their content to be used for AI training.

telegram · zaihuapd · Jul 2, 05:37

**Background**: Cloudflare is a leading content delivery network and security provider that protects websites from malicious traffic. Some AI companies, including Google, use web crawlers to collect data for training large language models. Previously, many websites blocked AI crawlers but allowed Google's search bots, inadvertently permitting Google to use their content for AI training via its search indexing loophole.

<details><summary>References</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/1982210831434412370">爬虫如何绕过Cloudflare？2025最实用的网页抓取解决方案 - 知乎</a></li>
<li><a href="https://developers.google.com/search/docs/fundamentals/ai-optimization-guide">Google's Guide to Optimizing for Generative AI Features on Google Search | Google Search Central | Documentation | Google for Developers</a></li>
<li><a href="https://www.bright.cn/blog/ai/scrape-google-ai-mode">如何抓取 Google AI 模式：完整指南与 API 方法</a></li>

</ul>
</details>

**Tags**: `#Cloudflare`, `#AI爬虫`, `#Google`, `#内容付费`, `#网络政策`

---

<a id="item-2"></a>
## [Virginia Bans Sale of Geolocation Data](https://www.hunton.com/privacy-and-cybersecurity-law-blog/virginia-bans-sale-of-geolocation-data) ⭐️ 8.0/10

Virginia has passed a law banning the sale of geolocation data, marking a significant step in state-level privacy regulation. This law could set a precedent for other states and addresses growing concerns about the misuse of location data, especially in contexts like abortion advertising and insurance pricing. The ban applies to the sale of geolocation data, but enforcement challenges remain, such as jurisdiction over out-of-state companies and data collected via cloud servers in Virginia.

hackernews · toomuchtodo · Jul 2, 21:03 · [Discussion](https://news.ycombinator.com/item?id=48767347)

**Background**: Geolocation data from mobile devices is often collected and sold by data brokers for various purposes without explicit user consent. Concerns have led to increased regulation, with Virginia being one of the first states to specifically ban its sale.

**Discussion**: Commenters expressed mixed views: some praised the law as a good start but noted enforcement difficulties, while others highlighted real-world abuses like tracking visits to Planned Parenthood. Questions were raised about how companies like ALPR (automatic license plate readers) would comply.

**Tags**: `#privacy`, `#geolocation`, `#data regulation`, `#legislation`

---

<a id="item-3"></a>
## [US Privacy Emergency: Aaronson Calls for Action](https://scottaaronson.blog/?p=9902) ⭐️ 8.0/10

Scott Aaronson argues that the United States faces a privacy emergency due to a lack of federal privacy legislation and excessive corporate influence, and he calls for the adoption of differential privacy and other measures. This argument highlights a critical gap in US privacy protections compared to other nations, potentially spurring public discourse and legislative action that could reshape data privacy laws and corporate practices. Aaronson specifically emphasizes differential privacy, a mathematical framework that adds noise to data to protect individual privacy while preserving statistical utility, as a technical solution that should be mandated.

hackernews · flowercalled · Jul 3, 00:01 · [Discussion](https://news.ycombinator.com/item?id=48768992)

**Background**: The United States currently lacks a comprehensive federal privacy law, unlike the EU's GDPR or China's Personal Information Protection Law. Differential privacy is a rigorous mathematical definition that ensures an algorithm's output does not reveal whether any individual's data was included, and it is already used by some government agencies and tech companies.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Differential_privacy">Differential privacy</a></li>
<li><a href="https://medium.com/georgian-impact-blog/a-brief-introduction-to-differential-privacy-eacf8722283b">A Brief Introduction to Differential Privacy | by Georgian | Medium</a></li>

</ul>
</details>

**Discussion**: Commenters discussed related issues: one noted that corporate influence blocks popular policies like parental leave, others debated the effectiveness of differential privacy in the 2020 Census, and some provided links to contact legislators or commented on the relationship between capital and state.

**Tags**: `#privacy`, `#differential privacy`, `#United States`, `#technology policy`, `#legislation`

---

<a id="item-4"></a>
## [Linux 6.9 regression: LUKS suspend no longer wipes keys from memory](https://mathstodon.xyz/@iblech/116769502749142438) ⭐️ 8.0/10

Since Linux kernel 6.9, the `cryptsetup luksSuspend` command no longer wipes disk-encryption keys from kernel memory during system suspend, leaving the master key potentially accessible. This regression undermines a core security feature of LUKS disk encryption, exposing encrypted data to attackers with physical access during suspend. Users relying on `luksSuspend` to erase keys before sleeping are now vulnerable. The bug was discovered through NixOS tests and affects the `luksSuspend` command, which is used to temporarily suspend a LUKS device and remove the encryption key from memory. The key remains in memory after suspend, contrary to intended behavior.

hackernews · IngoBlechschmid · Jul 2, 15:25 · [Discussion](https://news.ycombinator.com/item?id=48763035)

**Background**: LUKS (Linux Unified Key Setup) is a standard for disk encryption on Linux. The `luksSuspend` command blocks I/O to an encrypted device and wipes the encryption key from kernel memory, which is crucial when suspending to RAM to prevent key exposure. This command is part of cryptsetup and can be triggered via system scripts or systemd hooks. The regression only affects distributions that enable this extension, as it is not part of the upstream kernel.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48763035">Since Linux 6.9, LUKS suspend stopped wiping disk-encryption keys from memory | Hacker News</a></li>
<li><a href="https://github.com/vianney/arch-luks-suspend">GitHub - vianney/arch-luks-suspend: Lock encrypted root volume on suspend in Arch Linux · GitHub</a></li>

</ul>
</details>

**Discussion**: Commenters on Hacker News debated the severity: some noted that `luksSuspend` is a Debian extension and not officially supported upstream, so the regression may be limited in scope. Others clarified the difference between suspend-to-RAM (key remains in memory normally) and suspend-to-disk (key gets encrypted). Overall, the community appreciated the NixOS test that caught the bug but questioned whether the title was alarmist.

**Tags**: `#security`, `#linux kernel`, `#disk encryption`, `#LUKS`, `#regression`

---

<a id="item-5"></a>
## [Podman v6.0.0 Released with Enhanced Networking and Quadlet Support](https://blog.podman.io/2026/07/introducing-podman-v6-0-0/) ⭐️ 8.0/10

Podman v6.0.0 is a major version release featuring improved networking capabilities and enhanced Quadlet integration for declarative container management via systemd unit files. This release strengthens Podman's position as a leading Docker alternative, particularly for users seeking rootless container management and integration with systemd, potentially driving wider adoption in DevOps environments. Key improvements include better networking support, likely via netavark or CNI, and Quadlet enabling containers to run as systemd services with declarative unit files. Users can migrate from Docker with minimal changes since compose files are supported.

hackernews · soheilpro · Jul 2, 14:23 · [Discussion](https://news.ycombinator.com/item?id=48762098)

**Background**: Podman is a daemonless container engine that runs containers rootlessly, offering a drop-in replacement for Docker. Quadlet is a feature that allows containers to be managed declaratively as systemd units, simplifying deployment on Linux systems without requiring full orchestration tools like Kubernetes. This release builds on those capabilities to improve networking and usability.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.podman.io/en/latest/markdown/podman-systemd.unit.5.html">podman-systemd.unit — Podman documentation</a></li>
<li><a href="https://www.redhat.com/en/blog/quadlet-podman">Make systemd better for Podman with Quadlet</a></li>
<li><a href="https://docs.podman.io/en/latest/markdown/podman-quadlet.1.html">podman-quadlet — Podman documentation</a></li>

</ul>
</details>

**Discussion**: Community comments are largely positive, with users like cdmckay reporting seamless migration from Docker. Others praise Quadlet for simplifying rootless container hosting. However, rsyring criticizes the lack of official installation packages for Ubuntu, viewing it as a barrier to adoption.

**Tags**: `#containerization`, `#Podman`, `#DevOps`, `#open-source`, `#docker-alternative`

---

<a id="item-6"></a>
## [Immich 3.0 Release Sparks E2EE Debate](https://github.com/immich-app/immich/discussions/29439) ⭐️ 8.0/10

Immich 3.0, a major update to the self-hosted photo management tool, has been released, praised as a drop-in replacement for Apple Photos and Google Photos but criticized for lacking end-to-end encryption (E2EE). The community is actively debating whether the trade-offs are acceptable. This release highlights the ongoing tension in the self-hosting community between convenience and privacy. Immich's popularity as a self-hosted solution makes its design choices influential for the broader ecosystem, especially as users compare it to E2EE-focused alternatives like Ente. Immich 3.0 does not include end-to-end encryption, a deliberate decision due to performance and functionality trade-offs (e.g., server-side machine learning features). Some community members argue that the lack of E2EE is acceptable as long as the server is under personal control, while others point to alternatives like Ente that offer E2EE.

hackernews · hashier · Jul 2, 14:13 · [Discussion](https://news.ycombinator.com/item?id=48761944)

**Background**: Immich is an open-source, self-hosted photo and video management solution that allows users to back up, organize, and share their media on their own servers. It is often compared to cloud services like Google Photos and Apple Photos but gives users full control over their data. End-to-end encryption ensures that only the user can decrypt their data, but it can limit server-side features like AI-powered search and object recognition.

<details><summary>References</summary>
<ul>
<li><a href="https://immich.app/">Immich</a></li>
<li><a href="https://grokipedia.com/page/Immich">Immich</a></li>

</ul>
</details>

**Discussion**: The community is divided: some users, like AussieWog93, argue that E2EE is unnecessary for self-hosted setups because physical security threats are minimal and encryption can complicate data recovery. Others, like Cider9986, chose alternatives such as Ente specifically for E2EE. Overall, the discussion reflects a broader debate about the prioritization of privacy versus functionality in self-hosted software.

**Tags**: `#self-hosting`, `#photo management`, `#open-source`, `#encryption`, `#privacy`

---

<a id="item-7"></a>
## [Understand to Participate: A Principle for AI Collaboration](https://simonwillison.net/2026/Jul/2/understand-to-participate/#atom-everything) ⭐️ 8.0/10

Simon Willison highlights Geoffrey Litt's 'understand to participate' principle, which argues that developers collaborating with coding agents must maintain deep understanding of the code to avoid cognitive debt and remain actively creative in the process. As AI coding agents become more capable, developers risk accumulating cognitive debt—eroding their own mental model of the codebase. This principle offers a proactive approach to staying engaged and preventing loss of control over the software's evolution. Geoffrey Litt presented this concept at the AIE World's Fair 2026, and Simon Willison published a blog post echoing the idea. The principle emphasizes that understanding the code to a sufficient depth is necessary to enable further productive collaboration with the AI agent.

rss · Simon Willison · Jul 2, 17:07

**Background**: Cognitive debt refers to the erosion of shared understanding across a software system over time, similar to technical debt but in the minds of developers. As AI agents generate more code, developers may lose familiarity with the codebase, leading to difficulties in reasoning about and safely modifying the system. The 'understand to participate' principle advocates for continuous learning and engagement to counteract this drift.

<details><summary>References</summary>
<ul>
<li><a href="https://margaretstorey.com/blog/2026/02/09/cognitive-debt/">How Generative and Agentic AI Shift Concern from Technical Debt to Cognitive Debt</a></li>
<li><a href="https://getdx.com/blog/cognitive-debt-the-hidden-risk-in-ai-driven-software-development/">Cognitive debt: The hidden risk in AI-driven software development</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#cognitive debt`, `#code collaboration`, `#software engineering`

---

<a id="item-8"></a>
## [Meta's Neocloud Ambitions: Scaling RecSys and Custom Silicon](https://newsletter.semianalysis.com/p/meta-compute-everyone-wants-to-be) ⭐️ 8.0/10

Analysis from SemiAnalysis indicates Meta is pursuing a neocloud strategy, scaling its recommender systems by 10x and developing custom silicon under projects like 'Bedrock 2.0', while also competing in the GPU cloud market with a ClusterMAX ranking. This shift positions Meta as a potential major player in AI infrastructure, challenging traditional hyperscalers and neocloud providers, and could reshape the economics of AI training and inference. The content mentions 'Scaling RecSys by 10x' indicating massive growth in recommendation system workloads, and 'Bedrock 2.0' likely refers to Meta's next-generation compute platform; ClusterMAX is a GPU cloud rating system by SemiAnalysis that ranks providers across performance, networking, and other criteria.

rss · Semianalysis · Jul 2, 22:18

**Background**: Neocloud refers to specialized cloud providers focused on AI workloads using GPU accelerators, distinct from traditional hyperscale clouds. Meta, traditionally a hyperscaler, is now investing heavily in custom silicon and neocloud-like capabilities to reduce reliance on external vendors and optimize for its AI services like recommendation systems.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cisco.com/site/us/en/learn/topics/computing/what-is-neocloud.html">What Is Neocloud? - Cisco</a></li>
<li><a href="https://blog.equinix.com/blog/2025/10/14/what-is-a-neocloud/">What Is a Neocloud? - Interconnections - The Equinix Blog</a></li>
<li><a href="https://www.clustermax.ai/">GPU Cloud ClusterMAX ™ Rating & Ranking System | SemiAnalysis</a></li>

</ul>
</details>

**Tags**: `#cloud computing`, `#meta`, `#AI infrastructure`, `#recommender systems`

---

<a id="item-9"></a>
## [ECTC 2026: EMIB-T, Custom HBM, HBM4, Microfluidic Cooling, Photonic Interconnects](https://newsletter.semianalysis.com/p/ectc2026) ⭐️ 8.0/10

At ECTC 2026, Intel unveiled its EMIB-T packaging technology supporting HBM4 and UCIe, while Microsoft demonstrated microfluidic cooling for 3D heterogeneous integration. Other highlights included custom HBM solutions from SK Hynix and advances in photonic interconnects from Lightmatter. These announcements address critical bottlenecks in AI chip performance, including memory bandwidth, thermal management, and inter-chip connectivity. The advances pave the way for more powerful and efficient data center accelerators and high-performance computing systems. EMIB-T reduces defect vulnerability and scales to larger form factors beyond reticle limits, with Intel reporting 90% yield. Microfluidic cooling circulates coolant through microscopic channels etched directly into the silicon substrate, enabling efficient heat removal close to active cores.

rss · Semianalysis · Jul 2, 17:25

**Background**: Advanced packaging technologies like Intel's EMIB and TSMC's CoWoS integrate multiple dies in a small footprint to overcome transistor scaling limits. However, they face challenges in thermal dissipation and interconnect density. Microfluidic cooling and photonic interconnects are emerging solutions to these issues, with photonic interconnects using light instead of electricity to transmit data with lower power and higher bandwidth.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/ammhasib_driving-the-future-of-multi-chip-compute-activity-7408764535257317376-dVkb">Intel EMIB - T : Revolutionizing AI and HPC Packaging with... | LinkedIn</a></li>
<li><a href="https://abit.ee/en/hard/intel-introduces-emib-t-revolutionary-multi-die-packaging-technology-with-hbm4-support">Intel Introduces EMIB - T — Revolutionary Multi-Die Packaging...</a></li>
<li><a href="https://www.datacenterdynamics.com/en/analysis/microfluidics-cooling-inside-the-chip/">Microfluidics: Cooling inside the chip - DCD</a></li>
<li><a href="https://lightmatter.co/knowledge-hub/how-do-photonic-interconnects-work/">How Do Photonic Interconnects Work?</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#advanced packaging`, `#HBM`, `#photonic interconnects`, `#cooling`

---

<a id="item-10"></a>
## [OpenAI Proposes 5% US Government Stake, Could Extend to Google, Meta](https://www.bloomberg.com/news/articles/2026-07-02/openai-proposes-giving-the-us-government-a-5-stake-ft-says) ⭐️ 8.0/10

OpenAI has proposed that the US government take a 5% equity stake in the company, with discussions suggesting a similar 5% stake could be extended to other major AI firms such as Google, Meta, and Anthropic to allow the public to benefit directly from the AI boom. This proposal marks a paradigm shift in AI governance, potentially setting a precedent for government involvement in private AI companies and raising critical questions about control, regulation, and equitable distribution of AI profits. The proposal includes a government vehicle that would collectively hold 5% stakes in OpenAI, Anthropic, Google, and Meta; however, it remains unclear whether these companies would accept the arrangement, and concerns about regulatory conflicts and corporate control have been raised.

telegram · zaihuapd · Jul 2, 06:02

**Background**: The AI industry has experienced rapid growth, leading to debates about how to ensure its benefits are shared broadly. Government ownership stakes in technology companies are unusual in the US, where private enterprise is typically favored. This proposal would create a direct financial link between the public and AI profits.

**Tags**: `#AI`, `#Government Stake`, `#Regulation`, `#OpenAI`, `#Tech Policy`

---

<a id="item-11"></a>
## [Companies Restrict AI Use Due to Soaring Costs](https://www.404media.co/companies-are-throttling-employees-ai-use-because-its-too-expensive/) ⭐️ 8.0/10

Citibank, Atlassian, and Adobe are restricting employee access to advanced AI models like GPT-5.5 and Claude Opus 4.7 due to rapidly escalating costs under usage-based pricing. This trend signals that enterprise AI adoption faces a cost-management challenge, potentially slowing down deployment and forcing companies to rethink pricing models and usage policies. Citibank completely disabled Claude Opus 4.6, 4.7, and GPT-5.5 on June 24. Atlassian's AI monthly spending surged from $5 million in August 2025 to over $15 million by May 2026, leading to usage caps.

telegram · zaihuapd · Jul 2, 13:59

**Background**: Many AI tools are priced per token or per API call, known as usage-based pricing. Companies often buy AI credits in bulk and set internal policies to control costs. As models become more powerful, they consume more tokens per task, driving up expenses.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.5">GPT-5.5</a></li>
<li><a href="https://c-ai.chat/model-guides/">Models - Claude AI</a></li>
<li><a href="https://ordwaylabs.com/blog/ai-credits/">AI Credits : What They Are and How They Work</a></li>

</ul>
</details>

**Tags**: `#AI cost`, `#enterprise AI`, `#AI regulation`, `#technology news`

---

<a id="item-12"></a>
## [Anthropic Develops AI Chip, Talks Samsung Manufacturing](https://www.theinformation.com/articles/anthropic-talks-samsung-manufacture-custom-ai-chip) ⭐️ 8.0/10

Anthropic has initiated development of its own AI chip and is in talks with Samsung Electronics for potential manufacturing, aiming to gain more control over the infrastructure powering its Claude models. This move reflects a growing trend of vertical integration among leading AI companies, allowing Anthropic to optimize hardware-software co-design for efficiency and reduce dependence on external chip suppliers. The project is still at an early stage, and Anthropic is entering later than other firms that have already advanced custom server chips. Samsung would serve as a contract manufacturer for the chip.

telegram · zaihuapd · Jul 2, 15:57

**Background**: Major AI companies like OpenAI and Google have been developing custom chips to accelerate AI workloads and reduce costs. Samsung is the world's largest memory chip maker and a major foundry player. Contract manufacturing allows chip designers to fabricate their designs without building their own factories.

**Tags**: `#AI chips`, `#Anthropic`, `#Samsung`, `#hardware`, `#custom silicon`

---