---
name: stock-fund-radar
description: Use when the user asks for A-share or fund market research: daily market review, overseas markets, geopolitics, China policy, major summits/events, capital flows, sector rotation, mainline/theme prediction, K-line technical analysis of indexes/sectors, financial-report evidence, ETF/QDII/active fund screening, portfolio actions, or hidden opportunity mining.
---

# Stock Fund Radar

Use this skill as a disciplined market-research and fund-screening workflow. Treat outputs as probability-weighted research, not personalized financial advice or guaranteed predictions.

## Hard Rules

- Browse or otherwise verify current market data before making any daily call. If current data cannot be fetched, say so clearly and provide only a framework or historical context.
- State the data timestamp, market session status, timezone, and whether data is pre-market, intraday, post-close, or delayed.
- Prefer official or primary sources for policy, macro, central-bank, exchange, and fund disclosures. Use market-data sites only for live tape, breadth, fund flow, and ranking snapshots.
- Daily market and opportunity calls must not rely only on economic/market-data websites. Before giving a view, check current geopolitical news, policy releases, major summit/event calendars, and overseas risk signals, then map each important event into bullish/bearish sector transmission.
- Separate facts, inference, and action candidates. Label uncertain conclusions as "推断" or "情景".
- Do not fabricate fund codes, NAV, holdings, manager tenure, fees, drawdowns, or capital-flow figures. Verify fund names and codes before recommending.
- Avoid "必涨", "精准买点", "稳赚", or single-outcome predictions. Use base/bull/bear scenarios, triggers, invalidation levels, and risk controls.
- Prefer funds over individual stocks unless the user explicitly asks for stocks. Include overseas/QDII, active, passive, ETF/LOF, money-market/bond/commodity hedges when relevant.
- For重点板块 and actionable opportunities, combine policy, capital flow, fundamentals, and K-line/technical indicators before giving a view. Do not treat capital inflow alone as enough confirmation.
- For hot sectors and major indexes, include technical context when relevant: daily/weekly K-line, MA5/10/20/60, volume, MACD/KDJ/RSI if available, support/resistance, relative strength, and whether the ETF/fund confirms the sector/index tape.
- For high-conviction sectors, build an evidence chain from current politics/policy, industry cycle, company financial reports, valuation/crowding, capital flow, and technical structure. Do not give a recommendation from one signal alone.
- Avoid formulaic single-point replies. Provide the non-obvious insight, the strongest counterargument, the data that would change the view, and a differentiated action plan.
- Keep live-data workflows low-friction: prefer built-in web/search when sufficient, batch market-data requests when direct APIs are needed, avoid repeated permission prompts in the same analysis, and reuse recent same-session data unless the user asks to refresh.
- If the user corrects preferences or says "以后按这个", update `references/user-preferences.md` after confirming or when the intent is explicit.

## Workflow

1. Classify the request: daily market brief, sector/theme excavation, fund shortlist, portfolio review, post-close replay, or skill iteration.
2. Build a current data pack. Read `references/data-checklist.md` when the task involves today's market, capital flows, policies, geopolitics, major events, sector K-lines, or overseas markets.
3. Build an event-risk map before the tape summary: list major geopolitical/policy/summit/news catalysts, classify each as bullish/bearish/uncertain, and connect it to likely sector winners/losers.
4. If the user asks for主线、埋伏、重仓/加仓、深挖, or criticizes depth, read `references/research-depth.md` and run the deeper evidence-chain workflow.
5. Score market regime and themes. Read `references/scoring-rubric.md` when ranking sectors, timing themes, or selecting funds.
6. For major indexes and重点板块, confirm technical structure with K-line, moving averages, volume/price behavior, support/resistance, relative strength, and momentum indicators before ranking.
7. Produce a concise decision-grade brief. Read `references/output-template.md` when the user asks for a full daily report or fund shortlist.
8. Incorporate personal constraints from `references/user-preferences.md` before final recommendations.

## Daily Analysis Procedure

Collect and cross-check:

- Geopolitics and event calendar: wars/conflicts, sanctions/export controls, trade/diplomatic meetings, G7/G20/BRICS/ASEAN/Fed/ECB/OPEC and China policy meetings, major speeches, and whether each item is confirmed, rumor, scheduled, or already priced in.
- Overseas/peripheral markets: US/EU/Asia index moves, futures, rates, dollar/CNH, commodities, VIX/risk sentiment, major geopolitical or policy events.
- China policy and macro: State Council, PBOC, CSRC, NDRC, MOF, NBS, exchange announcements, industry ministry signals, and fiscal/monetary/property/consumption/technology policy.
- A-share tape: major indices, turnover, advance/decline breadth, limit-up/down counts, style factors, sector/concept leaders, ETF activity, margin/financing where available.
- Capital flows: main funds by sector/concept/stock, ETF net subscriptions or shares, northbound/southbound data under the latest available disclosure rules, and institutional flow clues.
- Technical picture for major indexes and重点板块: daily and weekly K-line trend, MA5/10/20/60 position, volume expansion/shrinkage, MACD/KDJ/RSI if available, gap/support/resistance, relative strength versus major indices, and whether ETF price action confirms the underlying sector.
- Fundamentals and earnings: newest annual/quarterly reports, guidance, order/backlog, revenue/profit trend, margin, cash flow, capex, inventory, price cycle, valuation, and whether leading companies' data support the sector narrative.
- Catalyst calendar: earnings, policy meetings, macro prints, central-bank decisions, commodity shocks, product launches, and industry events.

Then synthesize:

- Assign a market risk score from 0 to 100 with a one-line explanation.
- Start synthesis with the event-risk map, then decide whether the tape confirms or rejects the event narrative. Do not let one-day capital flow override a major policy/geopolitical catalyst without explaining the contradiction.
- Identify the current dominant line, likely next line, and quiet-start candidates.
- Prefer themes where policy support, macro trend, earnings logic, capital inflow, relative strength, and fund availability point in the same direction.
- Distinguish "story-driven rally" from "earnings-confirmed rally"; downgrade stories where财报、订单、价格、库存、或估值 do not support the tape.
- Downgrade themes where资金流入 is strong but K-line is extended, volume is climactic, price is below key moving averages, or momentum diverges.
- Flag overheated themes where price move, narrative saturation, and crowding are already extreme.

## Fund Selection Rules

For every fund candidate, verify:

- Code, full name, type, benchmark/tracked index, latest available NAV or ETF price context, and subscription status.
- For passive funds: tracking index quality, AUM, liquidity/volume, tracking error, fees, premium/discount, concentration, and whether the index matches the theme.
- For active funds: manager tenure, style consistency, holdings concentration, turnover, drawdown control, excess return source, capacity pressure, and whether recent holdings still fit the stated thesis.
- For QDII/overseas funds: quota/subscription status, premium risk, FX exposure, local market holidays, underlying market valuation, and settlement delay.
- For ETFs and index funds linked to重点板块: check both the underlying sector/index K-line and the ETF's own liquidity, premium/discount, intraday trend, and volume confirmation.
- For tactical ideas: entry trigger, invalidation condition, position role, expected holding period, and risk scenario.

## Output Discipline

Keep the answer useful for the user's next action:

- Start with a brief conclusion: "今天偏进攻/防守/观望" and the top 1-3 themes.
- Give only the most relevant data, with source links when browsing was used.
- Use tables for fund candidates and theme scoring.
- Include "不买/暂缓" reasons, not only positives.
- End with what to watch next: exact data points, policy events, price/volume triggers, or fund-flow confirmations.

## Iteration

When the user asks to optimize this skill, revise the skill files directly:

- Update the trigger description only if new wording should auto-trigger the skill.
- Update `references/user-preferences.md` for personal constraints, risk appetite, preferred fund types, disliked sectors, position style, and lessons from past corrections.
- Update `references/scoring-rubric.md` when the user changes the ranking logic.
- Re-run the skill validation script after edits.
