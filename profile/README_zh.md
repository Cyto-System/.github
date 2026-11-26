<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_system_banner_zh_dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_system_banner_zh_light.svg">
    <img alt="Cyto System — 北京中关村学院 · 华大研究院" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_system_banner_zh_light.svg" width="84%">
  </picture>
</p>

<h1 align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg">
    <img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="28" align="absmiddle">
  </picture>
  &nbsp;Cyto 模型家族
</h1>

<p align="center">
  <a href="https://github.com/Cyto-System">English</a> &nbsp;|&nbsp; <strong>简体中文</strong>
</p>

<p align="center">
  <strong>北京中关村学院 · 华大研究院联合研发</strong><br>
  <sub>读懂细胞状态，推演状态变化，预测干预响应，自主提出并验证科学问题。</sub>
</p>

<p align="center">
  <a href="https://cyto-system.github.io"><img src="https://img.shields.io/badge/%E5%AE%98%E7%BD%91-cyto--system.github.io-059669.svg" alt="Cyto 官网"></a>
  <a href="https://github.com/Cyto-System"><img src="https://img.shields.io/badge/%E7%BB%84%E7%BB%87-Cyto%20System-2f7d68.svg" alt="Cyto System"></a>
  <a href="https://github.com/Cyto-System"><img src="https://img.shields.io/badge/%E7%A0%94%E5%8F%91%E6%9C%BA%E6%9E%84-%E5%8C%97%E4%BA%AC%E4%B8%AD%E5%85%B3%E6%9D%91%E5%AD%A6%E9%99%A2%20%7C%20%E5%8D%8E%E5%A4%A7%E7%A0%94%E7%A9%B6%E9%99%A2-2f7d68.svg" alt="北京中关村学院 | 华大研究院"></a>
</p>

---

## 关于 Cyto 模型家族

**Cyto** 是由**北京中关村学院**与**华大研究院**联合研发的时空细胞模型家族。

Cyto 旨在构建一个有状态、可干预、可推理的多尺度时空细胞系统。系统在统一的跨尺度建模框架中串联基因与分子层面信息、单细胞状态和组织尺度信息，以读懂细胞状态、推演其变化与干预响应，并自主提出和验证科学问题。

Cyto 不是单一模型，而是一个由 7 个子模型协同构成的时空细胞系统，能够读懂细胞状态、推演其变化并预测干预响应。六个子模型分别构成**空间横轴**和**时间纵轴**，从不同尺度共同刻画细胞状态。**Cyto.CoScientist** 在系统层面整合两条轴线的证据，推动生物学发现。

| 组成 | 科学作用 | 对应模型 |
| :--- | :--- | :--- |
| **科学发现统筹** | 将空间与时间两条轴线上的证据整合为可检验的生物学假设，支持干预实验的设计与解释，并据此修正下一轮研究 | **Cyto.CoScientist** |
| **空间横轴** | 整合分子调控、单细胞多组学与组织尺度的空间信息 | **Cyto.Genome**（分子调控）、**Cyto.Multiomics**（单细胞多组学）、**Cyto.Spatial**（组织微环境 / Niche） |
| **时间纵轴** | 从细胞当前身份推演状态变化与干预响应 | **Cyto.Identity**（当前身份）、**Cyto.Dynamics**（状态随时间的变化）、**Cyto.Perturbation**（干预后的反事实响应） |

---

## 模型家族与仓库列表

| 模块 | 核心方法 | 适用任务 | 仓库与资源 |
| :--- | :--- | :--- | :--- |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **[Cyto.Spatial](https://github.com/Cyto-System/Cyto.Spatial)** | **SUDOKU**（面向空间转录组表征学习与生成的统一基础模型） | 从空间转录组中统一学习细胞与组织邻域表征、生成空间细胞状态，用于跨切片邻域检索、多尺度聚类和免疫募集预测 | [GitHub (Cyto.Spatial)](https://github.com/Cyto-System/Cyto.Spatial) |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **[Cyto.Identity](https://github.com/Cyto-System/Cyto.Identity)** | **scVerity**（流形引导的证据核验） | 面向未见细胞类型、近缘亚型与稀有谱系的细胞身份与状态注释，基于查询样本分子证据、本体约束及多模态校验 | [GitHub (Cyto.Identity)](https://github.com/Cyto-System/Cyto.Identity) |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **[Cyto.Perturbation](https://github.com/Cyto-System/Cyto.Perturbation)** | **RELAY**（均值锚定稠密响应对比迁移） | 同细胞系未见基因扰动、同细胞系未见药物扰动、跨细胞系迁移已知扰动 | [GitHub (Cyto.Perturbation)](https://github.com/Cyto-System/Cyto.Perturbation) · [Hugging Face](https://huggingface.co/KassdinZheng/Cyto.Perturbation) |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **[Cyto.CoScientist](https://github.com/Cyto-System/Cyto.CoScientist)** | **任务内递归自改进（RSI）** | 面向长程自主生物学研究，涵盖生物信息学算法开发和开放式多组学研究 | [GitHub (Cyto.CoScientist)](https://github.com/Cyto-System/Cyto.CoScientist) |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **Cyto.Genome** | **基因组到细胞多组学基础模型** | 从 DNA 序列到分子表达，预测细胞类型特异的多组学轨道并完成模态补全 | 近期开源 |

<sub>Cyto 模型家族的其他模块将在完成验证并开源后陆续纳入此列表。</sub>

---

## 研发机构

**Cyto System** 由以下机构联合研发：
- **北京中关村学院（Beijing Zhongguancun Academy）**
- **华大研究院（BGI Research）**
