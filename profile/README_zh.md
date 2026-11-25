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
  <sub>构建模块化、可验证、易部署的时空细胞计算模型体系</sub>
</p>

<p align="center">
  <a href="https://cyto-system.github.io"><img src="https://img.shields.io/badge/%E5%AE%98%E7%BD%91-cyto--system.github.io-059669.svg" alt="Cyto 官网"></a>
  <a href="https://github.com/Cyto-System"><img src="https://img.shields.io/badge/%E7%BB%84%E7%BB%87-Cyto%20System-2f7d68.svg" alt="Cyto System"></a>
  <a href="https://github.com/Cyto-System"><img src="https://img.shields.io/badge/%E7%A0%94%E5%8F%91%E6%9C%BA%E6%9E%84-%E5%8C%97%E4%BA%AC%E4%B8%AD%E5%85%B3%E6%9D%91%E5%AD%A6%E9%99%A2%20%7C%20%E5%8D%8E%E5%A4%A7%E7%A0%94%E7%A9%B6%E9%99%A2-2f7d68.svg" alt="北京中关村学院 | 华大研究院"></a>
</p>

---

## 关于 Cyto 模型家族

**Cyto** 是由**北京中关村学院**与**华大研究院**联合研发的时空细胞模型家族。

Cyto 不是单一模型，而是由 7 个能够表征细胞状态、支持干预并刻画时间变化的子模型组成。其中六个子模型构成 Cyto 时空细胞建模的两条互补主轴：**空间横轴**与**时间纵轴**。**Cyto.CoScientist** 则整合两条轴上的证据，推动生物学发现。

> [!IMPORTANT]
> ### Cyto.CoScientist · 科学发现统筹层
>
> **Cyto.CoScientist** 将两条轴线上的证据整合为可检验的生物学假设，支持干预实验的设计与解释，并依据实验结果修正下一轮研究。

| 维度 | 科学作用 | 子模型与递进关系 |
| :--- | :--- | :--- |
| **空间横轴** | 整合分子调控、单细胞多组学与组织尺度的空间信息 | **Cyto.Genome**（分子调控）→ **Cyto.Multiomics**（单细胞多组学）→ **Cyto.Spatial**（组织微环境 / Niche） |
| **时间纵轴** | 将细胞当前身份与自然演化及干预响应联系起来 | **Cyto.Identity**（当前身份）→ **Cyto.Dynamics**（自然演化轨迹）→ **Cyto.Perturbation**（干预后的反事实响应） |

在 Cyto 系统中，两条轴线共同构成对细胞状态的多尺度描述；系统整体进一步连接两条互补的研究路径：证据生成与转化应用。

**证据生成**：强化学习驱动的主动学习结合模型预测不确定性与已有组学证据，用于识别证据不足、但可通过现有实验进一步解析的细胞状态、调控程序或组织邻域。据此优先开展转录组、多组学或扰动实验，以补足证据缺口、区分竞争性假设并检验候选机制。新增测量随后更新相应模型，使计算预测与实验证据相互校正。

**转化应用**：Cyto 面向时空病理、复杂疾病队列和药物发现等问题，并通过共享基准支持系统比较与评估。

---

## 模型家族与仓库列表

| 模块 | 核心方法 | 适用任务 | 仓库与资源 |
| :--- | :--- | :--- | :--- |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **[Cyto.Spatial](https://github.com/Cyto-System/Cyto.Spatial)** | **SUDOKU**（空间离散去噪） | 从空间转录组中统一学习细胞与组织邻域表征、生成空间细胞状态，用于跨切片邻域检索、多尺度聚类和免疫募集预测 | [GitHub (Cyto.Spatial)](https://github.com/Cyto-System/Cyto.Spatial) |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **[Cyto.Identity](https://github.com/Cyto-System/Cyto.Identity)** | **scVerity**（循证推理单细胞注释） | 面向未见细胞类型、近缘亚型与稀有谱系的细胞身份与状态注释，基于查询样本分子证据、本体约束及多模态校验 | [GitHub (Cyto.Identity)](https://github.com/Cyto-System/Cyto.Identity) |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **[Cyto.Perturbation](https://github.com/Cyto-System/Cyto.Perturbation)** | **RELAY**（均值锚定稠密响应对比迁移） | 同细胞系未见基因扰动、同细胞系未见药物扰动、跨细胞系迁移已知扰动 | [GitHub (Cyto.Perturbation)](https://github.com/Cyto-System/Cyto.Perturbation) · [Hugging Face](https://huggingface.co/KassdinZheng/Cyto.Perturbation) |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **[Cyto.CoScientist](https://github.com/Cyto-System/Cyto.CoScientist)** | **任务内递归自改进（RSI）** | 面向长程自主生物学研究，涵盖生物信息学算法开发和开放式多组学研究 | [GitHub (Cyto.CoScientist)](https://github.com/Cyto-System/Cyto.CoScientist) |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **Cyto.Genome** | **基因组到细胞多组学基础模型** | 从 DNA 序列到分子表达，预测细胞类型特异的多组学轨道并完成模态补全 | 近期开源 |

<sub>Cyto 模型家族的其他模块将在完成验证并开源后陆续纳入此列表。</sub>

---

## 研发机构

**Cyto System** 由以下机构联合研发：
- **北京中关村学院（Beijing Zhongguancun Academy）**
- **华大研究院（BGI Research）**
