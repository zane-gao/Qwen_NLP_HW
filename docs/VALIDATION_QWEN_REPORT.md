# Qwen 报告验证记录

验证日期：2026-06-02

## 文件检查

- `docs/qwen_series_technical_evolution.md`：存在，约 28 KB。
- `docs/qwen_series_technical_evolution.html`：存在，约 21 KB。
- `docs/qwen_series_slides.html`：存在，约 29 KB，共 22 页。
- `docs/qwen_source_index.md`：存在，记录 60 个外部 URL 与本地图片来源。
- `docs/HANDOFF_QWEN_REPORT.md`：存在，记录后续维护注意事项。

## 本地资源检查

- 检查 `Markdown`、报告 HTML、slides HTML 中的 `assets/qwen_figures/*` 引用。
- 结果：共检查 54 个本地图片引用，未发现缺失文件。
- 图片目录：`docs/assets/qwen_figures/`，包含 12 张官方图片和 2 张自制 SVG 解释图。

## 外部链接检查

- 对 `docs/qwen_source_index.md` 中 60 个外部 URL 执行 `curl -L --max-time 12` 可达性检查。
- 结果：全部返回 HTTP 200。
- 已覆盖 arXiv、QwenLM GitHub、Qwen 官方博客、Hugging Face、NVIDIA 工程生态补充、官方图片 OSS 地址。

## 浏览器渲染检查

使用本机 Chrome headless 打开本地文件并截图：

- `docs/qwen_series_technical_evolution.html` 首页截图：`docs/assets/render_checks/report_home.png`
- `docs/qwen_series_slides.html#1` 截图：`docs/assets/render_checks/slides_01.png`
- `docs/qwen_series_slides.html#12` 截图：`docs/assets/render_checks/slides_12.png`

结果：

- 截图均生成成功，尺寸为 `1440 x 1000`。
- 报告首页、slides 封面、slides 中间图文页均非空白，图片和文字正常显示。
- Chrome 输出了若干后台 `SSL handshake failed` 日志，属于浏览器后台联网噪声；本地截图文件正常生成。

## 未做项目

- 未导出 PDF，因为原计划默认不做 PDF。
- 未安装 Playwright；Node REPL 环境缺少 `playwright`，已改用本机 Chrome headless 完成渲染检查。
