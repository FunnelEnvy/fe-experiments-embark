# Embark: Experiment Roadmap

## How to Read This Roadmap

Experiments are scored using the ICE framework:
- **Impact** (1-5): Expected effect on conversion or revenue if the variant wins
- **Confidence** (1-5): How certain we are this will produce a measurable result
- **Ease** (1-5): Implementation effort (5 = trivial, 1 = major engineering)

Experiments are grouped into three tiers:
- **Quick Wins:** High confidence, high ease. Run these first to build momentum.
- **Strategic Bets:** High impact, moderate confidence. Higher effort, higher payoff.
- **Explorations:** Lower confidence, high learning potential. Run when you have bandwidth.

---

## Roadmap Summary

| # | Experiment | Page | Tier | I | C | E | ICE |
|---|-----------|------|------|---|---|---|-----|
| 1 | Homepage Hero: Differentiation-Led Messaging with Proof | / | Strategic Bet | 5 | 4 | 3 | 12 |
| 2 | Homepage Secondary Conversion: Content Offer for Unready Visitors | / | Quick Win | 3 | 4 | 4 | 11 |
| 3 | Objection Preemption: Independence as Advantage | /contact, /what-we-do/* | Quick Win | 3 | 4 | 4 | 11 |
| 4 | Contact Page: Paid Traffic Message Alignment | /contact | Strategic Bet | 4 | 4 | 3 | 11 |
| 5 | Service Page Differentiation with Contextual Conversion Paths | /what-we-do/* | Strategic Bet | 4 | 3 | 3 | 10 |
| 6 | Segment-Based Hero Personalization | / | Exploration | 4 | 2 | 1 | 7 |
| 7 | Persona-Based Navigation Paths | Site-wide navigation | Exploration | 4 | 2 | 1 | 7 |
| 8 | Finance Function Readiness Assessment | New page | Exploration | 3 | 2 | 2 | 7 |

---

## Quick Wins

### 2. Homepage Secondary Conversion: Content Offer for Unready Visitors

**Page:** /
**What to test:** Add a mid-funnel content download offer to the homepage for visitors not ready to "Talk to an advisor."

**Current state:** The homepage has two CTAs ("What we do" and "Talk to an advisor") with no mid-funnel conversion path. Visitors who are interested but not ready for a sales conversation have no way to engage further. Zero form conversions happen on the homepage. Meanwhile, resource template pages elsewhere on the site convert at 6.55% (post-merger integration checklist at 6.44%, 13-week cash flow template at 12.66%).
**Baseline:** 6,673 sessions/mo, 59.5% bounce, 0% CVR
**Test Feasibility:** Cannot estimate duration (no conversion rate baseline for content offer). New mechanism, so baseline will be established during test.
**Proposed change:** Add a contextual content download offer below the hero section. Feature one of Embark's high-converting resource templates (e.g., Post-Merger Integration Checklist or 13-Week Cash Flow Template) with a brief value description and inline email capture. Position as secondary CTA, visually subordinate to "Talk to an advisor."

> **Before:** Two CTAs: "What we do" (navigational) and "Talk to an advisor" (high-commitment). No mid-funnel option. 0% homepage conversion.
> **After:** Same two CTAs plus a content offer section: "Download: Post-Merger Integration Checklist. The step-by-step guide used by PE-backed companies navigating complex integrations." [Email field] [Download]

**Why this should work:** The homepage gets 6,673 sessions/mo but converts zero. Most visitors are not ready for a sales conversation on their first visit (90% of site traffic is new visitors). Resource templates already convert at 6.55% when visitors find them. Placing a proven content offer on the highest-traffic page creates a capture mechanism for the interested-but-not-ready segment. This is a new conversion path, not a replacement for the primary CTA.

**Target metric:** Content offer download rate (new), secondary: "Talk to an advisor" click rate (monitor for cannibalization)
**Audience:** New visitors to homepage, all sources

**Scores:** Impact 3 | Confidence 4 | Ease 4
Impact 3: Adds a conversion mechanism to a zero-converting page, but this captures mid-funnel leads, not bottom-funnel. Incremental, not transformational. Confidence 4: Resource templates already convert at 6.55% elsewhere on the site, validating demand for this content type. GA4 data confirms high new-visitor volume. Ease 4: Adding a content section with an existing template requires no new content creation, just placement and form setup.

**What a win proves:** Homepage visitors will convert on mid-funnel content when given the option. Validates the content-offer model for deployment on service and industry pages (Experiment #5).
**What a loss teaches:** Homepage visitors may have different intent than resource page visitors. The template content that works for organic search visitors may not resonate with direct/paid traffic that dominates the homepage. Would suggest testing different offer types (assessment, consultation preview) instead.

---

### 3. Objection Preemption: Independence as Advantage

**Page:** /contact and /what-we-do/financial-advisory-consulting
**What to test:** Proactively reframe Embark's non-CPA status as a buyer advantage on high-intent pages, rather than leaving it as a footer disclaimer.

**Current state:** "Embark is not a CPA firm" appears only as a disclaimer in the website footer. The contact page and service pages make no proactive mention of why independence from audit and tax work benefits the buyer. The objection cheat sheet has a strong rebuttal ("No audit conflicts. No independence constraints. We advise you without restrictions."), but this messaging is not surfaced anywhere on the website. Buyers who notice the disclaimer or recognize that Embark is not a CPA firm receive no reframing context.
**Baseline:** /contact: 1,480 sessions/mo, 63.1% bounce, 1.19% CVR. /what-we-do/financial-advisory-consulting: 212 sessions/mo, 37.0% bounce, 0% CVR.
**Test Feasibility:** ~7 weeks at 15% MDE on /contact using engagement rate (2 variants, ~1,214 samples/variant). Extended. Consider form_start as micro-conversion for faster signal.
**Proposed change:** Add an "Independence is our advantage" content block on the /contact page (above or adjacent to the form) and on /what-we-do/financial-advisory-consulting. Content reframes the non-CPA status positively: why advisory independence means unrestricted counsel without audit conflicts.

> **Before:** Footer disclaimer: "Embark is not a CPA firm." No proactive reframing on any page.
> **After:** Content block on /contact: "Why independence matters. Your auditor should audit. We should advise. Because we don't perform audits or tax work, we advise you without the independence constraints that limit CPA firms who audit and advise the same client. No conflicts. No restrictions. Just unrestricted advisory from Big 4 Alumni who chose consulting."

**Why this should work:** Unanswered objections don't disappear. They become reasons to choose a competitor. Buyers evaluating Embark alongside CPA/advisory combo firms (Cherry Bekaert, Baker Tilly, RSM) will notice the non-CPA status. Without proactive reframing, the buyer defaults to "they can't do audits" as a limitation rather than "they can advise without restrictions" as a benefit. Preemptive reframing addresses the concern at the moment of highest intent (contact page), converting what looks like a weakness into a differentiator.

**Target metric:** Form start rate on /contact, secondary: contact_us_form_submit rate
**Audience:** All /contact and service page visitors, particularly those arriving from competitive search terms

**Scores:** Impact 3 | Confidence 4 | Ease 4
Impact 3: Addresses a specific subset of visitors who have this concern, not all visitors. Meaningful for those it affects, but not universal. Confidence 4: The objection is well-documented across competitive analysis and client intake. Strong rebuttal copy exists. Behavioral principle (loss aversion in reverse: show what buyer loses choosing a conflicted advisor) is well-established. Ease 4: Adding a content block to existing pages. Copy is already drafted in the objection cheat sheet. No structural changes required.

**What a win proves:** Proactive objection handling on high-intent pages influences conversion. Validates expanding this approach to other objections ("How do we know we'll get senior people?" and "Aren't you just a staffing agency?").
**What a loss teaches:** Visitors may not carry this objection to the contact page, or the reframe may not be strong enough to overcome it. Would suggest the objection is better handled in sales conversation than web copy, or that the reframe needs customer-attributed proof (a testimonial from someone who initially had the same concern).

---

## Strategic Bets

### 1. Homepage Hero: Differentiation-Led Messaging with Proof

**Page:** /
**What to test:** Replace the generic carousel hero with a static, differentiation-led hero section that leads with Embark's unique positioning and proof, replacing aspirational language with specific claims backed by quantified evidence.

**Current state:** The homepage hero is a three-slide carousel. Slide 1 uses the headline "High-impact consulting for growing companies" with the subhead "At Embark, we help ambitious businesses scale into their next chapter with strategic guidance and hands-on support." Slides 2 and 3 promote downloadable templates (controller transition template, external audit preparation guide). CTAs are "What we do" and "Talk to an advisor." None of Embark's structural differentiators (NPS 93, 9% attrition, 91% client retention, Happy Works, Big 4 Alumni talent) appear above the fold. The carousel dilutes the first impression by rotating between positioning and resource promotions.
**Baseline:** 6,673 sessions/mo, 59.5% bounce (up 13.5pp from prior period), 0% CVR, 1.06 pages/session. Carousel slide_navigation events increased 327% period-over-period, suggesting visitors interact with the carousel but don't convert.
**Test Feasibility:** ~2 weeks at 15% MDE (2 variants, ~1,045 samples/variant) using engagement rate as primary metric. Feasible.
**Proposed change:** Replace the three-slide carousel with a static hero section containing: (1) differentiation-led headline, (2) proof-backed subhead with specific metrics, (3) single prominent primary CTA with specific language, (4) case study proof strip with quantified outcomes from named clients. All elements serve the same hypothesis: differentiation + proof outperforms generic aspiration.

> **Before H1:** "High-impact consulting for growing companies"
> **After H1:** "Big 4 Alumni advisors who stay, execute, and care"
>
> **Before subhead:** "At Embark, we help ambitious businesses scale into their next chapter with strategic guidance and hands-on support."
> **After subhead:** "Financial advisory with an NPS of 93 and 9% attrition, half the Big 4 average. We deploy senior advisors for mid-market and PE-backed companies and stay until the job is done."
>
> **Before CTAs:** "What we do" / "Talk to an advisor" (two equal-weight options)
> **After CTA:** "Talk to an advisor" (single primary) with proof strip below: "96% reconciliation time reduction (Interstate Batteries) | 4-week SEC filing from three-way merger (Atlas Technical) | IPO with three acquisitions integrated (Solo Brands)"

**Why this should work:** B2B buyers decide within 3-5 seconds whether a page is relevant. The current headline ("High-impact consulting for growing companies") is category language that any advisory firm could use. It forces visitors to do cognitive work to figure out what makes Embark different. The proposed version leads with Embark's strongest differentiator (Big 4 Alumni who stay) and immediately backs it with proof no competitor can match (NPS 93, 9% attrition). The carousel currently spreads attention across three slides, two of which promote templates rather than positioning. A static hero eliminates this dilution and focuses the first impression on the message most likely to reduce bounce: "this company is different, and here's the proof." The positioning scorecard identifies Clarity as the top opportunity and Specificity as the top gap. This experiment addresses both simultaneously.

**Target metric:** Engagement rate (inverse of bounce), secondary: /contact page visits from homepage, "Talk to an advisor" CTA click rate
**Audience:** All homepage visitors

**Scores:** Impact 5 | Confidence 4 | Ease 3
Impact 5: Highest-traffic page (6,673/mo), worsening bounce trend (+13.5pp), and addresses both the top gap (specificity) and top opportunity (clarity) from the positioning scorecard. A win here changes the entire site's conversion trajectory. Confidence 4: "Before" copy is exact text from the website. "After" copy adapts directly from the positioning statement and channel adaptations. GA4 data confirms worsening bounce trend. Traffic adequacy is high. Capped at 4 (no evidence module calibration data). Ease 3: Requires carousel removal, layout restructuring for static hero, proof strip creation, and CTA consolidation. More than a copy swap. Moderate development effort.

**What a win proves:** Differentiation-led, proof-backed messaging resonates more than generic aspirational copy. Validates extending this approach to service pages (Experiment #5) and informs the content of personalized hero variants (Experiment #6).
**What a loss teaches:** Visitors may value the aspiration-first framing ("growing companies," "next chapter"), or the proof metrics may not carry meaning for visitors unfamiliar with NPS or attrition benchmarks. Would suggest testing proof-first (case studies above fold) separately from differentiation-first (headline change) to isolate which element failed.

---

### 4. Contact Page: Paid Traffic Message Alignment

**Page:** /contact
**What to test:** Align the contact page experience with paid campaign messaging for Cross-network (Performance Max) visitors, who currently convert at less than one-fifth the rate of Direct visitors.

**Current state:** Cross-network (Google Ads PMax) drives 3,084 sessions per 90 days to /contact, making it the dominant traffic source for this page (82% of landing sessions). These visitors convert at 0.42% (unified CVR), while Direct traffic converts at 2.24%, a 5.3x gap. The contact page presents the same generic experience regardless of traffic source: no message matching to ad creative, no campaign-specific value reinforcement, and full site navigation offering multiple exit paths. The contact_us_form_submit Key Event shows 52 completions on /contact over 90 days.
**Baseline:** 1,480 sessions/mo total, 63.1% bounce, 1.19% unified CVR. Cross-network: ~1,028 sessions/mo, 0.42% CVR.
**Test Feasibility:** ~7 weeks at 15% MDE (2 variants, ~1,214 samples/variant) using engagement rate as primary metric. Extended. Form completion CVR would require >300 weeks. Consider form_start as micro-conversion metric for faster signal.
**Proposed change:** For visitors arriving from Cross-network campaigns (identified by UTM parameters or campaign source), serve a modified contact page variant: (1) headline that echoes the ad campaign's value proposition, (2) form context reinforcement ("What happens next: a 15-minute call with a senior advisor to discuss your situation"), (3) relevant proof point adjacent to the form (e.g., NPS 93 or a short testimonial from a CFO), (4) reduced navigation to minimize exit paths.

> **Before:** Generic /contact page for all visitors. No ad-message continuity. Full site navigation. No form reinforcement.
> **After (paid variant):** Headline matching PMax ad theme + "What you'll get: A 15-minute call with a Big 4 Alumni advisor to discuss your specific situation. No pitch. No obligation." + proof: "NPS of 93. 91% of our clients come back." + streamlined navigation.

**Why this should work:** Paid visitors arrive with a specific expectation set by the ad creative. When the landing page doesn't echo that promise, cognitive dissonance causes immediate exit. The 5.3x conversion gap between Direct and Cross-network on /contact is strong evidence of a message-match failure. Direct visitors already know Embark (they typed the URL). Paid visitors need the page to confirm they're in the right place. Additionally, form context reinforcement ("what happens next") reduces submission anxiety by setting clear expectations. Full navigation on a conversion page gives paid visitors multiple low-intent exit paths that compete with the form.

**Target metric:** Form start rate (micro-conversion), secondary: contact_us_form_submit rate, bounce rate
**Audience:** Cross-network (PMax) visitors landing on /contact

**Scores:** Impact 4 | Confidence 4 | Ease 3
Impact 4: Primary conversion page with a documented 5.3x CVR gap between channels. Closing even 20% of this gap on 1,028 monthly paid sessions would add 3-4 incremental contact form completions per month. Confidence 4: Performance data confirms the channel-specific gap. The mechanism (message match + form reinforcement) is well-established in landing page optimization. GA4 traffic adequacy is high. Ease 3: Requires audience targeting capability in the testing platform (UTM-based), ad creative review for message matching, and page variant with modified headline, reinforcement copy, and navigation changes.

**What a win proves:** The paid-to-page messaging gap is the primary conversion blocker for PMax traffic. Validates building dedicated landing pages for future paid campaigns rather than sending all traffic to the generic /contact page.
**What a loss teaches:** The conversion gap may not be a messaging problem. PMax audience targeting may be too broad (attracting low-intent clicks), or the form itself may be the friction point regardless of surrounding copy. Would suggest auditing PMax audience segments before further page optimization.

---

### 5. Service Page Differentiation with Contextual Conversion Paths

**Page:** /what-we-do/* (13 service sub-pages)
**What to test:** Redesign service sub-pages with differentiation content blocks, relevant case study metrics, and contextual resource CTAs matched to the service area, replacing current generic descriptions with no conversion mechanism.

**Current state:** All 13 service sub-pages under /what-we-do/* collectively receive 1,408 sessions/mo with a group conversion rate of 0%. No conversion mechanism exists on any service page. The copy uses generic language: "Solving complex business challenges with industry-leading expertise and world-class hospitality" (positioning scorecard flags "industry-leading" as a generic superlative that breaks voice rules). The competitive claim overlap score is 0.50, meaning half of Embark's service-level claims could appear on a competitor's page unchanged. Embark has 17 published case studies with 6 quantified outcomes and 5 named clients, none of which are surfaced on service pages.
**Baseline:** 1,408 sessions/mo (group), 31.6% bounce, 0% CVR. Individual page traffic: /what-we-do/financial-advisory-consulting (212/mo), /what-we-do (538/mo), /what-we-do/m-and-a-consulting (~100/mo), others <100/mo each.
**Test Feasibility:** Cannot estimate (no conversion rate baseline). Group-level engagement metrics are feasible. Individual page testing is impractical at current traffic levels.
**Proposed change:** For the top 3-4 service pages by traffic, add: (1) a differentiation content block highlighting what makes Embark's approach unique for this service (e.g., for FARS: "Big 4 Alumni advisors with a 91% client retention rate handling your complex transactions"), (2) a relevant case study proof point (e.g., M&A page: "Atlas Technical: two years of audited financials prepared in 4 weeks for SEC filing from a three-way merger"), (3) a contextual resource CTA matching the service area (e.g., M&A page: "Download: Post-Merger Integration Checklist").

> **Before (financial-advisory-consulting):** "Solving complex business challenges with industry-leading expertise and world-class hospitality." No case studies. No conversion CTA. No differentiation from competitors.
> **After:** "Big 4 Alumni financial advisors with an NPS of 93 and 91% client retention. We reduced Interstate Batteries' bank reconciliation from 12 hours to 30 minutes." + Case study card + "Download: Audit Readiness Checklist" CTA.

**Why this should work:** Service page visitors are in evaluation mode, comparing Embark against 3-5 similar firms. When every vendor's page says "we help you with financial reporting," none stands out. Injecting specific differentiators (quantified culture proof, named case study outcomes) breaks the comparison pattern and creates a mental anchor that persists through the evaluation process. The contextual resource CTA adds a conversion mechanism to a page group that currently captures zero leads from 1,408 monthly sessions. Embark's resource templates already convert at 6.55% on their own pages, and service pages provide stronger buying intent context for the same content.

**Target metric:** Resource CTA click-through rate (new), secondary: engagement rate, /contact page visits from service pages
**Audience:** All service page visitors, with particular relevance to CFO and COO personas evaluating specific capabilities

**Scores:** Impact 4 | Confidence 3 | Ease 3
Impact 4: 1,408 sessions/mo with zero conversion represents Embark's largest structural opportunity. Performance profile sizes this as "large" impact: ~22 additional conversions/month at a conservative 3% capture rate. The current state is complete conversion absence. Confidence 3: Trigger conditions confirmed (generic copy, 0% CVR, case studies available), but "before" copy is described from messaging gap analysis rather than exact page text. Competitive landscape confidence is 2, limiting certainty about differentiation effectiveness. Ease 3: Requires content creation for differentiation blocks and case study cards across multiple pages, plus resource CTA integration. Can be templated, but still requires per-page adaptation.

**What a win proves:** Service page visitors respond to differentiation content and will convert on contextual resource offers. Validates the broader strategy of turning service pages from brochures into conversion-capable assets.
**What a loss teaches:** The conversion gap on service pages may be intent-based (visitors come to learn about capabilities, not to engage yet), or the generic copy may not be the conversion blocker (page structure or CTA placement could be). Would suggest testing CTA placement and offer type independently from content changes.

---

## Explorations

### 6. Segment-Based Hero Personalization

**Page:** /
**What to test:** Serve persona-matched hero messaging (headline, subhead, CTA) to different visitor segments based on traffic source signals, testing whether relevance-driven personalization outperforms a single best message.

**Current state:** All homepage visitors see the same hero regardless of their role, industry, or stage in the buying process. Embark serves four distinct personas (CFO, COO, CIO/CTO, CHRO/CPO) with different primary challenges, but the homepage speaks to none of them specifically. The persona messaging grid has detailed per-persona lead messages that have never been deployed.
**Baseline:** 6,673 sessions/mo, 59.5% bounce, 0% CVR
**Test Feasibility:** Depends on segment identification accuracy and per-segment traffic volume. With 4 segments and ~1,668 sessions/mo each (if evenly distributed), individual segment testing requires larger effect sizes or longer durations. Consider starting with 2 segments (CFO vs. all others).
**Proposed change:** For visitors identifiable by UTM parameters, paid campaign source, or referral path, serve a hero variant matched to their likely persona. CFO-segment visitors see: "Your finance team is stretched. Our Big 4 Alumni advisors close the gap." COO-segment visitors see operations-focused messaging. Unidentifiable visitors see the baseline hero from Experiment #1.

> **Before:** Single hero for all visitors: "High-impact consulting for growing companies" (or whatever wins from Experiment #1)
> **After (CFO segment):** "Your finance team is stretched. Audit season is coming. The PE sponsor wants investor-ready reporting yesterday. We deploy Big 4 Alumni advisors who close your reporting gaps and stay until the job is done."
> **After (COO segment):** "Scaling operations shouldn't mean scaling headcount at the same rate. We work alongside your team to redesign processes, implement systems, and make transformation stick."

**Why this should work:** Relevance is the strongest driver of B2B landing page conversion. A CFO evaluating advisory firms responds to finance-specific language; a COO responds to operations language. The current one-size-fits-all hero forces each persona to mentally translate generic copy to their context. Persona-matched messaging eliminates this translation step, increasing the speed from "page exists" to "page is for me." Four personas with distinct challenges create four distinct messaging opportunities.

**Target metric:** Segment-level engagement rate, secondary: segment-level /contact page visits
**Audience:** Identifiable persona segments via UTM, campaign source, or referral

**Scores:** Impact 4 | Confidence 2 | Ease 1
Impact 4: Personalization at the highest-traffic touchpoint has outsized conversion potential. Matching messaging to persona can shift engagement rates significantly when the default is generic. Confidence 2: Three of four personas (COO, CIO, CHRO) are inferred from website descriptions, not validated by buyer interviews. Segment identification via UTM is reliable for paid traffic but unavailable for Direct (54.5% of sessions) and most Organic. Actual per-segment traffic volume is unknown. Ease 1: Requires personalization infrastructure (dynamic hero content by visitor segment), UTM-based audience targeting, and creation of 4 persona-specific hero variants. Cross-team coordination between marketing, development, and paid media. Note: Confidence is lower because three of four personas are inferred rather than validated. Testing with CFO only (the validated persona) would increase confidence to 3.

**What a win proves:** Persona-specific messaging materially outperforms one-size-fits-all on Embark's homepage. Validates investment in personalization infrastructure for service pages, industry pages, and paid landing pages.
**What a loss teaches:** Either the segment detection is too inaccurate (wrong message to wrong person), the personas don't actually evaluate through the lens we assumed, or the incremental lift from personalization doesn't justify the infrastructure investment. Would suggest persona validation research before further personalization investment.

---

### 7. Persona-Based Navigation Paths

**Page:** Site-wide navigation
**What to test:** Add persona or use-case-based navigation paths ("For CFOs," "For Operations Leaders," "By Challenge") alongside or replacing the current feature-based navigation structure.

**Current state:** Site navigation is organized by capability: What We Do, Who We Serve, Resources, About. Visitors must self-filter through service descriptions to find relevance. With four distinct personas evaluating different capabilities, the feature-only navigation forces each persona to search across multiple pages. The Who We Serve section groups by industry vertical, not by buyer role.
**Proposed change:** Add role-based navigation entries: "For CFOs" (links to audit readiness, financial reporting, Office of the CFO, M&A advisory), "For Operations Leaders" (links to digital transformation, supply chain, data analytics). Each persona landing page leads with the persona-specific messaging from the messaging hierarchy and surfaces relevant case studies and proof points.

> **Before:** Navigation: What We Do | Who We Serve | Resources | About | Happy Works | Contact
> **After:** Navigation: What We Do | For CFOs | For Operations Leaders | Who We Serve | Resources | About | Contact

**Why this should work:** Multi-persona sites with feature-only navigation force every visitor to evaluate every service to find their own. Role-based navigation acts as a shortcut: a CFO clicking "For CFOs" immediately sees content curated for their challenges, reducing the cognitive effort of self-filtering. This pattern is common among competitors in adjacent markets but unused in Embark's competitive set, representing a potential white-space advantage.

**Target metric:** Navigation click-through rate by path, secondary: service page engagement rate by persona, /contact page visits
**Audience:** All site visitors

**Scores:** Impact 4 | Confidence 2 | Ease 1
Impact 4: Site-wide navigation changes affect all visitors and all downstream engagement. If visitors self-sort more efficiently, engagement increases across the entire site. Confidence 2: Four personas identified, but non-CFO personas lack direct evidence. Visitors may not identify with the role labels used in navigation. No data on whether current navigation is actually a friction point (enhanced measurement disabled, so click-path data is limited). Ease 1: Requires CMS navigation restructuring, creation of persona landing pages, content curation per persona, and potentially responsive design changes. Significant development and content effort.

**What a win proves:** Visitors self-select into persona paths when given the option, and this self-selection improves downstream engagement and conversion. Validates a persona-centric site architecture.
**What a loss teaches:** Visitors may not identify with role labels, or the current feature-based navigation may actually serve visitors better than assumed. The navigation change adds complexity (more options), which could increase decision paralysis rather than reduce it.

---

### 8. Finance Function Readiness Assessment

**Page:** New page (linked from homepage, service pages, and paid campaigns)
**What to test:** Build a short self-qualification diagnostic that helps visitors identify their finance function maturity level and receive a personalized recommendation for which Embark service fits their situation.

**Current state:** Embark serves five distinct segments (PE-backed portfolio companies, mid-market in transition, enterprise finance functions, high-growth SaaS/tech, energy and infrastructure) across seven core service lines. Visitors have no self-service mechanism to determine which service fits their situation. All paths lead to the generic /contact form, which asks visitors to commit before understanding what they'll get. The site lacks interactive content that helps visitors self-identify.
**Proposed change:** Build a 5-7 question diagnostic ("Finance Function Readiness Assessment") covering company stage, current challenges, team size, and timeline urgency. Output: personalized recommendation showing which service line fits, a relevant case study, and a suggested next step. Gate the detailed results behind email capture. Example: a PE-backed company with audit readiness concerns gets directed to FARS with the Atlas Technical case study (4-week SEC filing from three-way merger).

**Why this should work:** Visitors facing a classification problem ("which of these seven services do I need?") before an evaluation problem ("is Embark good at it?") experience friction at the wrong stage. A diagnostic solves classification, positions Embark as the expert guide, and captures email at the moment of peak engagement (the visitor has invested effort and wants their answer). The commitment-consistency principle suggests that visitors who complete the assessment are more likely to follow through on the recommended next step. Assessment data also enriches sales understanding of each lead.

**Target metric:** Assessment completion rate, email capture rate on results page, secondary: /contact page visits from assessment results
**Audience:** All visitors, particularly those arriving from non-branded search or paid campaigns who are still in early evaluation

**Scores:** Impact 3 | Confidence 2 | Ease 2
Impact 3: Creates a net-new conversion path and generates enriched leads with self-reported needs data. But as a new page, it depends on successful traffic routing. Without promotion, a new page has zero organic traffic. Confidence 2: No existing self-service qualification mechanism to benchmark against. The pattern is common in SaaS but less proven in professional services consulting. Embark's five segments and seven service lines do create genuine classification complexity, but whether visitors will engage with a diagnostic is uncertain. Ease 2: Requires custom development (assessment flow, branching logic, results engine), content creation (per-recommendation copy, case study matching), and form integration. Likely a multi-sprint project.

**What a win proves:** Visitors will engage with self-service qualification tools in professional services, and the diagnostic-to-lead path can supplement or outperform the direct contact form approach.
**What a loss teaches:** Professional services buyers may prefer human qualification over self-service tools, or the assessment may feel too generic to be useful. Would suggest the classification problem is better solved by persona-based navigation (Experiment #7) than by an interactive tool.

---

## Sequencing Rationale

The roadmap starts with two Quick Wins to build organizational confidence in testing. Experiment #2 (Homepage Secondary Conversion) validates whether resource downloads drive meaningful mid-funnel conversion from homepage traffic. If it wins, it proves content offers work as a conversion mechanism on high-traffic pages, directly justifying the contextual resource CTAs deployed on service pages in Experiment #5. Experiment #3 (Objection Preemption) tests whether proactively addressing the non-CPA objection influences conversion on high-intent pages, teaching Embark how to handle their most structural positioning challenge in web copy.

The Strategic Bets build on Quick Win learnings. Experiment #1 (Homepage Hero Overhaul) is the highest-impact test in the roadmap. It should run after Quick Wins establish testing process and internal buy-in, because a carousel removal and above-fold restructuring requires broader stakeholder alignment than adding a content block. If the hero overhaul wins, it validates differentiation-led messaging as Embark's web strategy, informing every downstream experiment. If it loses, the loss interpretation drives a fundamentally different direction: either the differentiation-led framing is wrong, or the proof metrics don't resonate, both of which reshape subsequent tests. Experiment #4 (Contact Page Paid Alignment) can run in parallel with #1 since it targets different traffic on a different page. Experiment #5 (Service Page Differentiation) should run after the homepage messaging is validated so it can extend the proven approach, rather than guessing which messaging direction to take.

The Explorations are sequenced by dependency. Experiment #6 (Segment Personalization) only makes sense after Experiment #1 proves which baseline messaging works. You need a validated default before you can test whether persona-specific variants outperform it. Experiment #7 (Persona Navigation) is the most structural change in the roadmap and should only proceed if Experiment #5 reveals persona-specific engagement patterns on service pages. Experiment #8 (Assessment Tool) is the longest build and should wait until positioning fundamentals are validated across the site.

Cross-tier dependencies: Experiment #2's result directly informs #5's CTA approach. If content offers on the homepage don't convert, the service page CTA strategy needs a different offer type. Experiment #1's result informs both #5 (messaging direction) and #6 (baseline for personalization). Experiment #3 is independent of other experiments and its learning (does proactive objection handling work in web copy?) applies broadly.

---

## What's Not Here (and Why)

### Patterns Evaluated and Excluded

**Pricing transparency.** Embark's pricing model is inherently variable: project-based, retainer, interim, and fractional engagements with scope-dependent pricing. No public pricing page exists. Competitors in this space also don't publish pricing. For project-based consulting where deal sizes depend on engagement scope, duration, and team composition, publishing price ranges risks either scaring qualified prospects (high anchor) or attracting unqualified ones (low anchor). Not recommended until competitive dynamics change.

**Form field reduction.** The current field count on the /contact form could not be confirmed from available context. If the form has 5+ fields, reducing to name, email, and company is a strong test. Recommendation: audit the /contact form structure, then evaluate. Session recording analysis would provide baseline drop-off data by field.

**Long-form vs. short-form page testing.** Page scroll depth and content length could not be confirmed. Enhanced measurement (scroll events) is currently disabled, so the baseline data needed to evaluate this pattern does not exist.

**Value-before-commitment sequencing.** Embark sells consulting services, which are inherently difficult to "preview" before commitment. Unlike SaaS products with interactive demos, consulting value is demonstrated through credentials and case studies. The assessment tool (Experiment #8) is the closest applicable variant of this pattern.

**Comparison-mode intervention.** GA4 data shows pages/session averaging 1.06-1.37, indicating most visitors view 1-2 pages per session. No significant deep-browsing segment exists that would benefit from session-depth-triggered offers.

### Patterns Skipped Due to Missing Data

**CTA click-through optimization and element engagement drop-off.** No element-level interaction data is available. Enhanced measurement (click events) has been disabled. Re-enabling would unlock CTA click-through analysis and carousel engagement decay data, enabling two additional experiment patterns.

**Form optimization (field reduction and multi-step).** Form field count, structure, and per-field abandonment data are unknown. A site audit or session recording analysis would provide the baseline needed to evaluate these patterns.

### Infeasible at Current Traffic

**Happy Works page: Is the existing form converting, and can it convert better?** The /happy-works page (117 sessions/mo, 25.3% bounce, 107s avg engagement) is one of the most engaging pages on the site. It houses Embark's strongest differentiator (Happy Works philosophy with NPS 93, 9% attrition, revenue growth trajectory) and has a form at the bottom of the page. The performance profile does not include conversion data for this page, so it is unknown whether the form generates any submissions. The testable question is whether culture-page visitors who are deeply engaged (107s avg, low bounce) can be converted through form optimization, contextual proof placement, or a different offer framing. At 117 sessions/mo, A/B testing is impractical. Suggested approach: first, instrument the form to confirm whether it fires form_submit or a dedicated event, and measure current conversion rate. If the form is converting, optimize via pre/post. If it is not, test a different offer framing (e.g., "See how Happy Works translates to client outcomes" with a case study CTA instead of or alongside the form) via pre/post analysis over 60-90 days.

**Office pages: Does local presence drive conversion intent?** /offices (617 sessions/mo, 29.4% bounce) is a consideration-stage page for buyers evaluating whether Embark has local coverage. No conversion mechanism exists. At 617 sessions/mo with no current CVR, an A/B test on conversion rate would be infeasible at primary metric level. Suggested approach: add a "Find your local advisor" or "Contact your nearest office" CTA and measure pre/post.

### Just-Do-It Fixes (Not Experiments)

These items should be implemented directly. They are not hypotheses requiring A/B testing because the correct action is clear:

- **Update NPS from 87 to 93 on the main site.** HubSpot landing pages already show the confirmed figure. The main site displays a stale number.
- **Re-enable enhanced measurement in GA4.** Scroll, click, and file_download events dropped to zero in the current period. This data is essential for engagement analysis across all experiments.
- **Add a download CTA to /13-week-cash-flow-forecast-model-template-best-practices.** This blog post (586 sessions/mo, 52.7% bounce) discusses a template that has a dedicated download page converting at 12.66%. Visitors likely can't find the actual download. Add a prominent link.
- **Update "Strategic Business Consulting" H1 on /what-we-do.** This framing doesn't match buyer vocabulary. "Financial Advisory and Consulting" aligns with how buyers search and how Parthenon Capital describes Embark.
- **Investigate Direct traffic quality.** Direct traffic (54.5% of all sessions) has an 85.2% bounce rate, up from 69.5% prior period. This is anomalous for legitimate Direct traffic. Check for: bot traffic, HubSpot/internal referral leakage, mobile app WebView traffic, or misconfigured CMS preview traffic. Fixing this may significantly change site-wide metrics.

---

## Prerequisites and Data Gaps

### Missing Baseline Data

- **Enhanced measurement disabled.** Scroll, click, and file_download events report zero in the current period despite significant volume in the prior period (36,708 scroll, 5,207 click, 645 file_download). Affects: all experiments (engagement depth metrics unavailable), plus blocks CTA click-through optimization and element engagement patterns entirely. Action: re-enable enhanced measurement in GA4 property settings.
- **Form field count and structure unknown.** The /contact form's field count, field types, and per-field abandonment rates are not documented in any context file. Affects: form optimization patterns (would enable Experiments targeting form friction if 5+ fields confirmed). Action: audit /contact form fields, implement form_start/form_submit step tracking with per-field instrumentation.
- **Element-level interaction data not available.** No per-element click tracking exists for CTAs, proof sections, or navigation elements. Affects: CTA click-through optimization and element engagement drop-off patterns. Action: implement element-level event tracking for primary CTAs, carousel slide interactions, and proof section visibility.
- **Per-page scroll depth not measured.** Scroll depth data is unavailable due to enhanced measurement being disabled. Affects: long-form vs. short-form page testing and content engagement assessment. Action: re-enable scroll event tracking.

### Context Verification Needed

- **NPS discrepancy.** Main site shows 87, HubSpot landing pages show 93, client confirmed 93. Affects: all proof-dependent experiments using NPS as a credibility signal. Action: update main site to confirmed 93 (listed as just-do-it above).
- **Non-CFO personas are inferred.** COO, CIO/CTO, and CHRO persona definitions are based on website service descriptions and job norms, not buyer interviews or sales data. Affects: Experiments #6 (Segment Personalization) and #7 (Persona Navigation), where persona accuracy directly determines messaging relevance. Action: interview 2-3 buyers in non-CFO roles to validate or revise persona definitions.
- **"Right-sized flexibility" value theme has weak proof.** Only Level 2 testimonial evidence supports this theme. Multiple competitors offer similar engagement flexibility. Affects: any experiment using flexibility as a differentiating claim. Action: collect engagement model data (average project duration, contract structure statistics, cost comparisons to Big 4 alternatives).
- **Competitive landscape confidence is 2.** Limited by single-page extractions for several competitors (Accordion, CFGI, Opportune, Forvis Mazars) and no pricing data across competitors. Affects: Experiment #5 (Service Page Differentiation), where differentiation effectiveness depends on competitive accuracy. Action: deeper competitive research on Riveron, Accordion, and CFGI service positioning and pricing signals.

### Infrastructure Prerequisites

- **Audience targeting in testing platform.** Required for Experiment #4 (paid traffic variant on /contact) and Experiment #6 (segment-based hero personalization). Experiments need the ability to serve different page variants based on UTM parameters, campaign source, or referral path. Action: verify whether the current testing platform supports UTM-based or source-based audience targeting.
- **Personalization infrastructure.** Required for Experiment #6 (dynamic hero content by visitor segment). Experiment needs the CMS or testing platform to support conditional content blocks. Action: evaluate whether existing CMS or FunnelEnvy's testing infrastructure can deliver dynamic hero content by visitor segment without custom development.
- **CMS navigation flexibility.** Required for Experiment #7 (persona navigation paths). The navigation restructuring requires the CMS to support adding role-based entries without major template changes. Action: assess CMS navigation capabilities and estimate development effort for adding persona-based navigation.

---
*Analysis produced by FunnelEnvy | 2026-03-08*
*Based on positioning analysis across 5 context sources and GA4 behavioral data (65,850 sessions, 90 days)*
