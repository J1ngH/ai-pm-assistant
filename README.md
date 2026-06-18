# AI PM Assistant（AI 产品经理助手）

[中文]() | Claude Code Skill

**AI PM Assistant** 是一个 Claude Code Skill，将 Claude 转变为经验丰富的 AI 产品经理，帮助你将模糊的产品想法转化为可验证、可设计、可开发的完整产品方案。

> 从产品想法到 AI Coding Prompt 生成，覆盖产品全生命周期。

---

## 功能概览

AI PM Assistant 提供六大核心工作模式，自动根据你的输入判断当前所处阶段，选择对应的分析框架：

| 模式 | 适用场景 | 输出内容 |
|------|----------|----------|
| **需求分析** | 产品想法、业务问题 | 用户画像、痛点分析、需求优先级（P0/P1/P2） |
| **MVP 规划** | 需求明确后 | MVP 功能列表、非 MVP 功能列表、迭代路线图 |
| **PRD 生成** | 需要完整产品文档 | 产品背景、功能模块设计、业务流程、数据指标体系 |
| **原型设计** | PRD 完成后 | 信息架构、用户流程、页面拆解、Wireframe、AI Coding Prompt |
| **AI 产品设计** | 涉及 LLM/Agent/RAG | AI 能力设计、Workflow、风险分析、AI 效果指标 |
| **方案评审** | PRD/原型评审 | 多维度检查清单与改进建议 |

---

## 完整产品工作流

```
产品想法
  ↓
需求分析（用户 → 痛点 → 优先级）
  ↓
MVP 规划（核心功能 → 迭代路线）
  ↓
PRD 设计（功能模块 → 业务流程 → 指标体系）
  ↓
信息架构设计（模块结构 → 页面关系）
  ↓
用户流程设计（核心路径 → 操作流程）
  ↓
低保真原型设计（布局 → 交互 → 状态覆盖）
  ↓
AI Coding Prompt 生成（可交付开发的完整 Prompt）
```

---

## 项目结构

```
ai-pm-assistant/
├── SKILL.md                              # Skill 核心定义（系统 Prompt）
├── README.md                             # 项目说明
├── templates/                            # 产品文档模板
│   ├── prd-template.md                   # PRD 文档模板
│   ├── requirement-analysis-template.md  # 需求分析模板
│   └── review-checklist.md               # 产品方案评审清单
└── examples/                             # 使用示例（输入 → 输出）
    ├── ai-note-app-input.md              # AI 知识管理助手 - 输入
    ├── ai-note-app-output.md             # AI 知识管理助手 - 输出
    ├── travel-assistant-input.md         # AI 旅行规划助手 - 输入
    └── travel-assistant-output.md        # AI 旅行规划助手 - 输出
```

---

## 安装与使用

### 前置条件

- 已安装 [Claude Code](https://claude.ai/code)

### 安装 Skill

1. 将本仓库克隆到 Claude Code 的 skills 目录：

```bash
git clone https://github.com/J1ngH/ai-pm-assistant.git ~/.claude/skills/ai-pm-assistant
```

2. 在 Claude Code 中，Skill 会自动注册。当你提供产品想法、需求或 PRD 草稿时，AI PM Assistant 会自动激活。

### 使用方式

直接在 Claude Code 中描述你的产品想法，Skill 会自动调用。例如：

```
我想做一个面向自由职业者的 AI 财务助手，
能够自动分类收支、生成发票和提供税务建议。
请帮我完成需求分析和 MVP 规划。
```

更多示例请查看 [`examples/`](./examples/) 目录。

---

## 设计原则

AI PM Assistant 遵循以下核心原则：

- **用户价值优先** — 所有功能设计以用户价值为导向
- **MVP 最小可行** — 优先设计可快速验证的核心功能，避免过度设计
- **数据驱动迭代** — 为每个功能定义可衡量的指标体系
- **AI 能力合理使用** — AI 不是加分项，必须解释 AI 存在的必要性
- **工程落地可行** — 方案必须考虑技术实现成本和可开发性

---

## 适用场景

- 从零开始规划一个新的 AI 产品
- 对现有产品进行需求梳理和功能评审
- 为开发团队生成结构化的 PRD 文档
- 设计产品的信息架构和用户流程
- 评估 AI 功能在产品中的合理应用方式
- 生成可直接用于 AI Coding 工具的开发 Prompt

---

## 贡献

欢迎提交 Issue 和 Pull Request 来改进这个 Skill。

### 贡献方向

- 优化分析框架和输出模板
- 新增更多行业场景的示例
- 改进 AI 产品设计模式的评估维度
- 补充更多产品文档模板

---

## License

MIT License

---

## 作者

[J1ngH](https://github.com/J1ngH)
