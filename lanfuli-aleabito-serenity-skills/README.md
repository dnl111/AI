# AleaBito / Serenity Skills

> A suite of **Claude / Codex agent skills** distilled from [@aleabitoreddit](https://x.com/aleabitoreddit) ("Serenity")'s **entire public archive** — ~11 months, 6,120 posts, 750 tickers (2025-07-02 → 2026-05-30).
> Track her, analyze *like* her, and anticipate where her attention is moving — grounded in real data, not vibes.

**📊 Live dashboard / 实时看板:** **[Lifetime attention tracker · 全周期注意力看板](https://lanfuli.github.io/follow-aleabito-skill/reports/aleabito-60d-dashboard.html)** — built on top of these skills · 基于这套技能制作

**🌐 Language / 语言:** **[English](#english)** · **[中文](#中文)**

`claude-skill` · `agent-skill` · `aleabito` · `serenity` · `investing` · `stock-research` · `supply-chain` · `first-principles` · `x-api`

---

<a name="english"></a>
## English

### What this is
Three interlocking skills that turn one prolific X (Twitter) research account into a reusable workflow:

| Skill | What it does | Key command |
| --- | --- | --- |
| **`follow-aleabito`** | **Data layer.** Fetches her posts via the X API, builds a beginner-friendly digest, cumulative ticker-mention analytics, and a durable research map. Includes a full-archive backfill. | `node skills/follow-aleabito/scripts/analyze-mentions.js --incremental --resume` |
| **`serenity-method`** | **Her analysis method, generalized.** Apply her style to *any* stock: critical-chokepoint / supply-chain-OSINT discovery → first principles → a Buffett-style quality gate (fields default to `unverified`) → narrative-vs-fundamentals hygiene → `research-map` vs `investable-conclusion`. | (invoked by request: "analyze $X like Serenity") |
| **`serenity-radar`** | **Where her attention is going.** Reads the mention archive for attention momentum (heating tickers, new entrants, conviction core, theme rotation) and generates candidates in her style — a *candidate generator + checklist*, never an oracle. | `node skills/serenity-radar/scripts/radar.js --window 14` |

**The pipeline:** `follow-aleabito` (data) → `serenity-method` (how she reasons) → `serenity-radar` (what she's likely to focus on next). Each later skill builds on the earlier one.

### Install
1. **Copy the skills** into your agent's skills directory:
   ```bash
   cp -R skills/* ~/.codex/skills/      # Codex
   # or
   cp -R skills/* ~/.claude/skills/     # Claude Code
   ```
2. **Node 18+** is required for the scripts.
3. **X API token** — put a bearer token in `~/.follow-aleabito/.env`:
   ```
   X_BEARER_TOKEN=your_token_here
   ```
   The full-archive backfill (`--archive`) needs an X API project entitled to **full-archive search** (`/2/tweets/search/all`); the daily incremental fetch works on the standard user-timeline endpoint.
4. **Point at your data dir** (where the analytics CSVs live):
   ```bash
   export FOLLOW_ALEABITO_REPORTS_DIR="$HOME/aleabito-reports"
   ```

### Quick start
```bash
# 1) Pull the latest posts incrementally (cheap; only fetches since the last run)
node skills/follow-aleabito/scripts/analyze-mentions.js --incremental --include-replies --resume

# 2) See where her attention is moving right now
node skills/serenity-radar/scripts/radar.js --window 14 --top 12
```
Sample radar output (trimmed):
```
## 🔥 Heating (attention momentum — recent vs prior mentions)
ticker=JBL   Δ=13  recent=25  prev=12
ticker=XFAB  Δ=12  recent=12  prev=0      # new entrant + heating = emerging focus
ticker=SIVE  Δ=10  recent=93  prev=83
## 🔄 Theme rotation
▲ Western supply chain / policy: +8     ▼ AI compute / neocloud: −12
```
Then ask your agent: *"Analyze $SIVE like Serenity"* → `serenity-method` produces the 5-block analysis. All output is **中文 by default, English on request**.

### Live dashboard
A self-contained, interactive **lifetime research dashboard** built on top of these skills — spanning her entire public archive, it maps attention momentum, mention structure (posts vs. replies vs. quotes), recent moves, and research priority across the tracked tickers, with linked price trends.

👉 **[Open the live dashboard](https://lanfuli.github.io/follow-aleabito-skill/reports/aleabito-60d-dashboard.html)** — no login, no external dependencies. For tracking & research only, not investment advice.

### How it was built
The skills are distilled from her complete public history, pulled with `follow-aleabito`'s archive backfill (X API full-archive search). The empirical patterns in `serenity-radar/references/patterns.md` (theme-rotation logic, selection signature, catalyst playbook, conviction tells) are mined directly from those 6,120 posts — including the November-2025 drawdown (IREN −38% / NBIS −35%) she held through, which is why the radar's signals aren't overfit to a single up-only window.

### Caveats & disclaimer
- **Candidate generator, not an oracle.** The radar predicts *her interest*, not price or correctness.
- **Survivorship bias.** Her archive over-weights names that worked; treat "she ramped X and it ran" as *not* evidence it repeats.
- **Single-account fragility.** One person, one style, one era.
- **Not investment advice.** For information tracking and research only. Do nothing with this that you wouldn't do after your own due diligence.

### License
[MIT](LICENSE).

---

<a name="中文"></a>
## 中文

### 这是什么
三个环环相扣的技能,把一个高产的 X(推特)研究账号变成一套可复用的工作流:

| 技能 | 作用 | 关键命令 |
| --- | --- | --- |
| **`follow-aleabito`** | **数据层。** 用 X API 抓取她的发帖,生成小白友好的简报、累计提及分析,以及持久的研究地图;含全档案回填。 | `node skills/follow-aleabito/scripts/analyze-mentions.js --incremental --resume` |
| **`serenity-method`** | **她的分析方法,通用化。** 把她的风格套到*任意*股票:关键卡点 / 供应链 OSINT 发现 → 第一性原理 → Buffett 五问质量门(默认 `unverified`)→ 叙事 vs 基本面卫生 → `研究地图` vs `可投资结论`。 | (按需调用:"用 Serenity 的方法分析 $X") |
| **`serenity-radar`** | **她的注意力流向。** 从提及档案算注意力动量(升温标的、新进、重仓核心、主题轮动),并按她的风格生成候选——**候选发生器 + 检查清单**,不是预言机。 | `node skills/serenity-radar/scripts/radar.js --window 14` |

**管线:** `follow-aleabito`(数据)→ `serenity-method`(她怎么推理)→ `serenity-radar`(她下一步可能看什么),后者建立在前者之上。

### 安装
1. **把技能复制**到你 agent 的技能目录:
   ```bash
   cp -R skills/* ~/.codex/skills/      # Codex
   # 或
   cp -R skills/* ~/.claude/skills/     # Claude Code
   ```
2. 脚本需要 **Node 18+**。
3. **X API token** —— 在 `~/.follow-aleabito/.env` 里放一个 bearer token:
   ```
   X_BEARER_TOKEN=你的token
   ```
   全档案回填(`--archive`)需要你的 X API 项目开通**全档案搜索**(`/2/tweets/search/all`);日常增量抓取用标准时间线端点即可。
4. **指定数据目录**(分析 CSV 存放处):
   ```bash
   export FOLLOW_ALEABITO_REPORTS_DIR="$HOME/aleabito-reports"
   ```

### 快速上手
```bash
# 1) 增量拉取最新发帖(很省;只抓上次之后的)
node skills/follow-aleabito/scripts/analyze-mentions.js --incremental --include-replies --resume

# 2) 看她现在注意力往哪走
node skills/serenity-radar/scripts/radar.js --window 14 --top 12
```
然后对你的 agent 说:*"用 Serenity 的方法分析 $SIVE"* → `serenity-method` 会产出五段式分析。所有输出**默认中文,可按需出英文**。

### 实时看板
一个基于这套技能制作、自包含的交互式 **全周期(lifetime)研究看板**——覆盖她的全部公开历史,把注意力动量、提及结构(发帖 vs. 回复 vs. 引用)、近期变化和研究优先级在所有跟踪标的上可视化,并联动价格趋势。

👉 **[打开实时看板](https://lanfuli.github.io/follow-aleabito-skill/reports/aleabito-60d-dashboard.html)** —— 无需登录、无外部依赖;仅作跟踪与研究用途,不构成投资建议。

### 数据怎么来的
这些技能蒸馏自她的**全部公开历史**,用 `follow-aleabito` 的全档案回填(X API 全档案搜索)抓取。`serenity-radar/references/patterns.md` 里的经验模式(主题轮动逻辑、选股签名、催化剂打法、重仓信号)直接从这 6,120 条帖子里挖出——其中包含她扛过的 2025 年 11 月回撤(IREN −38% / NBIS −35%),这也是雷达信号没有过拟合到"单边上涨窗口"的原因。

### 风险与免责
- **候选发生器,不是预言机。** 雷达预测的是*她的兴趣*,不是价格或对错。
- **幸存者偏差。** 她的档案天然偏向"成功的标的";别把"她加注 X 然后涨了"当成会重演的证据。
- **单账号脆弱性。** 一个人、一种风格、一个时代。
- **不构成投资建议。** 仅作信息跟踪与研究用途;请以你自己的尽调为准。

### 许可
[MIT](LICENSE)。

---

*Built with the [follow-aleabito](skills/follow-aleabito) · [serenity-method](skills/serenity-method) · [serenity-radar](skills/serenity-radar) skills. Not affiliated with @aleabitoreddit. 与 @aleabitoreddit 无隶属关系。*
