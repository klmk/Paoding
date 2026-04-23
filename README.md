# Paoding (庖丁)

> **AI 驱动开发框架** -- 让 AI 从"能跑就行"升级为"游刃有余"

```
庖丁为文惠君解牛，手之所触，肩之所倚，足之所履，膝之所踦，
砉然向然，奏刀騞然，莫不中音。
                              ——《庄子·养生主》
```

**庖丁解牛，进乎技矣。** AI 编程不应只是机械执行，而应通过持续的知识蒸馏与能力成长，对项目的理解达到"游刃有余"的境界。Paoding 正是这样一套框架——让 AI 成为项目资深专家。

---

## 项目简介

Paoding（庖丁）是一套面向 AI 辅助编程场景的完整开发方法论。它融合了 [Superpowers](https://github.com/obra/Superpowers)（57K⭐）和 [BMad Method](https://github.com/bmad-code-org/BMAD-METHOD)（43K⭐）的精华，并在此基础上加入了**双向画像、AI 错题本、项目知识蒸馏、约束有效性分析**等独创机制，系统性解决 AI 编程中的质量失控、需求偏差、知识流失、框架冗余等核心问题。

**一句话定位：** 让 AI 编程从"能跑就行"升级为"游刃有余"。

---

## 核心特色

### 1. 双向画像与对齐（Phase 0）-- 从源头控制变量

AI 编程项目有两个核心变量：使用者（需求方）和 AI（开发方）。大多数项目失败不是因为技术不行，而是因为双方的能力边界和期望没有对齐。

- **使用者画像**：评估技术背景、沟通偏好、决策风格、风险承受度
- **AI 能力画像**：如实评估 AI 在各维度上的实际能力（非理论能力）
- **交叉分析**：识别匹配度和风险点，制定补强策略
- **双向确认**：双方对能力边界、协作方式、预期产出达成共识

> 这是框架的第一道防线。不了解双方的能力边界就开工，等于盲人摸象。

### 2. 铁律 + 红旗 + 反模式 -- 三层约束防止 AI 行为偏差

AI 在编程中容易"合理化"地跳过质量步骤。框架通过三层约束体系系统性防止这种行为偏差：

- **铁律（Iron Laws）**：6 条不可违反的底线规则，约束力最高
  - 需求铁律：不清晰的需求不得进入开发
  - 测试铁律：没有失败的测试就没有生产代码
  - 审查铁律：每个实现必须经过审查
  - 验证铁律：完成声明必须有新鲜验证证据
  - 文档铁律：每个阶段必须有文档输出
  - 追溯铁律：每段代码必须可追溯到需求
- **红旗（Red Flags）**：针对每条铁律，列出 AI 可能用来绕过的常见借口及反驳
- **反模式（Anti-Patterns）**：AI 常见的"合理化借口"模式库，持续积累

### 3. TDD + 两阶段审查 + 系统化调试 -- 流程补强保证代码质量

- **TDD（测试驱动开发）**：RED-GREEN-REFACTOR 循环，确保代码行为正确
- **两阶段代码审查**：第一阶段检查规格合规（是否匹配 PRD），第二阶段检查代码质量
- **系统化调试**：根因调查先行，禁止"试错式"修复，3 次失败触发升级规则
- **子代理协作**：开发者代理、审查代理、调试代理、验证代理各司其职，信息隔离

### 4. AI 错题本 + 能力成长记录 -- 越用越好用的持续改进机制

- **AI 错题本**：记录 AI 犯过的每一个错误、根因分析、纠正措施，形成"经验数据库"
- **project-context.md**：项目全景上下文，让新 AI 实例快速理解项目
- **开发履历**：记录开发过程中的关键事件和里程碑
- **回顾报告**：每个阶段的经验教训总结和改进建议

> 这些知识资产随项目积累，让 AI 越用越好用，而不是每次都从零开始。

### 5. 项目知识蒸馏体系（Module 7）-- 让 AI 成为项目资深专家 ⭐ 独创

解决 AI 在长期开发中的"失忆"和"幻觉"问题，通过三层架构让 AI 持续成长：

- **自动记忆**：捕获每次会话的关键操作和决策（参考 claude-mem、agent-memory）
- **主动蒸馏**：从原始记忆中提炼专家级认知，生成 `project-brain.md`（项目大脑）
- **持续成长**：错题本 → 补强规则 → 注入 project-brain，能力画像跟踪成长曲线

> 与 claude-mem 的区别：claude-mem 只做被动记忆（记录发生了什么），我们做主动蒸馏（提炼出专家级认知）。project-brain.md 是 AI 写给 AI 看的，不是给人看的文档。

### 6. 约束有效性分析（Module 8）-- 数据驱动优化框架 ⭐ 独创

用真实项目的数据反向验证框架里每条规则到底有没有用：

- **约束追溯**：每个产出物 → 触发哪条约束 → 效果如何
- **迭代快照**：每次迭代完成后存档约束调用数据
- **聚合分析**：跨项目/跨迭代统计约束频率，识别高价值规则和冗余规则
- **框架优化闭环**：数据 → 分析 → 优化 → 再验证，持续精简框架

> 大多数框架的规则是"拍脑袋"写的，不知道哪些真的有用。Module 8 用数据驱动解决这个问题。

---

## 框架结构总览

```
AI-Dev-Framework/
├── README.md                          # 项目总览（本文件）
├── core/                              # 核心约束（贯穿全流程）
│   ├── SKILL.md                       # 核心技能入口
│   ├── iron-laws.md                   # 铁律清单（6 条）
│   ├── anti-patterns.md               # 反模式库
│   └── workflow-overview.md           # 全流程总览
│
├── phase-0-profiling/                 # Phase 0: 双向画像与对齐
│   ├── SKILL.md                       # 阶段技能定义
│   ├── user-profile-template.md       # 使用者画像模板
│   ├── ai-capability-profile-template.md  # AI 能力画像模板
│   └── alignment-strategy-template.md # 对齐策略模板
│
├── phase-1-analysis/                  # Phase 1: 需求分析
│   ├── SKILL.md                       # 阶段技能定义
│   ├── prd-template.md                # PRD 模板
│   ├── requirement-collection-guide.md    # 需求收集指南
│   └── requirement-alignment-checklist.md # 需求对齐检查清单
│
├── phase-2-planning/                  # Phase 2: 规划设计
│   ├── SKILL.md                       # 阶段技能定义
│   ├── architecture-template.md       # 架构文档模板
│   ├── plan-template.md               # 开发计划模板
│   └── design-review-checklist.md     # 设计评审检查清单
│
├── phase-3-implementation/            # Phase 3: 开发实施
│   ├── SKILL.md                       # 阶段技能定义
│   ├── tdd-guide.md                   # TDD 实践指南
│   ├── code-review-guide.md           # 代码审查指南
│   └── systematic-debugging-guide.md  # 系统化调试指南
│
├── phase-4-knowledge/                 # Phase 4: 知识沉淀
│   ├── SKILL.md                       # 阶段技能定义
│   ├── ai-error-notebook-template.md  # AI 错题本模板
│   ├── retrospective-template.md      # 项目回顾模板
│   └── project-context-template.md    # 项目上下文模板
│
├── phase-5-delivery/                  # Phase 5: 交付标准
│   ├── SKILL.md                       # 阶段技能定义
│   ├── delivery-checklist.md          # 交付校验清单
│   └── deliverables-template.md       # 交付物清单模板
│
├── module-7-knowledge-distillation/   # Module 7: 项目知识蒸馏 ⭐ 独创
│   ├── SKILL.md                       # 模块技能定义
│   ├── project-brain-template.md      # 项目大脑模板（核心产物）
│   ├── distillation-process-guide.md  # 蒸馏流程指南
│   └── memory-capture-guide.md        # 记忆捕获指南
│
└── module-8-constraint-analytics/     # Module 8: 约束有效性分析 ⭐ 独创
    ├── SKILL.md                       # 模块技能定义
    ├── constraint-trace-template.md   # 约束追溯记录模板
    ├── iteration-snapshot-template.md # 迭代快照模板
    ├── aggregate-analysis-template.md # 聚合分析报告模板
    └── optimization-loop-guide.md     # 框架优化闭环指南
```

### 阶段流程

```
Phase 0          Phase 1          Phase 2          Phase 3          Phase 4          Phase 5
双向画像  ──→  需求分析  ──→  规划设计  ──→  开发实施  ──→  知识沉淀  ──→  交付标准
  │                │                │                │                │                │
  ▼                ▼                ▼                ▼                ▼                ▼
[Gate 0]         [Gate 1]         [Gate 2]         [Gate 3]         [Gate 4]         [Gate 5]
硬性门控         硬性门控         硬性门控         硬性门控         软性门控         硬性门控

                    ↕ 贯穿全流程 ↕
          ┌─────────────────────────────────┐
          │ Module 7: 项目知识蒸馏（持续成长）  │
          │ Module 8: 约束有效性分析（数据驱动） │
          └─────────────────────────────────┘
```

每个阶段有明确的入口条件、核心活动、必输出物和出口条件。只有通过门控检查后，方可进入下一阶段。

---

## 快速开始

### 使用本框架启动一个新项目

**第一步：加载核心约束**

将 `core/SKILL.md` 的内容提供给 AI，确保 AI 理解并遵循铁律和优先级体系。

**第二步：执行 Phase 0 双向画像**

使用 `phase-0-profiling/` 下的模板，完成使用者画像和 AI 能力画像，制定对齐策略。

**第三步：按阶段推进**

按照 Phase 0 → 1 → 2 → 3 → 4 → 5 的顺序，在每个阶段：
1. 读取对应阶段的 `SKILL.md`
2. 按执行流程逐步完成
3. 使用模板产出必输出物
4. 通过门控检查后进入下一阶段

**第四步：交付验收**

在 Phase 5 使用交付校验清单逐项核查，完成使用者验收后正式交付。

### 核心原则

- **严格顺序**：不可跳过任何阶段
- **门控不可绕过**：未通过门控不得进入下一阶段
- **铁律不可违反**：任何情况下铁律优先级最高
- **文档不可缺失**：每个阶段必须有文档输出

---

## 致谢

- **[Superpowers](https://github.com/DavidHume/react-superpowers)** -- 提供了 AI 编程的核心理念和最佳实践启发
- **[BMad Method](https://github.com/bmadcode/BMAD-METHOD)** -- 提供了结构化的 AI 工作流设计方法论，包括对抗审查、阶段门控、子代理协作等关键机制

本框架在两者的基础上进行了系统性增强，加入了双向画像、AI 错题本、三层约束体系等独创机制，形成了更完整的 AI 编程开发方法论。

---

## 许可证

MIT License
