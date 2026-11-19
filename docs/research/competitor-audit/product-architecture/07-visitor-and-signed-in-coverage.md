# 五家 Desktop Web 游客与登录后可见范围

用同一套任务对照 Axiom、DeBot、GMGN、FOMO、LogEarn。OBS 表示实见页面、入口或提示，DOC 表示官方资料，UNVERIFIED 表示缺少可用会话或操作证据。「入口可见」只证明控件显示。连接外部钱包、平台自带钱包、注册身份和订阅等级需分别确认。

| 产品与样本 | 游客可见（OBS） | 游客访问边界（OBS） | 登录后可见范围与证据 |
| --- | --- | --- | --- |
| **Axiom** · 独立游客与已有 Chrome 登录会话 | 官网页内 Features、Execution、Rewards、FAQ、Docs 与认证入口 [官网](screenshots/a01.jpg) | 游客打开官网给出的 Discover 链接后回到官网。Start trading 打开认证 [认证](screenshots/a18.jpg) | **OBS** 终端七项为探索、Pulse、监控、永续、预测、投资组合、奖励。可见 Token 图表、活动、持有者入口、买卖、钱包筛选、用户设置入口和通知面板。跟踪创建、通知落点、免费/付费差异未验证 [终端](screenshots/a07.jpg) · [详情](screenshots/a08.jpg) · [投资组合](screenshots/a14.jpg) · [通知](screenshots/a16.jpg) |
| **DeBot** · 游客 | AI 信号、战壕、行情、监控管理框架、喊单、Token 图表/活动、搜索和底栏配置。合约另开新标签，公开可见盘口与个人区域框架 [现货](screenshots/d20.jpg) · [监控](screenshots/d22.jpg) · [合约](screenshots/d21.jpg) | 自选、资产、奖励及 Token 持仓分析触发登录。喊单关注选项禁用。游客延时一小时为页面声明，实际延时未测 [自选](screenshots/d14.jpg) · [资产](screenshots/d16.jpg) · [Holder](screenshots/d05.jpg) · [喊单](screenshots/d17.jpg) | **UNVERIFIED** 无已登录样本。优先复测持仓分析、钱包追踪创建、喊单关注、订单历史、设置、套餐与通知深链 |
| **GMGN** · 游客 | 战壕、热门、Token Holder、喊单、牛人榜、AI、搜索及公开永续盘口 [热门](screenshots/g06.jpg) · [Holder](screenshots/g07.jpg) · [喊单](screenshots/g19.jpg) · [永续](screenshots/g20.jpg) | Holder 地址的新标签和喊单作者路由出现登录提示。资产和收藏需登录，钱包跟单明确要求私钥账号，个人永续仓位提示连接钱包 [钱包](screenshots/g08.jpg) · [作者](screenshots/g25.jpg) · [自选](screenshots/g21.jpg) · [跟单](screenshots/g24.jpg) | **UNVERIFIED** 无已登录样本。应分同一账号登录、连接测试钱包和私钥账号三种条件核对提示是否解除 |
| **FOMO** · 游客 | 公开官网、市场总览及榜单、币种价格、永续介绍、资源及帮助 [市场](screenshots/f09.jpg) · [价格](screenshots/f06.jpg) · [帮助](screenshots/f08.jpg) | 官网和永续 CTA 进入 Apple/Google 认证。样本价格页 Buy CTA 进入 App 下载弹窗 [官网认证](screenshots/f03.jpg) · [永续认证](screenshots/f18.jpg) · [价格 CTA](screenshots/f07.jpg) | **DOC** 指南描述社交动态、排行榜和通知，官网描述网页永续。**UNVERIFIED** 登录后的真实主导航、交易、持仓、钱包、通知和深链 [指南](screenshots/f17.jpg) · [永续介绍](screenshots/f14.jpg) |
| **LogEarn** · 内置浏览器低状态样本与已有 Chrome 钱包状态 | **OBS** 内置浏览器可见九个顶栏入口、战壕、信号、市场、Token 的 Holder 等页签、策略入口、帮助及资产页空钱包视图 [战壕](screenshots/l03.jpg) · [信号](screenshots/l02.jpg) · [Token](screenshots/l10.jpg) · [资产](screenshots/l05.jpg) | **UNVERIFIED** 低状态样本顶部余额为零，但也显示充值和账户安全面板。当前采样无法用此判断游客身份，需用全新隔离配置和明确身份标识复测 | **OBS** 已有 Chrome 会话的 Token 页面出现钱包选择与账户余额控件；套餐和注册状态未确认，账户数值未归档。**UNVERIFIED** 真正匿名基线、正式登录前后权限增量、创建追踪与通知跳转 |

## 补齐登录后的统一流程

1. 用合法可用的测试账号，在同一类 Desktop 环境下分别记录根域、未认证状态、首次认证后的工作台和钱包连接状态。Axiom 已有登录态只作为旧样本，仍需按同一流程复跑。
2. 每家逐项核对发现与搜索、Token/Holder、钱包详情、追踪、交易准备、持仓、社交、通知、账户设置和帮助。每个功能记录可见、可点击、可读、可执行四层以及触发权限时的提示。覆盖公开站与交易终端的互跳，FOMO 分开计。
3. 用可用免费账号先统一对照。付费、托管钱包、私钥账号和外接钱包作为单独的权限层。任何未进入的目标保留 UNVERIFIED，禁止从文档推断实际授权。
4. 把样本 URL、截图和点击路径回填到本表及对应独立报告。对照研究只查看与走到安全预览，不需要真实交易。

当前依赖 DeBot、GMGN、FOMO 的可用既有测试会话，以及 LogEarn 的可确认匿名与登录样本。完成上述补测前，本页为可见范围与证据缺口清单。
