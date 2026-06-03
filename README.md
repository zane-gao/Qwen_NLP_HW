# Qwen NLP Homework

本仓库是 NLP 课程作业交付项目，主题为 **Qwen 系列大模型技术发展历程**。报告围绕 Qwen 从初代开放中文/中英 LLM，到 Qwen3/Qwen3.5/Qwen3.6、推理模型、多模态模型、代码/数学/长上下文、Embedding/Reranker 与 VLA 等分支的技术演进进行梳理。

## 交付内容

- [主报告 Markdown](docs/qwen_series_technical_evolution.md)：完整技术报告，适合直接在 GitHub 阅读。
- [网页版报告 HTML](docs/qwen_series_technical_evolution.html)：带排版与图片的报告版本，适合本地浏览器打开。
- [课堂展示 Slides](docs/qwen_series_slides.html)：22 页 HTML 幻灯片，适合课堂汇报。
- [来源索引](docs/qwen_source_index.md)：记录外部资料来源、本地图片来源与资料口径。
- [验证记录](docs/VALIDATION_QWEN_REPORT.md)：记录文件检查、图片引用检查、外部链接检查与本地渲染检查。
- [项目交接文档](docs/HANDOFF_QWEN_REPORT.md)：记录后续维护建议和注意事项。

## 快速查看

在 GitHub 上可以直接阅读 Markdown 报告：

- `docs/qwen_series_technical_evolution.md`

如果需要查看排版后的 HTML 版本，可以克隆仓库后在本地打开：

```bash
open docs/qwen_series_technical_evolution.html
open docs/qwen_series_slides.html
```

## 项目结构

```text
.
├── README.md
├── docs/
│   ├── qwen_series_technical_evolution.md
│   ├── qwen_series_technical_evolution.html
│   ├── qwen_series_slides.html
│   ├── qwen_source_index.md
│   ├── VALIDATION_QWEN_REPORT.md
│   ├── HANDOFF_QWEN_REPORT.md
│   └── assets/
│       ├── qwen_figures/
│       └── render_checks/
└── .gitignore
```

## 报告范围

报告重点覆盖以下技术主线：

- 通用 LLM：Qwen、Qwen1.5、Qwen2、Qwen2.5、Qwen3、Qwen3.5、Qwen3.6。
- 效率架构：GQA、MoE、Hybrid Attention、Gated Delta Networks、稀疏激活等。
- 推理与 Agent：QwQ/QVQ、thinking/non-thinking 统一、工具调用与 agentic coding。
- 多模态：Qwen-VL、Qwen-Audio、Qwen2.5-Omni、Qwen3-VL、Qwen3-Omni、Qwen-Image、Qwen-VLA。
- 专用分支：Coder、Math、Embedding、Reranker、ASR、TTS 等。

## 资料与验证

资料优先采用 Qwen 官方博客、QwenLM GitHub、Hugging Face / ModelScope 模型卡和 arXiv 技术报告。来源索引中记录了 60 个外部 URL，并在 2026-06-02 完成可达性检查；本地图片引用和 HTML 渲染也已完成检查，详细结果见 [验证记录](docs/VALIDATION_QWEN_REPORT.md)。

