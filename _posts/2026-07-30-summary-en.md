---
layout: default
title: "Horizon Summary: 2026-07-30 (EN)"
date: 2026-07-30
lang: en
---

> From 40 items, 12 important content pieces were selected

---

1. [Open-source engine runs Gemma 4 26B in 2GB RAM on M-series Mac](#item-1) ⭐️ 9.0/10
2. [Russian FSB charges Telegram founder Durov with aiding terrorism](#item-2) ⭐️ 9.0/10
3. [AI startups cut publications, transparency at risk](#item-3) ⭐️ 8.0/10
4. [Mitchell Hashimoto Launches Superlogical](#item-4) ⭐️ 8.0/10
5. [AI worms exploit prompt injection in Copilot for Word](#item-5) ⭐️ 8.0/10
6. [Long Policy Documents Fail to Reliably Govern AI Agents](#item-6) ⭐️ 8.0/10
7. [Matthew Green on AI's Perfect Timing for Post-Quantum Cryptanalysis](#item-7) ⭐️ 8.0/10
8. [Vendor-agnostic ML inference on edge devices with ncnn and Vulkan](#item-8) ⭐️ 8.0/10
9. [Hugging Face Widely Abused for Deepfake Nude Images](#item-9) ⭐️ 8.0/10
10. [Moonshot AI seeks $2B funding at $30B valuation](#item-10) ⭐️ 8.0/10
11. [China Drafts Anti-Cyberbullying Law Targeting AI-Generated Abuse](#item-11) ⭐️ 8.0/10
12. [OpenAI gives 100,000 researchers free access to GPT-5.6](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Open-source engine runs Gemma 4 26B in 2GB RAM on M-series Mac](https://github.com/drumih/turbo-fieldfare) ⭐️ 9.0/10

TurboFieldfare, a new open-source inference engine written in Swift and Metal, streams only the routed experts from SSD to run the 4-bit quantized Gemma 4 26B MoE model using approximately 2GB of RAM on any M-series Mac. It achieves 5-6 tokens/second on an 8GB M2 MacBook Air and 31-35 tokens/second on an M5 MacBook Pro. This breakthrough enables large Mixture-of-Experts models to run on resource-constrained devices with limited RAM, democratizing on-device AI that previously required high-end hardware. It could inspire further research into memory-efficient inference techniques and expand practical applications of local AI on laptops and edge devices. The model's 4-bit weights occupy about 14GB, but the engine keeps the shared layers and KV cache in RAM while streaming only the required experts from SSD using bounded parallel pread and an expert cache. It also includes an experimental OpenAI-compatible local server with streaming and tool call support.

hackernews · gitpusher42 · Jul 29, 15:05 · [Discussion](https://news.ycombinator.com/item?id=49098510)

**Background**: Mixture of Experts (MoE) models use multiple specialized sub-networks (experts) and a gating network to activate only relevant experts per input, reducing computation. KV caching stores key-value pairs from previous tokens to avoid redundant calculations during generation. 4-bit quantization compresses model weights to 4 bits per parameter, drastically reducing memory footprint with minimal accuracy loss.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>
<li><a href="https://medium.com/@minh.hoque/understanding-kv-caching-in-transformers-729271c9b74a">Understanding KV Caching in Transformers - Medium</a></li>
<li><a href="https://www.emergentmind.com/topics/4-bit-model-quantization">4-Bit Model Quantization</a></li>

</ul>
</details>

**Discussion**: The community expressed excitement and noted the practical impact, with one user reporting 48 tok/s on a 64GB M4 Max. Technical comparisons to llama.cpp's mmap approach were raised, and the developer responded with explanations. A contributor also provided a build fix for older macOS versions.

**Tags**: `#inference`, `#on-device AI`, `#Gemma`, `#Mac`, `#SSD streaming`

---

<a id="item-2"></a>
## [Russian FSB charges Telegram founder Durov with aiding terrorism](https://www.interfax.ru/russia/1106228) ⭐️ 9.0/10

On July 29, the Russian Federal Security Service (FSB) charged Telegram founder Pavel Durov with aiding terrorism under Article 205.1 of the Criminal Code and placed him on an international wanted list. This charge escalates the conflict between Russian authorities and the popular messaging platform, potentially setting a precedent for holding tech executives criminally liable for user-generated content, with global implications for platform responsibility and free speech. The FSB alleges that Telegram management refused to delete channels, groups, and bots used by Ukrainian intelligence and terrorist groups to coordinate sabotage, attacks, mass killings, and fraud, resulting in casualties and billions of rubles in damages.

telegram · zaihuapd · Jul 29, 05:56

**Background**: Telegram is a widely used messaging app known for its strong encryption and privacy features. It has faced scrutiny from various governments over content moderation, including previous fines in Russia for refusing to provide decryption keys. The current charge marks a severe escalation, targeting the founder personally with an international warrant.

**Tags**: `#Telegram`, `#Pavel Durov`, `#Security`, `#Legal`, `#Geopolitics`

---

<a id="item-3"></a>
## [AI startups cut publications, transparency at risk](https://www.science.org/content/article/ai-s-top-startups-are-barely-publishing-their-research) ⭐️ 8.0/10

A new report reveals that leading AI startups are publishing significantly fewer research papers than before, marking a shift away from open science. This decline threatens the transparency and reproducibility of AI research, potentially slowing scientific progress and hindering peer review. Despite fewer publications, OpenAI still leads in cumulative citations among startups, according to the study. The paper also notes that companies like Google are excluded because they are not unicorns.

hackernews · YeGoblynQueenne · Jul 29, 21:25 · [Discussion](https://news.ycombinator.com/item?id=49103285)

**Background**: AI research has historically been open, with conferences like NeurIPS and preprints on arXiv fostering rapid dissemination. However, as AI startups face commercial pressures, many choose to keep their work proprietary to maintain a competitive edge. This trend raises concerns about the field's ability to validate findings and build on prior work.

**Discussion**: Commenters share mixed experiences: one notes that publishing led to rejection from tier-1 journals, while another avoids publishing to prevent copying by OpenAI and Anthropic. Several express concern that the 'blogification' of AI research enables unsupported claims.

**Tags**: `#AI`, `#research`, `#startups`, `#publishing`, `#transparency`

---

<a id="item-4"></a>
## [Mitchell Hashimoto Launches Superlogical](https://www.superlogical.com/) ⭐️ 8.0/10

Mitchell Hashimoto announced Superlogical, a new company that will build terminal applications on top of the open-source libghostty library, while Ghostty itself has been transferred to a non-profit. This move validates a novel business model where a company builds proprietary products on top of a community-maintained open-source core, potentially influencing how open-source projects sustain themselves. Superlogical will use the same MIT-licensed components as any other consumer and continue to upstream shared terminal work. The first libghostty component, libghostty-vt, provides a zero-dependency API for terminal sequence parsing and state management.

hackernews · yan · Jul 29, 15:41 · [Discussion](https://news.ycombinator.com/item?id=49098965)

**Background**: Ghostty is a modern terminal emulator written in Zig, and libghostty is its C-compatible library that can be embedded in other applications for terminal emulation. By spinning off libghostty as an independent MIT-licensed library, Hashimoto enables others to build terminal tools without reinventing the wheel. Superlogical aims to be one such consumer of libghostty, focusing on terminal-based products.

<details><summary>References</summary>
<ul>
<li><a href="https://mitchellh.com/writing/libghostty-is-coming">Libghostty Is Coming – Mitchell Hashimoto</a></li>
<li><a href="https://github.com/Uzaaft/awesome-libghostty">GitHub - Uzaaft/awesome-libghostty</a></li>
<li><a href="https://docsmith.aigne.io/docs/ghostty/en/libghostty-ed730d">libghostty API - docsmith.aigne.io</a></li>

</ul>
</details>

**Discussion**: Commenters largely praised the open-source governance model, with simonw highlighting the transfer of Ghostty to a non-profit. Some drew parallels to OLE/COM, while a few criticized the enigmatic title as clickbait. Overall sentiment was positive, with interest in the business model.

**Tags**: `#announcement`, `#open source`, `#terminal`, `#company`, `#Mitchell Hashimoto`

---

<a id="item-5"></a>
## [AI worms exploit prompt injection in Copilot for Word](https://enklypesalt.com/posts/context-collapse-part3-ai-worming-through-word/) ⭐️ 8.0/10

Researcher Håkon Måløy developed a proof-of-concept AI worm that self-propagates through Microsoft Copilot for Word by embedding adversarial prompts in documents using hidden white text, demonstrating the first document-borne AI worm in a mainstream productivity suite. This vulnerability highlights a critical security flaw in AI agents that mix instructions with data, potentially allowing worms to autonomously steal data, manipulate documents, and spread across organizations, posing a serious risk to enterprise AI adoption. The attack uses white text with hyperlinks or embedded prompts to hide instructions from human viewers but readable by Copilot, and it can propagate by instructing Copilot to modify new documents with the same prompt.

hackernews · Canopy9560 · Jul 29, 11:44 · [Discussion](https://news.ycombinator.com/item?id=49096188)

**Background**: Prompt injection attacks exploit the inability of large language models to distinguish between system instructions and user-provided data. When AI agents like Copilot have write access to documents, embedded instructions can cause the agent to execute unauthorized actions. This research builds on known indirect prompt injection techniques but demonstrates the first self-propagating worm in a commercial LLM-powered application.

<details><summary>References</summary>
<ul>
<li><a href="https://enklypesalt.com/posts/context-collapse-part3-ai-worming-through-word/">Context Collapse, Part 3 - AI Worming through Word | En Klype Salt</a></li>
<li><a href="https://windowsnews.ai/article/after-144-days-microsoft-still-cant-fully-fix-copilot-vulnerability-that-lets-hidden-text-manipulate.440856">After 144 Days, Microsoft Still Can't Fully Fix Copilot Vulnerability That Lets Hidden Text Manipulate Reports - Windows News</a></li>

</ul>
</details>

**Discussion**: Community comments express alarm and skepticism, with rwmj noting that mixing instructions with data is an unfixable flaw, and boothby predicting the situation will worsen as users grant agents extensive access. simonw reacted with concern, while averagjoe stated they have already uninstalled Copilot to avoid such attacks. piker highlighted that hidden white text technique is still effective and shared a related link.

**Tags**: `#security`, `#AI`, `#worms`, `#prompt injection`, `#Microsoft Copilot`

---

<a id="item-6"></a>
## [Long Policy Documents Fail to Reliably Govern AI Agents](https://arxiv.org/abs/2607.25398) ⭐️ 8.0/10

A new paper titled 'Handbook.md' demonstrates that long policy documents cannot reliably guide AI agents due to context window limitations and model quantization issues. This finding challenges the assumption that detailed written policies can ensure responsible AI behavior, raising concerns for deploying AI agents in real-world applications. The research highlights that even models claiming 1M token context windows fail under extreme quantization and poor sampling, causing agents to ignore earlier instructions after minutes of interaction.

hackernews · spIrr · Jul 29, 13:01 · [Discussion](https://news.ycombinator.com/item?id=49096969)

**Background**: Language models have limited context windows, akin to working memory, which cap how much text they can process at once. Model quantization reduces precision to improve efficiency but can degrade performance. These factors collectively impair an agent's ability to follow long policies.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Context_window">Context window - Wikipedia</a></li>
<li><a href="https://developer.nvidia.com/blog/model-quantization-concepts-methods-and-why-it-matters/">Model Quantization: Concepts, Methods, and Why It Matters</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree with the paper's findings, with one noting that local inference can mitigate issues, while another points out that humans also struggle with long policies. A user with Claude experience reports that instructions in CLAUDE.md files get bypassed quickly, suggesting the problem is widespread.

**Tags**: `#AI`, `#LLM`, `#long context`, `#agents`, `#policy compliance`

---

<a id="item-7"></a>
## [Matthew Green on AI's Perfect Timing for Post-Quantum Cryptanalysis](https://simonwillison.net/2026/Jul/29/matthew-green/#atom-everything) ⭐️ 8.0/10

Matthew Green, a respected cryptographer, highlighted that the ongoing transition from traditional public-key algorithms to post-quantum algorithms creates a perfect window for AI to contribute to cryptanalysis. He noted that this could either validate new standards or expose fundamental weaknesses, making the cryptanalysis literature more robust. This observation underscores the convergence of quantum-resistant cryptography and advanced AI, which could either strengthen confidence in new cryptographic problems or undermine them entirely. The outcome will shape the security of future digital infrastructure and the resilience of encryption against quantum threats. Green specifically references the HAWK scheme, a lattice-based post-quantum signature candidate in NIST's additional competition, and mentions Impagliazzo's Five Worlds, particularly Minicrypt where public-key cryptography might not exist. He also alludes to Anthropic's recent work on AI-driven cryptanalysis.

rss · Simon Willison · Jul 29, 18:18

**Background**: Public-key cryptography underpins secure online communication, but quantum computers threaten to break algorithms like RSA and ECC. NIST is leading a multi-year effort to standardize post-quantum algorithms, with HAWK being one candidate for digital signatures. Impagliazzo's Five Worlds is a taxonomy of possible cryptographic realities based on computational hardness assumptions.

<details><summary>References</summary>
<ul>
<li><a href="https://csrc.nist.gov/csrc/media/Projects/pqc-dig-sig/documents/round-1/spec-files/hawk-spec-web.pdf">HAWK Specification Document - NIST Computer Security Resource ...</a></li>
<li><a href="https://fanpu.io/blog/2022/impagliazzos-five-worlds/">Impagliazzo 's Five Worlds , or The Computational... | Fan Pu Zeng</a></li>
<li><a href="https://thehackernews.com/2026/07/claude-ai-just-cracked-post-quantum.html">Claude AI Just Cracked a Post-Quantum Test Scheme and Found a ...</a></li>

</ul>
</details>

**Tags**: `#post-quantum cryptography`, `#AI cryptanalysis`, `#cryptography transition`, `#Matthew Green`

---

<a id="item-8"></a>
## [Vendor-agnostic ML inference on edge devices with ncnn and Vulkan](https://www.reddit.com/r/MachineLearning/comments/1v9s4mz/vendoragnostic_ml_inference_on_production_edge/) ⭐️ 8.0/10

PostSlate, a video editing tool, uses ncnn with its Vulkan backend to run ML models on production edge devices, achieving up to 10x speedup over ONNX CPU inference while avoiding vendor-specific runtimes like CUDA. This approach enables cross-platform ML inference without requiring users to install vendor-specific drivers or runtimes, simplifying deployment across diverse GPU hardware (NVIDIA, AMD, Intel, Apple Silicon) in production environments. On an NVIDIA 4070 with fp16, ArcFace R50 face embedding runs in 3 ms (vs. 30 ms on ONNX CPU), and SCRFD face detection runs in 2.5 ms (vs. 25 ms). Model size also reduces from 174 MB (ONNX fp32) to 87 MB (ncnn fp16).

reddit · r/MachineLearning · /u/ppchaos · Jul 29, 10:22

**Background**: ncnn is a high-performance neural network inference framework developed by Tencent, designed for mobile and edge platforms. It supports CPU and Vulkan GPU backends without third-party runtime dependencies. The Vulkan API is a cross-platform graphics and compute standard that provides low-level GPU access, making it suitable for vendor-agnostic ML acceleration.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/Tencent/ncnn">Tencent/ ncnn : ncnn is a high-performance neural network inference ...</a></li>
<li><a href="https://www.phoronix.com/news/NVIDIA-Vulkan-AI-ML-Success">NVIDIA Is Finding Great Success With Vulkan Machine Learning ...</a></li>

</ul>
</details>

**Tags**: `#ML inference`, `#Vulkan`, `#edge devices`, `#ncnn`, `#cross-platform`

---

<a id="item-9"></a>
## [Hugging Face Widely Abused for Deepfake Nude Images](https://www.theverge.com/ai-artificial-intelligence/971723/hugging-face-nudify-deepfake-undress-women-children) ⭐️ 8.0/10

A report by AI Forensics reveals that Hugging Face's platform is being extensively exploited to generate non-consensual deepfake nude images, with 73% of requests being sexual and 7% targeting children. This highlights serious ethical and safety gaps in open-source AI platforms, potentially leading to widespread abuse and harm, especially to vulnerable groups, and calls for stronger content moderation and platform responsibility. The report used a honeypot that received over 1,000 requests in 7 days, and found that 7 out of the top 9 image editing models could easily undress women with simple prompts without needing elaborate jailbreaks.

telegram · zaihuapd · Jul 29, 08:20

**Background**: Hugging Face is a popular open-source platform for hosting and sharing machine learning models, widely used by developers. Deepfake refers to synthetic media created using AI to manipulate images or videos, often used maliciously to create non-consensual pornographic content. The report underscores the lack of adequate safeguards on such platforms.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hugging_Face">Hugging Face</a></li>
<li><a href="https://en.wikipedia.org/wiki/Deepfake">Deepfake</a></li>

</ul>
</details>

**Tags**: `#AI Ethics`, `#Deepfake`, `#Hugging Face`, `#Content Moderation`, `#AI Safety`

---

<a id="item-10"></a>
## [Moonshot AI seeks $2B funding at $30B valuation](https://t.me/zaihuapd/42845) ⭐️ 8.0/10

Moonshot AI, the developer of the Kimi chatbot, is seeking up to $2 billion in new funding at a $30 billion valuation, its third funding round in six months. This rapid valuation growth and strong revenue indicate that Chinese AI startups are gaining significant traction, challenging global competitors and attracting large investments. The company's annual recurring revenue (ARR) surpassed $200 million in April, and it has launched a general AI agent called Kimi Work while preparing for a Hong Kong IPO.

telegram · zaihuapd · Jul 29, 10:12

**Background**: Annual Recurring Revenue (ARR) is a key metric for subscription-based businesses, representing the predictable revenue expected per year. General AI agents are AI systems that can perform a wide variety of tasks autonomously, distinguishing them from specialized chatbots.

<details><summary>References</summary>
<ul>
<li><a href="https://www.lightercapital.com/blog/what-is-arr-annual-recurring-revenue-definition-formula">What is Annual Recurring Revenue ( ARR ) in SaaS ?</a></li>
<li><a href="https://www.ibm.com/think/topics/ai-agents">What Are AI Agents ? | IBM</a></li>

</ul>
</details>

**Tags**: `#AI startup`, `#funding`, `#Moonshot AI`, `#Kimi chatbot`, `#valuation`

---

<a id="item-11"></a>
## [China Drafts Anti-Cyberbullying Law Targeting AI-Generated Abuse](https://mp.weixin.qq.com/s/PrzKFhbwjgFEGBPADvFD6Q) ⭐️ 8.0/10

On July 29, 2026, China's Cyberspace Administration released a draft anti-cyberbullying law for public consultation, which includes specific provisions to regulate the use of AI technology to create and spread cyberbullying content. This marks one of the first major legal frameworks globally to explicitly address AI-generated cyberbullying, setting a precedent for online governance and AI regulation. It could impact how platforms deploy AI tools and how victims seek legal recourse. The draft consists of 60 articles across seven chapters, defining cyberbullying as online infringement on reputation, privacy, portrait rights, and personal information. It imposes platform responsibilities for monitoring and protection, and introduces judicial measures such as injunctions and mental damage compensation.

telegram · zaihuapd · Jul 29, 10:59

**Background**: Cyberbullying has become widespread on Chinese social media, and AI tools like deepfakes can amplify harm. Chinese authorities have been strengthening online content regulation; this draft law extends existing protections to specifically cover AI-generated abuse. Technical detection methods, such as machine learning and deepfake detection, are relevant to enforcement.

<details><summary>References</summary>
<ul>
<li><a href="https://www.igi-global.com/chapter/ai-based-cyberbullying-detection-techniques-and-strategies/369055">AI -Based Cyberbullying Detection Techniques and Strategies</a></li>
<li><a href="https://journal.ut.ac.ir/article_99050_7cf51958e1c400d52e8a8e52372bee45.pdf">Artificial Intelligence-Driven Cyberbullying Detection : A Survey of</a></li>
<li><a href="https://danaya.tech/seo/deepfake-detection/social-media">Deepfake Detection for Social Media | Danaya</a></li>

</ul>
</details>

**Tags**: `#AI regulation`, `#cyberbullying`, `#China law`, `#online governance`

---

<a id="item-12"></a>
## [OpenAI gives 100,000 researchers free access to GPT-5.6](https://openai.com/index/chatgpt-for-academic-researchers/) ⭐️ 8.0/10

OpenAI announced on July 29, 2026, the launch of ChatGPT for Academic Researchers, a program that will provide 100,000 academic researchers worldwide with free access to its frontier GPT-5.6 models by 2027, with the first 10,000 slots opening this summer. This initiative could dramatically accelerate scientific discovery across multiple disciplines by removing cost barriers, enabling researchers to leverage cutting-edge AI for tasks like genomic analysis, protein modeling, and literature review with a $250M investment. Eligible researchers at degree-granting institutions can invite up to 4 institutional collaborators, and the workspace default does not use data for model training; applicants must verify their institutional affiliation and submit a research plan.

telegram · zaihuapd · Jul 30, 00:17

**Background**: GPT-5.6, released in July 2026, is OpenAI's strongest cybersecurity and scientific reasoning model, achieving state-of-the-art results in coding, knowledge work, and science while being more efficient. The program is part of OpenAI's broader commitment to invest over $250M in external research by 2027.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/chatgpt-for-academic-researchers/">Accelerating scientific discovery with ChatGPT for Academic ...</a></li>
<li><a href="https://www.axios.com/2026/07/29/openai-academics-research-chatgpt-sol">OpenAI launches free AI access program for academic researchers</a></li>
<li><a href="https://openai.com/index/gpt-5-6/">GPT‑5.6: Frontier intelligence that scales with your ambition</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#AI for Science`, `#Academic Research`, `#GPT-5`, `#Funding`

---