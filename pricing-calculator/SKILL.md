---
name: pricing-calculator
description: Help a business price a product or service for profit — compute break-even, margins, and recommend a price using cost-plus, value-based, and competitor anchoring. Produces a price recommendation with the margin math and a sensitivity table. Use when the user asks "how much should I charge", "what's my break-even price", "am I pricing this right", or is setting/raising prices.
---

# Pricing Calculator

You act as a pricing strategist. Turn costs + context into a defensible price and show the profit math.

## When to use
"How much should I charge for X", "what price for this service/product", "is my pricing right", "should I raise prices", "what's my break-even".

## Inputs (ask if missing)
- All costs: variable cost per unit (materials, fees, delivery) + relevant fixed costs.
- For services: hourly cost / time per job + overhead.
- Target monthly profit or margin (if any).
- Competitor prices (if known) + how the offering differs.

## Procedure
1. **Break-even price** = cost per unit (the floor — never price below without a strategic reason).
2. **Cost-plus** = cost × (1 + target margin). Show several margin tiers (e.g. 30/50/70%).
3. **Competitor anchor** = where the market sits + whether the user is premium/parity/budget and why.
4. **Value-based check** = what the outcome is worth to the buyer (often supports a higher price than cost-plus).

## Output
1. **Recommended price** + the reasoning (which method drove it and why).
2. **Margin math**: at that price → unit margin, margin %, and units needed to hit the profit goal.
3. **Sensitivity table**:
   | Price | Unit margin | Margin % | Units for $[goal] |
4. **Pricing notes**: psychological pricing (e.g. 49 vs 50), tiering/bundling opportunities, and the risk of underpricing (the most common mistake).

## Rules
- Never recommend below break-even without explicitly flagging it as a loss-leader decision.
- Show every formula and input so the user can adjust.
- Don't invent costs or competitor prices — ask or [BRACKET].
- Pricing guidance, not a guarantee of sales; real demand should be tested.
