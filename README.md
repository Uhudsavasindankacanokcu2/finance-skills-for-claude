# Finance Skills for Claude 💸

**Turn Claude into a finance analyst.** A pack of battle-tested [Claude Skills](https://docs.claude.com/en/docs/claude-code/skills) that handle the boring, error-prone money work: cash flow, invoices, budgets, and forecasting — from raw, messy data.

Built for founders, freelancers, bookkeepers, and finance teams who want decision-grade numbers without a spreadsheet marathon.

---

## ✨ What's inside (free core)

| Skill | What it does |
|-------|--------------|
| **cash-flow-analyzer** | Drop in bank/accounting transactions → categorized cash-flow statement, **burn rate, runway, and liquidity warnings** with the numbers attached. |
| **invoice-expense-extractor** | Paste an invoice/receipt (text, PDF, image) → clean line-item data + **CSV ready for your accountant** + duplicate/overcharge/tax-error flags. |
| **budget-vs-actual** | Budget + actuals → variance report, biggest swings, over-budget flags, and a simple forecast. |

Each skill is a single `SKILL.md` — no install, no dependencies. Drop it in your `.claude/skills/` folder and Claude uses it automatically.

---

## 🚀 Quick start
1. Copy the skill folder(s) into `~/.claude/skills/` (or your project's `.claude/skills/`).
2. Ask Claude: *"Here's our last 3 months of transactions — what's our runway?"*
3. Claude triggers the skill and returns a real analysis.

> Works with Claude Code, Claude Desktop, and the API.

---


---

## 👀 See it in action

**You paste this** (3 months of raw transactions, the kind you'd export from your bank):

```
Date,Amount,Description
2026-01-03,-4200,Payroll - Jan
2026-01-05,8500,Stripe payout - customer invoices
2026-01-08,-1200,AWS
2026-01-10,-450,Google Workspace + SaaS tools
2026-01-15,-2800,Office rent
2026-01-22,3100,Stripe payout
2026-01-28,-600,Meta Ads
2026-02-03,-4200,Payroll - Feb
2026-02-06,9200,Stripe payout
2026-02-09,-1250,AWS
2026-02-15,-2800,Office rent
2026-02-20,-1100,Meta Ads
2026-02-25,2400,Stripe payout
2026-03-03,-6300,Payroll - Mar (new hire)
2026-03-07,7100,Stripe payout
2026-03-10,-1400,AWS
2026-03-15,-2800,Office rent
2026-03-24,-1600,Meta Ads
Current cash balance: 41,000
```

**Claude returns this** (with the skill installed):

---

**Verdict:** Burning ~$1.4k/mo on average, but **March flipped negative (−$6.6k)** after the new hire — at March's rate you have **~6 months runway**. Watch payroll vs revenue.

**Monthly cash flow**

| Month | Operating In | Operating Out | Net Operating | End Balance |
|-------|-------------:|--------------:|--------------:|------------:|
| Jan   | $11,600 | $9,850  | **+$1,750** | $42,750 |
| Feb   | $11,600 | $9,350  | **+$2,250** | $45,000 |
| Mar   | $7,100  | $12,100 | **−$5,000** | $40,000 |

**Headline metrics**
- Avg monthly net (3mo): **−$333** (masked — Jan/Feb positive, Mar dragged it down)
- **March run-rate burn: $5,000/mo → ~6.6 months runway** on $41k
- Largest recurring outflows: Payroll ($4.2k→$6.3k), Rent ($2.8k), AWS ($1.2k), Meta Ads (rising: $600→$1.6k)
- Revenue concentration: 100% Stripe (single processor — fine, but revenue is lumpy)

**⚠️ Warnings**
1. **BURN ACCELERATING** — March out-spend (+$6.3k payroll) outpaced revenue, which *dropped* to $7.1k (from $9.2k). Two things moved the wrong way at once.
2. **AD SPEND CREEPING** — Meta Ads tripled ($600→$1.6k) with no matching revenue lift yet. Verify ROAS before scaling further.
3. **REVENUE VOLATILITY** — monthly inflow swings $7.1k–$11.6k. One slow month + the new payroll = faster burn than the average suggests.

**Top 3 actions to extend runway**
1. **Confirm the new hire pays for themselves** — they added $2.1k/mo cost. Runway holds only if revenue recovers to ≥$9k/mo. *(impact: the whole runway math)*
2. **Audit Meta Ads ROAS** — if the $1.6k isn't returning ≥$1.6k, cut it → +1 month runway. *(impact: ~$1.6k/mo)*
3. **Smooth revenue** — the lumpiness is the real risk; a slow month now breaks the model. Push for recurring/upfront billing.

*Analysis only — confirm material decisions with your accountant.*

---

> The skill **never invented a number** — every figure traces to the transactions you pasted. Missing data (e.g. no upcoming-invoice info) is flagged, not guessed.

---

## 💎 Pro pack — 6 skills, deeper analysis

The free core covers the essentials. **[Finance Skills Pro →](https://berkanova43.gumroad.com/l/mejcvwe)** adds:

- **financial-statement-builder** — full P&L + balance-sheet draft from raw ledger
- **scenario-modeler** — "what if we hire 2 people / lose our biggest client / raise prices 10%" with runway impact
- **kpi-dashboard** — auto-computes the metrics investors ask for (CAC, LTV, gross margin, MRR growth, quick ratio)
- Priority updates + new skills as the Claude Skills ecosystem grows

**One-time payment. No subscription.** [Get the Pro pack →](https://berkanova43.gumroad.com/l/mejcvwe)

---

## Who's this for
- 🧑‍💻 **Founders** — know your runway before the board asks
- 🧾 **Freelancers / agencies** — process invoices and prep for your accountant in seconds
- 📊 **Bookkeepers** — batch-categorize and catch billing errors
- 💼 **Finance teams** — faster monthly close

## Notes
These skills do analysis, not licensed financial advice — confirm material decisions with your accountant. Skills never invent numbers; missing data is flagged, not guessed.

---
⭐ **Star this repo** if it saved you a spreadsheet. New free skills added regularly.

*Made for the Claude Skills ecosystem.*

## 🔗 More Claude Skill Packs

- ⚖️ [Legal Skills](https://github.com/Uhudsavasindankacanokcu2/legal-skills-for-claude) — contract review, drafting, negotiation
- 🧑‍💼 [Recruiting & HR Skills](https://github.com/Uhudsavasindankacanokcu2/recruiting-skills-for-claude) — JDs, resume screening, interviews
- 🛒 [E-commerce Seller Skills](https://github.com/Uhudsavasindankacanokcu2/ecommerce-skills-for-claude) — listings, reviews, ad spend
