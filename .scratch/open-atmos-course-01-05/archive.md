# OpenAtmos 课程 01 第五课推进归档

Archived: 2026-08-22

## 本轮完成

- 新增第五课《水汽、云与降水的入门图景》；
- 建立“水汽来源 → 上升和冷却 → 饱和 → 凝结或凝华 → 粒子增长 → 降水可能”的入门过程链；
- 明确区分水汽、云和降水，并解释有云不一定有地面降水；
- 引入雨幡（virga）作为“降水粒子可能在到达地面前蒸发”的边界案例；
- 绘制原创 `water-vapor-cloud-precipitation.svg`，提供 SVG 语义描述和 Markdown 替代文字；
- 建立 `01.04-从水汽到降水` 练习，包含合成教学数据、问题、参考解答和概念讲解；
- 将 WMO International Cloud Atlas、WMO 云与降水定义、UCAR 和 NWS 入门资料记录到课程资源文档；
- 更新课程目录、任务状态和本地归档记录。

## 验证

- SVG XML 解析：PASS（`xmllint --noout`）；
- 课程、素材与练习文件存在性：PASS；
- 课程与练习本地链接：PASS（检查 28 个目标）；
- 练习 `problem`、`solution`、`explainer` 结构：PASS；
- SVG `title`、`desc`、`role="img"` 和边界文案：PASS；
- 禁止占位文件约定：PASS（无 `.gitkeep`、`speaker-notes.md`）；
- 尾随空格与 `git diff --check`：PASS；
- `pnpm ai-hero-cli internal lint`：BLOCKED，仓库当前没有 `package.json` 或课程专用 lint 配置；已用上述结构、链接、XML 和文案检查作为替代证据。

## 内容边界

本轮没有引入云微物理完整公式、真实雷达/卫星数据或降水数值模拟；合成时间序列只用于训练“观察事实—机制推断—进一步证据”的区分。后续继续进入时间尺度和空间尺度，再决定何时接入真实资料判读。
