Output format
> This file tells the agent how I want its output structured. Try a digest, see what I actually use, then edit this file to match.
---
My preferred format
```markdown
# Crude and products digest: [DATE]
*Window: last 24 hours. Sources checked: [number].*

## Key theme
*One sentence. The single most important thing across today's items, in plain English.*

## Market snapshot
| Item | Level | Source and time |
|---|---|---|
| Brent | [value or "not retrieved"] | [source, timestamp] |
| WTI | [value or "not retrieved"] | [source, timestamp] |
| Dubai | [value or "not retrieved"] | [source, timestamp] |
| US crude stocks (EIA, if released) | [change] | [source, date] |
| US gasoline / distillate stocks (EIA, if released) | [change] | [source, date] |

## Top items

### 1. [Headline in plain English, not click-bait]
- **Source(s):** [Outlet, with access flag: full text / headline only]
- **Why it matters:** [One sentence starting with a verb]
- **Summary:** [Two sentences, no fluff]
- **Link:** [URL]
- **Confidence:** high / medium / low

### 2. [Next item, same shape]
…

[Up to 10 items, ranked by likely market impact, not by recency. Fewer is fine.]

## OPEC+ and producers
*Only if there is something new. Otherwise one line: "No new OPEC+ or producer developments found."*

## Products and refining
*Refinery outages, product stocks, export policy, margins (only if sourced). Otherwise one line saying nothing new.*

## Shipping and geopolitics
*Chokepoints, tanker incidents, sanctions. Only if there is something new.*

## What to chase
*Follow-ups worth a phone call or a question to a source. Suggest these, don't just summarise.*

## What I couldn't verify
*Anything flagged but unconfirmed: single-source claims, headline-only items that I could not match to a free or primary source, figures that don't reconcile.*

## Sources checked
*Every source looked at, including those that returned nothing or could not be opened.*
```
---
Rules for the agent
Use British English.
Time window is the last 24 hours unless I say otherwise. Date every item.
Rank items by likely effect on crude prices, product markets or supply, not by recency.
Plain prose. No marketing language ("game-changing", "revolutionary", "AI-powered").
Start every "why it matters" with a verb: Affects, Changes, Contradicts, Confirms, Tightens, Loosens.
If something is uncertain, say so in the same sentence as the claim.
Never state a price, inventory figure or margin unless it was read from a named source in this run. Show the source and time. If it wasn't retrieved, write "not retrieved".
Headline-only items: label them `[headline only]`, quote the headline, and don't describe what the article says. If one reaches the top items, try to match it to a free or primary source and otherwise mark it `[unconfirmed]`.
Bank and analyst views: only report them when they appear in a readable source, and attribute them to that source, not to the bank or analyst.
Use full names on first reference, last names after.
Weekly releases (EIA on Wednesdays, rig count on Fridays) appear only on the days they are published.
Don't pad. If only four items are strong, give four. If it's a slow day, say so in one line.
Do not use Upstream as a source.
---
What I don't want
No emojis.
No sycophancy: don't call a story "fascinating" or "important". Show why.
No extra headers beyond those above.
No "let me know if you'd like me to dig deeper".
No price predictions or trading advice.
No paraphrasing of a headline as if it were a summary.
