<div align="center">

# ClickLeak 🩸

## The Meta Ads Strategist Skill for Claude

### Your ads aren't the problem. The leak after the click is.

**ClickLeak is a free, open-source Claude skill that audits your Facebook and Instagram ads like a senior media buyer, finds exactly where clicks stop turning into leads, and hands you a ranked fix list with the number behind every finding.**

[![Buy me a coffee](https://img.shields.io/badge/☕%20Buy%20me%20a%20coffee-support.ryanperez.ca-FFDD00?style=for-the-badge)](https://support.ryanperez.ca)
[![Star on GitHub](https://img.shields.io/github/stars/bowtiekreative/clickleak-meta-ads-strategist?style=for-the-badge&logo=github&label=Star)](https://github.com/bowtiekreative/clickleak-meta-ads-strategist)
[![MIT License](https://img.shields.io/badge/License-MIT-3F6EE9?style=for-the-badge)](LICENSE)

Facebook Ads · Instagram Ads · Meta Pixel · Conversions API · Ads Manager · Marketing API · Claude · Claude Code

**[Install in 60 seconds](#install-in-60-seconds)** · **[See an example](examples/sample-audit.md)** · **[☕ Support the developer](https://support.ryanperez.ca)**

</div>

---

## Why are people clicking your ads but never filling in the form?

I spent $247 on Meta ads. 521 people clicked. Zero leads came back.

On paper, the ads were winning. Click rate: **3.3%**. Cost per click: **$0.47**.

But the form on the landing page was never connected. The pixel wasn't on my pages. So Meta had no idea who actually inquired, and it did exactly what it's built to do: it found me more clickers. Cheap ones. At midnight. In the wrong country.

Most ad advice starts with "test more creatives." That advice would have cost me another $500. The real fix was upstream of every ad I made. Meta optimizes for the event it can see. **No event, no learning.**

Nobody audits the boring stuff first, because the boring stuff isn't fun to talk about. But the boring stuff is where the money leaks.

**ClickLeak does.**

> **One coffee costs less than one wasted day of ad spend.** If ClickLeak helps you, [buy me a coffee ☕](https://support.ryanperez.ca).

---

## What it does

| | |
|---|---|
| 🔍 **Audits** | Scores your account PASS / FAIL / UNKNOWN across tracking, delivery, creative, landing page and trust, with the number behind every line. |
| 🩺 **Diagnoses** | Shows you whether "zero leads" is bad luck or a broken funnel, using real math on your own visitor count. |
| 🗺️ **Plans** | Builds a funnel map, campaign structure and budget that actually adds up, then a launch checklist. |
| ✍️ **Creates** | Writes hooks, video scripts, static concepts, primary text, headlines and CTAs from your real proof, in a ready-to-load table. |
| ✂️ **Optimizes** | Applies kill and scale rules to this week's export: what to pause, what to scale, what to leave alone. |
| 📊 **Reports** | Turns raw numbers into a plain-language report a client can read in two minutes. |

---

## The core framework: The Leak Map

ClickLeak checks your account in the order the money flows, and fixes the upstream leak before touching anything downstream.

| Order | Area | The leak it hunts |
|---|---|---|
| **A** | **Measurement** | Pixel missing, forms going nowhere, campaigns optimizing for an event that never fires |
| **B** | **Delivery** | Budgets burning at midnight, money pouring into the biggest country instead of the best one, frequency stuck at 1.0 |
| **C** | **Creative** | Spend going to the cheapest impression, not the best ad. Angle vs format. Hook rate in the first 3 seconds |
| **D** | **After the click** | Slow pages losing clickers before they load, headlines that break the ad's promise |
| **E** | **Trust** | Hostile comments under the ad, the wrong Page running the ask |

**Most people start at C. The money usually leaks at A.**

---

## Why ClickLeak beats another "Facebook ads tips" thread

- ✅ **Measurement before money.** If conversions aren't tracked, that's finding #1, ahead of any creative or targeting advice.
- ✅ **No invented benchmarks.** It compares your account to itself. Every recommendation cites your number, or is labeled as a test.
- ✅ **It respects sample size.** It won't crown a winner on 100 impressions. It tells you how much data a test needs, with the formula.
- ✅ **It does the budget math out loud.** No plan leaves the room costing more than your stated budget.
- ✅ **It labels its confidence.** Every fix is marked strong, directional or test, so you know what's proven and what's a bet.
- ✅ **It refuses to fake proof.** No made-up testimonials, reviews or stats in your ads.

---

## What you get back

```
Verdict:        one sentence you can act on
Scorecard:      A to E, PASS / FAIL / UNKNOWN, evidence per line
Ranked fixes:   prerequisites first, then by impact, each with its number
                and a confidence label (strong / directional / test)
Not yet known:  what your data can't answer yet, and how much data it needs
Next 7 days:    a checklist
```

👉 **[See a full sample audit on a real account](examples/sample-audit.md)**

---

## Try it

```
Audit my Meta ads. Here's my Ads Manager export. Why am I getting clicks but no leads?
```

```
I got 400 landing page views and zero leads. Is that bad luck or is something broken?
```

```
Plan a $40/day campaign for my coaching offer, Canada and US. Make the budget math add up.
```

```
Write 6 Facebook ads from these 3 testimonials: hooks, primary text, headlines, CTAs and UTMs.
```

```
Here are 7 days of results. Apply kill rules and tell me what to pause and what to scale.
```

---

## Install in 60 seconds

### Claude apps (web, desktop, mobile)
1. Download **`meta-ads-strategist.zip`** from the [latest release](https://github.com/bowtiekreative/clickleak-meta-ads-strategist/releases/latest).
2. In Claude, go to **Customize > Skills**, click **+**, then **Create skill > Upload a skill**, and upload the ZIP.
3. Turn on **Code execution and file creation** in **Settings > Capabilities** if it isn't already.

### Claude Code
```bash
git clone https://github.com/bowtiekreative/clickleak-meta-ads-strategist ~/.claude/skills/meta-ads-strategist
```

### Any other agent
`SKILL.md` is plain Markdown. Drop it into your agent's instructions.

**That's it.** Ask Claude anything about your Meta, Facebook or Instagram ads and ClickLeak loads on its own.

> ⭐ **Installed it? [Star the repo](https://github.com/bowtiekreative/clickleak-meta-ads-strategist)** so the next founder staring at "521 clicks, 0 leads" can find it.

---

## Who it's for

- **Founders and solo operators** running their own ads with no media buyer
- **Coaches, speakers and consultants** selling high-trust services where one lead matters
- **Agencies and freelancers** who want a second set of eyes before a client asks why the leads stopped
- **Developers** building on the Meta Marketing API who want the fields mapped to strategy

---

## What's inside

```
meta-ads-strategist/
├── SKILL.md                         The strategist (this is the skill)
├── references/
│   ├── audit-checklist.md           Printable 40-point audit
│   ├── creative-playbook.md         Hooks, scripts, angles, formats
│   ├── testing-and-kill-rules.md    Sample sizes and automated rules
│   └── report-template.md           Client-ready report
├── examples/
│   └── sample-audit.md              A full audit on a real account
├── .github/FUNDING.yml              The support button on this repo
└── LICENSE                          MIT
```

---

## FAQ

**Is ClickLeak free?**
Yes. It's MIT licensed: use it, fork it, use it for clients. If it saves you money, [buy me a coffee ☕](https://support.ryanperez.ca).

**Does it connect to my ad account?**
No. It works on what you give it: Ads Manager exports, screenshots, numbers or Marketing API output.

**Does it work for Google, TikTok or LinkedIn ads?**
The measurement and testing rules apply everywhere. The structure, placement and API advice is Meta-specific.

**Will it guarantee me more leads?**
No. It finds leaks and ranks fixes using your own numbers. You still have to make the changes, and some fixes are labeled as tests because the data can't prove them yet.

**Does it replace a media buyer?**
It does the analysis a good media buyer does. You still press the buttons.

**Does it work with ChatGPT?**
It's built as a Claude skill. `SKILL.md` is plain Markdown, so you can paste it into other agents' instructions, but it's tested with Claude.

---

## Sources

- [Meta Marketing API reference](https://developers.facebook.com/docs/marketing-api)
- [Meta Marketing API: Insights parameters](https://developers.facebook.com/docs/marketing-api/insights/parameters)
- [Meta Pixel reference](https://developers.facebook.com/docs/meta-pixel/reference)
- [Conversions API: server event parameters](https://developers.facebook.com/docs/marketing-api/conversions-api/parameters/server-event)

---

<div align="center">

## ☕ If ClickLeak saves you one wasted ad budget, buy me a coffee.

I build tools like this on nights and weekends and give them away. Your support keeps them free, keeps them updated, and keeps new ones coming.

# [☕ support.ryanperez.ca](https://support.ryanperez.ca)

**⭐ Star the repo** so others find it · **🔁 Share it** with the founder who just said "the ads are getting clicks, but nobody's calling"

</div>

---

## About the author

**Ryan Perez** is a Cognitive Architect and Innovation Strategist, founder of [Bow Tie Kreative](https://bowtiekreative.com) (est. 2013, Calgary), keynote speaker, podcast host and author of three books. He builds websites, sales funnels and conversion systems for entrepreneurs, and he builds the machines that figure out what actually works.

Want the funnel behind the ads built for you? That's what [Bow Tie Kreative](https://bowtiekreative.com) does.

[ryanperez.ca](https://ryanperez.ca) · [Bow Tie Kreative](https://bowtiekreative.com) · [☕ Support the developer](https://support.ryanperez.ca)

---

## License

[MIT](LICENSE) © 2026 Ryan Perez. Use it, fork it, ship it, including commercially. A link back to [support.ryanperez.ca](https://support.ryanperez.ca) is always appreciated.

## Disclaimer

ClickLeak is an independent project. It is not affiliated with, endorsed by or sponsored by Anthropic, Meta, Facebook or Instagram. It gives analysis and recommendations, not guarantees of results. Always follow Meta's advertising policies.

<sub>Keywords: Claude skill, Meta ads strategist, Facebook ads audit, Instagram ads audit, Meta ads audit, why no leads from Facebook ads, clicks but no leads, Meta Pixel troubleshooting, Conversions API, Facebook ad copy generator, ad kill rules, Meta ads campaign plan, paid social strategist AI, Claude Code skills.</sub>
