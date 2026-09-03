# 智能体技能库 (Agent Skills Library)

本目录收纳各类专为自主智能体（AI Coding Agent / Reasoning Agent）打造的可复用能力模块。

---

## 1. 什么是 Agent Skill？

与普通的“单次对话提示词（Prompt）”不同，**Agent Skill 是一个包含目标、前置感知、多步骤执行规范、质量验证和工具调用指导的完备能力单元**。

每个 Skill 均按照标准格式维护，以 `SKILL.md` 命名，并通过顶部 YAML Frontmatter 声明元数据：

```yaml
---
name: code-reviewer
description: 审查拉取请求或特定代码文件的架构质量、潜在Bug与安全漏洞
---
```

---

## 2. 目录架构

- [`coding/`](./coding/)：代码审查、重构建议、单元测试编写、架构分析。
- [`research/`](./research/)：竞品分析、技术选型推演、学术论文与前沿论文总结。
- [`creative/`](./creative/)：分镜脚本推演、品牌文案调性统一、创意发散。
- [`productivity/`](./productivity/)：会议纪要提炼、工作周报结构化生成、项目看板管理。

---

## 3. 在不同平台中加载与使用

### 在 Antigravity 中加载
将对应的 Skill 目录软链接或复制到全局技能目录（`~/.gemini/antigravity/skills/`）或当前项目的 `.agent/skills/` 中，系统会自动感知并按需激活。

### 在 Claude Projects / Custom GPTs 中使用
直接将 `SKILL.md` 的内容拷贝为 Project Knowledge 或 Custom GPT Instruction 中的对应模块，实现即挂即用。
