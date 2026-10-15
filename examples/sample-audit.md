# Sample Audit: speaking campaign, 3 days

Account: a keynote speaker selling to event planners and HR leaders. Two A/B speaking campaigns (two landing pages) plus an old campaign that was switched back on. CAD. Numbers are from the account export.

**Verdict: the ads earned the clicks. The account could not see a single inquiry, so Meta optimized for clickers.**

| Spend | Impressions | Link clicks | CTR | CPC | Page views | Tracked leads |
|---|---|---|---|---|---|---|
| $184.42 | 11,835 | 291 | 2.46% | $0.63 | 244 | 0 |

## Scorecard

| Area | Check | Result | Evidence |
|---|---|---|---|
| A | Conversion event | FAIL | 244 page views, 0 Lead events; pixel saw 2 hits on the landing pages |
| A | Zero is bad luck? | No | If 2% converted, odds of 0 in 244 visits = 0.7% |
| A | Objective match | FAIL | Old campaign optimized for a conversion that never fired: $40.33 at $2.02 CPC, 0 page views |
| B | Spend cap | FAIL | Old campaign reactivated with no cap |
| B | Frequency | FAIL | 1.01 to 1.13 |
| B | Hourly pacing | FAIL | 81% of speaking spend in the 9pm and midnight hours; daytime CTR 7.1% vs 2.3% at night (also the best learning day, so partly confounded) |
| B | Geography | FAIL | Canada 4.1% CTR at $0.20; US 2.5% at $0.58; US took 95% of spend (Canada sample: $7) |
| B | Placements | FAIL | Facebook Reels overlay: 20% of spend at 1.85% CTR |
| B | Audience | FAIL | 0 to 1% lookalike: 1.53% CTR vs 2.98% for 1 to 3% |
| B | Age | FAIL | 18 to 24: $2.08, 0 clicks |
| C | Format | FAIL | Video 4.43% CTR at $0.32; statics 2.12% at $0.66; statics took 78% of spend |
| C | Angle | PASS (insight) | Testimonial video 6.3% CTR, 54% hook rate; self-intro videos about 1.6 to 1.8% |
| C | Sample size | WARN | Three promising videos had about 100 impressions each; need about 2,200 to judge |
| D | Load rate | PASS | 89 to 91% |
| D | Landing page A vs B | No winner | CTR gap explained by creative mix, not the page; leads untracked |

## Ranked fixes

1. **Fire a Lead event on form submit** (pixel + Conversions API), verify in Test Events. Or run Instant Forms. Prerequisite.
2. **Spend cap on every campaign.** Turn the old campaign off.
3. **Testimonial and story videos only**, captions burned in, name in the first 3 seconds. Give each promising video about 2,200 impressions before judging. (strong for the top video, directional for the rest)
4. **Lifetime budget with an 8am to 8pm schedule.** (directional: confounded with the best day)
5. **Separate Canada ad set with its own budget.** (directional: small Canada sample)
6. **Retargeting ad set**: 50% video viewers + site visitors, 2 to 3 impressions per week. (test)
7. **Exclude Reels overlay, drop the 0 to 1% lookalike, exclude 18 to 24.** (directional)

## Not yet knowable
- Which landing page converts better (needs about 1,140 visitors per page with tracking on)
- Lead quality
- Retargeting lift

Built with ClickLeak by Ryan Perez. Support the developer: https://support.ryanperez.ca
