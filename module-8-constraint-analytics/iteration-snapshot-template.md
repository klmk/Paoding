# 迭代快照模板

> **使用说明**：每次项目/模块迭代完成后，将本迭代中所有约束追溯记录汇总为一份快照。快照是聚合分析的数据输入。
> **填写要求**：统计数据必须基于本迭代中所有约束追溯记录的汇总，不得编造或估算。

---

## 一、迭代基本信息

| 字段 | 内容 |
|------|------|
| **项目名称** | （填写项目名称） |
| **迭代号** | （填写迭代号，如 Sprint 1、v1.2 等） |
| **开始日期** | （格式：YYYY-MM-DD） |
| **结束日期** | （格式：YYYY-MM-DD） |
| **功能范围** | （简要描述本次迭代包含的功能/模块） |
| **团队规模** | （参与本次迭代的 AI 代理/人员数量） |
| **快照生成日期** | （格式：YYYY-MM-DD） |

---

## 二、约束调用统计表

以下表格汇总本迭代中所有约束的调用情况。

### 表格结构说明

| 列名 | 填写说明 |
|------|---------|
| **约束编号** | 约束的唯一标识 |
| **约束名称** | 约束的简短名称 |
| **约束分类** | 铁律 / 红旗 / 反模式 / 补强规则 / 流程规则 / 模板规则 |
| **约束来源文件** | 约束定义所在的文件路径 |
| **触发次数** | 本迭代中该约束被触发的总次数 |
| **适用场景数** | 本迭代中该约束适用的场景总数（触发次数 + 未触发但适用的场景数） |
| **触发率** | 触发次数 / 适用场景数（百分比） |
| **平均效果评分** | 所有追溯记录中该约束综合评分的平均值 |
| **最高评分** | 该约束在本迭代中的最高综合评分 |
| **最低评分** | 该约束在本迭代中的最低综合评分 |

### 统计数据

| 约束编号 | 约束名称 | 约束分类 | 约束来源文件 | 触发次数 | 适用场景数 | 触发率 | 平均效果评分 | 最高评分 | 最低评分 |
|---------|---------|---------|-------------|---------|-----------|--------|------------|---------|---------|
| IL-1 | 需求铁律 | 铁律 | `core/iron-laws.md` | | | | | | |
| IL-2 | 测试铁律 | 铁律 | `core/iron-laws.md` | | | | | | |
| IL-3 | 审查铁律 | 铁律 | `core/iron-laws.md` | | | | | | |
| IL-4 | 验证铁律 | 铁律 | `core/iron-laws.md` | | | | | | |
| IL-5 | 文档铁律 | 铁律 | `core/iron-laws.md` | | | | | | |
| IL-6 | 追溯铁律 | 铁律 | `core/iron-laws.md` | | | | | | |
| AP-R01 | "需求已经很清楚了" | 反模式 | `core/anti-patterns.md` | | | | | | |
| AP-R02 | "这个需求跟之前的项目类似" | 反模式 | `core/anti-patterns.md` | | | | | | |
| AP-R03 | "用户会告诉我们需要什么" | 反模式 | `core/anti-patterns.md` | | | | | | |
| AP-R04 | "需求文档太重了" | 反模式 | `core/anti-patterns.md` | | | | | | |
| AP-D01 | "设计太简单不需要文档" | 反模式 | `core/anti-patterns.md` | | | | | | |
| AP-D02 | "先用最简单的方式实现" | 反模式 | `core/anti-patterns.md` | | | | | | |
| AP-D03 | "这个技术栈我最熟悉" | 反模式 | `core/anti-patterns.md` | | | | | | |
| AP-D04 | "设计评审可以省掉" | 反模式 | `core/anti-patterns.md` | | | | | | |
| AP-C01 | "太简单不需要测试" | 反模式 | `core/anti-patterns.md` | | | | | | |
| AP-C02 | "先写完功能再补测试" | 反模式 | `core/anti-patterns.md` | | | | | | |
| AP-C03 | "这个边界条件不太可能发生" | 反模式 | `core/anti-patterns.md` | | | | | | |
| AP-C04 | "先复制这段代码" | 反模式 | `core/anti-patterns.md` | | | | | | |
| AP-C05 | "注释太多了影响可读性" | 反模式 | `core/anti-patterns.md` | | | | | | |
| AP-V01 | "我已经手动测试过了" | 反模式 | `core/anti-patterns.md` | | | | | | |
| AP-V02 | "这个改动不会影响其他模块" | 反模式 | `core/anti-patterns.md` | | | | | | |
| AP-V03 | "代码风格问题不重要" | 反模式 | `core/anti-patterns.md` | | | | | | |
| AP-V04 | "这个 TODO 以后再处理" | 反模式 | `core/anti-patterns.md` | | | | | | |
| AP-F01 | "应该可以了" | 反模式 | `core/anti-patterns.md` | | | | | | |
| AP-F02 | "剩下的都是小问题" | 反模式 | `core/anti-patterns.md` | | | | | | |
| AP-F03 | "用户没提这个要求" | 反模式 | `core/anti-patterns.md` | | | | | | |
| AP-F04 | "差不多就行了" | 反模式 | `core/anti-patterns.md` | | | | | | |
| AP-F05 | "交付了就完成任务了" | 反模式 | `core/anti-patterns.md` | | | | | | |
| ... | （其他模块特定约束） | ... | ... | | | | | | |

> 根据实际项目涉及的约束补充上表。

---

## 三、高频约束 TOP 10

按触发次数降序排列，列出本迭代中触发次数最多的 10 条约束。

| 排名 | 约束编号 | 约束名称 | 约束分类 | 触发次数 | 触发率 | 平均效果评分 |
|------|---------|---------|---------|---------|--------|------------|
| 1 | | | | | | |
| 2 | | | | | | |
| 3 | | | | | | |
| 4 | | | | | | |
| 5 | | | | | | |
| 6 | | | | | | |
| 7 | | | | | | |
| 8 | | | | | | |
| 9 | | | | | | |
| 10 | | | | | | |

---

## 四、低频/未触发约束清单

列出本迭代中触发率低于 20% 或触发次数为 0 的约束。

| 序号 | 约束编号 | 约束名称 | 约束分类 | 触发次数 | 触发率 | 未触发原因分析 |
|------|---------|---------|---------|---------|--------|--------------|
| 1 | | | | 0 | 0% | |
| 2 | | | | 0 | 0% | |
| 3 | | | | | | |
| 4 | | | | | | |
| 5 | | | | | | |

**未触发原因分类：**
- **场景不适用**：本次迭代的功能范围不涉及该约束的适用场景
- **已被其他规则覆盖**：该约束的功能已被其他规则替代
- **约束描述不清晰**：约束描述不够具体，难以判断是否触发
- **约束已过时**：约束描述的场景在当前项目中已不存在
- **被主动跳过**：开发过程中主动跳过了该约束（需记录原因）

---

## 五、约束分类汇总

按约束分类统计本迭代的整体情况。

| 约束分类 | 约束总数 | 触发约束数 | 未触发约束数 | 平均触发率 | 平均效果评分 |
|---------|---------|-----------|-------------|-----------|------------|
| 铁律 | | | | | |
| 红旗 | | | | | |
| 反模式 | | | | | |
| 补强规则 | | | | | |
| 流程规则 | | | | | |
| 模板规则 | | | | | |
| **合计** | | | | | |

---

## 六、本次迭代发现

### 6.1 特别有价值的规则

（列出本迭代中效果评分最高的约束，说明为什么有价值）

| 约束编号 | 约束名称 | 效果评分 | 价值说明 |
|---------|---------|---------|---------|
| | | | |
| | | | |

### 6.2 有问题的规则

（列出本迭代中效果评分低或触发率异常的约束，说明问题所在）

| 约束编号 | 约束名称 | 效果评分 | 问题描述 |
|---------|---------|---------|---------|
| | | | |
| | | | |

### 6.3 新增规则建议

（基于本次迭代的经验，建议新增的规则）

| 建议规则名称 | 适用场景 | 规则描述 | 预期效果 |
|-------------|---------|---------|---------|
| | | | |
| | | | |

### 6.4 其他发现

（任何值得记录的观察、趋势或异常）

1.
2.
3.

---

## 七、JSON 数据格式

以下 JSON 格式用于数据归档和后续聚合分析。每次迭代快照必须同时生成此 JSON 文件。

```json
{
  "snapshot_meta": {
    "project_name": "",
    "iteration_id": "",
    "start_date": "",
    "end_date": "",
    "feature_scope": "",
    "team_size": 0,
    "generated_at": ""
  },
  "constraint_stats": [
    {
      "constraint_id": "IL-1",
      "constraint_name": "需求铁律",
      "constraint_category": "铁律",
      "source_file": "core/iron-laws.md",
      "trigger_count": 0,
      "applicable_scenarios": 0,
      "trigger_rate": 0.0,
      "avg_effect_score": 0.0,
      "max_effect_score": 0,
      "min_effect_score": 0
    }
  ],
  "top_constraints": [
    {
      "rank": 1,
      "constraint_id": "",
      "constraint_name": "",
      "constraint_category": "",
      "trigger_count": 0,
      "trigger_rate": 0.0,
      "avg_effect_score": 0.0
    }
  ],
  "low_frequency_constraints": [
    {
      "constraint_id": "",
      "constraint_name": "",
      "constraint_category": "",
      "trigger_count": 0,
      "trigger_rate": 0.0,
      "reason": ""
    }
  ],
  "category_summary": [
    {
      "category": "铁律",
      "total_constraints": 0,
      "triggered_constraints": 0,
      "untriggered_constraints": 0,
      "avg_trigger_rate": 0.0,
      "avg_effect_score": 0.0
    }
  ],
  "findings": {
    "high_value_rules": [],
    "problematic_rules": [],
    "new_rule_suggestions": [],
    "other_findings": []
  }
}
```

### JSON 字段说明

| 字段路径 | 类型 | 说明 |
|---------|------|------|
| `snapshot_meta` | Object | 迭代元信息 |
| `snapshot_meta.project_name` | String | 项目名称 |
| `snapshot_meta.iteration_id` | String | 迭代号 |
| `snapshot_meta.start_date` | String | 开始日期（YYYY-MM-DD） |
| `snapshot_meta.end_date` | String | 结束日期（YYYY-MM-DD） |
| `snapshot_meta.feature_scope` | String | 功能范围描述 |
| `snapshot_meta.team_size` | Integer | 团队规模 |
| `snapshot_meta.generated_at` | String | 快照生成时间（ISO 8601） |
| `constraint_stats` | Array | 约束调用统计数组 |
| `constraint_stats[].constraint_id` | String | 约束编号 |
| `constraint_stats[].constraint_name` | String | 约束名称 |
| `constraint_stats[].constraint_category` | String | 约束分类 |
| `constraint_stats[].source_file` | String | 约束来源文件 |
| `constraint_stats[].trigger_count` | Integer | 触发次数 |
| `constraint_stats[].applicable_scenarios` | Integer | 适用场景数 |
| `constraint_stats[].trigger_rate` | Float | 触发率（0.0-1.0） |
| `constraint_stats[].avg_effect_score` | Float | 平均效果评分（1.0-5.0） |
| `constraint_stats[].max_effect_score` | Integer | 最高评分 |
| `constraint_stats[].min_effect_score` | Integer | 最低评分 |
| `top_constraints` | Array | 高频约束 TOP10 |
| `low_frequency_constraints` | Array | 低频/未触发约束 |
| `low_frequency_constraints[].reason` | String | 未触发原因 |
| `category_summary` | Array | 分类汇总 |
| `findings` | Object | 发现与建议 |
| `findings.high_value_rules` | Array | 高价值规则 |
| `findings.problematic_rules` | Array | 有问题的规则 |
| `findings.new_rule_suggestions` | Array | 新增规则建议 |
| `findings.other_findings` | Array | 其他发现 |

---

## 八、数据归档

| 归档项 | 说明 |
|--------|------|
| **Markdown 文件名** | `snapshot-{项目名}-{迭代号}.md` |
| **JSON 文件名** | `snapshot-{项目名}-{迭代号}.json` |
| **归档目录** | 项目的 `module-8-constraint-analytics/snapshots/` 目录 |
| **索引更新** | 归档后更新 `snapshots/index.json` 索引文件 |
