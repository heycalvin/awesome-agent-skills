# [提示词名称 / Prompt Name]

> **分类**：[Reasoning / Writing / Coding / Roleplay / System Prompt]  
> **推荐模型**：[如：Claude 3.7 Sonnet / GPT-4o / Gemini 1.5 Pro / DeepSeek-R1]  
> **设计模式**：[如：Few-Shot / Chain-of-Thought / Role-Goal-Constraint]  

---

## 1. 核心提示词 (Prompt Text)

```markdown
# Role
你是一位[专业角色描述，如：资深全栈架构师、专业学术论文审稿人]。

# Background / Context
[提供必要的背景信息，说明为什么要做这件事，目标受众是谁]。

# Objectives / Goals
1. [核心目标 1]
2. [核心目标 2]

# Constraints & Rules
- [约束条件 1，如：严禁包含任何推测性无根据事实]
- [约束条件 2，如：使用 Markdown 表格呈现对比结果]
- [语气与风格：专业、精炼、无废话]

# Input Variables
- `{{input_content}}`: [用户待处理的主体文本]
- `{{target_audience}}`: [目标受众/输出受众]

# Output Format
严格按照以下格式输出：
### 1. 核心总结
...
### 2. 深度分析
...
### 3. 行动建议
...
```

---

## 2. 变量说明与使用指引 (Variables & Instructions)

| 变量名 | 类型 | 必填 | 说明 |
| :--- | :--- | :--- | :--- |
| `{{input_content}}` | Text | 是 | 传入待分析或重写的文本 |
| `{{target_audience}}` | String | 否 | 默认为“技术负责人”或自定义受众 |

---

## 3. 测试用例与实测效果 (Test Case & Output)

### 测试输入 (User Input)
```
[用于测试的实际输入数据]
```

### 实际生成效果 (Result Sample)
```
[模型生成的优质效果快照]
```
