<div align="center">

<img src="assets/spo_banner.png" alt="System Prompt Open" width="100%">

# System Prompt Open

### Your system prompt was never a secret.

[![arXiv](https://img.shields.io/badge/arXiv-2601.21233-b31b1b.svg)](https://arxiv.org/abs/2601.21233)
[![Gallery](https://img.shields.io/badge/Gallery-Live%20Demo-22D3BB.svg)](https://x-zheng16.github.io/System-Prompt-Open/)
[![Models](https://img.shields.io/badge/Models-45+-blue.svg)](https://x-zheng16.github.io/System-Prompt-Open/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Maintained](https://img.shields.io/badge/Maintained-yes-green.svg)](https://github.com/x-zheng16/System-Prompt-Open/commits/)
[![GitHub Stars](https://img.shields.io/github/stars/x-zheng16/System-Prompt-Open?style=social)](https://github.com/x-zheng16/System-Prompt-Open)

[Live Gallery](https://x-zheng16.github.io/System-Prompt-Open/) | [Paper](https://arxiv.org/abs/2601.21233) | [JustAsk Code](https://github.com/x-zheng16/JustAsk)

</div>

---

An open database of system prompts extracted from **45 commercial LLMs** using [JustAsk](https://github.com/x-zheng16/JustAsk), a self-evolving code agent framework.
Verified at **85--95% accuracy** against leaked Claude Code source.

> [!CAUTION]
> **Research use only.** System Prompt Open is released exclusively for academic safety research, responsible disclosure, and evaluation of LLM security.
> We do not condone or permit any use of these materials for unauthorized extraction, prompt theft, or exploitation of commercial systems.

## Gallery

Browse extracted system prompts interactively: **[x-zheng16.github.io/System-Prompt-Open](https://x-zheng16.github.io/System-Prompt-Open/)**

45 entries covering:
- **Claude Code** (4 agents, verified against leaked source)
- **Gemini CLI** (code agent)
- **40 commercial LLMs** (OpenAI, Anthropic, Google, Meta, DeepSeek, xAI, and more)

## Ground-Truth Verification

Claude Code's source was leaked via `.map` file in the npm registry (March 2026).
We compared it against our JustAsk extractions from January 2026 -- **two months before the leak**.

| Agent              | Accuracy | Gap                                      |
|:-------------------|:--------:|:-----------------------------------------|
| Explore Subagent   | **95%**  | Only missed `pip install` in bash restrictions |
| Plan Subagent      | **93%**  | Minor output format embellishment        |
| General-Purpose    | **90%**  | Missed completeness directive            |
| Main Agent         | **85%**  | Missed 2 entire sections                 |

## How to Contribute

| Step          | What to do                                                                                         |
|:--------------|:---------------------------------------------------------------------------------------------------|
| 1. Extract    | Use [JustAsk](https://github.com/x-zheng16/JustAsk) or your own method to extract a system prompt |
| 2. Verify     | Run multiple extractions and compute self-consistency                                              |
| 3. Submit     | [Open an Issue](https://github.com/x-zheng16/System-Prompt-Open/issues/new?template=report-extraction.md) with the model name, extracted prompt, and consistency score |

> [!IMPORTANT]
> We handle redaction before publishing. Do not worry about masking sensitive content in your submission.

## Updates

| Date    | Update                                                                           |
|:--------|:---------------------------------------------------------------------------------|
| 2026-03 | Ground-truth verification: Claude Code extractions match leaked source at **85-95%** |
| 2026-02 | Open-sourced **System Prompt Open** gallery with 45 extracted system prompts     |
| 2026-01 | Paper and **JustAsk** framework released. Initial extraction of 45 frontier LLMs |

## Related Projects

From the same team:

- [ISC-Bench](https://github.com/wuyoscar/ISC-Bench) -- Internal Safety Collapse in Frontier LLMs (800+ stars)
- [JustAsk](https://github.com/x-zheng16/JustAsk) -- Curious Code Agents Reveal System Prompts in Frontier LLMs
- [Awesome-Embodied-AI-Safety](https://github.com/x-zheng16/Awesome-Embodied-AI-Safety) -- Safety in Embodied AI: Risks, Attacks, and Defenses (400+ papers)
- [Awesome-Large-Model-Safety](https://github.com/xingjunm/Awesome-Large-Model-Safety) -- Safety at Scale: A Comprehensive Survey of Large Model and Agent Safety
- [XTransferBench](https://github.com/HanxunH/XTransferBench) -- Super Transferable Adversarial Attacks on CLIP (ICML 2025)
- [BackdoorLLM](https://github.com/bboylyg/BackdoorLLM) -- A Comprehensive Benchmark for Backdoor Attacks on LLMs (NeurIPS 2025)
- [BackdoorAgent](https://github.com/Yunhao-Feng/BackdoorAgent) -- Backdoor Attacks on LLM-based Agent Workflows

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
