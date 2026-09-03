# `dev-architecture-first`（架构优先决策预检）

- **所属大类**：💻 代码工程（Coding）
- **技能配置**：[`skills/coding/dev-architecture-first`](../skills/coding/dev-architecture-first/SKILL.md)
- **原始出处**：Adapted from [doublesq97-ui/su-architecture-first](https://github.com/doublesq97-ui/su-architecture-first) by [@doublesq97-ui](https://github.com/doublesq97-ui) (MIT License)

---

## 📌 是干什么的

一个面向编码 Agent 的**轻量级架构决策预检机制**。在 Agent 动手改动代码前，引导其先厘清真实目标、所属层次、唯一事实源（Source of Truth）与证据，杜绝“头痛医头、脚痛医脚”的补丁累积。

<p align="center">
  <img src="./assets/dev-architecture-first/hero.webp" width="100%" alt="dev-architecture-first 架构优先总览" />
</p>

### 核心决策脉络
```text
真实目标 (Goal) -> 现有相关结构 -> 归属层与根因 (Ownership & Root Cause)
                -> 变更分类 (Change Class) -> 下一步行动 -> 验证证据 (Validation)
```

### 两种预检深度
1. **轻量预检 (Quick pass)**：对明确、局部的改动，快速确认真实目标、责任对象与验收验证后直接开工，不做多余流程纠缠；
2. **完整预检 (Full pass)**：遇到复发故障、跨层改动、事实源冲突或高风险重构时，全面展开责任层追溯与回归设计，查明结构性根因。

---

## 💬 怎么用

在向 Agent 提出编码、Bug 排查或重构需求时，加入关键词即可触发：

### 常用触发词示例
- 💬 *“以**架构优先**的方式，帮我重构用户权限验证逻辑”*
- 💬 *“使用 `dev-architecture-first` 分析为什么这个状态会偶发不同步”*
- 💬 *“架构优先预检：为现有系统接入多模型路由模块，评估对既有架构的影响”*

---

## 📚 内置工程参考指南 (References)

技能包内自带 5 套实战架构规范指引（位于 `skills/coding/dev-architecture-first/references/`）：
- **分层模型与事实源 (`layer-model.md`)**：如何划分系统层次、维护唯一权威事实源；
- **结构性故障诊断 (`structural-diagnosis.md`)**：如何排查复发问题与打补丁导致的逻辑泄露；
- **变更类型划分 (`change-types.md`)**：清晰区分删除、重构、实现、隐藏与 UI 修饰；
- **回归与验收设计 (`regression-design.md`)**：改动前定义明确的边界与验证证据；
- **AI 工作台设计原则 (`ai-workbench.md`)**：Agent 系统、多智能体交互与工作流闭环规范。
