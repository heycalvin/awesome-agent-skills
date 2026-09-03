# ⚡ Awesome AI Arsenal

<p align="center">
  <b>个人专属全能 AI 资产兵器库 · 智能体技能 (Skills) · 深度对话 · 文生图 · 文生视频</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Status-Active%20%26%20Curated-success?style=flat-square" alt="Status">
  <img src="https://img.shields.io/badge/Agent-Antigravity%20Ready-blue?style=flat-square" alt="Antigravity">
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square" alt="License">
</p>

---

## 📖 目录索引 (Table of Contents)

- [⚡ Awesome AI Arsenal](#-awesome-ai-arsenal)
  - [📖 目录索引 (Table of Contents)](#-目录索引-table-of-contents)
  - [🎯 仓库定位与设计哲学](#-仓库定位与设计哲学)
  - [📂 资产全景速览](#-资产全景速览)
    - [1. 智能体技能库 (Agent Skills)](#1-智能体技能库-agent-skills)
    - [2. 对话与推理提示词 (Chat Prompts)](#2-对话与推理提示词-chat-prompts)
    - [3. 文生图提示词与工具库 (Image Prompts)](#3-文生图提示词与工具库-image-prompts)
    - [4. 生视频提示词与运镜库 (Video Prompts)](#4-生视频提示词与运镜库-video-prompts)
  - [📐 录入与贡献模板 (Templates)](#-录入与贡献模板-templates)
  - [🚀 如何在日常中即插即用](#-如何在日常中即插即用)
    - [在 Antigravity / Coding Agent 中挂载 Skill](#在-antigravity--coding-agent-中挂载-skill)
    - [在日常 Web 对话与生成中复用](#在日常-web-对话与生成中复用)
  - [🤝 贡献指南与版本记录](#-贡献指南与版本记录)

---

## 🎯 仓库定位与设计哲学

这是一个面向生成式 AI 时代打造的**个人高生产力工具库**。拒绝泛滥且不可用的粗糙提示词，坚持以下原则：
1. **模块化与工程化**：将复杂的 Agent 行为拆解为标准可执行的 `SKILL.md`；
2. **结构化与参数化**：生图与生视频提示词均拆解主体、光影、镜头、动态与负向参数，便于灵活替换；
3. **消除“AI味”**：对话类 Prompt 强调逻辑推导深度（First Principles / CoT）与语言质感，远离假大空的排比套话。

---

## 📂 资产全景速览

### 1. 智能体技能库 (Agent Skills)
> 规范详见：[`skills/README.md`](./skills/README.md)

| 技能名称 | 分类 | 适用场景 | 核心文件 |
| :--- | :--- | :--- | :--- |
| **Code Reviewer** | Coding | 架构质量审查、阻断性漏洞/性能缺陷排查、输出 Before/After 方案 | [`skills/coding/code-reviewer/SKILL.md`](./skills/coding/code-reviewer/SKILL.md) |
| *（待录入）* | Research | 竞品分析、论文前沿精读与学术交叉对比 | `skills/research/` |
| *（待录入）* | Productivity | 会议纪要提炼、工作周报结构化生成与 OKR 对齐 | `skills/productivity/` |

---

### 2. 对话与推理提示词 (Chat Prompts)

| 提示词名称 | 分类 | 推荐模型 | 核心特色 | 链接 |
| :--- | :--- | :--- | :--- | :--- |
| **第一性原理深度推演者** | Reasoning | Claude 3.7 / o1 / DeepSeek-R1 | 剥离经验主义，追溯底层物理与事实，推导破坏性创新方案 | [`first-principles-thinker.md`](./prompts/chat/reasoning/first-principles-thinker.md) |
| **顶级科技智库主编润色器** | Writing | Claude 3.5 Sonnet / GPT-4o | 严格剔除 AI 八股文套话，重构呼吸节奏感与词汇质感 | [`editorial-polisher.md`](./prompts/chat/writing/editorial-polisher.md) |

---

### 3. 文生图提示词与工具库 (Image Prompts)

> 🎨 **必备速查表**：[`prompts/image/styles-cheat-sheet.md`](./prompts/image/styles-cheat-sheet.md)（含媒介、光影、镜头焦段、材质高频中英词典）

| 提示词条目 | 适用模型 | 艺术风格 / 构图特点 | 链接 |
| :--- | :--- | :--- | :--- |
| **电影质感叙事肖像** | Midjourney v6.1 | 35mm 阿莱电影机、伦勃朗光影、深邃故事感 | [`cinematic-character-portrait.md`](./prompts/image/midjourney/cinematic-character-portrait.md) |
| **高端时尚编辑纪实摄影** | Flux.1 [dev] | 哥本哈根极简建筑、天然毛孔与羊毛质感、无塑料感 | [`realistic-editorial-photo.md`](./prompts/image/flux/realistic-editorial-photo.md) |

---

### 4. 生视频提示词与运镜库 (Video Prompts)

> 🎬 **运镜必读**：[`prompts/video/camera-movements.md`](./prompts/video/camera-movements.md)（运镜指令、转场、动态控制词典）

| 提示词条目 | 适用模型 | 运镜机制 / 动态特征 | 链接 |
| :--- | :--- | :--- | :--- |
| **赛博朋克雨夜街道穿梭** | 可灵 Kling 1.5 | 低机位贴地向前推进 + 涟漪倒影 + 抬头仰拍天际线 | [`cyberpunk-street-drone-shot.md`](./prompts/video/kling/cyberpunk-street-drone-shot.md) |
| **昼夜交替延时穿梭长镜头** | Runway Gen-3 | 高速向前穿行 + 黄金时刻平滑演变为繁星夜景车流 | [`hyperlapse-cityscape.md`](./prompts/video/runway/hyperlapse-cityscape.md) |

---

## 📐 录入与贡献模板 (Templates)

随时使用预定义的标准模板快速扩展新能力：
- 🛠️ [智能体技能模板 (Agent Skill)](./templates/skill-template/SKILL.md)
- 💬 [对话与文本提示词模板 (Chat Prompt)](./templates/chat-prompt-template.md)
- 🖼️ [文生图提示词模板 (Image Prompt)](./templates/image-prompt-template.md)
- 🎥 [生视频提示词模板 (Video Prompt)](./templates/video-prompt-template.md)

---

## 🚀 如何在日常中即插即用

### 在 Antigravity / Coding Agent 中挂载 Skill
1. 将 `skills/<category>/<skill-name>` 整个目录复制或软链接至你的工作区技能配置中。
2. Agent 将自动在对应任务（如代码审查、深度调研）时激活该技能。

### 在日常 Web 对话与生成中复用
- **复制提示词**：直接打开对应的 Markdown 文件，点击复制提示词区块中的英文/中文内容。
- **变量填充**：将 `{{variable}}` 替换为你的真实上下文内容即可。

---

## 🤝 贡献指南与版本记录

详细录入规范参见：[`CONTRIBUTING.md`](./CONTRIBUTING.md)
- `v0.1.0` (2026-09): 初始化仓库架构，确立分类标准、录入模板、词典速查表与核心示例。
