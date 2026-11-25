<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_system_banner_dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_system_banner_light.svg">
    <img alt="Cyto System — Beijing Zhongguancun Academy & BGI Research" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_system_banner_light.svg" width="84%">
  </picture>
</p>

<h1 align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg">
    <img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="28" align="absmiddle">
  </picture>
  &nbsp;Cyto Model Family
</h1>

<p align="center">
  <strong>English</strong> &nbsp;|&nbsp; <a href="https://github.com/Cyto-System/.github/blob/main/profile/README_zh.md">简体中文</a>
</p>

<p align="center">
  <strong>Jointly developed by Beijing Zhongguancun Academy &amp; BGI Research</strong><br>
  <sub>Building modular, verifiable, and practical computational models for spatiotemporal cell simulation and cellular response prediction.</sub>
</p>

<p align="center">
  <a href="https://cyto-system.github.io"><img src="https://img.shields.io/badge/Website-cyto--system.github.io-059669.svg" alt="Cyto Website"></a>
  <a href="https://github.com/Cyto-System"><img src="https://img.shields.io/badge/Organization-Cyto%20System-2f7d68.svg" alt="Cyto System"></a>
  <a href="https://github.com/Cyto-System"><img src="https://img.shields.io/badge/Institution-Beijing%20Zhongguancun%20Academy%20%7C%20BGI%20Research-2f7d68.svg" alt="Beijing Zhongguancun Academy | BGI Research"></a>
</p>

---

## About the Cyto Family

**Cyto** is a family of spatiotemporal cell models jointly developed by **Beijing Zhongguancun Academy** and **BGI Research**. Rather than treating cellular modeling as a single opaque black box, **Cyto System** organizes spatiotemporal cell capabilities into focused, composable modules with explicit biological grounding, leak-free evaluation protocols, and lightweight deployment.

Our core design principles:

- **Biology-Grounded Modeling**: Explicitly combine curated biological priors with high-throughput single-cell measurements so models isolate perturbation- and state-specific signals instead of memorizing gene-level baseline biases.
- **Rigorous & Leak-Free Benchmarking**: Evaluate on strictly held-out perturbations, cell lines, and compounds using fine-grained discrimination metrics (such as within-gene balanced accuracy and orthogonal MSE decomposition).
- **Accessible & Reproducible Compute**: Deliver compact, integrity-verified checkpoints and transparent inference pipelines that run reliably in standard research environments—including CPU-only workstations.

---

## Model Family & Repositories

| Module | Method | Scope | Repository & Resources |
| :--- | :--- | :--- | :--- |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **Cyto.Genome** | **Genome-to-Expression Foundation** | Genomic sequence and cis-regulatory modeling from DNA sequence to cell-type-specific molecular expression | Open-sourcing soon |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **[Cyto.Spatial](https://github.com/Cyto-System/SUDOKU)** | **SUDOKU** (Generative Spatial Foundation) | Cross-slice spatial transcriptomics niche representation, multi-scale clustering, and masked cell-state generation | [GitHub (SUDOKU)](https://github.com/Cyto-System/SUDOKU) |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **[Cyto.Identity](https://github.com/Cyto-System/Cyto.Identity)** | **scVerity** (Evidence-Grounded Reasoning) | Open-world single-cell annotation, ontology-grounded verification, and rare-lineage discovery | [GitHub (Cyto.Identity)](https://github.com/Cyto-System/Cyto.Identity) |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **[Cyto.Perturbation](https://github.com/Cyto-System/Cyto.Perturbation)** | **RELAY** (Anchored Dense Response Contrast Transfer) | Same-cell unseen genetic & drug perturbations, plus zero-shot cross-cell perturbation transfer (CPU-only) | [GitHub (Cyto.Perturbation)](https://github.com/Cyto-System/Cyto.Perturbation) · [Hugging Face](https://huggingface.co/KassdinZheng/Cyto.Perturbation) |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **[Cyto.CoScientist](https://github.com/Cyto-System/Cyto.CoScientist)** | **Within-Task RSI** (Evidence-Gated Autonomous Research) | Autonomous hypothesis refinement, multi-branch candidate evolution, and auditable multi-omics workflows | [GitHub (Cyto.CoScientist)](https://github.com/Cyto-System/Cyto.CoScientist) |

<sub>Additional modules in the Cyto model family will be added to this index as they are open-sourced.</sub>

---

## Institutions

**Cyto System** is jointly developed by:
- **Beijing Zhongguancun Academy**
- **BGI Research**
