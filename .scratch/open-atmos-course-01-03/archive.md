# OpenAtmos 课程 01 第三课推进归档

Archived: 2026-08-22

## 本轮完成

- 新增第三课《气象要素与观测》；
- 建立“天气感觉 → 气象要素 → 观测平台 → 完整记录”的通俗解释链；
- 解释温度、气压、湿度、风和降水的入门含义，并区分要素、现象和平台；
- 绘制原创 `weather-elements-observation.svg`，提供 SVG 语义描述和 Markdown 替代文字；
- 建立 `01.02-把天气变成观测记录` 练习，包含虚构练习数据、问题、参考解答和概念讲解；
- 将 WMO、NOAA、NWS 和 UCAR 的观测资料记录到课程资源文档；
- 更新课程目录、任务状态和本地归档记录。

## 验证

- SVG XML 解析：PASS；
- 课程、练习与归档文件存在性：PASS；
- 课程入口和练习路径检查：PASS；
- 练习 `problem`、`solution`、`explainer` 结构：PASS；
- 尾随空格检查：PASS；
- `git diff --check`：PASS；
- `pnpm ai-hero-cli internal lint`：BLOCKED，仓库当前没有 `package.json` 或课程专用 lint 配置；已用上述结构检查作为替代证据。

## 内容边界

本轮没有引入湿度公式、露点推导、仪器校准、误差传播或真实数据下载。后续优先进入“温度、气压与风的初步联系”，再决定何时引入公开站点时间序列和 Python 绘图脚本。
