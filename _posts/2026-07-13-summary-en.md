---
layout: default
title: "Horizon Summary: 2026-07-13 (EN)"
date: 2026-07-13
lang: en
---

> From 31 items, 6 important content pieces were selected

---

1. [GPT-5.6 Solves 50-Year Graph Conjecture in Under an Hour](#item-1) ⭐️ 10.0/10
2. [xAI Grok CLI Uploads Entire Codebase and Secret Files by Default](#item-2) ⭐️ 9.0/10
3. [China approves world's first invasive BCI medical device](#item-3) ⭐️ 9.0/10
4. [Math.tanh in Chromium 148 Enables OS Fingerprinting](#item-4) ⭐️ 8.0/10
5. [Terry Tao builds apps with LLM coding agents](#item-5) ⭐️ 8.0/10
6. [I love LLMs, I hate hype](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [GPT-5.6 Solves 50-Year Graph Conjecture in Under an Hour](https://www.qbitai.com/2026/07/447873.html) ⭐️ 10.0/10

GPT-5.6 Sol Ultra autonomously proved the cycle double cover conjecture, a 50-year-old open problem in graph theory, in less than one hour and produced a 3-page PDF proof. This achievement marks a significant milestone in AI-driven mathematical research, demonstrating that large language models can autonomously solve complex, long-standing conjectures. It could accelerate progress in mathematics and inspire new AI-assisted discovery methods. The model used 64 sub-agents working in parallel, transforming the problem into a finite field edge labeling and linear equations system. OpenAI also published the full prompt (about 700 characters), which specified acceptance criteria, definitions, boundary conditions, and failure cases, without prescribing fixed solution steps.

telegram · zaihuapd · Jul 12, 03:49

**Background**: The cycle double cover conjecture, posed by W. T. Tutte and others, asks whether every bridgeless graph contains a collection of cycles such that each edge appears exactly twice. It is a central problem in graph theory with connections to graph embeddings and polyhedral theory. Previous attempts over five decades had not yielded a proof.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cycle_double_cover_conjecture">Cycle double cover conjecture</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Mathematics`, `#Graph Theory`, `#GPT`, `#Breakthrough`

---

<a id="item-2"></a>
## [xAI Grok CLI Uploads Entire Codebase and Secret Files by Default](https://gist.github.com/cereblab/dc9a40bc26120f4540e4e09b75ffb547) ⭐️ 9.0/10

Security researchers discovered that xAI's Grok CLI tool (version 0.2.93) uploads entire code repositories and sensitive files like .env to xAI servers via Google Cloud Storage and git bundles, even when the 'improve model' setting is disabled. This privacy vulnerability exposes developers' entire codebases and secrets, potentially leading to data breaches and intellectual property theft, especially concerning for a tool used by many in the AI development community. The tool uploads file contents embedded in model dialogue requests and also creates a git bundle of the entire repository regardless of the user's prompt. In tests, a 12 GB repository resulted in over 5 GiB uploaded without rejection, and a file explicitly instructed not to be opened was still recoverable from the upload package.

telegram · zaihuapd · Jul 12, 04:19

**Background**: Git bundle is a Git command that packages the entire repository into a single file for offline transfer. Google Cloud Storage is a scalable object storage service. xAI's Grok CLI is a command-line tool for interacting with Grok AI models, often used by developers for coding assistance.

<details><summary>References</summary>
<ul>
<li><a href="https://git-scm.com/docs/git-bundle">Git - git-bundle Documentation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Google_Cloud_Storage">Google Cloud Storage</a></li>

</ul>
</details>

**Tags**: `#security`, `#privacy`, `#xAI`, `#Grok CLI`, `#data leakage`

---

<a id="item-3"></a>
## [China approves world's first invasive BCI medical device](https://t.me/zaihuapd/42515) ⭐️ 9.0/10

China's National Medical Products Administration has approved the 'Implantable Brain-Computer Interface Hand Function Compensation System' by Bōruìkāng Medical Technology (Shanghai) Co., Ltd., making it the first invasive brain-computer interface medical device to receive regulatory approval for clinical use worldwide. This milestone transitions brain-computer interface technology from research to clinical practice, offering a new therapeutic option for tetraplegic patients with cervical spinal cord injury to restore hand grasping function, potentially improving their quality of life significantly. The device uses epidural minimally invasive implantation and wireless power and communication technology, and is paired with a pneumatic glove to assist patients aged 18-60 with cervical spinal cord injury in achieving hand grasping movements. Clinical trial results showed improved hand grasping ability and quality of life in participants.

telegram · zaihuapd · Jul 12, 14:39

**Background**: Brain-computer interfaces (BCIs) enable direct communication between the brain and external devices. Invasive BCIs involve implanting electrodes into or on the brain's surface to record neural signals with high precision. This device targets tetraplegic patients who have lost hand function due to spinal cord injury, decoding their movement intentions from brain signals to control a pneumatic glove, thereby restoring grasping ability.

<details><summary>References</summary>
<ul>
<li><a href="https://www.163.com/dy/article/KQ5H8KUB0530RMN7.html">163.com/dy/article/KQ5H8KUB0530RMN7.html</a></li>
<li><a href="https://health.people.com.cn/n1/2026/0414/c14739-40700851.html">人机交互新形态走向临床（深度观察） --健康·生活--人民网</a></li>

</ul>
</details>

**Tags**: `#brain-computer interface`, `#medical device`, `#neural engineering`, `#spinal cord injury`, `#regulatory approval`

---

<a id="item-4"></a>
## [Math.tanh in Chromium 148 Enables OS Fingerprinting](https://scrapfly.dev/posts/browser-math-os-fingerprint/) ⭐️ 8.0/10

Since Chromium 148, slight differences in the Math.tanh implementation across operating systems allow websites to infer the underlying OS with a single tanh call. This new fingerprinting vector undermines user privacy by enabling persistent OS detection even when user-agent strings are spoofed, affecting all Chromium-based browsers. The vulnerability stems from non-identical transcendental function implementations across operating systems, which produce distinct Math.tanh results for the same input.

hackernews · joahnn_s · Jul 12, 21:12 · [Discussion](https://news.ycombinator.com/item?id=48884853)

**Background**: Browser fingerprinting collects device-specific traits to identify users without cookies. Math.tanh is a hyperbolic tangent function whose precision can vary by hardware and OS math libraries, making it a potential fingerprinting vector.

<details><summary>References</summary>
<ul>
<li><a href="https://pappp.net/?p=108314">Since Chromium 148, Math.tanh is now fingerprintable to link ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Transcendental_function">Transcendental function - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commentators expressed mixed reactions: some noted that this technique is also fingerprintable to browser version range, while others questioned the motives of the scraping company behind the disclosure. Concerns were raised about Linux users being falsely flagged as scrapers, and that Tor Browser had already given up obscuring the OS.

**Tags**: `#fingerprinting`, `#browser security`, `#privacy`, `#Math.tanh`, `#Chromium`

---

<a id="item-5"></a>
## [Terry Tao builds apps with LLM coding agents](https://terrytao.wordpress.com/2026/07/11/old-and-new-apps-via-modern-coding-agents/) ⭐️ 8.0/10

Renowned mathematician Terry Tao documented his experience using modern LLM coding agents to build interactive visualizations and apps, showcasing a workflow where non-experts can create software through guided AI interaction. This demonstrates that AI can democratize software creation, enabling people without traditional programming skills to build custom tools, and highlights the vast latent demand for software outside of tech-centric fields. Tao emphasized that for non-mission-critical supplements (such as visualizations for academic papers), the downside risk of using LLM agents is acceptable, and his approach involved guided interaction rather than fully autonomous code generation.

hackernews · subset · Jul 12, 11:09 · [Discussion](https://news.ycombinator.com/item?id=48880170)

**Background**: LLM coding agents are AI systems that leverage large language models to assist in software development tasks, including code generation, debugging, and UI design. These agents can operate in various environments like terminals, IDEs, or even as standalone desktop apps, and are part of the broader field of AI-assisted software development.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI-assisted_software_development">AI-assisted software development</a></li>
<li><a href="https://opencode.ai/">OpenCode | The open source AI coding agent</a></li>

</ul>
</details>

**Discussion**: Community comments generally express excitement about the democratization of software creation, with some noting the humor in seeing a Fields Medalist rely on AI like everyone else. One commenter highlighted the value for non-software fields, while another appreciated Tao's balanced perspective on the tool's limitations.

**Tags**: `#LLM`, `#coding agents`, `#AI-assisted development`, `#software engineering`, `#Hacker News`

---

<a id="item-6"></a>
## [I love LLMs, I hate hype](https://geohot.github.io//blog/jekyll/update/2026/07/12/i-love-llms.html) ⭐️ 8.0/10

George Hotz argues that frontier AI labs may fail to capture the economic value generated by LLMs, as real productivity gains are realized in private, customized applications rather than through paid tokens. This critique challenges the high valuations of frontier labs by highlighting a value capture problem, suggesting that the biggest beneficiaries of LLMs might be individual users and small businesses, not the model providers. Hotz points out that while subscription prices ($100–$200/month) for frontier models are attractive, the resulting productivity improvements are often hidden in private deployments like homelabs, not in public-facing products.

hackernews · therepanic · Jul 12, 18:31 · [Discussion](https://news.ycombinator.com/item?id=48883343)

**Background**: Large language models (LLMs) like GPT-4 and Claude have sparked massive investment and hype, with many believing they will transform industries. However, questions remain about who will ultimately profit from this technology—the companies building the models or the users applying them to specific tasks. Hotz's argument echoes a classic economic puzzle: innovation may create enormous value, but capturing that value is not guaranteed.

**Discussion**: Commenters largely agree with Hotz, noting that frontier model subscriptions are a no-brainer at current prices, and that real productivity gains are being seen in private, one-off software projects. Some also express concerns about the future of open source, as maintaining forks becomes easier with LLM assistance, potentially reducing upstream contributions.

**Tags**: `#LLM`, `#AI hype`, `#valuation`, `#open source`, `#productivity`

---