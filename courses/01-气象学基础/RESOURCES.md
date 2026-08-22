# 01 气象学基础：资源与教学方法调研

> 本文件记录课程 01 当前采用的教学方法、外部资源和待验证事项。链接是学习入口，不替代 OpenAtmos 自己的解释。

## 结论摘要

当前项目内最适合直接复用的教学 skills 是：

- `teach`：适合设定学习目标、维护资源、编写短课、使用检索练习和沉淀学习记录；
- `scaffold-exercises`：适合把课程按章节、题目、解答和讲解拆开；
- `research`：适合把外部资料核验后写成带来源的 Markdown 调研；
- `prototype`：适合在正式铺开前试做一张图、一个交互或一个课程切片。

本仓库当前没有专门的 `academic-figure` 或“论文作图” skill。系统提供的 `visualize` 更适合交互式可视化和探索工具，不等于论文图表的可复现生产流程。因此本轮先写下作图规范，等数据实践路线确定后，再单独创建项目 skill。

## 教学方法：先采用，后验证

### 1. 检索练习与间隔复习

每篇课文结束时先让学习者合上页面回答问题，再展开答案。后续单元开头回收前几篇的一个旧问题，形成低成本的间隔复习和交错复习。

- [Carpenter, Pan & Butler (2022), *The science of effective learning with spacing and retrieval practice*](https://www.nature.com/articles/s44159-022-00089-1)：综述间隔学习、检索练习及学习者对学习策略的判断；
- [McDermott (2021), *Practicing Retrieval Facilitates Learning*](https://pubmed.ncbi.nlm.nih.gov/33006925/)：综述检索练习如何支持之后的记忆提取。

在 OpenAtmos 中的落法：每课 2—3 道短题，答案放在折叠区或下一段；新课不只讲新内容，也回收旧概念。题目优先问“如何判断”和“为什么”，不只问术语背诵。

### 2. 分段、提示和图文邻近

图不是越多越好。每张图先回答一个学习问题，正文中的指代词要能直接找到图中的对应位置，颜色不能成为唯一编码方式。用标题、箭头、局部高亮和短标签把注意力引向必要信息。

- [Mayer (2017), *Using multimedia for e-learning*](https://onlinelibrary.wiley.com/doi/full/10.1111/jcal.12197)：总结多媒体学习中的连贯、提示、空间邻近、分段和预训练等设计原则；
- [Fiorella & Mayer (2021), *Five Strategies for Optimizing Instructional Materials*](https://pmc.ncbi.nlm.nih.gov/articles/7940870/)：讨论多媒体原则、分散注意、冗余、提示和分段对教学材料设计的启发。

在 OpenAtmos 中的落法：第一课用一张关系图解释“天气—气候—大气科学—应用气象”的边界，而不是在正文中堆四个定义。

### 3. 先看一个完整例子，再逐步放手

基础学习者面对数据或公式时，先看一个完整、带解释的例子，再做一个只缺少一步的练习，最后独立完成类似问题。这样可以把注意力放在气象意义上，避免一开始被无关的操作细节淹没。

- [van Gog & Rummel (2010), *Example-Based Learning*](https://doi.org/10.1007/s10648-010-9134-7)：综述示例学习何时有助于概念理解、程序学习和迁移；
- [van Gog, Paas & Sweller (2010), *Cognitive Load Theory: Advances in Research on Worked Examples, Animations, and Cognitive Load Measurement*](https://link.springer.com/article/10.1007/s10648-010-9145-4)：讨论示例、分段和管理认知负荷的关系。

在 OpenAtmos 中的落法：后续“资料判读”单元先给一张已标注的站点时间序列，再让学习者自己指出峰值、变化和可能的资料限制。

## 气象领域资源

| 资源 | 适合做什么 | 使用边界 |
| --- | --- | --- |
| [NOAA NCEI：Weather vs. Climate](https://www.ncei.noaa.gov/news/weather-vs-climate) | 为第一课的天气/气候区分提供官方入门解释 | OpenAtmos 自己组织中文脉络，不复制原文 |
| [NOAA Ocean Service：Weather and Climate](https://oceanservice.noaa.gov/facts/weather_climate.html) | 给初学者补充天气与气候的长期统计视角 | 适合作为延伸阅读，不替代课程练习 |
| [NOAA JetStream：The Atmosphere](https://prod-01-alb-www-noaa.woc.noaa.gov/jetstream/atmosphere) | 核对干空气近似组成、水汽变化和气压背景 | 数字以近似和资料页面的限定条件为准 |
| [UCAR：What’s in the Air?](https://scied.ucar.edu/learning-zone/air-quality/whats-in-the-air) | 解释水汽、气溶胶和微量气体为什么不能完全忽略 | 采用概念和原始链接，不复用其图件 |
| [UCAR：Layers of Earth’s Atmosphere](https://scied.ucar.edu/learning-zone/atmosphere/layers-earths-atmosphere) | 核对对流层、平流层等层次的入门特征 | 高度范围保留“约”和纬度/季节差异 |
| [UCAR：Change in the Atmosphere with Altitude](https://scied.ucar.edu/learning-zone/atmosphere/change-atmosphere-altitude) | 解释气压、密度和温度随高度的变化 | 用于概念校验，不把示意剖面当作实测数据 |
| [UCAR：Exploring the Atmosphere with Weather Balloons](https://scied.ucar.edu/learning-zone/atmosphere/weather-balloons) | 将垂直结构连接到探空观测和气球膨胀现象 | 作为第二课的现象入口 |
| [UCAR：How We Study the Atmosphere](https://scied.ucar.edu/learning-zone/atmosphere/how-we-study) | 连接地面观测、原位观测、卫星和模式资料 | 用于第三课的平台比较，不把不同资料混为观测 |
| [WMO-No. 8：Guide to Instruments and Methods of Observation](https://community.wmo.int/site/knowledge-hub/programmes-and-initiatives/instruments-and-methods-of-observation-programme-imop/guide-instruments-and-methods-of-observation-wmo-no-8) | 核对温度、气压、湿度、地面风、降水和观测系统的规范主题 | 作为专业延伸入口，不在基础课中展开全部技术细节 |
| [NOAA：Weather observations](https://prod-01-alb-www-noaa.woc.noaa.gov/office-education/outreach-communication/science-olympiad/2026-meteorology) | 为初学者说明温度、湿度、降水、气压和风是常用观测变量 | 教学页面，正式数据仍需回到具体站点和数据文档 |
| [NWS：Upper Air Observations](https://www.weather.gov/chs/upperair) | 说明探空可获取温度、风、相对湿度和气压的垂直资料 | 只作为平台理解入口，不替代探空数据说明 |
| [NOAA JetStream：Origin of Wind](https://prod-01-alb-www-noaa.woc.noaa.gov/jetstream/synoptic/origin-of-wind) | 解释等压线、压力梯度和风速的入门联系 | 将“线密风强”作为线索，不当作精确预报公式 |
| [NWS：Pressure Gradient Force](https://www.weather.gov/jkl/education) | 补充压力梯度力、地转偏向和近地面风的关系 | 课程只取入门层面的力和限制条件 |
| [Met Office：Wind Flow](https://weather.metoffice.gov.uk/learn-about/weather/how-weather-works/high-and-low-pressure/wind-flow) | 用气球类比说明压力差，并解释真实风受地转偏向影响 | 作为概念延伸阅读，不复制页面图片 |
| [WMO：International Cloud Atlas](https://cloudatlas.wmo.int/en/home.html) | 核对云、降水和其他水成物的术语、分类与专业定义 | 作为权威查词入口，OpenAtmos 自己组织中文解释，不复制图件 |
| [WMO：Clouds](https://cloudatlas.wmo.int/en/clouds.html) | 核对云由悬浮的微小液态水粒子和/或冰粒子组成的入门定义 | 用于第五课概念边界，不延伸到完整云微物理 |
| [WMO：Falling particles and precipitation](https://cloudatlas.wmo.int/hydrometeors-falling-particles.html) | 区分云中悬浮粒子、下落粒子、降水和雨幡等现象 | 用于第五课的“云不等于地面降水”边界 |
| [UCAR：Making Raindrops](https://scied.ucar.edu/kids/clouds-raindrops/making-raindrops) | 用初学者语言解释凝结核、小水滴增长和雨滴形成 | 采用过程线索，不复用页面插图 |
| [NWS：Basic Weather Education](https://www.weather.gov/jkl/education) | 回顾蒸发、上升冷却、饱和、凝结、云和降水的基础过程链 | 作为入门复习入口，具体观测仍需回到站点和仪器资料 |
| [ECMWF training](https://github.com/stewartchrisecmwf/training) | 进入气候、再分析资料和 Jupyter Notebook 实践 | 先从课程导航进入，不默认读者已有数据基础 |
| [MetPy](https://github.com/Unidata/MetPy) | 后续用 Python 读取、计算和可视化气象变量 | 它是工具库，不是从零开始的气象学教材；以仓库当前许可证为准 |
| [NMC-WFT/nmcdev](https://github.com/nmcdev) | 了解中国气象业务中的资料、绘图、雷达和检验工具 | 先说明数据和业务背景，再决定是否引入具体模块 |

## 作图资源

- [Matplotlib 官方文档：颜色](https://matplotlib.org/stable/users/explain/colors/colors.html)：颜色表示、透明度和可读性基础；
- [Matplotlib 官方文档：样式与 rcParams](https://matplotlib.org/stable/users/explain/customizing.html)：把字体、线宽、色板和版式写进可复用样式；
- [Matplotlib 官方示例：模拟色觉差异](https://matplotlib.org/stable/gallery/user_interfaces/mplcvd.html)：检查图表是否过度依赖颜色；
- [xarray 官方文档](https://docs.xarray.dev/en/stable/)：面向带坐标的多维气象数据；
- [Cartopy 官方文档](https://cartopy.readthedocs.io/latest/)：地图投影、海岸线和地理坐标；
- [MetPy 官方文档](https://unidata.github.io/MetPy/latest/)：气象单位、诊断计算和专业绘图辅助。

## 还需要验证的问题

1. 课程是否需要同时提供“纯阅读路径”和“Python 实践路径”，还是先完成一条再扩展？
2. 南京及江苏案例优先使用哪些开放、稳定、可引用的数据源？
3. 课程图表的中文字体、移动端尺寸和无障碍替代文字如何统一测试？
4. 学习者完成短题后，哪些题目真的能区分“记住术语”和“理解关系”？

本轮暂不把这些问题假设成已解决的规范，后续以试读反馈和可复现实验补充。
