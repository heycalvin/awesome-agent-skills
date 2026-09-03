# 昼夜交替延时穿梭长镜头 (Hyperlapse Cityscape Day-to-Night)

> **适用模型**：Runway Gen-3 Alpha  
> **模式**：文生视频 (Text-to-Video)  
> **运镜重点**：高速平滑向前推进 (Fast Forward Dolly) + 昼夜光影平滑演变  

---

## 1. 结构化提示词 (Runway Gen-3 Prompt)

```text
[Camera Movement]: Fast and smooth forward hyperlapse tracking shot flying along a bustling metropolitan boulevard between glass skyscrapers.
[Lighting & Time Evolution]: Seamless temporal transition from late golden hour sunset into starry twilight and vibrant deep-night neon illuminations.
[Motion Dynamics]: Streaking trails of long-exposure headlights and taillights flowing in rapid motion below, clouds sweeping across the sky, windows of skyscrapers gradually lighting up one by one.
[Atmosphere & Quality]: Photorealistic architectural details, crystalline reflections in glass facades, 8k cinematic masterpiece, continuous fluid motion without flickering or jump cuts.
```

---

## 2. Runway Gen-3 提示词编写要诀

- **明确指定摄像机动作**：Runway Gen-3 对 `Camera Movement`、`Lighting`、`Atmosphere` 的四段式结构识别极其敏锐。
- **避免多动作冲突**：在一个 5s 或 10s 的片段中，运镜方向最好保持单一矢量（如纯前进或纯升镜），避免同时要求“左转又右看又后退”。
