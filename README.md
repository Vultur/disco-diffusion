# Disco Diffusion V5

<center>

<a href="https://colab.research.google.com/github/Vultur/disco-diffusion/blob/main/Disco_Diffusion.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="在线运行"/></a>

<h2>使用 AI 创作令人震撼的艺术和动画！</h2>

</center>

参数 | 说明 | 默认值
--- | --- | ---
**视觉效果**
`text_prompts` | 文字提示 | N/A
`image_prompts` | 图像提示 | N/A
**图像质量**
`clip_guidance_scale` | 图像相似图 | 1000
`tv_scale` |  图像平滑度 | 150
`range_scale` |  RGB 值范围 | 150
`sat_scale` | 图像饱和度 | 0
`cutn` | 特征提取量 | 16
`cutn_batches` | 梯度积累值  | 2
**初始参数**
`init_image` | 参考图像，支持 URL 或本地路径 | None
`init_scale` |  效果增强，建议的值：1000 | 0
`skip_steps` | 起点步长 | 0
`perlin_init` |  使用噪声 | False
`perlin_mode` |  噪声模式 | 'mixed'
**高级参数**
`skip_augs` | 跳过视觉增强 | False
`randomize_class` | 随机对象类别 | True
`clip_denoised` | 分析图像噪声 | False
`clamp_grad` | 自适应梯度裁剪 | True
`seed` | 设定随机种子 | random_seed
`fuzzy_prompt` | 模糊推导提示 | False
`rand_mag` | 随机噪声振幅 | 0.1
`eta` | DDIM 超参数 | 0.5


**模型设置**
---

参数 | 说明 | 默认值
--- | --- | ---
`timestep_respacing` | 时间跨度 | ddim100
`diffusion_steps` | 扩散步长 | 1000
`clip_models`  | CLIP 模型 | ViT-B/32, ViT-B/16, RN50x4
