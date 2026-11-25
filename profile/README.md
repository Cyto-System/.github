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

**Cyto** is a family of spatiotemporal cell models jointly developed by **Beijing Zhongguancun Academy** and **BGI Research**.

Cyto comprises seven submodels that represent cellular state, support perturbation, and capture changes over time. Six models form two complementary axes of cellular description, while **Cyto.CoScientist** integrates evidence across both axes to advance biological discovery.

> [!IMPORTANT]
> ### Cyto.CoScientist · Scientific Discovery Coordination Layer
>
> **Cyto.CoScientist** integrates evidence from the two axes into testable biological hypotheses. It supports the design and interpretation of perturbation experiments, then uses their outcomes to refine the next round of inquiry.

| Axis | Scientific role | Models and progression |
| :--- | :--- | :--- |
| **Spatial axis** | Integrates molecular regulation, single-cell multi-omics, and tissue-scale spatial context | **Cyto.Genome** (molecular regulation) → **Cyto.Multiomics** (single-cell multi-omics) → **Cyto.Spatial** (tissue microenvironment / niche) |
| **Temporal axis** | Relates current cell identity to natural trajectories and perturbation responses | **Cyto.Identity** (current identity) → **Cyto.Dynamics** (natural trajectory) → **Cyto.Perturbation** (counterfactual response to intervention) |

Together, the two axes provide a multiscale description of cellular state. The framework connects two complementary lines of inquiry: evidence generation and translational application.

**Evidence generation.** An active-learning procedure guided by reinforcement learning identifies where model uncertainty is greatest and prioritizes measurements that can resolve it. New measurements update the relevant models, forming an iterative cycle between computational prediction and experimental validation.

**Translational application.** Cyto addresses spatiotemporal pathology, complex disease cohorts, and drug discovery. Shared benchmarks provide a common basis for comparison and evaluation.

---

## Model Family & Repositories

| Module | Method | Scope | Repository & Resources |
| :--- | :--- | :--- | :--- |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **[Cyto.Spatial](https://github.com/Cyto-System/Cyto.Spatial)** | **SUDOKU** (Spatial Discrete Denoising) | Unified cell and tissue-niche representation and spatial cell-state generation from spatial transcriptomics; cross-section niche retrieval, multi-scale clustering, and immune-recruitment prediction | [GitHub (Cyto.Spatial)](https://github.com/Cyto-System/Cyto.Spatial) |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **[Cyto.Identity](https://github.com/Cyto-System/Cyto.Identity)** | **scVerity** (Evidence-Grounded Reasoning) | Cell identity and state annotation across unseen cell types, sibling subtypes, and rare lineages, with query-sample molecular evidence, ontology constraints, and multimodal validation | [GitHub (Cyto.Identity)](https://github.com/Cyto-System/Cyto.Identity) |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **[Cyto.Perturbation](https://github.com/Cyto-System/Cyto.Perturbation)** | **RELAY** (Anchored Dense Response Contrast Transfer) | Same-cell unseen genetic & drug perturbations, plus zero-shot cross-cell perturbation transfer | [GitHub (Cyto.Perturbation)](https://github.com/Cyto-System/Cyto.Perturbation) · [Hugging Face](https://huggingface.co/KassdinZheng/Cyto.Perturbation) |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **[Cyto.CoScientist](https://github.com/Cyto-System/Cyto.CoScientist)** | **Within-Task Recursive Self-Improvement (RSI)** | Long-horizon autonomous biological research across bioinformatics algorithm development and open-ended multi-omics inquiry | [GitHub (Cyto.CoScientist)](https://github.com/Cyto-System/Cyto.CoScientist) |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **Cyto.Genome** | **Genome-to-Multi-Omics Foundation** | Cell-type-specific multi-omics track prediction and modality completion from DNA sequence to molecular expression | Open-sourcing soon |

<sub>Additional modules in the Cyto model family will be added to this index as they are open-sourced.</sub>

---

## Institutions

**Cyto System** is jointly developed by:
- **Beijing Zhongguancun Academy**
- **BGI Research**
