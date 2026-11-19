---
name: analysis-patterns-review
description: |
  当用户给出业务需求、对象图、数据模型或接口并要求建模或评审时调用。依据 Fowler《Analysis Patterns》比较候选领域模型，给出适用条件、能击穿现有模型的反例和可执行验收样例。
metadata:
  cangjie.generated-by: cangjie-tools v2.5.0
  cangjie.variant: single
  cangjie.bundle-id: bundle.analysis-patterns-review
  cangjie.capability-count: 12
  cangjie.entrypoint-count: 1
---
# Analysis Patterns: Reusable Object Models — 全书能力入口

## 触发与不触发

**适用**：与本书能力域相关的咨询与任务（见下方路由表的意图列）。
**不适用**：
- 证券买卖建议、实际行情、税率与法律适用。
- 纯翻译、无业务语义的语法查询和排版。

## 核心原则（常驻速览，概览类问题读到这里即可回答）

1. 先摘出用户原有业务词、必须回答的查询及一个具体事件。区分已知事实与需要领域专家裁定的规则。
2. 新设计先试最简单的候选。评审已有设计先用它重演实例，按“发现、失败样例、业务影响、最小改动、验收”记录问题。
3. 按下表取卡。对每个候选列对象及身份、带方向的关系与多重性、时间语义、不变量。比较替代方案并给选用条件。
4. 交付可复核的实例：用给定值走通正常路径，再给会改变设计选择的反例，并写明输入、操作、期望输出。标注章节出处，把自行约定的细节标明。

## 能力路由（先读本表，按意图加载 1 张能力卡）

| 用户意图 | 先读 | 补读/备注 |
|---|---|---|
| 汇报 / 岗位 / 委托的建模或评审 | references/capabilities/accountability.md | references/capabilities/historic-mapping.md |
| 测量 / 单位 / 检查的建模或评审 | references/capabilities/observation.md | references/capabilities/historic-mapping.md |
| 指标 / 汇总 / 分母的建模或评审 | references/capabilities/enterprise-metric.md | references/capabilities/observation.md |
| 同名 / 重档 / 外部编号的建模或评审 | references/capabilities/object-identity.md | references/capabilities/accountability.md |
| 库存 / 复式 / 费用的建模或评审 | references/capabilities/posting.md | references/capabilities/enterprise-metric.md |
| 预约 / 排程 / 取消的建模或评审 | references/capabilities/action-plan.md | references/capabilities/observation.md |
| 组合 / 估值 / 买卖价的建模或评审 | references/capabilities/market-scenario.md | references/capabilities/contract-lifecycle.md |
| 期权 / 产品 / 交割的建模或评审 | references/capabilities/contract-lifecycle.md | references/capabilities/market-scenario.md |
| 模块 / 可见性 / 插件的建模或评审 | references/capabilities/package-visibility.md | references/capabilities/type-template.md |
| 应用层 / 表单 / 前端的建模或评审 | references/capabilities/application-facade.md | references/capabilities/package-visibility.md |
| 动态分类 / 双向关联 / 构造的建模或评审 | references/capabilities/type-template.md | references/capabilities/historic-mapping.md |
| 归属 / 生效区间 / 指定日期的建模或评审 | references/capabilities/historic-mapping.md | references/capabilities/observation.md |

**非能力类查询**：
- 书名/作者/章节/整书概览 → references/overview.md
- 术语解释 → references/glossary.md
- 决策规则速查（不需要原文依据时） → references/cheatsheet.md
- 完整意图与关键词索引（本表未覆盖的意图先查这里） → references/capability-index.md

## 加载规则

- 每次任务先读本文件，再按路由表加载 **1** 张能力卡；任务明确跨域时最多加载 2 张。
- 概览/书名类问题不加载能力卡，用「核心原则」与 overview.md 回答。
- 路由表与 capability-index.md 都无法命中的意图，明确告知超出本书范围，不要硬套。

## 边界与判停

- 只有项目名称时先索取一个业务事件或一张模型图、一个必须回答的问题。
- 缺计量单位、定价条款、有效期或身份认定依据时，列可选分支与最小补问，在已知部分给出有条件的结论。
