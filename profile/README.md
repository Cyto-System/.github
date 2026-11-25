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
  <sub>A multiscale spatiotemporal cell model family for the life sciences: reading cellular state, inferring its changes and intervention responses, and autonomously formulating and validating scientific questions.</sub>
</p>

<p align="center">
  <a href="https://cyto-system.github.io"><img src="https://img.shields.io/badge/Website-cyto--system.github.io-059669.svg" alt="Cyto Website"></a>
  <a href="https://github.com/Cyto-System"><img src="https://img.shields.io/badge/Organization-Cyto%20System-2f7d68.svg" alt="Cyto System"></a>
  <a href="https://github.com/Cyto-System"><img src="https://img.shields.io/badge/Institution-Beijing%20Zhongguancun%20Academy%20%7C%20BGI%20Research-2f7d68.svg" alt="Beijing Zhongguancun Academy | BGI Research"></a>
</p>

---

## About the Cyto Family

**Cyto** is a family of spatiotemporal cell models jointly developed by **Beijing Zhongguancun Academy** and **BGI Research**.

Cyto aims to build a state-aware, intervention-capable, and reasoning-enabled multiscale spatiotemporal cell system. Within one cross-scale modeling framework, it links gene- and molecule-level information, single-cell states, and tissue-scale context to read cellular state, infer its changes and intervention responses, and autonomously formulate and validate scientific questions.

Cyto is not a single model, but a spatiotemporal cell system composed of seven submodels that jointly read cellular state, infer its changes, and predict responses to intervention. Six of these submodels form two complementary axes: a **spatial axis** and a **temporal axis**. Together, these axes characterize cellular state across scales. At the system level, **Cyto.CoScientist** integrates evidence from both axes to advance biological discovery.

| Component | Scientific role | Associated models |
| :--- | :--- | :--- |
| **Scientific discovery coordination** | Integrates evidence from the spatial and temporal axes into testable biological hypotheses, supports the design and interpretation of perturbation experiments, and refines the next round of inquiry | **Cyto.CoScientist** |
| **Spatial axis** | Integrates molecular regulation, single-cell multi-omics, and tissue-scale spatial context | **Cyto.Genome** (molecular regulation), **Cyto.Multiomics** (single-cell multi-omics), and **Cyto.Spatial** (tissue microenvironment / niche) |
| **Temporal axis** | Infers state changes and intervention responses from the current cell identity | **Cyto.Identity** (current identity), **Cyto.Dynamics** (state changes over time), and **Cyto.Perturbation** (counterfactual response to intervention) |

---

## Model Family & Repositories

| Module | Method | Scope | Repository & Resources |
| :--- | :--- | :--- | :--- |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **[Cyto.Spatial](https://github.com/Cyto-System/Cyto.Spatial)** | **SUDOKU** (Unified Foundation Model for Spatial Transcriptomics Representation Learning and Generation) | Unified cell and tissue-niche representation and spatial cell-state generation from spatial transcriptomics; cross-section niche retrieval, multi-scale clustering, and immune-recruitment prediction | [GitHub (Cyto.Spatial)](https://github.com/Cyto-System/Cyto.Spatial) |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **[Cyto.Identity](https://github.com/Cyto-System/Cyto.Identity)** | **scVerity** (Manifold-Guided Evidence Verification) | Cell identity and state annotation across unseen cell types, sibling subtypes, and rare lineages, with query-sample molecular evidence, ontology constraints, and multimodal validation | [GitHub (Cyto.Identity)](https://github.com/Cyto-System/Cyto.Identity) |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **[Cyto.Perturbation](https://github.com/Cyto-System/Cyto.Perturbation)** | **RELAY** (Anchored Dense Response Contrast Transfer) | Same-cell unseen genetic & drug perturbations, plus zero-shot cross-cell perturbation transfer | [GitHub (Cyto.Perturbation)](https://github.com/Cyto-System/Cyto.Perturbation) · [Hugging Face](https://huggingface.co/KassdinZheng/Cyto.Perturbation) |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **[Cyto.CoScientist](https://github.com/Cyto-System/Cyto.CoScientist)** | **Within-Task Recursive Self-Improvement (RSI)** | Long-horizon autonomous biological research across bioinformatics algorithm development and open-ended multi-omics inquiry | [GitHub (Cyto.CoScientist)](https://github.com/Cyto-System/Cyto.CoScientist) |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **Cyto.Genome** | **Genome-to-Multi-Omics Foundation** | Cell-type-specific multi-omics track prediction and modality completion from DNA sequence to molecular expression | Open-sourcing soon |

<sub>Additional modules in the Cyto model family will be added to this index as they are open-sourced.</sub>

---

## Institutions

**Cyto System** is jointly developed by:
- **Beijing Zhongguancun Academy**
- **BGI Research**
