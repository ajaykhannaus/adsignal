<div align="center">

# AdSignal

### The Paid-Ads Operating System

Turn Claude into a full marketing auditor that checks **250 rules** across Google,
Meta, LinkedIn, TikTok & Microsoft Ads — and tells you **exactly what to fix**.

[**🌐 Website**](https://ajaykhannaus.github.io/adsignal) ·
[**📋 Signal Library**](reference/signal-library.md) ·
[**MIT License**](LICENSE)

</div>

---

## What it is

AdSignal is an open-source [Claude Code](https://claude.com/claude-code) plugin. It
gives Claude four paid-media skills so you can audit, plan, write, and out-position
ad campaigns from your terminal — an agency-grade workflow that's **100% free and
open source**.

| Skill | What it does | Try it with |
|-------|--------------|-------------|
| **`ads-audit`** | Grades an account against 250 rules and returns a prioritized, dollar-impact fix list | *"Audit my Google Ads account"* |
| **`ads-plan`** | Builds a media plan, budget split, forecast, and 90-day test roadmap | *"Plan my $10k/mo ad budget"* |
| **`ads-create`** | Writes platform-spec ad copy and creative, with a testing matrix | *"Write Google RSAs for my SaaS"* |
| **`ads-compete`** | Competitive teardown → messaging map → the wedge you can own | *"Analyze my competitors' ads"* |

## Install

AdSignal is a standard Claude Code plugin. Clone it and point Claude Code at the
skills, or add it to your plugin marketplace.

```bash
git clone https://github.com/ajaykhannaus/adsignal.git
```

Then in Claude Code, the skills activate automatically when you ask an ads question
("audit my campaigns", "plan my budget", "write me some ads", "analyze competitors").

## How an audit works

1. You tell AdSignal the platform, spend, goal, and target CPA/ROAS.
2. You hand it a data export, screenshots, or a description — **it never invents numbers.**
3. It scores every applicable signal across 8 categories.
4. You get a scorecard, a fix list ranked by **$ impact**, quick wins, and the single
   highest-leverage action for this week.

See the full checklist in [`reference/signal-library.md`](reference/signal-library.md).

## The 8 signal categories

1. Account structure & settings
2. Budget & bidding
3. Targeting — keywords & audiences
4. Waste control — negatives & exclusions
5. Creative & copy
6. Landing page & post-click
7. Conversion tracking & measurement
8. Reporting, attribution & incrementality

## Safety & scope

AdSignal **audits and advises**. It never edits, pauses, or spends inside a live ad
account on your behalf — it tells you exactly what to change so you stay in control.

## Contributing

Issues and PRs welcome — especially new signals, platform-specific checks, and
real-world audit examples. This is an open-source project under the MIT license.

## License

[MIT](LICENSE) © Ajay Khanna
