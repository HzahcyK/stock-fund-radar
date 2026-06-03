# Stock Fund Radar

Daily stock and fund market research skill for A-share investors and fund allocators.

This skill is designed for Chinese-language market research workflows, including:

- A-share daily market review
- Overseas and peripheral market checks
- China policy and macro tracking
- Main capital flow analysis
- Sector and theme rotation scoring
- Fund-first opportunity screening
- Technical confirmation with K-line, moving averages, volume, and momentum indicators

## Current Focus

The skill is optimized for decision-grade Chinese market briefs. It requires an evidence chain before making sector or fund calls:

- Latest geopolitics, policy releases, major summits/events, and overseas risk signals
- A-share tape, turnover, breadth, main capital flow, and ETF activity
- K-line confirmation for major indexes and hot sectors, including MA5/10/20/60, volume, support/resistance, and relative strength
- Fundamentals, financial reports, valuation, crowding, and fund availability when making higher-conviction recommendations

## Privacy Note

The original local skill may include a personal `references/user-preferences.md` file. This public package intentionally replaces it with a template so private portfolio preferences are not uploaded.

## Install With Codex

In Codex, ask:

```text
帮我安装这个 skill：https://github.com/HzahcyK/stock-fund-radar
```

After installation, restart Codex so the skill list is re-indexed.

## Manual Install

Clone or copy the repository into your Codex skills directory as `stock-fund-radar`:

```powershell
git clone https://github.com/HzahcyK/stock-fund-radar.git $env:USERPROFILE\.codex\skills\stock-fund-radar
```

Then restart Codex.

## Trigger Examples

```text
Use $stock-fund-radar to analyze today's A-share market, main themes, capital flows, and fund opportunities.
```

```text
分析今日A股盘面，结合地缘政治、政策、主力资金、K线技术面和我的基金持仓给建议。
```

## Local Sync Workflow

The author's local working setup keeps two copies:

- Installed skill used by Codex: `C:\Users\cdv\.codex\skills\stock-fund-radar`
- GitHub repository copy: `C:\Users\cdv\Documents\Codex\2026-05-08\skill-a-1-2-3\stock-fund-radar-github`

The sync script copies the installed skill into the GitHub repository, replaces private preferences with the public template, commits, and pushes:

```powershell
C:\Users\cdv\Documents\Codex\2026-05-08\skill-a-1-2-3\sync-stock-fund-radar-github.ps1 -Message "Sync stock fund radar skill"
```

For HTTPS pushes, GitHub passwords are not accepted. Use a GitHub Personal Access Token with repository contents read/write access when the credential prompt asks for a password.

## Troubleshooting

- If the skill cannot be found in the Codex skill list, restart Codex and open a new conversation so local skills are re-indexed.
- If manual installation uses a different folder name, rename it to `stock-fund-radar`.
- If GitHub repeatedly asks for credentials, clear stale cached credentials and sign in again using a Personal Access Token.
