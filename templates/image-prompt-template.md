# [生图提示词名称 / Image Prompt Name]

> **适用模型**：[如：Midjourney v6.1 / Flux.1 Schnell/Dev / SDXL 1.0]  
> **画面风格**：[如：电影质感肖像 / 赛博朋克概念设计 / 扁平矢量插画 / 3D 渲染]  
> **长宽比例**：[如：16:9 / 9:16 / 1:1 / 3:4]  

---

## 1. 完整提示词 (Full Prompt)

### 英文提示词 (Primary English Prompt)
```text
[主体描述], [场景与环境], [艺术媒介与风格], [光影与色彩氛围], [相机视角与焦段], [高画质修饰词]
```

### 中文释义 (Chinese Translation & Breakdown)
> **主体**：[描述]  
> **环境**：[描述]  
> **风格**：[描述]  
> **光影**：[描述]  
> **构图**：[描述]  

---

## 2. 模型专属参数与设置 (Model Parameters)

### Midjourney 格式
```text
/imagine prompt: [Prompt Text] --ar 16:9 --v 6.1 --style raw --stylize 250
```

### Flux / SD 格式
- **Negative Prompt (负向提示词)**:
  ```text
  lowres, bad anatomy, bad hands, text, error, missing fingers, extra digit, fewer digits, cropped, worst quality, low quality, normal quality, jpeg artifacts, signature, watermark, username, blurry.
  ```
- **Steps**: `25 - 35`
- **CFG Scale / Guidance Scale**: `3.5 - 7.0`
- **Sampler**: `Euler / DPM++ 2M Karras`

---

## 3. 核心关键词拆解与替换建议 (Keyword Variations)

| 维度 | 当前关键词 | 替换备选词汇 | 效果差异 |
| :--- | :--- | :--- | :--- |
| **光影** | volumetric cinematic lighting | golden hour / moody neon / Rembrandt lighting | 由冷峻转温暖/赛博或复古油画感 |
| **镜头** | 85mm f/1.4 lens, shallow depth of field | wide angle 24mm / drone aerial shot | 特写人像虚化 vs 宏大场景展现 |
| **材质** | matte textures, subtle film grain | hyper-glossy / rough canvas / ceramic porcelain | 胶片纪实质感 vs 3D反光或手绘质感 |

---

## 4. 效果预览参考 (Preview & Notes)
- 效果亮点说明：[记录哪些词对画面的影响最显著]
- 避坑提示：[记录容易跑偏或画面崩坏的词]
