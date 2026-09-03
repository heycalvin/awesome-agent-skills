# [生视频提示词名称 / Video Prompt Name]

> **适用模型**：[如：Kling 1.5 (快手可灵) / Runway Gen-3 Alpha / Luma Dream Machine / Sora / Hailuo (海螺AI)]  
> **模式**：[文生视频 (Text-to-Video) / 图生视频 (Image-to-Video)]  
> **推荐时长与帧率**：[如：5s / 10s, 24fps / 30fps]  
> **画面比例**：[如：16:9 / 9:16]  

---

## 1. 结构化提示词 (Structured Video Prompt)

### 英文提示词 (Standard English Prompt)
```text
[Camera Movement]: [e.g., Slow cinematic push-in shot, low-angle tracking]
[Subject & Initial State]: [e.g., A cybernetic samurai standing under rainy neon billboards]
[Subject Action & Motion Dynamics]: [e.g., Slowly turns head towards the camera, rain droplets splashing on armor]
[Atmospheric Lighting & Environment Change]: [e.g., Flickering holographic ads casting cyan and magenta reflections]
[Temporal Consistency / Ending]: [e.g., Smooth fluid motion, cinematic motion blur, 4k ultra-realistic]
```

### 中文格式（适用于可灵/海螺等国产模型）
```text
【运镜】：低机位缓慢向前推进，跟随主体平移
【主体】：一名身穿黑色风衣的年轻男子，站在雨夜潮湿的街头
【动作变化】：从背对镜头缓缓侧身转头，眼神从冷漠变为警惕，风衣下摆随微风摆动
【环境动态】：路面积水倒映着远处霓虹招牌的闪烁光芒，细雨在灯光下形成微光粒子
【画质要求】：电影级景深虚化，无鬼影畸变，平滑自然动态
```

---

## 2. 运镜与控制参数 (Camera & Generation Parameters)

| 参数项 | 推荐值 | 说明 |
| :--- | :--- | :--- |
| **Camera Motion (运镜)** | `Pan Right`, `Zoom In`, `Pedestal Down` 等 | 控制摄像机空间轨迹 |
| **Motion Strength (运动幅度)** | `3 - 5` (中等) | 过大容易画面变形或肢体撕裂，过小则接近静止 |
| **End Frame (尾帧控制)** | 支持 / 不支持 | 图生视频若有目标尾帧可大幅提升连贯度 |
| **Negative Prompt** | `morphing, flickering, distorted faces, sudden cuts, glitch, static image` | 减少突变、鬼影与抽搐 |

---

## 3. 实测要点与踩坑记录 (Observations & Tips)
- **图生视频首帧要求**：[首帧画质与主体清晰度如何影响生成结果]
- **常见问题处理**：[如人物动作太大导致的面部失真，如何通过降低运动幅度或增加约束解决]
