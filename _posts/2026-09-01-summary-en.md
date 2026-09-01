---
layout: default
title: "Horizon Summary: 2026-09-01 (EN)"
date: 2026-09-01
lang: en
---

> From 35 items, 5 important content pieces were selected

---

1. [Google Removes MV2 Extensions, Including uBlock Origin, from Chrome Web Store](#item-1) ⭐️ 8.0/10
2. [Sliding-Window Attention with Sinks Outperforms Linear Attention on Long-Context Reasoning](#item-2) ⭐️ 8.0/10
3. [OpenClaw 2.0 Released: Massive Update with 16,000+ Pull Requests](#item-3) ⭐️ 8.0/10
4. [Apple Names John Ternus CEO; Tim Cook Becomes Executive Chairman](#item-4) ⭐️ 8.0/10
5. [DeepSeek Releases Vision-Language Model deepseek-v4-flash-vision-exp on API](#item-5) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Google Removes MV2 Extensions, Including uBlock Origin, from Chrome Web Store](https://webiterate.dev/google-removed-extensions-ublock-origin-108/) ⭐️ 8.0/10

Google has removed all remaining Manifest V2 extensions from the Chrome Web Store, including the popular ad blocker uBlock Origin. The removal follows the official deprecation timeline, and starts taking effect for the majority of users. This change severely undermines effective ad blocking and privacy protection in Chrome because Manifest V3 limits extensions' abilities to inspect and block network requests. Millions of users who rely on extensions like uBlock Origin for safety and a cleaner browsing experience are directly affected. Manifest V2 extensions installed on Chrome 138 or earlier remain installed but can no longer receive updates or be reinstalled once removed. Under Manifest V3, ad blockers are limited to 30,000 rules, whereas effective blockers often need 300,000 or more, and they must use declarativeNetRequest instead of the more capable WebRequest API.

hackernews · twapi · Aug 31, 21:10 · [Discussion](https://news.ycombinator.com/item?id=49514878)

**Background**: Chrome extensions use a manifest file to declare their capabilities. Manifest V2 allowed extensions like uBlock Origin to use the WebRequest API to intercept and block network requests in real time. Manifest V3, introduced in 2020, moves background scripts to service workers and replaces WebRequest with declarativeNetRequest, which is less flexible but designed to improve performance and security. Google has been phasing out Manifest V2 for years, and the final removal from the Chrome Web Store is scheduled for July 8, 2026.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.chrome.com/docs/extensions/develop/migrate/mv2-deprecation-timeline">Manifest V2 support timeline | Chrome for Developers</a></li>
<li><a href="https://developer.chrome.com/docs/extensions/develop/migrate/what-is-mv3">Extensions / Manifest V3 | Chrome for Developers</a></li>
<li><a href="https://nordvpn.com/blog/manifest-v3-ad-blockers/">Is Google's Manifest V3 the end of ad blockers? | NordVPN</a></li>

</ul>
</details>

**Discussion**: Commenters overwhelmingly criticize Google's move, with many stating they have already switched to Firefox or will do so. Several highlight that ad blocking is a safety issue, particularly for older or less tech-savvy users who may fall for malicious ads, and view Firefox as the only real alternative.

**Tags**: `#Chrome`, `#Manifest V3`, `#uBlock Origin`, `#Ad Blocking`, `#Browser Extensions`

---

<a id="item-2"></a>
## [Sliding-Window Attention with Sinks Outperforms Linear Attention on Long-Context Reasoning](https://www.reddit.com/r/MachineLearning/comments/1w3j1vw/slidingwindow_attention_beats_linear_on/) ⭐️ 8.0/10

A new arXiv preprint by Alexia Jolicoeur-Martineau and colleagues reports that Sliding Window Attention (SWA) with attention sinks matches or outperforms post-trained linear attention models on long-context reasoning tasks. On the Needle-in-a-Haystack and BABILong benchmarks, SWA achieves 2 to 10 times higher performance than linear attention variants. This finding challenges the prevailing linear-attention paradigm in efficient LLM deployment, which often relies on costly post-training. It suggests that a simple, untrained baseline like SWA with sinks could redirect research focus and practical recommendations for long-context models. The paper argues that prior comparisons of post-trained linear models were not benchmarked against proper baselines. The authors state that linear attention models likely require training from scratch or extensive post-training to match SWA, and they recommend switching to SWA instead.

reddit · r/MachineLearning · /u/Justgototheeffinmoon · Aug 31, 16:35

**Background**: Standard softmax attention has quadratic computational cost with sequence length, making long-context inference expensive. Linear attention variants reduce this cost but often require additional training to preserve quality. Sliding window attention (SWA) limits each token's attention to a local window, and attention sinks are special tokens that stabilize attention by absorbing excess focus. BABILong is a benchmark that uses a needle-in-a-haystack setup to test reasoning across long documents.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2608.28444v1">Sliding - window beats linear attention</a></li>
<li><a href="https://carnotresearch.medium.com/let-the-chaos-sink-in-481c8a37471e">Let the Chaos Sink In. Balancing attention in transformers | Medium</a></li>
<li><a href="https://github.com/booydar/babilong">GitHub - booydar/babilong: BABILong is a benchmark for LLM evaluation using the needle-in-a-haystack approach. · GitHub</a></li>

</ul>
</details>

**Tags**: `#attention mechanisms`, `#long-context reasoning`, `#LLM efficiency`, `#linear attention`, `#arXiv preprint`

---

<a id="item-3"></a>
## [OpenClaw 2.0 Released: Massive Update with 16,000+ Pull Requests](https://openclaw.ai/blog/openclaw-2-accidentally) ⭐️ 8.0/10

OpenClaw released version 2.0 on August 30, its largest update ever, incorporating over 16,000 pull requests from 933 contributors, including 569 first-time participants. The update overhauls installation, messaging, memory, skills, models, browser, plugins, and security, and adds shared cloud sessions for multi-user collaboration. This release represents a major milestone for one of the most active open-source AI agent projects, demonstrating the strength of community-led development. The sheer scale of contributions — roughly half of the project's total pull requests — signals a maturing ecosystem and may push competition in the autonomous agent space. The team deliberately paused new versions for nearly seven weeks to consolidate the changes. Simplified installation, a rebuilt browser experience, and shared cloud sessions for real-time collaboration are among the headline features.

telegram · zaihuapd · Aug 31, 04:38

**Background**: OpenClaw is a free and open-source autonomous AI agent that executes tasks using large language models (LLMs) through messaging platforms as its main interface. It runs locally on the user's machine and works from chat apps users already have, lowering the barrier to AI automation. Pull requests are a standard way for developers to propose and merge code changes in collaborative software projects, and the 16,000+ PRs here represent a vast array of improvements from the community.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenClaw">OpenClaw - Wikipedia</a></li>
<li><a href="https://openclaw.ai/">OpenClaw — Open -Source AI Assistant</a></li>

</ul>
</details>

**Tags**: `#OpenClaw`, `#release`, `#open-source`, `#AI`, `#major-update`

---

<a id="item-4"></a>
## [Apple Names John Ternus CEO; Tim Cook Becomes Executive Chairman](https://t.me/zaihuapd/43516) ⭐️ 8.0/10

Apple has announced a leadership transition in which CEO Tim Cook will step down and become executive chairman of the board, with hardware engineering senior vice president John Ternus taking over as CEO on September 1, 2026. The board unanimously approved the plan, and Cook will remain CEO through the summer to complete the handover. This is Apple's first CEO transition since Tim Cook took the role in 2011, marking a new era for one of the world's most valuable companies. Ternus, a long-time hardware executive, signals continuity in product-focused leadership, but his appointment still carries significant implications for Apple's future product direction and corporate strategy. John Ternus joined Apple in 2001, became vice president of hardware engineering in 2013, and joined the executive team in 2021; he has been responsible for iPhone, Mac, iPad, and AirPods hardware. Current chairman Arthur Levinson will become lead independent director on September 1, and Ternus will join the board on the same day.

telegram · zaihuapd · Aug 31, 10:21

**Background**: The CEO position at Apple has changed only a few times in its history; Tim Cook succeeded Steve Jobs in 2011 after serving as chief operating officer, leading the company through major product launches and service expansions. In a corporate board structure, an executive chairman typically oversees board activities while remaining involved in company leadership, while the CEO manages day-to-day operations. John Ternus has been a central figure in Apple's hardware development for years, but this move makes him only the fourth CEO in Apple's history.

**Tags**: `#Apple`, `#Leadership`, `#CEO`, `#Tech Industry`

---

<a id="item-5"></a>
## [DeepSeek Releases Vision-Language Model deepseek-v4-flash-vision-exp on API](https://t.me/zaihuapd/43518) ⭐️ 8.0/10

DeepSeek has launched an experimental vision-language model, deepseek-v4-flash-vision-exp, on its API as of August 21, 2026, with official documentation and pricing already updated. The model accepts both images and text, enabling tasks such as image description, text extraction from screenshots, and chart analysis. This release marks DeepSeek's entry into multimodal AI serving, allowing developers to build vision-powered applications without relying on proprietary rivals like GPT-4V, Gemini, or Claude. By offering an experimental vision model with API access, DeepSeek strengthens its position in the increasingly competitive AI infrastructure market. The model can be accessed through Chat Completions, Responses, and the Anthropic-compatible Messages API, with images supplied via URL, Base64, or file upload. According to DeepSeek, deepseek-v4-flash-vision-exp shows substantial improvements in multimodal agent tasks compared to DeepSeek-V4-Flash-0731, while maintaining comparable performance on text-only agent tasks.

telegram · zaihuapd · Aug 31, 11:41

**Background**: A vision-language model (VLM) is an AI system that jointly interprets and generates information from both images and text, extending large language models (LLMs) that handle only text. OpenAI introduced computer vision to ChatGPT via GPT-4V, and similar capabilities later appeared in Google Gemini, Anthropic Claude, and Microsoft Copilot. DeepSeek, a leading AI lab, has been releasing open-weight models and API services, and this new experimental vision model adds multimodal capabilities to its lineup.

<details><summary>References</summary>
<ul>
<li><a href="https://api-docs.deepseek.com/guides/vision/?ref=upstract.com">Vision | DeepSeek API Docs</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash-Vision-Exp">deepseek-ai/ DeepSeek - V 4 - Flash - Vision - Exp · Hugging Face</a></li>
<li><a href="https://en.wikipedia.org/wiki/Vision-language_model">Vision-language model</a></li>

</ul>
</details>

**Tags**: `#deepseek`, `#api`, `#vision`, `#language-model`, `#ai`

---