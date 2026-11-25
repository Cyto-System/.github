<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_system_banner_dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_system_banner_light.svg">
    <img alt="Cyto System — BGI Research & Zhongguancun Academy" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_system_banner_light.svg" width="84%">
  </picture>
</p>

<h1 align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg">
    <img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="28" align="absmiddle">
  </picture>
  &nbsp;Cyto Spatiotemporal Cell Model Family
</h1>

<p align="center">
  <strong>English</strong> &nbsp;|&nbsp; <a href="https://github.com/Cyto-System/.github/blob/main/profile/README_zh.md">简体中文</a>
</p>

<p align="center">
  <strong>Jointly developed by BGI Research &amp; Zhongguancun Academy</strong><br>
  <sub>Building modular, verifiable, and practical computational models for spatiotemporal cell simulation and cellular response prediction.</sub>
</p>

<p align="center">
  <a href="https://cyto-system.github.io"><img src="https://img.shields.io/badge/Website-cyto--system.github.io-059669.svg" alt="Cyto Website"></a>
  <a href="https://github.com/Cyto-System"><img src="https://img.shields.io/badge/Organization-Cyto%20System-2f7d68.svg" alt="Cyto System"></a>
  <a href="https://github.com/Cyto-System/Cyto.Perturbation"><img src="https://img.shields.io/badge/Institution-BGI%20Research%20%7C%20Zhongguancun%20Academy-2f7d68.svg" alt="BGI Research | Zhongguancun Academy"></a>
  <a href="https://huggingface.co/KassdinZheng/Cyto.Perturbation"><img src="https://img.shields.io/badge/HuggingFace-Cyto.Perturbation-yellow.svg" alt="Hugging Face"></a>
</p>

---

## About the Cyto Family

**Cyto** is a family of spatiotemporal cell models jointly developed by **BGI Research** and **Zhongguancun Academy**. Rather than treating cellular modeling as a single opaque black box, **Cyto System** organizes spatiotemporal cell capabilities into focused, composable modules with explicit biological grounding, leak-free evaluation protocols, and lightweight deployment.

Our core design principles:

- **Biology-Grounded Modeling**: Explicitly combine curated biological priors with high-throughput single-cell measurements so models isolate perturbation- and state-specific signals instead of memorizing gene-level baseline biases.
- **Rigorous & Leak-Free Benchmarking**: Evaluate on strictly held-out perturbations, cell lines, and compounds using fine-grained discrimination metrics (such as within-gene balanced accuracy and orthogonal MSE decomposition).
- **Accessible & Reproducible Compute**: Deliver compact, integrity-verified checkpoints and transparent inference pipelines that run reliably in standard research environments—including CPU-only workstations.

---

## Model Family

| Module | Method | Scope | Compute | Repository & Weights |
| :--- | :--- | :--- | :--- | :--- |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **[Cyto.Identity](https://github.com/Cyto-System/Cyto.Identity)** | **scVerity** (Evidence-Grounded Reasoning) | Open-world single-cell annotation, ontology-grounded verification, and rare-lineage discovery | Adaptive manifold + Agent/Meta review | [GitHub](https://github.com/Cyto-System/Cyto.Identity) |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **[Cyto.Perturbation](https://github.com/Cyto-System/Cyto.Perturbation)** | **RELAY** (Anchored Dense Response Contrast Transfer) | Unseen genetic knockdowns (CRISPRi), zero-shot cross-cell transfer, and unseen small-molecule compounds | CPU-only (~7.6 s full suite) | [GitHub](https://github.com/Cyto-System/Cyto.Perturbation) · [Hugging Face](https://huggingface.co/KassdinZheng/Cyto.Perturbation) |

<sub>Additional modules in the Cyto spatiotemporal cell family will be added to this repository index as they are released.</sub>

---

## Featured Module: Cyto.Perturbation (RELAY)

**[Cyto.Perturbation (RELAY)](https://github.com/Cyto-System/Cyto.Perturbation)** is the perturbation-prediction module of the **Cyto** spatiotemporal cell model family. It predicts differential expression (**DE**), direction of change (**DIR**), calibrated three-class calls (**`non_de` / `down` / `up`**), and full-transcriptome continuous response profiles for unseen genetic knockdowns and small-molecule compounds—without a language model and running entirely on **CPU**.

### Core Architecture

1. **Mean-Anchored Contrast Decomposition**: Centers continuous responses $R$ and magnitudes $|R|$ around per-gene training means $(\mu(g), \nu(g))$, separating baseline gene responsiveness from perturbation-specific contrasts.
2. **Five-Source Knowledge Kernel & Masked Ridge Transfer**: Encodes perturbations using a source-balanced unsigned TF-IDF kernel over **GO, Reactome, CORUM, STRING, and BioPlex** (and target-protein aggregation for small molecules), transferring dense signed and magnitude contrasts via regularized kernel ridge regression.
3. **Task-Specific Calibrated Readouts**: Uses an analytic mean-anchored readout for **DIR** and a compact 3-seed PCA-context MLP (**6,434 parameters**) for **DE**, with optional standardized effect increments when $(F, \mathrm{SE})$ statistics are available.

### Key Results

- **PerturbQA Same-Cell Unseen CRISPRi** *(4-cell mean across K562, HepG2, Jurkat, RPE1; 116,041 DE / 16,208 DIR queries)*:
  - **DE**: Macro-F1 **0.8941**, WG-BAcc **0.6574** (+4.65 pp over the strongest baseline), pgAUROC **0.7732**
  - **DIR**: Macro-F1 **0.8722**, WG-BAcc **0.7672** (+4.41 pp over the strongest baseline), pgAUROC **0.8611**
- **Continuous Response Profiles** *(1,264 held-out perturbations)*:
  - Total MSE **4.849 × 10⁻³** (vs. 6.154 × 10⁻³ gene-mean baseline), per-perturbation $r = \mathbf{0.5165}$, per-gene $r = \mathbf{0.3141}$.
- **Zero-Shot Unseen Cell Line (RPE1)** *(37,942 queries; control cells only)*:
  - 3-class Macro-F1 **0.7597**, DE WG-BAcc **0.5933**, DIR WG-BAcc **0.7333**.
- **Unseen Small-Molecule Compounds (GeneTAK / Tahoe-100M)** *(5 tumor cell lines, 95 held-out compounds)*:
  - DE Macro-F1 **0.9179** / WG-BAcc **0.5463** / pgAUROC **0.6138**; DIR Macro-F1 **0.7828** / WG-BAcc **0.5574** / pgAUROC **0.6284**.

### Released Checkpoints & Licensing

- **Checkpoints**: `perturbqa-samecell-v1` (~633 MB `float32`) and `genetak-compounds-v1` (~39 MB `float32`) on [Hugging Face](https://huggingface.co/KassdinZheng/Cyto.Perturbation), with SHA-256 verification, zero-pickle loading, and exact `float64` decision parity.
- **Licensing**: Source code under **Apache-2.0**; pretrained checkpoints under **CC BY-NC 4.0**.

---

## Institutions

**Cyto System** is jointly developed by:
- **BGI Research**
- **Zhongguancun Academy**
