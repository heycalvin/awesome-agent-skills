# 贡献与录入规范 (Contributing Guidelines)

欢迎将你发现的高价值 Agent Skill 或优质 Prompt 收纳进本仓库。为了保持仓库的结构一致性与实用性，请遵守以下录入规范。

---

## 1. 录入原则

1. **真实可用**：所有录入的 Skill 和 Prompt 必须经过实际模型测试验证（附带推荐模型版本与效果）。
2. **结构规范**：统一使用 [`templates/`](./templates/) 目录下的对应模板，不得随意省略关键字段。
3. **分类明确**：
   - **Skill**：面向自主智能体（Agent）的系统能力与指令，必须包含 YAML frontmatter 及明确的操作流程。
   - **Chat Prompt**：面向文本交互、角色设定、逻辑推导、写作与代码辅助。
   - **Image Prompt**：包含主体、风格、光影、媒介、参数（如 `--ar` / steps / cfg）。
   - **Video Prompt**：明确镜头运动、主体运动、帧率、首尾帧或时长要求。
4. **尊重版权**：若引用自公开开源社区或知名创作者，请在文档末尾注明出处链接。

---

## 2. 命名规范

- 文件夹与文件名统一使用全小写英文加中划线（kebab-case），例如：
  - `skills/coding/code-reviewer/SKILL.md`
  - `prompts/chat/reasoning/first-principles-thinker.md`
  - `prompts/image/midjourney/cinematic-character-portrait.md`
  - `prompts/video/kling/cyberpunk-street-drone-shot.md`
- 文档内部一级标题为该技能或提示词的正式名称（可使用中文或英文）。

---

## 3. 模板使用说明

| 类别 | 模板文件 | 说明 |
| :--- | :--- | :--- |
| **Agent Skill** | [`templates/skill-template/SKILL.md`](./templates/skill-template/SKILL.md) | 包含 name, description 及详细工作流 |
| **对话提示词** | [`templates/chat-prompt-template.md`](./templates/chat-prompt-template.md) | 包含角色定义、背景、限制、变量占位符 |
| **生图提示词** | [`templates/image-prompt-template.md`](./templates/image-prompt-template.md) | 包含核心词、风格修饰、参数及负向词 |
| **生视频提示词** | [`templates/video-prompt-template.md`](./templates/video-prompt-template.md) | 包含运镜方式、动态变化、时长与比例 |

---

## 4. 提交步骤

1. 拷贝对应模板至对应的分类目录下。
2. 填写内容并移除占位注释。
3. 在主目录 [`README.md`](./README.md) 的索引表格中追加一行该条目的链接与简述。
4. 提交变更并更新版本记录。
