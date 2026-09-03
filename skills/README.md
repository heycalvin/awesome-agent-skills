# 智能体技能库 (Agent Skills Library)

本目录收纳各类专为自主智能体（AI Coding Agent / Reasoning Agent）打造的可复用能力模块。

---

## 1. 什么是 Agent Skill？

与普通的“单次对话提示词（Prompt）”不同，**Agent Skill 是一个包含目标、前置感知、多步骤执行规范、质量验证和工具调用指导的完备能力单元**。

每个 Skill 均按照标准格式维护，以 `SKILL.md` 命名，并通过顶部 YAML Frontmatter 声明元数据：

```yaml
---
name: art-split-poster
description: 照片转 3:4 高端编辑海报，上方严格写实保真，下方质感纸张微型手绘与克制排版
---
```

---

## 2. 目录架构

- [`creative/`](./creative/)：图像与视觉生成、创意发散（已收录：[`art-split-poster`](./creative/art-split-poster/)）。
- [`coding/`](./coding/)：代码审查、重构建议、单元测试编写、架构分析等【待补充】。
- [`research/`](./research/)：竞品分析、技术选型推演、学术论文与前沿论文总结等【待补充】。
- [`productivity/`](./productivity/)：会议纪要提炼、工作周报结构化生成、项目看板管理等【待补充】。

---

## 3. 如何安装与激活技能

直接在对话框中向你的 AI Agent 发送指令即可：
> 💬 **“请帮我安装 `skills/creative/art-split-poster` 技能”**

智能体会自动识别宿主环境并挂载到正确目录（如当前工程的 `.agents/skills/` 或全局技能目录）。
