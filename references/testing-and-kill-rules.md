# Testing and Kill Rules

## How much data a test needs
Two-sided test, 80% power, alpha 0.05, per variant:

| To detect | Needed per variant |
|---|---|
| CTR 2.5% → 3.0% | about 16,800 impressions |
| CTR 2.5% → 4.0% | about 2,200 impressions |
| Conversion 2% → 4% | about 1,140 landing page views |

n = (1.96 * sqrt(2p(1-p)) + 0.84 * sqrt(p1(1-p1) + p2(1-p2)))^2 / (p2 - p1)^2, where p = (p1 + p2) / 2.

Creative tests cost impressions. Landing page tests cost visitors. Test creative first.

## Zero conversions
- 95% upper bound on the true rate: about 3 / n (rule of three)
- Chance of 0 if the true rate is r: (1 - r)^n
- Before calling it zero: check inbox, forms, payment processor, calendar

## Default rules (adapt to the account)
| Rule | Condition | Action | How |
|---|---|---|---|
| Dead on arrival | spend at least 3x target CPC, 0 link clicks | pause ad | Meta automated rule |
| Low CTR | 1,000+ impressions, CTR under half the account average | pause ad | Meta automated rule |
| Expensive clicks | spend 4x target CPC, CPC over 2x target | pause ad | Meta automated rule |
| Clicks, no landing | 20+ clicks, load rate under 50% | fix page or message match | weekly check |
| No conversions | spend 2x target cost per lead, 0 leads, tracking verified | pause ads to that page | weekly check |
| Hard ceiling | every campaign | spend cap = budget | campaign setting |
| Winner | CTR above account average, conversions above target | +20% budget every 3 days | weekly check |

A rule that needs a conversion cannot fire without tracking.

## Change discipline
- One variable per ad set at a time
- Big edits restart learning (Meta's guidance: roughly 50 optimization events per ad set per week to exit learning)
- Write down every change with the date
