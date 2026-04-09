# 仓颉.skill v2.0 (Cangjie)
> *「不仅看透灵魂，还要穿上皮囊，感受体温」*

**仓颉是「女娲」与「同事」的深度融合。它负责蒸馏任何团队、公众号或机构的写作风格，并将其转化为可运行的高仿生写作引擎。v2.0 新增「情感层」建模和「黄金语料锚定」，目标仿生度 ≥ 95%。**

---

## 🌪️ v2.0 核心升级
1. **四位一体提炼**：
   - **理 (Logic)**：心智模型三重验证。
   - **文 (Expression)**：写作指纹量化还原 + `Writing_Pattern.json` 硬编码参数。
   - **情 (Emotion)** ⭐新增：Valence-Arousal-Empathy 三维情感建模 + 情感弧线 + 情感禁区。
   - **神 (Evolution)**：`Correction.md` 分层补丁（C-理/C-文/C-情/C-排）。
2. **9路 Sub-Agents 并行**：新增「情感基调 Agent」，确保情感维度的地毯式采集。
3. **黄金语料锚定** ⭐新增：精选 3-5 段原文作为 few-shot 示例，直接嵌入 Prompt。
4. **风格审计 Agent** ⭐新增：自动化仿生指数评估（0-100），< 85 分打回重写。

---

## 🛠️ 目录结构
```
cangjie-skill/
├── SKILL.md                         # 仓颉 v2.0 全局核心逻辑
├── references/
│   ├── extraction-framework.md      # 提炼方法论（理/文/情/神）
│   └── skill-template.md            # 生成具体风格包的模板
└── outputs/                         # 存放已复刻的团队风格包
    └── [team-name]-perspective/
        ├── SKILL.md                 # 该团队的仿生写作操作系统
        ├── Correction.md            # 进化纠错记录（分层）
        ├── Writing_Pattern.json     # 量化参数
        ├── Golden_Corpus.md         # 黄金语料锚点
        └── references/research/     # 9路Agent调研结果
```

---

## 📊 v1.0 → v2.0 核心升级对比

| 维度 | v1.0 | v2.0 |
|:---|:---|:---|
| 架构 | 理-文-神 (3层) | **理-文-情-神 (4层)** |
| 调研 Agent | 8 路 | **9 路** (新增情感基调 Agent) |
| 精度保障 | 定性描述 | **量化参数 + Few-Shot 锚定 + 风格审计** |
| 情感还原 | 完全缺失 | **Valence-Arousal-Empathy 三维建模** |
| 验证机制 | 人工主观 | **自动化仿生指数 (0-100)** |
| Correction | 扁平列表 | **C-理/C-文/C-情/C-排 四层分类** |
| 预期仿生度 | ~75% | **≥ 95%** |

---

## 📜 许可证
MIT — 随便用，随便改，随便造。

---

> 本 Skill 由 [仓颉 · 高仿生写作引擎 v2.0] 驱动
> 理论基础：[GCE Framework (2026)](https://arxiv.org/html/2604.04387v2)、[ACL Style Imitation (2025)](https://arxiv.org/html/2509.14543v1)
