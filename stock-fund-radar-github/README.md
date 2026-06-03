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

## Privacy Note

The original local skill may include a personal `references/user-preferences.md` file. This public package intentionally replaces it with a template so private portfolio preferences are not uploaded.

## Install

Copy this folder into your Codex skills directory:

```powershell
Copy-Item -Recurse stock-fund-radar $env:USERPROFILE\.codex\skills\
```

Then trigger it with market or fund research questions such as:

```text
Use $stock-fund-radar to analyze today's A-share market, main themes, capital flows, and fund opportunities.
```
