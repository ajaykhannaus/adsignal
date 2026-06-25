# I open-sourced a 250-point paid-ads audit. Here's AdSignal.

### A free Claude Code plugin that turns Claude into a full ad auditor — and tells you exactly what to fix, ranked by dollar impact.

Most ad accounts aren't underperforming because of one big, obvious mistake. They're underperforming because of 250 small things nobody has the time to check — a duplicated conversion tag here, a budget-capped winner there, nineteen junk search terms quietly burning spend.

Agencies turn that checklist into a $1,500 one-off "ad audit." I thought the checklist itself should just be free. So I open-sourced it.

Meet **AdSignal** — the Paid-Ads Operating System.

It's a free, MIT-licensed [Claude Code](https://claude.com/claude-code) plugin that gives Claude four paid-media skills. You point it at a Google, Meta, LinkedIn, or TikTok account, and it grades the account against 250 rules across 8 categories, then hands you a prioritized fix list ranked by **how much money each issue is costing you** — not by how easy it is to spot.

- 🌐 Live site: https://ajaykhannaus.github.io/adsignal
- 📦 Repo: https://github.com/ajaykhannaus/adsignal
- 🧪 Sample audit report: https://ajaykhannaus.github.io/adsignal/demo.html

## The problem: paid ads die by a thousand cuts

If you've ever inherited an ad account, you know the feeling. Performance is "fine," spend is high, and nobody can point to *why* it's not better. The truth is usually boring: dozens of small misconfigurations compounding.

The hard part isn't fixing them — it's *finding* all of them, consistently, every time, without forgetting the unglamorous ones (tracking, negatives, attribution) that actually move the number.

That's exactly what a checklist is for. And that's what AdSignal is.

## Four commands, one operating system

Each is a Claude Code skill that activates automatically when you ask.

**/ads audit** — Grades any account against the 250 rules and returns a fix list ranked by dollar impact, with evidence and a specific instruction for each issue.

**/ads plan** — Turns a goal and a budget into a media plan: channel split, an honest forecast range (with assumptions), and a 90-day testing roadmap.

**/ads create** — Writes platform-spec ad copy — Google RSAs, Meta, LinkedIn, TikTok — starting from strategic angles, with a testing matrix so creatives ship as a structured test, not a pile.

**/ads compete** — Competitive teardown → a messaging map of crowded vs. open space → the wedge angle you can credibly own.

## How an audit actually works

1. You tell AdSignal the platform, spend, goal, and target CPA/ROAS.
2. You hand it a data export, screenshots, or a description. **It never invents numbers** — anything it can't verify is flagged "needs data," not guessed.
3. It scores every applicable rule across 8 categories.
4. You get a scorecard, a fix list ranked by $ impact, the quick wins, and the single highest-leverage action for this week.

Here's the shape of the output (sample, mock data):

```
# Ad Account Audit — Acme Co. (Google Ads, last 30 days)

Health score 62/100 · 41 pass · 12 warn · 7 fail · ~$9.4k/mo recoverable

Top fixes (ranked by $ impact)
[FAIL] Conversion tracking double-counts leads   ~$3,100/mo
[FAIL] Top campaign capped by budget             ~$2,400/mo
[WARN] 19 zero-conversion search terms           ~$1,800/mo

▸ Do this week: fix the duplicate conversion tag first.
```

You can click through a live, interactive version of that report here: https://ajaykhannaus.github.io/adsignal/demo.html

## The 250 rules, across 8 categories

1. **Account structure & settings**
2. **Budget & bidding**
3. **Targeting — keywords & audiences**
4. **Waste control — negatives & exclusions**
5. **Creative & copy**
6. **Landing page & post-click**
7. **Conversion tracking & measurement**
8. **Reporting, attribution & incrementality**

Tracking failures and starved/over-capped winners are weighted heaviest — broken data or strangled performers cost the most money. The full enumerated list (R001–R250) lives in the repo: https://github.com/ajaykhannaus/adsignal/blob/main/reference/signal-library.md

## It advises — it never touches your account

AdSignal audits and recommends. It never edits, pauses, or spends inside a live ad account on your behalf. It tells you exactly what to change, and you stay in control. That's a deliberate design choice, not a limitation.

## Why it's free

Because a checklist wants to be shared. The more people run audits and contribute rules, the better the library gets. It's MIT-licensed — use it on your own accounts, use it on your clients', fork it, add your own signals, send a PR.

## Try it

```bash
git clone https://github.com/ajaykhannaus/adsignal.git
```

Then, in Claude Code, just ask: *"audit my Google Ads account."* The skill activates on its own.

If you run paid ads — or audit them for a living — I'd love to know: **what's the one signal you'd add to the checklist?**

⭐ Star it, fork it, break it: https://github.com/ajaykhannaus/adsignal

---

*Built with Claude Code. Free & open source.*
