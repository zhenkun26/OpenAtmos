# GitHub 气象学习资源调研

> 调研日期：2026-08-22

## 调研目的

确认 OpenAtmos 应该重复编写哪些内容，哪些部分可以通过链接复用，并为首期内容路线选择可靠的外部入口。

## 主要观察

### 1. 工程工作流可以作为项目内约定

[mattpocock/skills](https://github.com/mattpocock/skills) 提供可复制到项目内的 Agent skills，并通过 `setup-matt-pocock-skills` 配置 issue tracker、triage 标签和领域文档布局。OpenAtmos 已将它作为项目内工作流使用，而不是把气象内容交给外部 skill 代写。

### 2. ECMWF 的训练仓库适合作为资料实践入口

[ECMWF training](https://github.com/stewartchrisecmwf/training) 以 Jupyter Notebook 组织 C3S 和 CAMS 的气候、大气资料教程，覆盖数据访问和分析案例，并在仓库中声明 Apache-2.0 许可证。它适合在 OpenAtmos 的“资料与数据实践”章节中作为延伸入口。

### 3. MetPy 适合作为气象 Python 工具入口

[Unidata/MetPy](https://github.com/Unidata/MetPy) 将气象数据读取、可视化和计算组织成 Python 工具，仓库声明 BSD-3-Clause 许可证，并面向研究者、教育者和气象分析脚本使用者。OpenAtmos 可以解释“为什么要做某种计算”，再把具体工具链接到 MetPy。

### 4. 国内业务工具提供了应用气象的连接点

[NMC-WFT/nmcdev](https://github.com/nmcdev) 汇总了 MICAPS、卫星云图、天气雷达、天气图绘制、预报检验和雷达处理等项目。它们更偏业务和工程，不应被当作入门课程，但可以作为应用气象和中国业务资料的后续实践入口。

### 5. 基础概念仍然需要 OpenAtmos 自己组织

[NOAA NCEI 的 Weather vs. Climate 文章](https://www.ncei.noaa.gov/news/weather-vs-climate) 和 [NOAA Ocean Service 的解释](https://oceanservice.noaa.gov/facts/weather_climate.html) 都强调：天气描述具体时间和地点的大气状态，气候描述较长时间尺度上的典型状态和统计特征。它们可以作为事实核验来源，但中文学习路径、术语关联和练习设计仍需要由 OpenAtmos 自己完成。

## 对 OpenAtmos 的决定

1. 核心知识用原创中文解释，不复制外部仓库的整篇文档。
2. 外部项目只承担工具、课程、数据和权威解释的入口角色。
3. 每个外部链接都写明“它是什么、适合什么时候用、OpenAtmos 为什么推荐”。
4. 首期从概念区分开始，再逐步连接到观测资料和 Python 实践。
5. 资源调研结果落到内容路线，而不是单独维护一个没有学习顺序的链接清单。

## 来源清单

- [mattpocock/skills](https://github.com/mattpocock/skills)
- [ECMWF training](https://github.com/stewartchrisecmwf/training)
- [Unidata/MetPy](https://github.com/Unidata/MetPy)
- [NMC-WFT/nmcdev](https://github.com/nmcdev)
- [NOAA NCEI: What’s the Difference Between Weather and Climate?](https://www.ncei.noaa.gov/news/weather-vs-climate)
- [NOAA Ocean Service: What is the difference between weather and climate?](https://oceanservice.noaa.gov/facts/weather_climate.html)
