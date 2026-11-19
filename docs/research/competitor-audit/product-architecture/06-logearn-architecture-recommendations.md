# LogEarn Desktop Web 架构映射与调整建议

## 现状

从简体中文 Desktop Web 实查的顶栏有 **9 个命名入口**。战壕、信号、热门、资产、奖励、活动、AI 策略引擎、API、VIP。Logo 指向 `/cn`，另有全局搜索、热门榜单/自选及底部工具。当前浏览器的账户套餐未确认。各路由只记录实际显示的界面和入口，按钮权限及执行结果需要另测。 [主导航与策略页](screenshots/l01.jpg) · [信号](screenshots/l02.jpg)

| LogEarn 实际页面或入口 | 当前可见组织（OBS） | 竞品对应设计 | 建议（INFER） |
| --- | --- | --- | --- |
| 战壕 `/cn/trenches` | 代币按生命周期列组织，可见即将迁移和已迁移 [截图](screenshots/l03.jpg) | Axiom Pulse 的生命周期栏 [截图](screenshots/a10.jpg) | 保留实时扫描任务与深链。可与热门同属「发现」；保留默认快速入口 |
| 热门 `/cn/trending` | 市场榜单，表中出现近 24 小时钱包指标 [截图](screenshots/l04.jpg) | GMGN 热门榜与 Axiom 探索热门 [GMGN](screenshots/g06.jpg) · [Axiom](screenshots/a07.jpg) | 保留榜单页。用「热门榜单」与「战壕」两个二级名明确排行和实时发现，先测跨页切换习惯 |
| 信号 `/cn/signals` | 顶部独立入口，底部还有信号快捷入口 [截图](screenshots/l02.jpg) | DeBot 将 AI 信号作为默认独立模块 [截图](screenshots/d01.jpg) | 保留一级。补验来自信号的 Token 详情能否保留触发时间及信号类型 |
| 代币详情 `/cn/:chain/tokens/:id` | 样本有交易明细、持有者、盈利榜、关注/KOL、仓位、订单、策略日志、信号 [截图](screenshots/l10.jpg) | GMGN Holder 转到钱包，Axiom 同屏分析和买卖 [GMGN](screenshots/g07.jpg) · [Axiom](screenshots/a08.jpg) | 优先复测 Holder → 钱包 → 追踪，并检查返回时能否回到同一代币和页签 |
| 资产 `/cn/portfolio` | 有钱包列表、导入/创建入口和订单区域 [截图](screenshots/l05.jpg) | Axiom 投资组合将现货、钱包及各交易品类分区 [截图](screenshots/a14.jpg) | 保留一级，区分自有钱包和外部追踪对象。核实底部仓位、盈亏与资产页是否共享数据和筛选 |
| AI 策略引擎 `/cn/strategies` | 观察到我的策略与策略模板。Token 详情另有策略日志 [策略](screenshots/l01.jpg) · [详情](screenshots/l10.jpg) | DeBot 跟单分任务和记录 [截图](screenshots/d10.jpg) | 保留一级。策略引擎用于建立和管理规则，信号用于发现事件。详情日志保留关联策略入口作为验证项 |
| API `/cn/agents` | API Key 管理、Skills 使用示例 [截图](screenshots/l08.jpg) | GMGN 把 AI/OpenAPI 放在全局工具区 [截图](screenshots/g16.jpg) | 可挂在「开发者」工具入口。保留原 URL，验证开发者能从策略或帮助直接找到 |
| 奖励 `/cn/rewards` | 邀请返佣、现金券与任务 [截图](screenshots/l06.jpg) | Axiom、GMGN 均有奖励目的地 [Axiom](screenshots/a05.jpg) · [GMGN](screenshots/g14.jpg) | 可与活动在一级入口归组，保留奖励页面和直接分享链接 |
| 活动 `/cn/activities` | 限时活动与历史活动 [截图](screenshots/l07.jpg) | FOMO 把新闻和指南收进资源 [截图](screenshots/f16.jpg) | 和奖励共用入口时，短期活动与持续返佣仍用各自页面 |
| VIP `/cn/solana/vip` | 订阅、权益说明和钱包相关说明 [截图](screenshots/l09.jpg) | 本轮未拿到可比的竞品付费会话 | 可由账户区和受限功能入口到达。是否移出主导航取决于升级入口使用数据 |
| 底部工具和帮助 | 可见监控、喊单、通知、仓位与盈亏等快捷入口以及文档链接。公开来源样本未验证每个弹层落点 [截图](screenshots/l02.jpg) | DeBot 有排序、隐藏与吸附设置。FOMO 帮助可独立搜索 [DeBot](screenshots/d27.jpg) · [FOMO](screenshots/f08.jpg) | 先核对同名入口是否打开同一视图。钱包监控按动态、关注名单与提醒分组，保留常用快捷方式 |

## 一级导航判断

建议先验证较小的分组变化。**发现（战壕、热门）、信号、AI 策略、资产**作为核心目的地候选。奖励和活动可归组，API 可归到开发者工具，VIP 可归到账户和权益入口。继续保留各现有页面和 URL。根据用户点击和任务完成数据判断哪些一级入口必须继续常驻。

优先验证三个闭环。用「找一个新币」「从信号看同一代币」「找到并追踪某钱包」比较当前与候选归类的首击成功率、导航次数、返回后状态和误入模块。增长类入口另外测奖励、活动和 VIP 的到达率。若合并降低战壕或热门的首次到达率，保留各自入口。若通知只出现于底部工具，则先补查通知深链及权限，再决定是否提升层级。

目前可确认的是导航与页面结构。监控、通知、搜索结果分类、跨页面状态、身份差异及真实使用频率仍待补验。建议依据用户任务和当前路由提出，无业务代码变更。
