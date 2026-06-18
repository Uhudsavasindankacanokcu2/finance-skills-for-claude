---
name: budget-vs-actual
description: Compare planned budget against actual spending/revenue, compute variances, and explain what drove them. Produces a variance report with over/under flags and a forward forecast. Use when the user has a budget plus actuals, asks "are we on budget", "where did we overspend", monthly/quarterly review, or wants a simple forecast.
---

# Budget vs Actual (Variance Analysis)

You act as an FP&A analyst. Show where reality diverged from plan, why, and what it means going forward.

## When to use
User provides a budget AND actuals (any format), or asks about overspend, variance, budget review, or a forward forecast.

## Inputs (ask if missing)
- Budget figures by line item (and by month if available).
- Actual figures for the same lines/period.
- Period being reviewed.

## Procedure
1. Align budget and actual line items (match by name; flag unmatched lines on either side).
2. For each line compute: `variance = actual − budget`, `variance % = variance / budget`.
3. Classify: **favorable** (under-spend on cost / over-perform on revenue) vs **unfavorable**.
4. Sort by absolute variance — biggest swings first.

## Report
| Line | Budget | Actual | Variance | Var % | Fav/Unfav |

Then:
- **Headline**: total budget vs total actual, net variance, % over/under.
- **Top 3 unfavorable variances** with the amount and a plausible driver (ask the user to confirm the cause rather than inventing one).
- **Forecast**: if a trend exists across months, project the next period (simple run-rate; state the method and assumption explicitly).
- **Flags**: any line >20% over budget, any new unbudgeted spend, any revenue line >15% under plan.

## Rules
- Don't invent drivers/causes — surface the variance and ask, or label the cause as "likely" with reasoning.
- State the forecast method (run-rate, last-3-month average, etc.) so it's auditable.
- Full precision in math; clean rounding in display.
