# AdSignal — The 250 Rules

The complete checklist that powers `ads-audit`. **250 numbered rules** across
**8 categories**. Most rules apply to Google, Microsoft, Meta, LinkedIn and TikTok —
where a rule is platform-specific it says so.

For each rule an auditor records: **status** (Pass / Warn / Fail / N/A),
**evidence**, and the **estimated monthly $ impact** of fixing it. A rule that can't
be checked with the available data is **N/A — needs data**, never a guess.

> Severity weighting: tracking failures (category 7) and starved/over-capped winners
> (category 2) are weighted heaviest — broken data or strangled performers cost the
> most money.

---

## 1. Account structure & settings  (R001–R028)

- **R001** — Campaigns are segmented by intent, margin, or funnel stage, not lumped together.
- **R002** — Ad groups are tightly themed (a handful of closely-related keywords each).
- **R003** — Search and Display are split into separate campaigns (no Display riding on a "Search" campaign).
- **R004** — Search-partner / audience-network settings are reviewed and chosen deliberately.
- **R005** — Geo-targeting uses *presence* ("people in") not *presence-or-interest*, unless interest is intended.
- **R006** — Regions you can't serve are added as location exclusions.
- **R007** — Ad scheduling reflects when conversions actually happen, not 24/7 by default.
- **R008** — Device bid adjustments match device-level performance (mobile vs. desktop vs. tablet).
- **R009** — Language and audience settings match the real market and customer.
- **R010** — A consistent, human-readable naming convention is used across campaigns and ad groups.
- **R011** — Portfolio / shared bid strategies are applied intentionally, not inherited by accident.
- **R012** — Shared budgets aren't masking which campaign actually deserves the money.
- **R013** — No paused-but-still-spending experiments or drafts are bleeding budget.
- **R014** — Campaign types are right for the goal (Search vs. PMax vs. Demand Gen vs. Shopping).
- **R015** — PMax and standard Shopping aren't cannibalizing the same inventory uncontrolled.
- **R016** — Auto-applied recommendations are turned off (or reviewed), not silently rewriting the account.
- **R017** — Account-level brand exclusions / brand lists are configured for PMax and Demand Gen.
- **R018** — Conversion goals are set at the right level (account default vs. campaign-specific override).
- **R019** — Final-URL expansion / dynamic URLs are controlled, not sending traffic anywhere.
- **R020** — Currency, time zone, and billing settings are correct (wrong time zone skews dayparting).
- **R021** — Account access and MCC/manager links are clean; no orphaned or over-privileged users.
- **R022** — Campaign experiments / drafts are used for changes instead of editing live winners blind.
- **R023** — Seasonality adjustments are scheduled for known peaks instead of reacting late.
- **R024** — Ad rotation is set deliberately (optimize vs. rotate) per campaign intent.
- **R025** — Frequency caps are set on awareness/Display/video campaigns to avoid over-serving.
- **R026** — Campaign priorities (Shopping low/med/high) are configured so the right one wins the auction.
- **R027** — There are no duplicate campaigns competing against each other in the same auction.
- **R028** — Account structure is documented so anyone can understand it in five minutes.

## 2. Budget & bidding  (R029–R058)

- **R029** — Best-performing campaigns are not capped by budget (check "lost IS — budget").
- **R030** — Bid strategy matches the goal (tCPA / tROAS / max-conv vs. max-clicks vs. manual).
- **R031** — Target CPA is set from real data, not an aspirational guess.
- **R032** — Target ROAS is realistic for the margin and historical conversion value.
- **R033** — Each campaign has enough conversions (~15–30/mo) for smart bidding to learn.
- **R034** — No campaign is stuck in "Learning" indefinitely after every small edit.
- **R035** — Bid changes are made in moderate steps, not 50%+ swings that reset learning.
- **R036** — Budget follows performance — winners funded, persistent losers starved.
- **R037** — No budget sits on zero-conversion campaigns "just in case".
- **R038** — Spend paces evenly across the month, not front-loaded then dark.
- **R039** — Dayparting and weekday/weekend patterns are reflected in budgets or schedules.
- **R040** — Bid adjustments (device × location × audience) aren't stacking into runaway CPCs.
- **R041** — tCPA/tROAS targets aren't so aggressive they choke volume to near-zero.
- **R042** — tCPA/tROAS targets aren't so loose they overpay for easy conversions.
- **R043** — Manual/enhanced CPC is only used where smart bidding genuinely lacks data.
- **R044** — Branded and non-branded campaigns have separate, appropriate targets.
- **R045** — Seasonality adjustments (not target changes) are used for short spikes.
- **R046** — Budget headroom exists on scaling campaigns so smart bidding can capture demand.
- **R047** — Impression share lost to rank vs. budget is diagnosed and acted on separately.
- **R048** — CPA / ROAS is compared against the business break-even, not just an internal KPI.
- **R049** — Top-of-funnel and bottom-of-funnel campaigns are budgeted to their distinct roles.
- **R050** — Retargeting budget is sized to audience size (not overspending a tiny list).
- **R051** — New campaigns get a deliberate learning budget, not a trickle that never exits learning.
- **R052** — Bid strategy changes are logged with dates to correlate with performance shifts.
- **R053** — Value rules / conversion-value adjustments are used where some conversions are worth more.
- **R054** — Shopping/PMax budgets account for product margin, not just blended ROAS.
- **R055** — Budget isn't spread so thin across campaigns that none can learn.
- **R056** — Automated rules / scripts guard against runaway spend and broken-tracking spend.
- **R057** — Bid floors/ceilings (where supported) protect against auction-price spikes.
- **R058** — The single highest-spend, lowest-return line item is identified every review.

## 3. Targeting — keywords & audiences  (R059–R092)

- **R059** — Match types are intentional; broad match is only paired with smart bidding + strong negatives.
- **R060** — High-spend keywords are mapped to their actual converting search terms.
- **R061** — Zero-conversion, high-spend keywords are flagged for pause or rework.
- **R062** — Quality Score components (expected CTR, ad relevance, LP experience) are diagnosed, not ignored.
- **R063** — Single-theme or single-keyword ad groups are used where relevance matters most.
- **R064** — Brand and non-brand keywords live in separate campaigns and are measured separately.
- **R065** — Competitor-term campaigns are deliberate, compliant, and measured for ROI.
- **R066** — Keyword cannibalization / duplicates across ad groups are removed.
- **R067** — Long-tail, high-intent terms are captured, not just expensive head terms.
- **R068** — Match-type overlap is managed so the cheapest qualifying match wins.
- **R069** — Remarketing lists exist, are populated, and aren't expired or too small.
- **R070** — Customer-match lists are uploaded, fresh, and segmented (buyers, churned, high-value).
- **R071** — Lookalike / similar audiences are built from high-quality seed lists, not all-traffic.
- **R072** — In-market and affinity audiences are layered (observe → then bid) where they perform.
- **R073** — Demographic targeting/exclusions reflect actual converter data (age, gender, income).
- **R074** — Meta: Advantage+ / detailed-targeting expansion is monitored, not blindly trusted.
- **R075** — Audience sizes are neither too narrow (no delivery) nor too broad (no relevance).
- **R076** — Retargeting windows match the buying cycle (7/14/30/90 days as appropriate).
- **R077** — Existing customers are excluded from prospecting (unless upsell is the goal).
- **R078** — Recent converters are excluded from campaigns where re-serving wastes spend.
- **R079** — LinkedIn: targeting uses the right lever (job function + seniority, not just title).
- **R080** — LinkedIn: audience expansion and Audience Network are toggled deliberately.
- **R081** — TikTok: interest + behavior targeting is tested against broad/auto-targeting.
- **R082** — Geo-layered bid adjustments reflect where conversions actually come from.
- **R083** — Dayparting audiences/segments align with when the target audience converts.
- **R084** — First-party data (CRM, purchase, LTV) feeds audiences, not just pixel traffic.
- **R085** — Sequential retargeting moves users down-funnel with different messages per stage.
- **R086** — Suppression lists (current customers, do-not-target, refunds) are applied.
- **R087** — Audience overlap between ad sets is checked to avoid self-competition.
- **R088** — Placements are chosen/excluded deliberately (feed vs. Audience Network vs. Reels).
- **R089** — Keyword/audience themes map cleanly to a matching landing page.
- **R090** — Dynamic Search Ads (if used) have tight page feeds and strong negatives.
- **R091** — PMax audience signals are seeded with real first-party + high-intent data.
- **R092** — New audiences are introduced as tests with a clear hypothesis, not bulk-dumped.

## 4. Waste control — negatives & exclusions  (R093–R120)

- **R093** — Negative keyword lists exist and are applied to the correct campaigns.
- **R094** — The search-terms report is mined regularly for irrelevant queries.
- **R095** — Converting-zero search terms above a spend threshold are negated.
- **R096** — Brand terms are negated out of non-brand campaigns (and vice versa).
- **R097** — Competitor/irrelevant-intent terms ("free", "jobs", "diy") are negated where they don't convert.
- **R098** — A master negative list of universally-irrelevant terms is maintained.
- **R099** — Negative match types are correct (phrase/exact) so you don't over-block good traffic.
- **R100** — Placement exclusions remove junk apps, MFA sites, and autoplay video on Display.
- **R101** — Mobile-app category and game-app placements are excluded on Display unless intended.
- **R102** — Content/topic exclusions keep ads off sensitive or off-brand content.
- **R103** — Negative audiences (existing customers, recent converters) are applied where relevant.
- **R104** — Out-of-stock / discontinued products are excluded from Shopping/PMax feeds.
- **R105** — Low-margin or loss-leader SKUs are excluded or down-weighted where they erode ROAS.
- **R106** — IP exclusions block office, agency, and known-bot traffic.
- **R107** — Non-target locations are excluded, not just unselected.
- **R108** — Duplicate-keyword cannibalization across campaigns is removed.
- **R109** — Frequency caps stop over-serving the same user into fatigue/waste.
- **R110** — Audience-network / search-partner traffic is excluded if it converts poorly.
- **R111** — Broad-match terms are reined in with a robust negative strategy.
- **R112** — Spam/lead-quality filters catch junk form fills before they pollute conversion data.
- **R113** — Click fraud / invalid traffic patterns are monitored and reported.
- **R114** — Day/hour windows with zero conversions and real spend are scheduled out.
- **R115** — Devices that consistently lose money are bid down or excluded.
- **R116** — Demographics that never convert are excluded after enough data.
- **R117** — Underperforming placements identified in reports are added to exclusion lists.
- **R118** — Negative keyword conflicts (a negative blocking an active keyword) are detected.
- **R119** — Seasonal/event negatives are added when irrelevant spikes appear.
- **R120** — A recurring "waste review" cadence (weekly/biweekly) is in place, not ad hoc.

## 5. Creative & copy  (R121–R156)

- **R121** — Every ad group has at least one strong RSA with the recommended asset count.
- **R122** — Headlines cover multiple distinct angles, not 15 paraphrases of one idea.
- **R123** — The primary keyword appears in several headlines where it lifts relevance.
- **R124** — At least one clear, singular call-to-action is present per ad.
- **R125** — The offer/value proposition is explicit, not buried in features.
- **R126** — Benefits lead; features support — copy isn't a spec sheet.
- **R127** — Ad copy matches the searcher's intent and the keyword theme.
- **R128** — Pricing, promotions, or urgency are used where they genuinely apply.
- **R129** — Ad extensions/assets are complete: sitelinks, callouts, structured snippets, images, price, lead form.
- **R130** — Sitelinks point to distinct, relevant pages (not all to the homepage).
- **R131** — Callouts communicate real differentiators, not generic filler.
- **R132** — At least 3–4 creative variations per ad set are live for testing.
- **R133** — Creative fatigue is monitored (rising frequency, falling CTR over time).
- **R134** — Fresh creative is shipped on a regular cadence before fatigue sets in.
- **R135** — Video hooks land in the first 3 seconds (the scroll-stopper).
- **R136** — Aspect ratios and formats are native to each placement (9:16 Reels/TikTok, 1:1 feed, etc.).
- **R137** — On-screen text/captions are present for sound-off viewing.
- **R138** — Branding appears early enough to register but not so early it repels.
- **R139** — Social proof (reviews, counts, logos, testimonials) is used where credible.
- **R140** — Claims are verifiable and compliant (no unsupported superlatives or restricted claims).
- **R141** — Message match: the ad's promise is answered above the fold on the landing page.
- **R142** — UGC / native-style creative is tested against polished studio ads on social.
- **R143** — Different angles (pain, outcome, status, risk-reversal, speed) are tested, not just colors.
- **R144** — Headlines respect character limits and don't truncate awkwardly.
- **R145** — Display/responsive display assets include enough images, logos, and text variants.
- **R146** — Thumbnails (YouTube/Demand Gen) are designed to earn the click, not auto-picked.
- **R147** — CTAs/buttons match the funnel stage (Learn More for cold, Shop/Sign Up for warm).
- **R148** — Emojis, symbols, and formatting are used tastefully and within policy.
- **R149** — Localization/translation is correct for each market (not machine-mangled).
- **R150** — A/B tests isolate one variable at a time for a clean read.
- **R151** — Winning creatives are scaled and losers are retired on a schedule.
- **R152** — Dynamic creative optimization is used where the platform rewards it.
- **R153** — Brand voice is consistent across ads, extensions, and landing pages.
- **R154** — Seasonal/timely creative is refreshed for events, holidays, and launches.
- **R155** — Each ad has a logged hypothesis and a success metric — creatives ship as tests, not a pile.
- **R156** — Compliance/policy review is done before launch to avoid disapprovals and account flags.

## 6. Landing page & post-click  (R157–R188)

- **R157** — Page load time is fast, especially on mobile (LCP under ~2.5s).
- **R158** — The above-the-fold answers the ad's promise within ~5 seconds.
- **R159** — There is one primary CTA, repeated, not competing CTAs.
- **R160** — Forms ask only for what's needed; every extra field costs conversions.
- **R161** — The mobile layout is genuinely usable, not a shrunk desktop page.
- **R162** — Trust signals (reviews, guarantees, security badges, real photos) are present.
- **R163** — The page matches the keyword/audience intent and the ad creative.
- **R164** — There are no broken links, 404s, or redirect chains burning click budget.
- **R165** — Form submissions, calls, and chats actually fire a tracked conversion.
- **R166** — The headline restates the core promise/offer from the ad.
- **R167** — Copy is scannable: short paragraphs, subheads, bullets — not a wall of text.
- **R168** — Friction (forced account creation, surprise costs, long forms) is minimized.
- **R169** — Social proof is specific (named testimonials, real numbers) not generic.
- **R170** — A clear value proposition appears before any ask.
- **R171** — The CTA button copy is action- and value-oriented ("Get my quote", not "Submit").
- **R172** — Exit-intent or remarketing capture is in place for non-converters where appropriate.
- **R173** — Thank-you / confirmation pages exist and fire conversion events reliably.
- **R174** — Multi-step funnels don't leak users at an identifiable step (funnel drop-off checked).
- **R175** — Page speed and Core Web Vitals are monitored, not assumed.
- **R176** — Personalization/dynamic text matches the campaign or keyword where used.
- **R177** — The offer on the page is current (no expired promos from old campaigns).
- **R178** — Navigation distractions are removed on dedicated landing pages (focused path).
- **R179** — Accessibility basics (contrast, alt text, tab order) are met.
- **R180** — Phone numbers are click-to-call on mobile and tracked.
- **R181** — Live chat / messaging, if present, is staffed during ad-serving hours.
- **R182** — Pricing/qualification info is clear enough to filter out bad-fit leads.
- **R183** — The page works across major browsers and devices (cross-browser QA).
- **R184** — Consent banners/cookie prompts don't block the CTA or break tracking.
- **R185** — A/B tests are run on headlines, CTAs, and form length, with enough sample size.
- **R186** — Post-conversion next steps (calendar, onboarding, follow-up) are defined.
- **R187** — Landing pages are kept in sync with seasonal/creative changes upstream.
- **R188** — Lead-to-sale quality is fed back so the best landing pages get more budget.

## 7. Conversion tracking & measurement  (R189–R218)

- **R189** — Conversion tracking is installed and actually firing (verify this first — bad data breaks everything else).
- **R190** — No duplicate or double-counted conversions inflate performance.
- **R191** — Primary vs. secondary conversions are classified correctly (only true goals bid toward).
- **R192** — Conversion values are populated for value-based bidding (not all "1").
- **R193** — Enhanced conversions / server-side tracking / CAPI is deployed where available.
- **R194** — The attribution window is set deliberately (click and view windows reviewed).
- **R195** — The attribution model is chosen on purpose (data-driven vs. last-click).
- **R196** — Cross-domain tracking works where the funnel spans multiple domains.
- **R197** — Consent mode / privacy signals are configured so conversions still model correctly.
- **R198** — Offline conversion import connects CRM outcomes back to clicks (for lead-gen).
- **R199** — Phone-call tracking (call extensions, dynamic numbers) is validated end-to-end.
- **R200** — Form-fill tracking is validated with a real test submission.
- **R201** — E-commerce purchase tracking matches backend revenue within tolerance.
- **R202** — Conversion lag is understood so recent data isn't misread as a drop.
- **R203** — There are no tracking gaps after recent site, CMS, or tag changes.
- **R204** — The pixel/tag fires once per event, on the right trigger, on the right page.
- **R205** — UTM parameters are consistent and not stripped by redirects.
- **R206** — Google Ads ↔ GA4 ↔ platform conversion counts are reconciled and explained.
- **R207** — Bot/spam conversions are filtered out of optimization data.
- **R208** — Micro-conversions are tracked as secondary signals, not optimized as primary.
- **R209** — Conversion values reflect margin/LTV where possible, not just order value.
- **R210** — Server-side / first-party data collection is in place against cookie loss.
- **R211** — Deduplication between platform pixel and CAPI is configured (event IDs).
- **R212** — Tag firing is monitored continuously (tag-health alerts), not checked once.
- **R213** — Test/staging traffic and internal users are excluded from conversion data.
- **R214** — Each campaign's conversion action is the right one for its funnel stage.
- **R215** — Imported/derived conversions are documented so reports are interpretable.
- **R216** — Conversion definitions are consistent across all platforms being compared.
- **R217** — Data retention and consent settings won't silently erode reporting windows.
- **R218** — A documented "tracking spec" exists so changes don't quietly break measurement.

## 8. Reporting, attribution & incrementality  (R219–R250)

- **R219** — KPIs tie to business outcomes (revenue, pipeline, LTV), not vanity clicks.
- **R220** — Brand and non-brand are reported separately so brand doesn't flatter the account.
- **R221** — New-customer vs. returning-customer performance is visible and tracked.
- **R222** — The attribution model isn't over-crediting last-click (or any single touch).
- **R223** — Incrementality is tested for big channels (geo holdout, lift, or conversion-lift study).
- **R224** — Wasted spend and the CPA/ROAS gap to target are surfaced every report.
- **R225** — Pacing vs. budget and forecast is monitored, with anomaly alerts.
- **R226** — A documented testing roadmap exists and is actively followed.
- **R227** — Reports compare against the right benchmark (prior period, YoY, and goal).
- **R228** — Statistical significance is respected before declaring test winners.
- **R229** — Blended/cross-channel performance is viewed, not just platform-reported silos.
- **R230** — Platform-reported conversions are sanity-checked against true backend sales.
- **R231** — Assisted conversions / path analysis inform upper-funnel value.
- **R232** — Cohort / LTV analysis distinguishes cheap-but-bad from costlier-but-loyal customers.
- **R233** — Lead quality (close rate, revenue per lead) feeds back into optimization.
- **R234** — Reports separate signal from noise (smoothing, not reacting to one bad day).
- **R235** — Spend, CPA, ROAS, and volume trends are reviewed together, not in isolation.
- **R236** — Marginal ROAS (next-dollar return) guides scaling, not just average ROAS.
- **R237** — Seasonality and external events are annotated on performance charts.
- **R238** — Competitive metrics (impression share, auction insights) are tracked over time.
- **R239** — A clear, repeatable reporting cadence and owner exist.
- **R240** — Dashboards show the few decisions-driving metrics, not 50 vanity tiles.
- **R241** — Forecasts are presented as ranges with stated assumptions, never single-point promises.
- **R242** — Budget reallocation decisions are documented and revisited.
- **R243** — Channel mix is reviewed against funnel role (capture vs. demand-gen vs. retention).
- **R244** — Creative-level performance is reported so winners inform the next round.
- **R245** — Audience/segment-level performance is reported to guide targeting shifts.
- **R246** — Data-driven attribution is validated against incrementality, not trusted blindly.
- **R247** — Year-over-year and account-health trends are tracked, not just last 7 days.
- **R248** — Every recurring report ends with prioritized actions, not just numbers.
- **R249** — Learnings are logged in a shared place so tests aren't repeated.
- **R250** — Each review closes with the single highest-leverage action for the coming week.

---

### Scoring
Health score = weighted pass rate, with **tracking failures (cat. 7)** and
**starved/over-capped winners (cat. 2)** weighted heaviest. Always rank the fix list
by **estimated $ impact**, surface quick wins (high impact, low effort) separately,
and end with the one action that matters most this week.
