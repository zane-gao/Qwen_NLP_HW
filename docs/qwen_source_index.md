# Qwen 系列技术发展历程来源索引

访问日期：2026-06-02。优先级为官方博客、官方 GitHub、Hugging Face / ModelScope 模型卡与 arXiv 技术报告；少量社区/厂商材料仅用于工程生态补充，不作为模型能力结论的唯一依据。

| 主题 | 关键结论 | 主要来源 |
|---|---|---|
| Qwen 初代 | 1.8B/7B/14B/72B，最多 3T 预训练 token，Base/Chat、Int4/Int8、工具使用和长上下文能力 | https://github.com/QwenLM/Qwen ，https://arxiv.org/abs/2309.16609 |
| Qwen-VL | 基于 Qwen-LM 增加视觉 receptor、输入输出接口、三阶段训练，覆盖理解、定位、OCR、多语多模态 | https://arxiv.org/abs/2308.12966 |
| Qwen-Audio | 面向通用音频理解，覆盖语音、自然声音、音乐、歌曲等 30+ 任务 | https://arxiv.org/abs/2311.07919 ，https://qwen-audio.github.io/Qwen-Audio/ |
| Qwen1.5 | 0.5B 到 110B，多尺寸开源；统一 32K 上下文；`transformers>=4.37` 原生支持；AWQ/GPTQ/GGUF/vLLM/SGLang 生态 | https://qwenlm.github.io/blog/qwen1.5/ |
| Qwen1.5-MoE | Qwen 首个 MoE，Qwen1.5-MoE-A2.7B 用约 2.7B 激活参数逼近 7B 模型 | https://qwenlm.github.io/blog/qwen-moe/ |
| Qwen2 | 0.5B/1.5B/7B/72B dense + 57B-A14B MoE；7T 预训练；GQA；最高 128K 上下文；29+ 语言 | https://qwenlm.github.io/blog/qwen2/ ，https://arxiv.org/abs/2407.10671 |
| Qwen2.5 | 0.5B/1.5B/3B/7B/14B/32B/72B；18T 预训练；指令跟随、结构化输出、长文本、代码/数学增强 | https://qwenlm.github.io/blog/qwen2.5/ ，https://arxiv.org/abs/2412.15115 |
| Qwen2.5-1M | 在 128K 基础上通过长上下文预训练/后训练扩展到 1M，上线 7B/14B/ Turbo 等版本 | https://arxiv.org/abs/2501.15383 ，https://qwenlm.github.io/blog/qwen2.5-1m/ |
| Qwen2.5-Coder | 基于 Qwen2.5 架构，代码语料继续预训练，覆盖 0.5B 到 32B，强调 128K、FIM 与代码智能 | https://arxiv.org/abs/2409.12186 ，https://github.com/QwenLM/Qwen2.5-Coder |
| Qwen2.5-Math | CoT + Tool-integrated Reasoning，支持中英数学，发布 Math-RM-72B 奖励模型 | https://arxiv.org/abs/2409.12122 ，https://github.com/QwenLM/Qwen2.5-Math |
| Qwen2-VL / Qwen2.5-VL | 动态分辨率、视频理解、文档/OCR/grounding，Qwen3-VL 进一步加入 Interleaved-MRoPE、DeepStack、文本-时间戳对齐 | https://arxiv.org/abs/2409.12191 ，https://arxiv.org/abs/2502.13923 ，https://github.com/QwenLM/Qwen2.5-VL |
| Qwen2-Audio | 语音聊天和音频分析双模式，DPO 优化事实性和指令遵循 | https://qwenlm.github.io/blog/qwen2-audio/ ，https://arxiv.org/abs/2407.10759 |
| QwQ / QVQ | 从 QwQ-Preview 到 QwQ-32B，强化长 CoT 与 RL 推理；QVQ-72B-Preview 探索视觉推理 | https://qwenlm.github.io/blog/qwq-32b-preview/ ，https://qwenlm.github.io/blog/qwq-32b/ ，https://qwenlm.github.io/blog/qvq-72b-preview/ |
| Qwen2.5-Omni | Thinker-Talker 架构，文本/图像/音频/视频输入，文本和自然语音流式输出，TMRoPE 做音视频时间对齐 | https://github.com/QwenLM/Qwen2.5-Omni ，https://arxiv.org/abs/2503.20215 |
| Qwen3 | Dense + MoE；0.6B 到 235B；thinking/non-thinking 统一；36T 预训练；119 语言；四阶段后训练 | https://qwenlm.github.io/blog/qwen3/ ，https://arxiv.org/abs/2505.09388 |
| Qwen3-Embedding | 0.6B/4B/8B embedding 与 reranker；MRL 支持；指令感知；100+ 语言 | https://github.com/QwenLM/Qwen3-Embedding ，https://arxiv.org/abs/2506.05176 |
| Qwen3-Next | Qwen3-Next-80B-A3B，Hybrid Attention、Gated DeltaNet、超稀疏 MoE，约 3B 激活参数 | https://qwen.ai/blog?id=qwen3-next ，https://huggingface.co/Qwen/Qwen3-Next-80B-A3B-Instruct ，NVIDIA 工程生态补充：https://developer.nvidia.com/blog/new-open-source-qwen3-next-models-preview-hybrid-moe-architecture-delivering-improved-accuracy-and-accelerated-parallel-processing-across-nvidia-platform/ |
| Qwen3-Coder / Coder-Next | 480B-A35B/30B-A3B/Next，面向 agentic coding、浏览器/终端任务、仓库级理解，支持 256K/1M 与 358 编程语言 | https://github.com/QwenLM/Qwen3-Coder ，https://arxiv.org/abs/2603.00729 |
| Qwen-Image | 20B MMDiT 图像基础模型，强调复杂文字渲染、中文文字、图像编辑；后续 2512/2.0 改进真实感与排版 | https://github.com/QwenLM/Qwen-Image ，https://arxiv.org/abs/2508.02324 |
| Qwen3-Omni | 原生端到端多语 omni-modal，MoE Thinker-Talker、AuT 预训练、多 codebook、低延迟语音/视频交互 | https://github.com/QwenLM/Qwen3-Omni ，https://arxiv.org/abs/2509.17765 |
| Qwen3-VL | Dense/MoE、Instruct/Thinking；视觉 agent、空间/视频/文档理解；Interleaved-MRoPE、DeepStack | https://github.com/QwenLM/Qwen3-VL ，https://arxiv.org/abs/2511.21631 |
| Qwen3-ASR | 0.6B/1.7B ASR，52 种语言/方言识别，NAR forced aligner，基于 Qwen3-Omni 音频能力 | https://github.com/QwenLM/Qwen3-ASR ，https://arxiv.org/abs/2601.21337 |
| Qwen3-TTS | 多语、可控、鲁棒、流式 TTS；12.5Hz 16 codebook tokenizer；0.6B/1.7B 级别模型 | https://arxiv.org/abs/2601.15621 ，https://github.com/QwenLM/Qwen3-TTS |
| Qwen-VLA | 基于 Qwen3.5-4B VLM backbone + 1.15B DiT flow-matching action decoder，统一 manipulation/navigation/trajectory | https://github.com/QwenLM/Qwen-VLA ，https://arxiv.org/abs/2605.30280 |

## 本地图片来源

| 本地文件 | 来源类型 | 原始来源 |
|---|---|---|
| `assets/qwen_figures/qwen_technical_timeline.svg` | 自制解释图 | 根据本索引来源整理 |
| `assets/qwen_figures/qwen_architecture_evolution.svg` | 自制解释图 | 根据本索引来源整理 |
| `assets/qwen_figures/qwen1_radar_72b.jpg` | 官方图 | https://github.com/QwenLM/Qwen/blob/main/assets/radar_72b.jpg |
| `assets/qwen_figures/qwen3_base.jpg` | 官方图 | https://qianwen-res.oss-accelerate-overseas.aliyuncs.com/qwen3-base.jpg |
| `assets/qwen_figures/qwen3_post_training.png` | 官方图 | https://qianwen-res.oss-accelerate.aliyuncs.com/assets/blog/qwen3/post-training.png |
| `assets/qwen_figures/qwen25_omni_arch.png` | 官方图 | https://qianwen-res.oss-cn-beijing.aliyuncs.com/Qwen2.5-Omni/overview.png |
| `assets/qwen_figures/qwen3_vl_arch.jpg` | 官方图 | https://qianwen-res.oss-accelerate.aliyuncs.com/Qwen3-VL/qwen3vl_arc.jpg |
| `assets/qwen_figures/qwen3_omni_arch.png` | 官方图 | https://qianwen-res.oss-cn-beijing.aliyuncs.com/Qwen3-Omni/overview.png |
| `assets/qwen_figures/qwen_image_bench.png` | 官方图 | https://qianwen-res.oss-cn-beijing.aliyuncs.com/Qwen-Image/bench.png |
| `assets/qwen_figures/qwen_image_merge.jpg` | 官方图 | https://qianwen-res.oss-cn-beijing.aliyuncs.com/Qwen-Image/merge3.jpg |
| `assets/qwen_figures/qwen25_math_allsize.png` | 官方图 | https://qianwen-res.oss-accelerate-overseas.aliyuncs.com/Qwen2.5/2024-08-qwen2.5-math-allsize.png |
| `assets/qwen_figures/qwen35_397b_score.png` | 官方图 | https://qianwen-res.oss-accelerate.aliyuncs.com/Qwen3.5/Figures/qwen3.5_397b_a17b_score.png |
| `assets/qwen_figures/qwen36_35b_a3b_score.png` | 官方图 | https://qianwen-res.oss-accelerate.aliyuncs.com/Qwen3.6/Figures/qwen3.6_35b_a3b_score.png |
| `assets/qwen_figures/qwen36_27b_score.png` | 官方图 | https://qianwen-res.oss-accelerate.aliyuncs.com/Qwen3.6/Figures/qwen3.6_27b_score.png |
