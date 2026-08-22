# OpenAtmos 课程 01 推进归档

Archived: 2026-08-22

## 本轮完成

- 将课程 01 从第一课推进到第二课《大气组成与垂直结构》；
- 建立“干空气近似—水汽与气溶胶—气压/密度—温度趋势—大气分层”的通俗解释链；
- 绘制原创 `atmosphere-layers.svg`，提供 SVG 语义描述和 Markdown 替代文字；
- 建立 `01.01-读懂大气垂直结构` 练习，包含问题、参考解答和概念讲解；
- 将 UCAR、NOAA 和 WMO 的来源及使用边界记录到课程资源文档；
- 更新课程目录、任务状态和本地归档记录。

## 验证

- SVG XML 解析：PASS；
- 课程与练习本地文件存在性：PASS；
- 课程入口和练习路径检查：PASS；
- 尾随空格检查：PASS；
- `git diff --check`：PASS；
- `git diff --cached --check`：PASS；
- `pnpm ai-hero-cli internal lint`：BLOCKED，仓库当前没有 `package.json` 或课程专用 lint 配置；已用上述结构检查作为替代证据。

## 内容边界

本轮没有引入静力学、递减率、稳定度、辐射传输或臭氧化学公式，也没有复制外部图片。后续优先进入“气象要素与观测”，再决定何时加入真实探空数据和 Python 图表。
