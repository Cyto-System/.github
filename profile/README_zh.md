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

**Cyto** 是由**北京中关村学院**与**华大研究院**联合研发的时空细胞模型家族。**Cyto System** 采用模块化思路组织时空细胞建模能力，将先验生物知识、高通量单细胞观测与严格评测体系结合，面向真实科研与计算生物学场景提供透明、可复现的模型与工具。

核心设计原则：

- **显式融合生物先验与实验观测**：将目标基因的固有基线倾向与特定扰动/状态引发的特异性信号解耦建模，避免模型被基因先验偏差主导。
- **严格无泄漏评测**：面向未见扰动、未见细胞系与未见化合物设定严格域隔离，结合基因内平衡准确率（WG-BAcc）与正交 MSE 分解等指标检验真实判别力。
- **轻量化与低门槛部署**：提供经过完整校验的紧凑权重与清晰推理链路，支持在常规 CPU 环境下秒级运行，便于复现与集成。

---

## 模型家族与仓库列表

| 模块 | 核心方法 | 适用任务 | 仓库与资源 |
| :--- | :--- | :--- | :--- |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **Cyto.Genome** | **基因组到分子表达** | 从参考基因组序列与顺式调控元件出发，预测细胞类型特异染色质可及性与分子表达谱 | 近期开源 |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **[Cyto.Spatial](https://github.com/Cyto-System/SUDOKU)** | **SUDOKU**（生成式空间转录组基座） | 跨切片空间邻域表征、多尺度空间域聚类与掩码细胞状态补全 | [GitHub (SUDOKU)](https://github.com/Cyto-System/SUDOKU) |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **[Cyto.Identity](https://github.com/Cyto-System/Cyto.Identity)** | **scVerity**（循证推理单细胞注释） | 开放世界细粒度单细胞注释、本体证据链核验与罕见亚群发现 | [GitHub (Cyto.Identity)](https://github.com/Cyto-System/Cyto.Identity) |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **[Cyto.Perturbation](https://github.com/Cyto-System/Cyto.Perturbation)** | **RELAY**（均值锚定稠密响应对比迁移） | 同细胞系未见基因扰动、同细胞系未见药物扰动、跨细胞系迁移已知扰动 | [GitHub (Cyto.Perturbation)](https://github.com/Cyto-System/Cyto.Perturbation) · [Hugging Face](https://huggingface.co/KassdinZheng/Cyto.Perturbation) |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **[Cyto.CoScientist](https://github.com/Cyto-System/Cyto.CoScientist)** | **Within-Task RSI**（循证自主科研智能体） | 任务内递归自我改进、多分支候选演化与可审计多组学研究闭环 | [GitHub (Cyto.CoScientist)](https://github.com/Cyto-System/Cyto.CoScientist) |

<sub>Cyto 模型家族的其他模块将在完成验证并开源后陆续纳入此列表。</sub>

---

## 研发机构

**Cyto System** 由以下机构联合研发：
- **北京中关村学院（Beijing Zhongguancun Academy）**
- **华大研究院（BGI Research）**
