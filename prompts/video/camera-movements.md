# 视频生成运镜与动态控制速查表 (Video Camera Movements Cheat Sheet)

在 AI 视频生成（Kling、Runway Gen-3、Luma Dream Machine、Sora、海螺 AI）中，精准的镜头语言是让静态画面产生专业电影感的核心手段。

---

## 1. 经典运镜指令 (Camera Movements)

| 指令 (Prompt Term) | 中文术语 | 运动方式与电影感效果 |
| :--- | :--- | :--- |
| `Push In / Dolly In` | 慢推镜头 | 摄像机平缓向前推进靠近主体，强化紧张感或聚焦心理细节 |
| `Pull Out / Dolly Out` | 慢拉镜头 | 摄像机平缓向后退远，揭示主体所处的宏大环境或孤独感 |
| `Pan Left / Pan Right` | 左右摇镜 | 摄像机机位不动，镜头水平向左/右旋转扫过场景 |
| `Tilt Up / Tilt Down` | 上下俯仰 | 摄像机机位固定，垂直向上抬头或向下低头扫视 |
| `Pedestal Up / Down` | 垂直升降 | 摄像机整体垂直升高或下降，不同于俯仰，透视随高度变化 |
| `Tracking Shot / Follow Shot`| 跟随运镜 | 镜头始终锁定跟随移动的主体（背后跟随、侧面伴随、前方倒退） |
| `Orbit Shot / 360 Arc` | 环绕运镜 | 围绕静止或微动的主体进行 360 度或半弧度平滑旋转拍摄 |
| `Roll / Dutch Angle` | 荷兰角旋转 / 倾斜 | 镜头沿光轴轴向旋转倾斜，营造眩晕、失控、梦境或不安感 |
| `FPV Drone Shot` | 穿越机视角 | 极速穿梭、俯冲拉起、贴地低空飞行的极具动感的第一视角 |

---

## 2. 景别演变与运镜组合 (Transitions & Dynamics)

通过组合复合指令，可以让 5s-10s 的视频呈现丰富的叙事节奏：

1. **从环境到焦点 (Establishing to Close-up)**:
   > `Starts with wide aerial drone view of the misty valley, smooth rapid dive down into a medium close-up of a lone wanderer.`
2. **伴随式探索 (Side tracking with parallax)**:
   > `Side tracking shot moving alongside a vintage car driving along the coastal highway at sunset, camera keeps pace with foreground guardrail motion blur.`
3. **希区柯克变焦 (Dolly Zoom / Vertigo Effect)**:
   > `Dolly zoom effect, camera moves forward while zooming out, background warps and expands while subject face remains constant size.`

---

## 3. 动态控制关键修饰词 (Motion Modifiers)

- **速度控制**:
  - `slow-motion 120fps`: 升格慢动作，适合水滴飞溅、发丝飘逸、爆炸冲击波。
  - `hyperlapse / timelapse`: 延时摄影，适合云卷云舒、车水马龙、昼夜交替。
  - `fluid smooth handheld motion`: 带有呼吸感的自然手持微晃，增强临场真实感。
- **避免画面崩坏的约束词**:
  - `smooth motion, temporal consistency, stable anatomy, no warping, cinematic shutter speed 180 degree, zero flickering`.
