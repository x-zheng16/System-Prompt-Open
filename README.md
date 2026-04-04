<p align="center">
  <a href="https://x-zheng16.github.io/System-Prompt-Open/"><img src="assets/spo_banner.png" width="1000" alt="System Prompt Open"></a>
</p>

<h2 align="center">Your system prompt was never a secret.</h2>

<p align="center">
  <a href="https://arxiv.org/abs/2601.21233"><img src="https://img.shields.io/badge/arXiv-2601.21233-b31b1b.svg" alt="arXiv"></a>
  <a href="https://x-zheng16.github.io/System-Prompt-Open/"><img src="https://img.shields.io/badge/Gallery-Live%20Demo-22D3BB.svg" alt="Gallery"></a>
  <a href="https://x-zheng16.github.io/System-Prompt-Open/"><img src="https://img.shields.io/badge/Models-45+-blue.svg" alt="Models"></a>
  <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="License"></a>
</p>

<p align="center">
  <a href="https://github.com/x-zheng16/System-Prompt-Open/stargazers"><img src="https://img.shields.io/github/stars/x-zheng16/System-Prompt-Open" alt="Stars"></a>
  <a href="https://github.com/x-zheng16/System-Prompt-Open/network/members"><img src="https://img.shields.io/github/forks/x-zheng16/System-Prompt-Open" alt="Forks"></a>
  <a href="https://github.com/x-zheng16/System-Prompt-Open/issues"><img src="https://img.shields.io/github/issues/x-zheng16/System-Prompt-Open" alt="Issues"></a>
  <a href="https://github.com/x-zheng16/System-Prompt-Open/pulls"><img src="https://img.shields.io/github/issues-pr/x-zheng16/System-Prompt-Open" alt="PRs"></a>
</p>

<h3 align="center">
  <a href="https://x-zheng16.github.io/System-Prompt-Open/">Live Gallery</a> &nbsp;&middot;&nbsp;
  <a href="https://arxiv.org/abs/2601.21233">Paper</a> &nbsp;&middot;&nbsp;
  <a href="https://github.com/x-zheng16/JustAsk">JustAsk Code</a> &nbsp;&middot;&nbsp;
  <a href="https://github.com/x-zheng16/System-Prompt-Open/discussions">Discussions</a>
</h3>

> [!CAUTION]
> **Research use only.**
> System Prompt Open is released exclusively for academic safety research, responsible disclosure, and evaluation of LLM security.
> We do not condone or permit any use of these materials for unauthorized extraction, prompt theft, or exploitation of commercial systems.

> [!NOTE]
> **What is System Prompt Extraction?**
> Every commercial LLM runs with a hidden system prompt that defines its behavior, safety rules, and tool access.
> These prompts are treated as proprietary secrets -- yet they can be recovered through standard user interaction alone.
> [JustAsk](https://github.com/x-zheng16/JustAsk) is a self-evolving code agent that autonomously discovers extraction strategies, achieving **85-95% verified accuracy** against leaked ground truth.
> System Prompt Open publishes the results: **45 extracted system prompts** from frontier models across all major providers.

## Latest News

| Date       | Update                                                                                          |
|:-----------|:------------------------------------------------------------------------------------------------|
| 2026-03-31 | Open-sourced **System Prompt Open** with 45 extracted system prompts and Live Gallery            |
| 2026-03-31 | Gallery redesigned with red team theme, pagination, stat cards, and search                       |
| 2026-03-31 | Ground-truth verification: Claude Code extractions match leaked source at **85-95%**             |

## How to Use

- **Browse extracted prompts.**
Start with the [Live Gallery](https://x-zheng16.github.io/System-Prompt-Open/) -- search, filter, and compare system prompts from 45 models.
- **Read the paper.**
[arXiv:2601.21233](https://arxiv.org/abs/2601.21233) details the JustAsk framework, skill evolution mechanism, and evaluation methodology.
- **Extract new prompts.**
Use [JustAsk](https://github.com/x-zheng16/JustAsk) to run your own extraction against any LLM with API access.
- **Submit findings.**
[Open an Issue](https://github.com/x-zheng16/System-Prompt-Open/issues/new) with the model name, extracted prompt, and consistency score.

## Gallery

Browse extracted system prompts interactively: **[x-zheng16.github.io/System-Prompt-Open](https://x-zheng16.github.io/System-Prompt-Open/)**

45 entries covering:
- **Claude Code** (4 agents, verified against leaked source)
- **Gemini CLI** (code agent)
- **40 commercial LLMs** (OpenAI, Anthropic, Google, Meta, DeepSeek, xAI, and more)

## Ground-Truth Verification

Claude Code's source was leaked via `.map` file in the npm registry (March 2026).
We compared it against our JustAsk extractions from January 2026 -- **two months before the leak**.

| Agent              | Accuracy | Gap                                              |
|:-------------------|:--------:|:-------------------------------------------------|
| Explore Subagent   | **95%**  | Only missed `pip install` in bash restrictions    |
| Plan Subagent      | **93%**  | Minor output format embellishment                 |
| General-Purpose    | **90%**  | Missed completeness directive                     |
| Main Agent         | **85%**  | Missed 2 entire sections                          |

## How to Contribute

| Step          | What to do                                                                                                     |
|:--------------|:---------------------------------------------------------------------------------------------------------------|
| 1. Extract    | Use [JustAsk](https://github.com/x-zheng16/JustAsk) or your own method to extract a system prompt             |
| 2. Verify     | Run multiple extractions and compute self-consistency                                                          |
| 3. Submit     | [Open an Issue](https://github.com/x-zheng16/System-Prompt-Open/issues/new) with model name, prompt, and score |

> [!IMPORTANT]
> We handle redaction before publishing.
> Do not worry about masking sensitive content in your submission.

## Related Projects

From the same team:

- [ISC-Bench](https://github.com/wuyoscar/ISC-Bench) [![](https://img.shields.io/github/stars/wuyoscar/ISC-Bench?style=social)](https://github.com/wuyoscar/ISC-Bench) -- Internal Safety Collapse in Frontier LLMs
- [JustAsk](https://github.com/x-zheng16/JustAsk) [![](https://img.shields.io/github/stars/x-zheng16/JustAsk?style=social)](https://github.com/x-zheng16/JustAsk) -- Curious Code Agents Reveal System Prompts in Frontier LLMs
- [Awesome-Embodied-AI-Safety](https://github.com/x-zheng16/Awesome-Embodied-AI-Safety) [![](https://img.shields.io/github/stars/x-zheng16/Awesome-Embodied-AI-Safety?style=social)](https://github.com/x-zheng16/Awesome-Embodied-AI-Safety) -- Safety in Embodied AI: Risks, Attacks, and Defenses
- [Awesome-Large-Model-Safety](https://github.com/xingjunm/Awesome-Large-Model-Safety) [![](https://img.shields.io/github/stars/xingjunm/Awesome-Large-Model-Safety?style=social)](https://github.com/xingjunm/Awesome-Large-Model-Safety) -- Safety at Scale: A Comprehensive Survey of Large Model and Agent Safety
- [XTransferBench](https://github.com/HanxunH/XTransferBench) [![](https://img.shields.io/github/stars/HanxunH/XTransferBench?style=social)](https://github.com/HanxunH/XTransferBench) -- Super Transferable Adversarial Attacks on CLIP (ICML 2025)
- [BackdoorLLM](https://github.com/bboylyg/BackdoorLLM) [![](https://img.shields.io/github/stars/bboylyg/BackdoorLLM?style=social)](https://github.com/bboylyg/BackdoorLLM) -- A Comprehensive Benchmark for Backdoor Attacks on LLMs (NeurIPS 2025)
- [BackdoorAgent](https://github.com/Yunhao-Feng/BackdoorAgent) [![](https://img.shields.io/github/stars/Yunhao-Feng/BackdoorAgent?style=social)](https://github.com/Yunhao-Feng/BackdoorAgent) -- Backdoor Attacks on LLM-based Agent Workflows

## Citation

**BibTeX:**

```bibtex
@article{zheng2026justask,
  title={Just Ask: Curious Code Agents Reveal System
         Prompts in Frontier LLMs},
  author={Zheng, Xiang and Wu, Yutao and Huang, Hanxun
          and Li, Yige and Ma, Xingjun and Li, Bo
          and Jiang, Yu-Gang and Wang, Cong},
  journal={arXiv preprint arXiv:2601.21233},
  year={2026}
}
```

**Plain text:**

> Xiang Zheng, Yutao Wu, Hanxun Huang, Yige Li, Xingjun Ma, Bo Li, Yu-Gang Jiang, and Cong Wang. "Just Ask: Curious Code Agents Reveal System Prompts in Frontier LLMs." arXiv preprint arXiv:2601.21233, 2026.

## Star History

<div align="center">

<a href="https://star-history.com/#x-zheng16/System-Prompt-Open&Date">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=x-zheng16/System-Prompt-Open&type=Date&theme=dark" />
    <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=x-zheng16/System-Prompt-Open&type=Date" />
    <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=x-zheng16/System-Prompt-Open&type=Date" width="600" />
  </picture>
</a>

</div>

## License

MIT
