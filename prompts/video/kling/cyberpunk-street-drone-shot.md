# 赛博朋克雨夜街道低空穿梭镜头 (Cyberpunk Street Drone Shot)

> **适用模型**：可灵 Kling 1.5 / 1.0 (文生视频 / 图生视频)  
> **模式**：文生视频 (Text-to-Video) 或 图生视频 (Image-to-Video)  
> **运镜重点**：低机位平滑推进 + 贴地飞行穿梭 + 霓虹水洼倒影动态  

---

## 1. 结构化提示词 (Structured Prompt)

### 中文提示词（可灵推荐中文直出）
```text
电影级低机位向前极速平滑推进，摄像机贴近湿漉漉的黑色沥青路面。细雨淅淅沥沥落下，路面水洼中泛起密集的同心圆涟漪，倒映着两侧高耸摩天楼闪烁的品红与青色霓虹广告牌。镜头平稳穿越一处水洼，溅起轻微水花，随后顺势微微上仰抬头（Tilt Up），展现远处悬浮穿梭的飞行汽车与雨雾缭绕的赛博未来都市天际线。画面运动平滑连贯，电影级景深虚化，无镜头晃动畸变。
```

### 英文提示词 (English Prompt)
```text
Low-angle cinematic forward tracking shot, camera skimming inches above wet asphalt street in a rain-soaked cyberpunk metropolis. Delicate raindrops causing ripples in puddles reflecting magenta and cyan holographic billboards. Smooth motion passes through neon reflections then seamlessly tilts up to reveal towering futuristic skyscrapers with flying vehicles gliding through misty volumetric fog. Smooth 24fps motion, anamorphic lens flare, sharp reflections, zero glitch.
```

---

## 2. 可灵参数与操作技巧

- **创意想象力 (Creativity)**：`0.4 - 0.5`（文生视频时保持结构稳定）
- **运动幅度**：`4 - 5`（过大容易导致建筑物边缘扭曲拉扯）
- **图生视频技巧**：如果使用图生视频，首帧请选择地面积水倒影清晰、景深层次丰富的高清概念图，提示词直接重点写“运镜轨迹与雨水涟漪动态”即可。
