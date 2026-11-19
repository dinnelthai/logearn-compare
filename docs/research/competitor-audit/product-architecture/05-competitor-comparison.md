# 四家 Desktop Web 产品架构对照

本页保留原始采样口径。用户提供会话后的新增实测见[五家登录后补验](07-visitor-and-signed-in-coverage.md#登录后补验)。

## 比较口径

| 产品 | 本轮身份 | 可比较的证据 | 权限边界 |
| --- | --- | --- | --- |
| Axiom | 游客官网 + 已有登录会话 | 公开入口与签入终端结构 | 账号套餐和外部钱包连接未知 |
| DeBot | 游客 | 公开现货和永续工作台、详情与工具 | 个人数据和部分分析受限 |
| GMGN | 游客 | 公开市场、详情、喊单、永续及搜索 | 钱包目标、作者、个人资产和跟单部分受限 |
| FOMO | 游客 | 公开市场、学习内容和认证入口 | 登录后终端未进入 |

下表中，OBS 指实际看到的界面或走过的路径，DOC 指官方描述，未验证代表缺少证据。一级数只统计当时主导航，排除 Logo、搜索、链切换、认证和工具按钮。FOMO 的官网数量与三家终端数量不可直接比较。打开目标路由与访问目标数据分开记录。无同身份、同任务的计时测试。

## 统一分类与层级

**分类标准**以用户任务为轴。以下四种层级独立于功能类别，一个类别可以对应多个层级。L1 是主导航目的地，L2 是页面内部的分类、页签或功能分区，OBJ 是以 Token、钱包或人物为主键的详情，GLOBAL 是跨页面搜索、快捷浮层、账户和帮助入口。公开站以「公开」标注，权限未知记为 **UNVERIFIED**。可见入口和成功操作分别说明。**OBS** 是实际验证，**DOC** 是官方资料，**INFER** 是据此推断。单元格同时涉及受限页面时，OBS 仅覆盖实见入口与反馈。

| 统一类别 | Axiom | DeBot | GMGN | FOMO 公开站 | FOMO 交易终端 |
| --- | --- | --- | --- | --- | --- |
| 发现与行情 | OBS · L1 探索、Pulse；L2 热门、趋势、雷达及生命周期列 [证据](screenshots/a07.jpg) | OBS · L1 AI 信号、战壕、行情；L2 热门、趋势、新币、主题 [证据](screenshots/d02.jpg) | OBS · L1 战壕、热门；L2 精选、新币、蓝筹、热搜 [证据](screenshots/g06.jpg) | OBS · L1 加密货币、Meme；L2 市值、涨跌、新币 [证据](screenshots/f09.jpg) | UNVERIFIED · 登录后发现首页及层级 |
| 代币分析与现货 | OBS · OBJ Token；L2 图表、活动、持有者入口与买卖面板 [证据](screenshots/a08.jpg) | OBS · OBJ Token；L2 活动、分析与买卖。持仓分析遇登录 [证据](screenshots/d05.jpg) | OBS · OBJ Token；L2 活动、持有人与买卖区 [证据](screenshots/g07.jpg) | OBS · OBJ 价格详情；L2 市场统计、相似币、App 下载弹窗 [证据](screenshots/f07.jpg) | UNVERIFIED · 下单、Holder 及详情布局 |
| 钱包研究与监控 | OBS · L1 监控；L2 钱包动态和扫描入口。扫描结果未验证 [证据](screenshots/a11.jpg) | OBS · L1 监控；L2 动向、管理、备注及提醒配置。钱包详情未知 [证据](screenshots/d22.jpg) | OBS · L1 监控、追踪；L2 钱包/社媒；OBJ 钱包路由遇登录 [证据](screenshots/g08.jpg) · [追踪](screenshots/g12.jpg) | OBS · GLOBAL 帮助中心有钱包与账户栏目 [证据](screenshots/f08.jpg) | UNVERIFIED · 钱包研究、个人钱包与追踪入口 |
| 衍生品与自动执行 | OBS · L1 永续、预测；L2 盘口、订单面板及事件列表。独立 AI 策略未验证 [永续](screenshots/a12.jpg) · [预测](screenshots/a13.jpg) | OBS · L1 合约及跟单；合约开新标签。L2 订单表、历史与跟单记录 [合约](screenshots/d21.jpg) · [跟单](screenshots/d10.jpg) | OBS · L1 合约、跟单；L2 永续仓位、钱包跟单与狙击。GLOBAL AI/OpenAPI [合约](screenshots/g20.jpg) · [跟单](screenshots/g24.jpg) · [AI](screenshots/g16.jpg) | OBS · L1 永续介绍；CTA 打开认证 [证据](screenshots/f18.jpg) | DOC · 官网描述网页永续订单管理与持仓。实际终端层级未验证 [证据](screenshots/f14.jpg) |
| 社交与通知 | OBS · L2 探索内喊单、主播；GLOBAL 用户菜单通知。通知深链未验证 [主播](screenshots/a06.jpg) · [通知](screenshots/a16.jpg) | OBS · L1 喊单；OBJ 卡片到 Token，作者外链；L2 监控提醒。独立通知中心未验证 [喊单](screenshots/d17.jpg) · [提醒](screenshots/d22.jpg) | OBS · L1 喊单；OBJ 卡片到 Token，作者目标遇登录 [喊单](screenshots/g19.jpg) · [作者](screenshots/g25.jpg) | OBS · GLOBAL 页脚社交指南 [证据](screenshots/f17.jpg) | DOC · 动态、排行榜、通知。导航位置、深链和作者页未验证 [证据](screenshots/f17.jpg) |
| 自有资产与账户 | OBS · L1 投资组合、奖励；L2 现货、钱包等；GLOBAL 设置入口 [资产](screenshots/a14.jpg) · [账户](screenshots/a15.jpg) | OBS · L1 资产、奖励；GLOBAL 登录。游客遇认证 [资产](screenshots/d16.jpg) · [登录](screenshots/d19.jpg) | OBS · L1 资产、奖励；GLOBAL 登录和收藏。游客资产遇认证 [资产](screenshots/g13.jpg) · [收藏](screenshots/g21.jpg) | OBS · GLOBAL Apple/Google 认证、帮助 [认证](screenshots/f03.jpg) · [帮助](screenshots/f08.jpg) | UNVERIFIED · 资产、持仓、钱包管理、设置和身份权限 |
| 全局查找与工作台 | OBS · GLOBAL 代币/合约搜索、底部快捷工具 [证据](screenshots/a07.jpg) | OBS · GLOBAL 代币/钱包搜索弹层与底栏布局。搜索结果和配置持久化未验证 [搜索](screenshots/d24.jpg) · [布局](screenshots/d27.jpg) | OBS · GLOBAL 搜索弹层返回同名币，钱包/KOL 查询结果未验证 [证据](screenshots/g23.jpg) | OBS · GLOBAL 帮助文章搜索；公开首页未见 Token/钱包全局搜索 [证据](screenshots/f08.jpg) | UNVERIFIED · 全局搜索、快捷工具和工作台设置 |

## 可以作出的判断

| 问题 | 当前判断（INFER） | 判断边界 |
| --- | --- | --- |
| 产品架构谁更清楚 | **Axiom 是已观察交易终端中的首选参考。** 主导航把发现、盯盘、交易品类和资产分开，探索吸收多个发现视图 | 评价可见分类。Axiom 是登录态，FOMO 终端未知，不能判定四家整体第一 |
| 功能分类谁最合理 | **Axiom 更适合作为一级分类参考，DeBot 更适合作为监控内部分类参考。** DeBot 管理页把对象和提醒放一起，GMGN 的监控、追踪、跟单有术语重叠 | 评价分组语义，不涉及账号套餐、功能覆盖率 |
| 导航谁最高效 | **GMGN 的已验证跨对象链最强。** 榜单到 Token、Holder、钱包均有实际入口，喊单也直达 Token。Axiom 的榜单到分析和交易准备同页 | GMGN 钱包落点遇登录。缺少同身份、同任务的点击/时间数据，整体速度无法排名 |
| 哪些设计适合 LogEarn | 按任务归类发现入口，保留 Token 与信号上下文，把钱包名单与提醒放同一工作区 | 逐项对应到实际页面，见 [LogEarn 架构映射](06-logearn-architecture-recommendations.md) |

## 下一阶段注册体验统一条件

1. 每家用同一 Desktop 浏览器版本和视窗、同一地区条件、各自独立的干净浏览器配置。统一语言、起点为官方根域、无邀请参数、无现有 Cookie、无连接钱包，先录游客基线。无法对齐的条件单独记录。
2. 分两条路径测试。各自默认注册入口作为生态差异记录。各家共同支持的认证方式才进入同方法横评。没有共同方式时按方法分组。使用获准的全新测试身份，记录从 CTA 到首个可用工作台的点击数、时间、校验、条款、错误和回退。
3. 按身份逐层留证。游客、刚注册未存款、连接测试钱包、免费使用、合法可用付费方案分别记录。注册状态和免费套餐是两个字段。钱包连接和平台托管钱包分别记。各层重复相同任务，记录入口是否显示、是否可点、是否可读、是否可执行。
4. 登录成功后测同一组闭环：发现 → Token → Holder → 钱包 → 追踪；行情 → 交易准备；通知 → 对象。报告登录后的首屏和权限差异。未达目标记阻断节点，独立记录新标签、返回、筛选恢复、操作次数及完成时间。以读页面和订单预览为止。
