# Qwen 报告项目交接

更新时间：2026-06-02

## 当前交付物

- `docs/qwen_series_technical_evolution.md`：主报告 Markdown。
- `docs/qwen_source_index.md`：来源索引与本地图片来源。
- `docs/assets/qwen_figures/`：官方下载图片与自制 SVG。
- 后续待生成：`docs/qwen_series_technical_evolution.html`、`docs/qwen_series_slides.html`。

## 已完成资料核验

- 官方来源优先：Qwen 官方博客、QwenLM GitHub、Hugging Face/ModelScope、arXiv。
- 已核验主线：Qwen、Qwen1.5、Qwen2、Qwen2.5、QwQ/QVQ、Qwen3、Qwen3-Next、Qwen3.5、Qwen3.6。
- 已核验分支：Coder、Math、VL、Audio/ASR/TTS、Omni、Image、VLA、Embedding/Reranker。
- 注意：`QwenLM/Qwen2` 和 `QwenLM/Qwen2.5` 的 README 当前会显示 Qwen3 内容，不能作为 Qwen2/Qwen2.5 的直接来源；应使用官方博客/arXiv/模型卡。

## 素材说明

- 官方图片已下载到 `docs/assets/qwen_figures/`。
- `qwen_technical_timeline.svg` 和 `qwen_architecture_evolution.svg` 是自制解释图。
- 文档图注已标明来源类型和访问日期。

## 后续建议

- 若要更学术：补充每篇 arXiv 的 BibTeX 和更多 benchmark 表。
- 若要做课堂展示：优先完善 `qwen_series_slides.html`，保留 18-24 页。
- 若要交 PDF：先确认 HTML 渲染后，用浏览器打印或 pandoc/markdown-exporter 转出。
