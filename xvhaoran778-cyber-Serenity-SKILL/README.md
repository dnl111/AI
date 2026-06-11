# Serenity Chokepoint Investing Skill

一个可复用的 Codex skill，用来做跨市场的“供应链瓶颈 / 需求冲击 / 贝叶斯更新”式投资研究。

它从 Serenity（`@aleabitoreddit`）公开推文、交易披露和社区整理材料中蒸馏出研究方法，但不复制其身份、收益叙事或喊单风格。这个项目的目标是把方法变成可执行的研究流程，适用于 A 股、美股、港股、台股、日股、欧洲股票等不同市场。

## 能做什么

- 拆解 AI、半导体、光通信、CPO、数据中心电力、先进封装、材料、设备等产业链。
- 寻找真实供应链卡点：材料、衬底、封装、设备、产能、资格认证、政府背书。
- 把产品/行业需求冲击转译成公司层面的财务影响。
- 用贝叶斯方式更新投资假设：先验、正证据、反证据、后验方向。
- 抓取并纳入公司新闻、公告、财报、交易所披露和政策文件。
- 区分“明确交易披露”和“观点/看多/目标价”。

## 目录结构

```text
serenity-chokepoint-investing/
├── README.md
├── docs/
│   ├── PROJECT_INTRO.md
│   └── SOURCE_AND_RISK_NOTES.md
└── skills/
    └── serenity-chokepoint-investing/
        ├── SKILL.md
        ├── agents/
        │   └── openai.yaml
        └── references/
            ├── market-data-and-news.md
            ├── pattern-library.md
            └── research-rubric.md
```

## 安装

把 `skills/serenity-chokepoint-investing` 复制到本机 Codex skills 目录：

```bash
cp -R skills/serenity-chokepoint-investing ~/.codex/skills/
```

然后在 Codex 中使用类似提示：

```text
用 serenity-chokepoint-investing 分析一下某家公司是否有供应链瓶颈机会。
```

## 使用示例

```text
用 serenity-chokepoint-investing 分析 300xxx 在 AI 数据中心电力链条里的卡点价值。
```

```text
用 Serenity 的方法比较 AAOI、SIVE、IQE、XFAB 谁的 chokepoint 更强。
```

```text
按贝叶斯更新框架，重新评估某家公司最近公告对原投资假设的影响。
```

## 重要说明

- 这不是投资建议，也不是自动荐股工具。
- Serenity 的收益率和持仓披露来自公开材料，无法视为经审计事实。
- Skill 会要求优先检查官方公告和一手资料，新闻和社交媒体只作为线索。
- 对 A 股、美股、港股等不同市场，skill 会使用不同披露源和风险检查清单。

