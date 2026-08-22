# OpenAtmos 课程 01 第六课推进归档

Archived: 2026-08-22

## 本轮完成

- 新增第六课《时间尺度与空间尺度》；
- 区分时间尺度、空间尺度、时间分辨率、空间分辨率和观测代表性；
- 用局地/小尺度、中尺度、天气/大尺度三个典型层次建立量级直觉，并明确它们不是硬边界；
- 解释小尺度过程可以嵌套在大尺度天气系统中；
- 绘制原创 `time-space-scales.svg`，提供 SVG 语义描述和 Markdown 替代文字；
- 建立 `01.05-为问题选择尺度和资料` 练习，包含合成教学情境、问题、参考解答和概念讲解；
- 将 WMO 全球观测系统、WMO-No. 8 和 UCAR 尺度教材记录到课程资源文档；
- 更新课程目录、任务状态和本地归档记录。

## 验证

- SVG XML 解析：PASS（`xmllint --noout`）；
- 课程、素材与练习文件存在性：PASS；
- 课程与练习本地链接：PASS（检查 32 个目标）；
- 练习 `problem`、`solution`、`explainer` 结构：PASS；
- SVG `title`、`desc`、`role="img"` 和尺度边界文案：PASS；
- 禁止占位文件约定：PASS（无 `.gitkeep`、`speaker-notes.md`）；
- 尾随空格与 `git diff --check`：PASS；
- `pnpm ai-hero-cli internal lint`：BLOCKED，仓库当前没有 `package.json` 或课程专用 lint 配置；已用上述结构、链接、XML 和文案检查作为替代证据。

## 内容边界

本轮没有引入 Rossby 半径、无量纲数、尺度分析方程或真实产品性能比较；练习中的 A/B/C 资料是合成教学情境，不代表真实产品规格。后续进入第七课“从天气现象到资料判读”，把尺度框架用于具体站点图和时间序列。
