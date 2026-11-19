# 五家 Desktop Web 游客与登录后可见范围

用同一套任务对照 Axiom、DeBot、GMGN、FOMO、LogEarn。OBS 表示实见页面、入口或提示，DOC 表示官方资料，UNVERIFIED 表示缺少可用会话或操作证据。「入口可见」只证明控件显示。连接外部钱包、平台自带钱包、注册身份和订阅等级需分别确认。

| 产品与样本 | 游客可见（OBS） | 游客访问边界（OBS） | 登录后可见范围与证据 |
| --- | --- | --- | --- |
| **Axiom** · 独立游客与已有 Chrome 登录会话 | 官网页内 Features、Execution、Rewards、FAQ、Docs 与认证入口 [官网](screenshots/a01.jpg) | 游客打开官网给出的 Discover 链接后回到官网。Start trading 打开认证 [认证](screenshots/a18.jpg) | **OBS** 终端七项为探索、Pulse、监控、永续、预测、投资组合、奖励。可见 Token 图表、活动、持有者入口、买卖、钱包筛选、用户设置入口和通知面板。跟踪创建、通知落点、免费/付费差异未验证 [终端](screenshots/a07.jpg) · [详情](screenshots/a08.jpg) · [投资组合](screenshots/a14.jpg) · [通知](screenshots/a16.jpg) |
| **DeBot** · 游客 | AI 信号、战壕、行情、监控管理框架、喊单、Token 图表/活动、搜索和底栏配置。合约另开新标签，公开可见盘口与个人区域框架 [现货](screenshots/d20.jpg) · [监控](screenshots/d22.jpg) · [合约](screenshots/d21.jpg) | 自选、资产、奖励及 Token 持仓分析触发登录。喊单关注选项禁用。游客延时一小时为页面声明，实际延时未测 [自选](screenshots/d14.jpg) · [资产](screenshots/d16.jpg) · [Holder](screenshots/d05.jpg) · [喊单](screenshots/d17.jpg) | **OBS** 已补验资产、监控入口和同一 Token 持仓分析。见下方登录后补验 |
| **GMGN** · 游客 | 战壕、热门、Token Holder、喊单、牛人榜、AI、搜索及公开永续盘口 [热门](screenshots/g06.jpg) · [Holder](screenshots/g07.jpg) · [喊单](screenshots/g19.jpg) · [永续](screenshots/g20.jpg) | Holder 地址的新标签和喊单作者路由出现登录提示。资产和收藏需登录，钱包跟单明确要求私钥账号，个人永续仓位提示连接钱包 [钱包](screenshots/g08.jpg) · [作者](screenshots/g25.jpg) · [自选](screenshots/g21.jpg) · [跟单](screenshots/g24.jpg) | **OBS** 已补验同一钱包路由、资产和追踪页。见下方登录后补验 |
| **FOMO** · 游客 | 公开官网、市场总览及榜单、币种价格、永续介绍、资源及帮助 [市场](screenshots/f09.jpg) · [价格](screenshots/f06.jpg) · [帮助](screenshots/f08.jpg) | 官网和永续 CTA 进入 Apple/Google 认证。样本价格页 Buy CTA 进入 App 下载弹窗 [官网认证](screenshots/f03.jpg) · [永续认证](screenshots/f18.jpg) · [价格 CTA](screenshots/f07.jpg) | **OBS** 已补验 Discover、Token、Leaderboard 和 Feed。**DOC** 官网另描述网页永续与通知 [指南](screenshots/f17.jpg) · [永续介绍](screenshots/f14.jpg) |
| **LogEarn** · 内置浏览器低状态样本与已有 Chrome 钱包状态 | **OBS** 内置浏览器可见九个顶栏入口、战壕、信号、市场、Token 的 Holder 等页签、策略入口、帮助及资产页空钱包视图 [战壕](screenshots/l03.jpg) · [信号](screenshots/l02.jpg) · [Token](screenshots/l10.jpg) · [资产](screenshots/l05.jpg) | **UNVERIFIED** 低状态样本顶部余额为零，但也显示充值和账户安全面板。当前采样无法用此判断游客身份，需用全新隔离配置和明确身份标识复测 | **OBS** 已有 Chrome 会话的 Token 页面出现钱包选择与账户余额控件；套餐和注册状态未确认，账户数值未归档。**UNVERIFIED** 真正匿名基线、正式登录前后权限增量、创建追踪与通知跳转 |

## 补齐登录后的统一流程

1. 用合法可用的测试账号，在同一类 Desktop 环境下分别记录根域、未认证状态、首次认证后的工作台和钱包连接状态。Axiom 已有登录态只作为旧样本，仍需按同一流程复跑。
2. 每家逐项核对发现与搜索、Token/Holder、钱包详情、追踪、交易准备、持仓、社交、通知、账户设置和帮助。每个功能记录可见、可点击、可读、可执行四层以及触发权限时的提示。覆盖公开站与交易终端的互跳，FOMO 分开计。
3. 用可用免费账号先统一对照。付费、托管钱包、私钥账号和外接钱包作为单独的权限层。任何未进入的目标保留 UNVERIFIED，禁止从文档推断实际授权。
4. 把样本 URL、截图和点击路径回填到本表及对应独立报告。对照研究只查看与走到安全预览，不需要真实交易。

现已使用用户提供的既有会话补验。LogEarn 的匿名身份基线仍待确认。

## 登录后补验

在用户已打开的 Chrome 标签中复查五家。保持原账号和链状态。以下覆盖登录后可见界面、所选权限边界和只读操作，付费等级、订单提交及通知到对象仍需单独验证。公开截图遮盖了可能关联个人账户的区域。

| 产品 | 游客 → 签入后实际差异（OBS） | 尚未验证 |
| --- | --- | --- |
| Axiom | 游客官网与登录终端分离。重进 `/trackers` 可见钱包和监控视图，并有拆分 Solana/EVM 监控器的设置入口。已实查的七项终端导航和通知菜单继续以原快照为证 [终端](screenshots/a07.jpg) · [监控](screenshots/a11.jpg) · [通知](screenshots/a16.jpg) | 追踪创建、通知深链、套餐 |
| DeBot | 十项现货导航继续可见，资产从认证提示变成钱包列表和个人盈亏区。下方有持仓、最近盈亏、活动、交易日志、订单。监控出现进阶监控配置入口。打开同一 Solana Token 提示该链没有钱包，关闭提示后仍可打开持仓分析及分类界面 [资产](screenshots/ds02.jpg) · [监控](screenshots/ds03.jpg) · [钱包提示](screenshots/ds04.jpg) · [持仓分析](screenshots/ds05.jpg) | 创建钱包后的交易或监控执行、付费/免费差异、通知到对象 |
| GMGN | 同一个 `/sol/address/:address` 由游客登录提示变为钱包详情，实际显示胜率、总盈亏、近期盈亏和活动，另有追踪及钱包跟单入口。资产页从认证提示变为钱包页面及创建钱包入口，追踪页显示「添加钱包」和「APP 通知」 [游客同路由](screenshots/g08.jpg) · [签入钱包](screenshots/gs03.jpg) · [资产](screenshots/gs04.jpg) · [追踪](screenshots/gs05.jpg) | 提交追踪、通知深链、已签入是否符合私钥跟单要求、连接钱包及付费差异 |
| FOMO | 从公开导航进入另一套交易界面。签入后实查 `/discover` 与 `/tokens/:chain/:address`。Discover 周边可见 Tokens、Perps、Following、Watchlist、Leaderboard、Feed。点击 Leaderboard 展开 Traders/Positions；Feed 是可切换的侧区。Token 详情包含图表和买卖控件 [Token](screenshots/fs01.jpg) · [排行榜](screenshots/fs03.jpg) · [Discover 与 Feed](screenshots/fs05.jpg) | 通知中心和社交深链、排行榜交易者详情、个人持仓及账户设置、钱包管理权限 |
| LogEarn | 用户提供的现有 Chrome 会话中，Token 详情可见关注钱包类别和钱包选择；进入 `/cn/portfolio` 可见导入、创建钱包、盈亏和订单框架，顶部钱包选择与资产页空钱包列表在抽样同时出现。低状态对照也能打开资产框架 [低状态资产](screenshots/l05.jpg) · [现有会话 Token](screenshots/ls01.jpg) · [现有会话资产](screenshots/ls02.jpg) | 真正匿名基线、该资产空状态的链或筛选原因、会员差异及通知落点 |
