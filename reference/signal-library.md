# AdSignal — The Signal Library

The checklist that powers `ads-audit`. It is organized into **8 categories**. Most
signals apply across platforms (Google, Microsoft, Meta, LinkedIn, TikTok), so the
base list below multiplies out to **250+ checks** once you fan it across the
platforms a given account runs on.

For each signal an auditor records: **status** (Pass / Warn / Fail / N/A),
**evidence**, and **estimated monthly $ impact** of fixing it.

---

## 1. Account structure & settings
- Campaigns segmented by intent / margin / funnel stage, not lumped together
- Ad groups tightly themed (a handful of closely-related keywords each)
- Search and Display separated (no Display on a "Search" campaign)
- Network settings correct (search partners / audience network reviewed)
- Geo-targeting set to *presence*, not *presence or interest*, unless intended
- Excluded locations for regions you can't serve
- Ad scheduling aligned to when conversions actually happen
- Device bid adjustments reflect device-level performance
- Language & audience settings match the market
- Naming convention consistent and human-readable
- Shared budgets / portfolio bid strategies used intentionally, not by accident
- Conflicting or paused-but-spending experiments cleaned up

## 2. Budget & bidding
- Budget not capped on your best campaigns (lost impression share to budget)
- Bid strategy matches the goal (tCPA/tROAS vs. max clicks vs. manual)
- Target CPA / ROAS set to a realistic, data-backed number
- Enough conversions per campaign for smart bidding to learn (volume check)
- No campaigns stuck in "Learning" indefinitely
- Bid adjustments not stacking into runaway CPCs
- Budget allocation follows performance (winners funded, losers starved)
- Dayparting / seasonality accounted for
- No orphan budget on zero-conversion campaigns
- Spend pacing smooth, not front-loaded and dark by mid-month

## 3. Targeting — keywords & audiences
- Match types intentional (broad only with strong negatives + smart bidding)
- Single-keyword or tightly-themed ad groups where it matters
- High-spend / zero-conversion keywords identified
- Quality Score / relevance diagnosed (expected CTR, ad relevance, LP experience)
- Audience layering (in-market, remarketing, customer match) applied
- Remarketing lists present, populated, and not expired
- Customer match / lookalikes uploaded and fresh
- Demographic exclusions where data justifies
- Placement / publisher lists reviewed (Display, PMax, Audience Network)
- Detailed-targeting expansion / Advantage+ behavior understood, not blindly on

## 4. Waste control — negatives & exclusions
- Negative keyword lists exist and are applied to the right campaigns
- Search-terms report mined for irrelevant / converting-zero queries
- Brand vs. non-brand separated and measured independently
- Competitor terms handled deliberately
- Placement exclusions for junk apps / MFA sites / autoplay video
- Mobile-app category exclusions on Display
- Negative audiences (existing customers, recent converters) where relevant
- Duplicate-keyword cannibalization removed
- Out-of-stock / discontinued products excluded from Shopping/PMax feeds
- IP / location exclusions for offices, bots, and non-markets

## 5. Creative & copy
- Each ad group has ≥1 strong RSA with the recommended asset count
- Multiple distinct angles tested, not 15 paraphrases of one idea
- Keyword present in headlines where it raises relevance
- Ad extensions / assets complete (sitelinks, callouts, structured snippets, image, etc.)
- CTAs clear and singular
- Creative fatigue checked (frequency, declining CTR over time) on social
- Thumb-stopping first 3 seconds on video
- Aspect ratios / placements native to each surface
- Brand safety and compliance (no unverifiable claims, policy violations)
- Landing-page promise matches the ad's promise (message match)

## 6. Landing page & post-click
- Page load speed acceptable on mobile
- Above-the-fold answers the ad's promise in 5 seconds
- One primary CTA, friction removed from the form
- Mobile layout actually usable, not a shrunk desktop
- Trust signals present (proof, reviews, guarantees)
- Page matches the keyword/audience intent
- No broken links, 404s, or redirect chains burning click budget
- Form submissions / calls actually fire a conversion

## 7. Conversion tracking & measurement
- Conversion tracking installed and firing (the #1 thing to verify first)
- No duplicate or double-counted conversions
- Primary vs. secondary conversions classified correctly
- Conversion values populated for value-based bidding
- Enhanced conversions / server-side / CAPI deployed where available
- Attribution window and model set deliberately
- Cross-domain / consent-mode handled
- Offline conversion import for lead-gen pipelines
- Phone-call and form tracking validated end-to-end
- No tracking gaps after recent site or tag changes

## 8. Reporting, attribution & incrementality
- KPIs tie to business outcomes (revenue / pipeline), not vanity clicks
- Brand and non-brand reported separately so brand doesn't flatter the account
- New-customer vs. returning split visible
- Attribution model understood; not over-crediting last-click
- Incrementality / geo-holdout or lift testing for big channels
- Wasted-spend and CPA-gap surfaced in the regular report
- Anomaly / pacing alerts in place
- A documented testing roadmap exists and is being followed

---

### Scoring
Health score = weighted pass rate, with **tracking failures and budget-capped
winners weighted heaviest** (broken data or starved winners cost the most money).
A signal that can't be checked with the available data is **N/A — needs data**,
never a guess.
