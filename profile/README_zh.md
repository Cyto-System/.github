<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_system_banner_zh_dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_system_banner_zh_light.svg">
    <img alt="Cyto System — 华大研究院 · 北京中关村学院" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_system_banner_zh_light.svg" width="84%">
  </picture>
</p>

<h1 align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg">
    <img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="28" align="absmiddle">
  </picture>
  &nbsp;Cyto 时空细胞模型家族
</h1>

<p align="center">
  <a href="https://github.com/Cyto-System">English</a> &nbsp;|&nbsp; <strong>简体中文</strong>
</p>

<p align="center">
  <strong>华大研究院 · 北京中关村学院联合研发</strong><br>
  <sub>构建模块化、可验证、易部署的时空细胞计算模型体系</sub>
</p>

<p align="center">
  <a href="https://cyto-system.github.io"><img src="https://img.shields.io/badge/%E5%AE%98%E7%BD%91-cyto--system.github.io-059669.svg" alt="Cyto 官网"></a>
  <a href="https://github.com/Cyto-System"><img src="https://img.shields.io/badge/%E7%BB%84%E7%BB%87-Cyto%20System-2f7d68.svg" alt="Cyto System"></a>
  <a href="https://github.com/Cyto-System/Cyto.Perturbation"><img src="https://img.shields.io/badge/%E7%A0%94%E5%8F%91%E6%9C%BA%E6%9E%84-%E5%8D%8E%E5%A4%A7%E7%A0%94%E7%A9%B6%E9%99%A2%20%7C%20%E5%8C%97%E4%BA%AC%E4%B8%AD%E5%85%B3%E6%9D%91%E5%AD%A6%E9%99%A2-2f7d68.svg" alt="华大研究院 | 北京中关村学院"></a>
  <a href="https://huggingface.co/KassdinZheng/Cyto.Perturbation"><img src="https://img.shields.io/badge/HuggingFace-Cyto.Perturbation-yellow.svg" alt="Hugging Face"></a>
</p>

---

## 关于 Cyto 模型家族

**Cyto** 是由**华大研究院**与**北京中关村学院**联合研发的时空细胞模型家族。**Cyto System** 采用模块化思路组织时空细胞建模能力，将先验生物知识、高通量单细胞观测与严格评测体系结合，面向真实科研与计算生物学场景提供透明、可复现的模型与工具。

核心设计原则：

- **显式融合生物先验与实验观测**：将目标基因的固有基线倾向与特定扰动/状态引发的特异性信号解耦建模，避免模型被基因先验偏差主导。
- **严格无泄漏评测**：面向未见扰动、未见细胞系与未见化合物设定严格域隔离，结合基因内平衡准确率（WG-BAcc）与正交 MSE 分解等指标检验真实判别力。
- **轻量化与低门槛部署**：提供经过完整校验的紧凑权重与清晰推理链路，支持在常规 CPU 环境下秒级运行，便于复现与集成。

---

## 模型家族列表

| 模块 | 核心方法 | 适用任务 | 推理环境 | 仓库与权重 |
| :--- | :--- | :--- | :--- | :--- |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **[Cyto.Identity](https://github.com/Cyto-System/Cyto.Identity)** | **scVerity**（循证推理单细胞注释） | 开放世界细粒度单细胞注释、本体证据链核验与罕见亚群发现 | 自适应流形 + 智能体/元评审 | [GitHub](https://github.com/Cyto-System/Cyto.Identity) |
| <picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_dark.svg"><source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg"><img alt="Cyto" src="https://raw.githubusercontent.com/Cyto-System/.github/main/profile/assets/cyto_logo_light.svg" width="16" align="absmiddle"></picture> **[Cyto.Perturbation](https://github.com/Cyto-System/Cyto.Perturbation)** | **RELAY**（均值锚定稠密响应对比迁移） | 未见 CRISPRi 遗传敲低、未见细胞系零样本迁移、未见小分子化合物扰动预测 | 纯 CPU（全量评测约 7.6 s） | [GitHub](https://github.com/Cyto-System/Cyto.Perturbation) · [Hugging Face](https://huggingface.co/KassdinZheng/Cyto.Perturbation) |

<sub>Cyto 时空细胞家族的其他功能模块将在完成验证后陆续发布并纳入此列表。</sub>

---

## 代表模块：Cyto.Perturbation (RELAY)

**[Cyto.Perturbation (RELAY)](https://github.com/Cyto-System/Cyto.Perturbation)** 是 **Cyto** 时空细胞模型家族中的单细胞扰动预测模块。该方法不依赖大语言模型、仅需纯 CPU 即可秒级运行，面向未见遗传敲低与未见小分子化合物扰动输出校准后的差异表达判定（DE）、上下调方向判定（DIR）、联合三分类结果（`non_de` / `down` / `up`）以及全转录组连续响应谱。

### 核心机制

1. **均值锚定的对比分解**：围绕训练集逐基因均值 $(\mu(g), \nu(g))$ 对连续响应 $R$ 与幅度 $|R|$ 中心化，将基因固有基线倾向与扰动特异性对比显式分离。
2. **五源生物知识核与核岭回归迁移**：基于 **GO、Reactome、CORUM、STRING、BioPlex** 构建分源均衡的无符号 TF-IDF 知识核（对小分子化合物采用靶蛋白聚合编码），通过正则化核岭回归迁移全量稠密符号对比与幅度对比。
3. **任务定制校准读出头**：DIR 采用解析均值锚定读出，DE 采用 3 种子、仅 **6,434 参数**的 PCA 全局上下文 MLP 读出头，并在具备 $(F, \mathrm{SE})$ 统计量时叠加标准化效应增量。

### 核心实验结果

- **PerturbQA 同细胞未见 CRISPRi 敲低**（K562、HepG2、Jurkat、RPE1 四细胞系等权均值，覆盖 116,041 条 DE / 16,208 条 DIR 查询）：
  - **DE**：Macro-F1 **0.8941**，WG-BAcc **0.6574**（领先最强基线 +4.65 个百分点），pgAUROC **0.7732**
  - **DIR**：Macro-F1 **0.8722**，WG-BAcc **0.7672**（领先最强基线 +4.41 个百分点），pgAUROC **0.8611**
- **连续表达响应谱**（1,264 个未见测试扰动）：
  - 总 MSE 降至 **4.849 × 10⁻³**（训练集基因均值基线为 6.154 × 10⁻³），逐扰动相关性 $r = \mathbf{0.5165}$，逐基因相关性 $r = \mathbf{0.3141}$。
- **未见细胞系 RPE1 零样本迁移**（37,942 条查询，目标细胞系仅提供未扰动对照）：
  - 三分类 Macro-F1 **0.7597**，DE WG-BAcc **0.5933**，DIR WG-BAcc **0.7333**。
- **未见小分子化合物迁移（GeneTAK / Tahoe-100M）**（5 个肿瘤细胞系，95 个未见化合物）：
  - DE Macro-F1 **0.9179** / WG-BAcc **0.5463** / pgAUROC **0.6138**；DIR Macro-F1 **0.7828** / WG-BAcc **0.5574** / pgAUROC **0.6284**。

### 权重与协议

- **预训练权重**：在 [Hugging Face](https://huggingface.co/KassdinZheng/Cyto.Perturbation) 发布 `perturbqa-samecell-v1`（约 633 MB，`float32`）与 `genetak-compounds-v1`（约 39 MB，`float32`），支持 SHA-256 校验与无 pickle 安全加载，与 `float64` 参考实现保持零决策差异。
- **开源协议**：代码采用 **Apache-2.0** 协议，预训练权重采用 **CC BY-NC 4.0** 协议。

---

## 研发机构

**Cyto System** 由以下机构联合研发：
- **华大研究院（BGI Research）**
- **北京中关村学院（Zhongguancun Academy）**
