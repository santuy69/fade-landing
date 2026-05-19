# FADE — Xiaomi MiMo 100T 申请材料

> Xiaomi MiMo Orbit 百万亿 Token 创造者激励计划 · 申请文档
> 表单地址：https://100t.xiaomimimo.com/

---

## 一、表单填写速查表（中英对照）

| 表单字段 | 填写值 |
|---|---|
| 项目名称 / Project Name | **FADE** |
| 项目英文名 | FADE — Onchain Prediction Markets |
| 项目类别 / Category | DeFi · 预测市场 · Consumer Crypto |
| 阶段 / Stage | Concept · Pre-launch（落地页已上线，合约私有开发中） |
| 公链 / Chain | Base（USDC 结算） |
| 仓库 URL / Repo | `https://github.com/santuy69/fade-landing` |
| 项目网站 / Demo | `https://santuy69.github.io/fade-landing/` |
| License | MIT |
| 一句话 Tagline | long the truth. fade the cope.（看多事实，做空喊单） |
| 团队规模 | 1 人独立开发者 |
| 联系方式 / Contact | X: @0x_Missy22 |
| 申请用邮箱 | （请填写已注册 platform.xiaomimimo.com 的邮箱，或将用此邮箱注册） |

> 重要提示（来自 FAQ 02 和 09）：
> - **申请用邮箱必须与 Xiaomi MiMo 开放平台账号一致**（或已绑定）；
> - 否则权益无法到账，需到 https://id.mi.com 换绑后等 24h 自动到账。

---

## 二、使用的 AI 工具与底层模型（评估关键项 — FAQ 06）

> 评估标准明确写明：「填写越详细、项目越具体，评估通过率和权益档位越高」。
> 务必把 Hermes Agent + MiMo API 写在显眼位置。

### 底层模型（Underlying Models）

| 工作负载 | 模型 | 说明 |
|---|---|---|
| 主推理 / 长文规划 | Anthropic Claude Sonnet/Opus 4.7 | 设计稿、文案、架构 |
| 代码生成 | Claude / OpenAI Codex / **MiMo V2.5（计划接入）** | 一键生成单文件 HTML 落地页 |
| 视觉评审 | Gemini 2.0 Flash | 截图检查（当前免费额度，准备升级） |
| 嵌入 / 检索 | OpenAI text-embedding-3-small | 历史会话记忆与跨会话搜索 |

### AI 编程工具（AI Coding Tools）

| 工具 | 用途 | 是否对接 MiMo |
|---|---|---|
| **Hermes Agent v0.14.0** | 主控代理框架（自托管） | ✓ 计划用 MiMo V2.5 替换主推理后端 |
| Claude Code CLI | PR 工作流 | ✓ 可配置 MiMo API 作为 OpenAI 兼容端点 |
| Cursor | 本地代码编辑 | ✓ 支持配置自定义 OpenAI 兼容 base_url |
| OpenCode CLI | 代码评审子任务 | ✓ 同上 |
| OpenClaw | 项目上下文托管（AGENTS.md 自动注入） | ✓ FAQ 中明确提及 |

### 接入 MiMo API 的具体计划

1. 将 `~/.hermes/.env` 的 `OPENAI_API_BASE` 改为 `https://platform.xiaomimimo.com/v1`；
2. 设置 `OPENAI_API_KEY=<MiMo Token Plan key>`；
3. Cursor / Claude Code / OpenCode 同步配置；
4. 主推理负载（FADE 落地页迭代、合约文档撰写、Solidity 草稿）切到 MiMo V2.5；
5. 周维度对比 MiMo V2.5 vs Claude 4.7 在 Solidity / TypeScript / 文案三类任务的输出质量，结果回写到本仓库 `/benchmarks` 目录公开。

---

## 三、项目描述（按表单字数限制选用）

### A. 一句话（≤ 60 字）
> FADE — 面向 Crypto 原生用户的链上预测市场，Base 上 USDC 结算。

### B. 短描述（≤ 140 字 · 适合 tagline 字段）
> FADE 是为 Crypto 原生用户打造的链上预测市场。每个市场是 1¢–99¢ 的 YES/NO 二元合约，价格即实时概率。USDC 结算于 Base 主网，自托管、无 KYC、Gas 低于 1 美分，结算通过链上预言机自动完成。

### C. 中等描述（≤ 500 字 · 适合「项目简介」字段）

> **FADE** 是为 Crypto 原生用户打造的链上预测市场协议。
>
> 每个市场是一份 1¢–99¢ 的 YES/NO 二元合约，价格即资本加权的实时概率：你以 62¢ 买入 YES，赢得结算 $1.00，输则归零，期间任意时刻可按市价平仓。结算资产为 USDC，部署在 Base 主网，Gas 低于 1 美分，全程自托管，无 KYC、无客服提现队列。结算通过链上 commit-reveal 预言机 + 多签紧急通道完成，赢家的 share 在结算时自动按 $1.00 兑付。
>
> Polymarket 的 UX 是为记者和政治分析师设计的；FADE 的 UX 是为 Twitter/X 时间线上的 degen 设计的。我们专注于 Polymarket 故意低权重的题材：
>
> - **AI 发布窗口**（GPT-6 是否在 Q4 发布、Claude 是否在某窗口达成基准分数）；
> - **Memecoin 翻转**（PEPE 是否市值超过 DOGE、板块轮动）；
> - **链上 KPI**（BTC 主导率突破 60%、ETF 流入门槛、L2 TVL 反超）；
> - **Crypto 原生政策**（美联储主席决议、SEC 监管时点）。
>
> 当前阶段：本仓库托管的是公开版落地页与品牌识别系统（Acid Lime 主题 + 终端字体），合约层、订单簿引擎、预言机层在私有开发中。寻求生态支持 / 激励计划，以及在预言机解析层面的整合伙伴。
>
> 团队：1 人独立运营。所有公开制品 MIT 许可。

### D. 长描述（≤ 1200 字 · 适合「详细描述」字段，最高档位评估推荐）

> **FADE** 是一套面向 Crypto 原生用户的链上预测市场协议，专为「Twitter/X 已经在喊单但缺乏低摩擦做多/做空通道」的用户群体设计。
>
> **市场结构。** 每个市场是一份 1¢–99¢ 的 YES/NO 二元合约。价格即市场资本加权概率，订单成交时实时更新。62¢ 买入 YES，结算时若结果为真，每份 share 兑付 $1.00；若结果为假，归零。期间任意时刻可按订单簿中点平仓。
>
> **结算层。** Base 主网，USDC 原生结算，EVM 兼容，Gas 低于 1 美分，使 5¢ 量级的小额交易经济上可行。这一点是与 Polymarket（Polygon 上 USDC.e）的关键差异：FADE 的最小可行交易单位低一个数量级。
>
> **撮合层。** 订单簿 + LMSR AMM 混合：流动性厚的市场走订单簿，流动性薄的市场由 AMM 兜底报价。AMM 参数随订单簿厚度动态衰减。
>
> **结算预言机。** 链上 commit-reveal 模式，多签紧急通道处理模糊结果。无中心化客服队列，无管理员提现冻结。
>
> **UI 与品牌。** 单文件 PWA，钱包登录，无邮箱、无 Cookies 同意墙、无 KYC 障碍。视觉系统为深色 + 酸性绿（Acid Lime `#bfff00`）+ 霓虹绿 YES（`#00ff88`）+ 热粉 NO（`#ff2d8d`），字体为 Space Grotesk + JetBrains Mono，刻意拒绝主流 SaaS 模板的圆角玻璃态语言。
>
> **题材覆盖与差异化：**
>
> 1. 🪙 Crypto — BTC/ETH 价格目标、主导率、ETF 批准；
> 2. 🤖 AI — 模型发布窗口、基准分数门槛；
> 3. 🎰 Memes — 板块轮动、市值翻转；
> 4. 📉 Macro — 美联储动作、衰退正式宣告；
> 5. 🗳️ 政策 / 地缘 — 监管节点、选举二元；
> 6. ⚽ 体育 — 高交易量决赛与冠军赔率。
>
> 这些类目在 Polymarket 上历史交易速度最高，但被通用选举合约掩盖。
>
> **AI 工具栈。** FADE 项目从落地页设计到 GitHub Pages 部署，由 Hermes Agent v0.14.0（自托管开源代理框架）+ Claude 4.7（主推理）+ Codex/Cursor（代码生成）端到端交付，单人 6 分 24 秒从「一句需求」到「可访问 URL + 完整提交包」。技能注册中心当前装载 100 项程序化技能（设计、部署、链上交互、提示工程等），按需加载。**计划在获得 Token Plan 后，将主推理负载切换至 MiMo V2.5 系列**，对比基线为 Claude 4.7，覆盖 Solidity 草稿、TypeScript 前端、技术文案三类任务，结果在 `/benchmarks` 目录每周公开。
>
> **当前阶段。**
> - ✅ 落地页 + 品牌系统已上线（github.com/santuy69/fade-landing）；
> - ✅ 申请材料、截图证据、终端验证产物已打包；
> - 🔄 智能合约（Solidity）私有开发中；
> - 🔄 订单簿引擎（Rust + EVM bridge）私有开发中；
> - 🔄 预言机层正在评估 UMA / Pyth / 自建多签三方案。
>
> **诉求。** 申请 MiMo 100T Token Plan，用于：
>
> 1. 将 Hermes Agent 主推理后端切到 MiMo V2.5，作为长期可持续的开发主力模型；
> 2. 用 MiMo 多模态模型生成营销素材（OG、X 卡片、Telegram 贴纸）；
> 3. 用 MiMo 语音合成模型生成 Web3 社区内的 Bahasa Indonesia / 英文播客内容；
> 4. 公开发布 MiMo V2.5 vs Claude 4.7 在 Web3 任务上的基准对比，回馈生态。
>
> **公开制品清单。**
> - 仓库：https://github.com/santuy69/fade-landing
> - 落地：https://santuy69.github.io/fade-landing/
> - 截图证据：仓库 `/proof` 目录下 8 个 PNG（4 张产品 + 4 张终端验证）
> - 操作者：X / @0x_Missy22

---

## 四、上传截图清单（共 8 张，仓库 `/proof` 目录已 commit）

### 产品端（4 张）

| 文件 | 用途 | 尺寸 |
|---|---|---|
| `proof/landing-desktop.png` | 表单主截图 | 1440×1080 |
| `proof/landing-fullpage.png` | 全页滚动截图（推荐用于「详细描述」配图） | 1200×1200 |
| `proof/landing-hero.png` | OG / X 卡片格式 | 1200×630 |
| `proof/landing-mobile.png` | 移动端响应式证据 | 420×315 |

### 终端验证（4 张 — 评估「真实交付」加分项）

| 文件 | 证明内容 | 尺寸 |
|---|---|---|
| `proof/proof-git-history.png` | git log — AI 端到端交付时间线 | 820×412 |
| `proof/proof-deployment.png` | curl -sI — 生产环境 HTTP 200 + HSTS | 802×566 |
| `proof/proof-repos.png` | GitHub API — santuy69 公开仓库清单 | 892×478 |
| `proof/proof-skills.png` | Hermes Agent skill registry — 100 项 | 802×830 |

### 直接引用 URL（适用于支持图片链接的字段）

```
https://raw.githubusercontent.com/santuy69/fade-landing/main/proof/landing-desktop.png
https://raw.githubusercontent.com/santuy69/fade-landing/main/proof/landing-fullpage.png
https://raw.githubusercontent.com/santuy69/fade-landing/main/proof/landing-hero.png
https://raw.githubusercontent.com/santuy69/fade-landing/main/proof/landing-mobile.png
https://raw.githubusercontent.com/santuy69/fade-landing/main/proof/proof-git-history.png
https://raw.githubusercontent.com/santuy69/fade-landing/main/proof/proof-deployment.png
https://raw.githubusercontent.com/santuy69/fade-landing/main/proof/proof-repos.png
https://raw.githubusercontent.com/santuy69/fade-landing/main/proof/proof-skills.png
```

---

## 五、提交前检查清单（复制 FAQ 04 的要求）

- [ ] **申请用邮箱** = MiMo 开放平台账号邮箱（或可绑定）
- [ ] 项目仓库公开可访问（已验证 HTTP 200）
- [ ] 落地页公开可访问（已验证 HTTP 200，HSTS 启用）
- [ ] 描述中点名了「Hermes Agent」+「Claude Code / Cursor / OpenClaw」（FAQ 01 中明确列举）
- [ ] 描述中说明计划如何使用 MiMo V2.5（FAQ 06 评估关键）
- [ ] 截图证据已上传至公开 raw URL
- [ ] License 已设置为 MIT 并提交

---

## 六、提交后流程（来自 FAQ 03 + 08）

1. 提交后等待评估邮件（**约 3 个工作日**）；
2. 收到通过邮件后，**24 小时内**权益自动到账；
3. 若 3 天未收到，先检查垃圾邮件 → 重新提交一次表单；
4. 仍未到账：通过 https://platform.xiaomimimo.com/contact 反馈；
5. 收到权益后，立刻在 Hermes Agent + Cursor + Claude Code 三处配置 MiMo API base URL 并跑首个调用记录截图存档。

---

License: MIT · Operator: santuy69 · Driven by: Hermes Agent v0.14.0
