# 高端时尚编辑纪实摄影 (Realistic Editorial Fashion Photo)

> **适用模型**：Flux.1 [dev] / Flux.1 [schnell]  
> **画面风格**：纪实街拍时尚大片、自然采光、高真实度织物纹理  
> **长宽比例**：`3:4` 或 `4:5` (标准杂志排版画幅)  

---

## 1. 提示词 (Flux Prompt)

### 完整英文提示词
```text
An authentic medium shot candid photograph of a stylish 28-year-old Scandinavian man in an oversized charcoal wool coat and cream cable-knit sweater, walking past a modernist brutalist concrete museum in Copenhagen. Overcast diffuse northern daylight, subtle mist in the cold air, crisp focus on the textured wool fabric and natural skin pores, neutral candid facial expression. Hasselblad medium format camera aesthetic, 50mm lens at f/2.8, high dynamic range with preserved shadow details, no plastic smoothing, raw candid color grading.
```

### 提示词解析 (Flux 自然语言技巧)
- **Flux 特征**：Flux 对长句自然语言具有极佳的理解力，因此不需要 SD 时代的逗号堆砌式 Tag，直接使用具备主谓宾与环境逻辑的完整英文长句即可。
- **质感控制**：使用 `crisp focus on the textured wool fabric and natural skin pores` 以及 `no plastic smoothing` 可有效避免 AI 生成人物常见的“塑料假人感”。

---

## 2. 推荐生成参数

- **Steps**: `28 - 32` (Dev) / `4 - 8` (Schnell)
- **Guidance Scale (CFG)**: `3.5` (Flux 推荐较低的 guidance scale 以保持写实逼真度)
- **Resolution**: `896 x 1152` (约 100 万像素，符合 3:4 比例)
