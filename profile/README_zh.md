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

Cyto 不是单一模型，而是由 7 个具备状态感知、可干预和可演化能力的子模型组成。其中六个领域模块构成空间与时间两条轴线，**Cyto.CoScientist** 负责统筹各模块并衔接科学发现过程。

> [!IMPORTANT]
> ### Cyto.CoScientist · 科学发现统筹层
>
> **Cyto.CoScientist** 将两条轴线上的模型输出转化为可检验的生物学假设，衔接细胞干预实验的设计与验证，并将结果带入下一轮分析。

| 维度 | 作用 | 子模型与递进关系 |
| :--- | :--- | :--- |
| **空间横轴** | 在不同空间尺度上解析细胞组成与组学关联 | **Cyto.Genome**（分子调控）→ **Cyto.Multiomics**（单细胞多组学）→ **Cyto.Spatial**（组织微环境 / Niche） |
| **时间纵轴** | 刻画细胞当前状态及其随时间的变化 | **Cyto.Identity**（当前身份）→ **Cyto.Dynamics**（自然演化轨迹）→ **Cyto.Perturbation**（干预后的反事实响应） |

两条轴线共同刻画细胞在空间和时间中的完整状态。模型两端分别对应**数据端**与**应用端**。

**数据端**：基于强化学习的主动学习机制识别模型不确定性最高的位置，优先补充最能降低不确定性的测量，并将新增数据回流到相应模块，从而形成计算预测与湿实验验证之间的迭代闭环。

**应用端**：Cyto 面向时空病理、复杂疾病队列和药物发现等场景，并配套统一基准，以支持系统比较与评估。

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
