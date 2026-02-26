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
| 1 | Homepage Hero: Static Positioning with Optimized Content Offer | / | Quick Win | 5 | 4 | 5 | 14 |
| 2 | Homepage Proof Strip: Case Study Metrics Above Fold | / | Quick Win | 4 | 4 | 4 | 12 |
| 3 | Contact Page: PMax Retargeting Form Completion + Mobile Optimization | /contact | Quick Win | 4 | 4 | 3 | 11 |
| 4 | Service Pages: Contextual Resource CTAs | /what-we-do/* | Strategic Bet | 5 | 4 | 4 | 13 |
| 5 | Homepage CTA: Specific Action Language | / | Quick Win | 4 | 4 | 5 | 13 |
| 6 | Service Page Differentiation Injection | /what-we-do/financial-advisory-consulting | Strategic Bet | 4 | 3 | 4 | 11 |
| 7 | Objection Preemption: "Not a CPA Firm" Reframe | /contact, /what-we-do | Strategic Bet | 4 | 4 | 3 | 11 |
| 8 | Happy Works Page: Conversion Path Addition | /happy-works | Exploration | 2 | 3 | 4 | 9 |
| 9 | Persona-Based Navigation Paths | Site-wide navigation | Exploration | 4 | 3 | 2 | 9 |
| 10 | Segment-Based Hero Personalization | / | Exploration | 5 | 2 | 2 | 9 |

---

## Quick Wins

### 1. Homepage Hero: Static Positioning with Optimized Content Offer

**Page:** Homepage (/)
**What to test:** Replace the 3-slide hero carousel with a static hero that combines differentiated positioning copy with a single high-converting content offer.

**Current state:** The homepage H1 reads "High-impact consulting for growing companies." This is a line any advisory firm could use. The subhead ("At Embark, we help ambitious businesses scale into their next chapter with strategic guidance and hands-on support") reinforces generic positioning. The homepage carousel rotates between this positioning slide and two resource promotions (an accounting template and an audit preparation guide), which further dilutes the first impression.

**Carousel engagement data (90-day GA4 pull, 2025-11-28 to 2026-02-25):**

The homepage received 21,596 page views from 15,646 users over this period. Carousel interaction is near-zero:

| Metric | Events | Unique Users | Rate (of 15,646 users) |
|---|---|---|---|
| Slide navigation (arrow/dot clicks) | 256 | 92 | 0.6% |
| Hero CTA clicks (all slides combined) | 129 | ~111 | 0.7% |

Slide navigation by index:
- Slide 0 (main positioning): 115 events / 74 users
- Slide 1 (template download): 73 events / 45 users
- Slide 2 (guide download): 68 events / 46 users

Hero CTA clicks by label:
- "What we do" (Slide 1): 78 clicks / 73 users
- "Download the template" (Slide 2): 30 clicks / 18 users
- "Talk to an advisor" (Slide 1): 12 clicks / 11 users
- "Download the guide" (Slide 3): 9 clicks / 9 users

For comparison, the header "Contact Us" button received 78 clicks and nav menu links received 857 total clicks from the same page. Visitors are bypassing the hero entirely and using the navigation.

**The carousel is promoting the wrong content.** The two resources featured in Slides 2-3 are among the lowest-converting content on the site:

| Resource | Sessions | Form Submits | CVR | Hero Placement |
|---|---|---|---|---|
| Post-Merger Integration Checklist | 1,266 | 84 | 6.6% | Not in carousel |
| 13-Week Cash Flow Forecast | 401 | 51 | 12.7% | Not in carousel |
| Quality of Earnings Template | 227 | 27 | 11.9% | Not in carousel |
| ASC 606 Revenue Recognition Template | 760 | 32 | 4.2% | Not in carousel |
| Controller Transition Template (Slide 2) | 126 | 8 | 6.3% | **In carousel** |
| External Audit Prep Guide (Slide 3) | 140 | 5 | 3.6% | **In carousel** |

The two carousel resources generated 13 combined form submits in 90 days. The top 3 resources (none of which are in the hero) generated 162 form submits. A previous test of a butterbar (top banner) to replace carousel content promotion showed the carousel converting better, but the carousel's absolute performance is still very low: 39 content download clicks from the hero in 90 days.

**Important context:** Content downloads drive a majority of Embark's leads historically. The issue is not whether content should be promoted prominently, but that the current carousel (a) promotes the wrong resources and (b) uses a format with a 0.6% interaction rate that hides slides 2-3 from 99.4% of visitors.

**Baseline:** ~6,700 sessions/month, 59.5% bounce rate, 0% conversion rate. Direct traffic (11,438 sessions) bounces at 74.5% vs Organic Search at 37.5%.

**Proposed variants (test one):**

**Option A -- Static hero with single best content offer:**
Replace the carousel with a static hero combining the positioning headline with a single CTA for the Post-Merger Integration Checklist (the highest-volume converter at 84 submits/90 days, 6.6% CVR).

> **Before:** 3-slide carousel cycling generic positioning + two low-performing resource offers
> **After:** Static hero with "Big 4 Alumni advisors who stay, execute, and care. NPS 93." headline + primary CTA "Download the Post-Merger Integration Checklist" + secondary CTA "Book a 15-Minute Intro Call"

Rationale: Concentrates hero real estate on one proven resource instead of splitting across three slides that nobody navigates. The PMI Checklist already pulls 1,266 organic sessions on its own page, proving market demand.

**Option B -- Static positioning hero + rotating content offer CTA:**
Keep the hero headline and subhead static (no full-slide rotation), but rotate just the content offer CTA below the positioning copy. Test the top 3 resources in rotation: PMI Checklist vs. Cash Flow Forecast vs. Quality of Earnings Template.

> **Before:** Full carousel rotating entire hero sections
> **After:** Fixed positioning copy with a single rotating content CTA strip beneath it

Rationale: Preserves the content lead gen mechanism Embark values while eliminating the positioning dilution of the full carousel. Tests which resource resonates best from the hero position.

**Option C -- Static hero with content promotion moved below the fold:**
Static hero with positioning copy only. Move content promotion to a dedicated module immediately below the hero fold (featured resource card or sticky banner). This separates the jobs of "communicate who Embark is" (hero) from "capture leads via content" (below-fold module).

> **Before:** Hero tries to do both positioning and lead gen, does neither well
> **After:** Hero owns positioning. Below-fold module owns content lead gen with the top-performing resource.

Rationale: The hero's primary job should be reducing the 59.5% bounce rate by communicating relevance in 3-5 seconds. Content promotion can happen immediately below the fold where engaged visitors (the 40.5% who don't bounce) are more likely to act. This is the cleanest separation of concerns but the most different from current state, which may face internal resistance.

**Recommended variant:** Option A. It's the smallest change from current behavior (hero still has a content download CTA), addresses the client's concern about content-driven leads, swaps in a resource that actually converts, and adds the differentiated positioning copy. Options B and C are viable follow-ups depending on results.

**Why this should work:** B2B buyers scanning above the fold decide in 3-5 seconds whether a page is relevant. "High-impact consulting" forces the visitor to do cognitive work: what kind of consulting? For whom? The proposed headline self-qualifies financial advisory buyers immediately and communicates something no competitor can claim (NPS 93). Replacing the carousel with a static hero eliminates a format that 99.4% of visitors ignore. Swapping in the PMI Checklist (84 submits) for the Controller Transition Template (8 submits) and External Audit Prep Guide (5 submits) puts a proven lead magnet in the hero position.

**Target metric:** Bounce rate (primary), hero CTA click-through rate and form_submit volume (secondary), content download volume (guardrail -- must not decrease site-wide content leads)
**Audience:** All visitors, with particular importance for Direct traffic where the 74.5% bounce rate indicates first-impression failure

**Scores:** Impact 5 | Confidence 4 | Ease 5
Impact 5 because this is the highest-traffic page on the site (20K sessions/90 days) and the scorecard identifies Clarity as the top opportunity. Homepage bounce worsened 13.5pp vs the prior period. Confidence 4 because the carousel engagement data directly validates the problem (0.6% nav rate, wrong resources promoted), the before state is exact copy from the website, the replacement resource has proven conversion data, and traffic adequacy is high. Ease 5 because this is a text change and resource swap in the CMS hero module.

**What a win proves:** Validates two things simultaneously: (1) that differentiated positioning copy outperforms generic category language in the hero, and (2) that a static hero with one high-converting resource outperforms a carousel promoting low-converting resources. This informs all downstream page design: lead with proof, promote proven content, stop hiding offers behind carousels.
**What a loss teaches:** If bounce rate doesn't improve but content downloads hold steady, the positioning copy needs work but the static format is fine. If content downloads drop, hero placement genuinely matters for content lead gen and the below-fold approach (Option C) should be tested next. If both metrics decline, the carousel format itself may have value that the engagement data doesn't capture (e.g., auto-rotation exposing offers to passive viewers), and the issue is purely about which resources are promoted -- swap the carousel content to top performers without changing the format.

---

### 2. Homepage Proof Strip: Case Study Metrics Above Fold

**Page:** Homepage (/)
**What to test:** Add a scannable evidence strip below the hero headline featuring quantified outcomes from published case studies.

**Current state:** The homepage contains no quantified client outcomes. Embark has 17 published case studies, 6 with specific metrics: Interstate Batteries saw 96% time reduction in bank reconciliation, Atlas Technical Consultants prepared two years of audited financials in 4 weeks for SEC filing, Solo Brands completed a successful IPO with three acquisitions integrated. None of these numbers appear in the first scroll of the homepage or any high-traffic page.

**Baseline:** ~6,700 sessions/month, 59.5% bounce rate. The scorecard identifies Specificity as the top gap: proof metrics exist but are absent from positioning copy.

**Proposed change:** Add a proof strip between the hero section and the services overview. Format: 3-4 quantified outcomes in a scannable horizontal layout.

Example strip:
- "96% reduction in bank reconciliation time" (Interstate Batteries)
- "2 years of SEC-ready financials in 4 weeks" (Atlas Technical Consultants)
- "IPO completed with 3 acquisitions integrated" (Solo Brands)
- "NPS 93 | 9% attrition | 91% retention"

**Why this should work:** The Specificity gap means visitors see claims without evidence. The homepage says "high-impact" but never defines what that impact looks like. Specific metrics activate a different trust evaluation than vague claims: the precision implies confidence in the work, and named clients make the outcomes verifiable. B2B buyers in comparison mode (looking at 3-5 advisory firms) anchor on the first concrete number they see. Embark's competitors do not publish equivalent outcome metrics, making this a differentiating signal.

**Target metric:** Bounce rate (primary), /contact page visits and resource downloads (secondary)
**Audience:** All visitors, especially mid-funnel evaluators comparing advisory firms

**Scores:** Impact 4 | Confidence 4 | Ease 4
Impact 4 because this directly addresses the top positioning gap (Specificity) on the highest-traffic page, but as an additive content element (not replacing the primary hero), its conversion effect is indirect. Confidence 4 because the proof points are verified with named clients, the before state is confirmed (no metrics on homepage), and traffic adequacy is high. Ease 4 because this requires adding a new content block, not just editing text, but the content already exists.

**What a win proves:** Confirms that surfacing existing proof in positioning copy closes the specificity gap and changes visitor behavior. This validates the approach of promoting case study metrics to all high-traffic pages (service pages, about page, landing pages).
**What a loss teaches:** Indicates that above-fold proof strips feel like marketing claims rather than evidence in this industry. Visitors may need the full case study narrative context (challenge, approach, result) rather than stripped-down metrics. Test case study summaries or linked proof instead of standalone numbers.

---

### 3. Contact Page: PMax Retargeting Form Completion + Mobile Optimization

**Page:** /contact
**What to test:** Improve form completion rate for retargeted Cross-network visitors, with emphasis on mobile form UX.

**Current state (90-day GA4 pull, 2025-11-28 to 2026-02-25):**

The /contact page received 3,684 sessions over the period. Cross-network traffic dominates at 81% of all sessions, and virtually all of it (3,034 of 2,986 Cross-network sessions) comes from a single campaign: **"Performance Max - Handraisers - Retargeting."** These are not cold prospects -- they are previous site visitors being retargeted back to /contact.

Traffic and conversion by channel:

| Channel | Sessions | Bounce Rate | Form Starts | Form Submits | Start Rate | Completion Rate |
|---|---|---|---|---|---|---|
| **Cross-network** | 2,986 | 72.0% | 149 | 18 | 5.0% | **12.1%** |
| **Direct** | 418 | 87.8% | 33 | 17 | 7.9% | **51.5%** |
| **Organic Search** | 191 | 52.9% | 15 | 7 | 7.9% | **46.7%** |
| Referral | 47 | 53.2% | 8 | 3 | 17.0% | 37.5% |
| Paid Search | 3 | 66.7% | 4 | 3 | -- | -- |
| **Total** | ~3,684 | -- | 214 | 49 | 5.8% | **22.9%** |

The critical finding: **form completion rate, not form start rate, is where Cross-network traffic falls apart.** Cross-network visitors start forms at a reasonable 5.0% rate (149 starts from 2,986 sessions), but only 12.1% of those starters finish (18 submits). Direct visitors complete at 51.5% (17 of 33 starters). That's a **4.3x form completion gap**, which is a stronger and more actionable signal than the overall CVR gap.

Device breakdown for Cross-network /contact traffic:

| Device | Sessions | % of Cross-network | Bounce Rate |
|---|---|---|---|
| Mobile | 2,123 | 71% | 70.8% |
| Desktop | 559 | 19% | 66.5% |
| Tablet | 393 | 13% | 66.2% |

The PMax retargeting campaign sends 71% mobile traffic. Mobile Direct visitors to /contact bounce at 93.2%. The form likely has a mobile UX problem independent of messaging.

**Reframing the hypothesis:** The original hypothesis assumed an ad-to-page messaging mismatch: cold paid visitors hitting a generic contact page. The data tells a different story. These are retargeted visitors who already know Embark. They've been to the site before, got served a PMax ad, clicked back to /contact, and 72% still bounced. Of the 5% who started the form, nearly 88% abandoned it. The problem is less "did I click the right link?" and more "why should I finish this form right now, on my phone?"

**Baseline:** ~1,230 sessions/month, 72.0% bounce for Cross-network, 0.60% Cross-network CVR. 49 total form submits in 90 days across all channels. Form completion rate for Cross-network: 12.1% vs. Direct at 51.5%.

**Proposed variants (test one, prioritized by data signal strength):**

**Option A -- Mobile form optimization (recommended):**
Reduce form friction specifically for mobile visitors, who represent 71% of Cross-network traffic. This could include: reducing field count, enabling autofill-friendly field types, breaking the form into a multi-step flow (name/email first, details second), or adding a "Call Us" alternative for mobile visitors who won't type on a phone.

> **Before:** Same form experience on mobile and desktop
> **After:** Mobile-optimized form with fewer fields, larger tap targets, and/or a click-to-call alternative

Rationale: The 4.3x form completion gap is the strongest signal. Mobile visitors start the form but can't or won't finish it. Fixing the form for 2,123 mobile sessions/quarter has a larger potential impact than messaging changes. If the current form has 5+ fields, reducing to 3 (name, email, company) on mobile could meaningfully close the completion gap. **Prerequisite: audit the /contact form field count and structure.**

**Option B -- Retargeting-specific messaging + value reinforcement:**
Since these are returning visitors, the page copy should acknowledge their familiarity rather than introduce Embark from scratch. Add a contextual proof point near the form and a headline that reinforces why they should take the next step now.

> **Before:** Generic "Contact Us" with no value reinforcement
> **After:** "Ready to close the gap in your finance function? Talk to an advisor who's done it for companies like yours." + proof point: "91% of clients stay with Embark year over year."

Rationale: Even though messaging mismatch is less likely for retargeted visitors, the /contact page is still generic. Adding a reason to convert now (social proof, reduced commitment language) could improve both form start rate and completion rate. This is additive to Option A.

**Option C -- Combined: mobile form optimization + messaging reinforcement:**
Run Options A and B together as a single variant. Reduce form friction on mobile AND add retargeting-aware messaging/proof. This maximizes the chance of a measurable result but makes it harder to isolate which change drove the improvement.

Rationale: With only 18 Cross-network form submits in 90 days, the base conversion volume is low. Running a subtle single-variable test may not reach significance in a reasonable timeframe. Combining changes increases the effect size at the cost of attribution clarity. Given the low base, this is the pragmatic choice if the team can only run one test.

**Recommended variant:** Option A if form audit reveals 5+ fields or mobile UX issues. Option C if the form is already short and the team wants to maximize signal. Option B alone is the weakest bet because the primary bottleneck is form completion, not form starts.

**Why this should work:** The data shows that the funnel breaks at form completion, not at page engagement or form initiation. Cross-network visitors start forms at 5.0% (comparable to other channels) but complete at 12.1% (vs. 51.5% for Direct). The 71% mobile skew of the PMax campaign means most form interactions happen on a phone, where form friction is highest. Reducing mobile form friction directly addresses the widest gap in the conversion funnel. The retargeting context also means these visitors have already expressed interest -- they are warm leads losing motivation at the last step.

**Target metric:** Form completion rate for Cross-network mobile traffic (primary), overall /contact form_submit volume (secondary), form start rate (guardrail -- should not decrease)
**Audience:** Cross-network retargeted visitors, particularly mobile (71% of PMax traffic)

**Scores:** Impact 4 | Confidence 4 | Ease 3
Impact 4 because the opportunity sizing is clear: 149 form starts with only 18 completions means 131 abandoned forms in 90 days. Even closing half that gap adds ~7 conversions/month from a retargeted (warm) audience. Confidence 4 because the form completion gap (12.1% vs 51.5%) is large and the mobile skew provides a clear causal hypothesis. The single-campaign concentration (PMax Retargeting = 99% of Cross-network) means changes will be testable against a consistent traffic source. Ease 3 (reduced from 4) because mobile form optimization may require development work beyond simple copy changes, and the form audit is a prerequisite.

**What a win proves:** Validates that the /contact conversion bottleneck is form UX (especially mobile), not messaging or traffic quality. This informs all form-based conversion points across the site and justifies mobile-first form design for any future landing pages receiving PMax traffic.
**What a loss teaches:** If form completion doesn't improve despite mobile optimization, the problem is upstream of the form: either the PMax retargeting audience is low-quality (clicking ads without real intent) or visitors are landing on /contact but deciding Embark isn't the right fit during form interaction. Next step would be auditing the PMax campaign audience signals, placement quality, and whether /contact is the right landing page for retargeting (vs. a resource download page with lower commitment).

---

### 5. Homepage CTA: Specific Action Language

**Page:** Homepage (/)
**What to test:** Replace vague CTA language with specific, expectation-setting action language.

**Current state:** The homepage has two CTAs: "What we do" (navigational, sends visitors to services overview) and "Talk to an advisor" (conversion intent). GA4 data (90-day pull) shows hero CTA clicks: "What we do" at 78 clicks (73 users), "Talk to an advisor" at 12 clicks (11 users). Neither CTA communicates what happens next or reduces the fear of unknown commitment.

**Baseline:** ~6,700 sessions/month. Hero CTA combined click rate: 0.7% of homepage users (129 clicks / 15,646 users). "Talk to an advisor" specifically: 12 clicks in 90 days (0.08% click rate). 0% homepage conversion rate.

**Proposed change:** Replace both CTAs with a clear primary/secondary hierarchy.

> **Before:** "What we do" | "Talk to an advisor"
> **After:** Primary: "Book a 15-Minute Intro Call" | Secondary: "See How We've Helped Companies Like Yours" (links to case studies)

**Why this should work:** Hick's Law: two CTAs of equal visual weight create decision paralysis, and visitors default to the easier action (leaving). "Talk to an advisor" triggers commitment fear: How long will this take? Will I get a sales pitch? "Book a 15-Minute Intro Call" sets a time expectation and reduces perceived commitment. The secondary CTA provides an off-ramp for visitors who aren't ready for direct contact, capturing mid-funnel interest instead of losing it entirely.

**Target metric:** CTA click-through rate (primary), /contact page visits and form submissions (secondary)
**Audience:** All homepage visitors

**Scores:** Impact 4 | Confidence 4 | Ease 5
Impact 4 because the current CTA click rate is nearly zero, so there is a large improvement gap, and the homepage is the highest-traffic page. Confidence 4 because the before state is exact copy, the causal mechanism (commitment reduction via time-boxing) is well-established in CRO, and traffic adequacy is high. Ease 5 because this is a text change in the CMS.

**What a win proves:** Confirms that Embark's visitors are deterred by open-ended commitment language. This informs all CTAs site-wide: specificity and time-boxing reduce friction.
**What a loss teaches:** Indicates that Embark's audience prefers the advisory framing ("Talk to an advisor") over transactional scheduling language. This would suggest the audience values the relationship signal of "advisor" over the efficiency signal of "15-minute call." Test hybrid language: "Talk to an Advisor, 15 Minutes, No Commitment."

---

## Strategic Bets

### 4. Service Pages: Contextual Resource CTAs

**Page:** /what-we-do/* and /who-we-serve/* (30 pages total)
**What to test:** Add contextual resource download CTAs to service and industry pages, which currently have zero conversion mechanism.

**Current state (90-day GA4 pull, 2025-11-28 to 2026-02-25):**

Service and industry pages received 4,441 sessions across 30 pages. The engagement data confirms these pages are visited and read, but have no conversion path:

Top service pages by traffic:

| Page | Sessions | Bounce Rate | Avg Session Duration | CTA Clicks | Form Events |
|---|---|---|---|---|---|
| /what-we-do/financial-advisory-consulting | 642 | 36.6% | 88s | 7 | 0 |
| /what-we-do/digital-transformation-consulting | 349 | 30.1% | 63s | 1 | 0 |
| /what-we-do/cfo-consulting | 337 | 21.7% | 72s | 1 | 0 |
| /what-we-do/m-and-a-consulting | 280 | 40.0% | 72s | 2 | 0 |
| /who-we-serve/cfo | 205 | 30.2% | 58s | 1 | 0 |
| /what-we-do/team-continuity | 195 | 39.0% | 69s | 1 | 0 |
| /who-we-serve/energy-utilities | 193 | 33.2% | 67s | 0 | 0 |
| /what-we-do/deal-advisory | 179 | 28.5% | 85s | 0 | 0 |
| /what-we-do/outsourcing-services | 165 | 29.7% | 87s | 0 | 0 |
| /who-we-serve/healthcare-life-sciences | 151 | 37.7% | 84s | 0 | 0 |

Across all 30 service/industry pages: **14 total CTA clicks** and **3 form starts** in 90 days. The only CTA clicks tracked are "Contact Us" in the header (14 clicks). There are zero on-page conversion mechanisms.

Traffic sources to service/industry pages:

| Channel | Sessions | Bounce Rate |
|---|---|---|
| Direct | 1,812 | 67.8% |
| Organic Search | 1,449 | 29.4% |
| Cross-network | 603 | 32.3% |
| Referral | 208 | 33.7% |
| Organic Social | 177 | 29.9% |
| Paid Search | 74 | 39.2% |

Organic Search (1,449 sessions, 29.4% bounce) is the highest-quality channel to these pages. These visitors found Embark through search queries related to specific services, meaning they have active intent. Cross-network (603 sessions, 32.3% bounce) is the PMax retargeting audience arriving on service pages instead of /contact, also showing reasonable engagement. Direct traffic bounces at 67.8%, consistent with the site-wide Direct traffic quality issue.

What visitors do instead of converting: nav menu interaction dominates. 707 nav_dropdown_open events and 334 nav_link_click events across these pages. Top nav destinations from service pages:

| Destination | Clicks |
|---|---|
| /team | 53 |
| /partners | 21 |
| /careers/overview | 16 |
| /what-we-do/financial-advisory-consulting | 14 |
| /what-we-do/cfo-consulting | 13 |
| /happy-works | 12 |

Visitors are exploring (team page, other services, culture page) rather than converting. They navigate laterally across the site because there's no on-page next step that matches their evaluation intent. The /team and /happy-works clicks are notable: visitors on service pages are looking for "who will actually do the work?" and "what's this company's culture like?" -- both are trust/evaluation signals, not conversion signals.

**Baseline:** ~1,480 combined monthly sessions (excluding Direct noise), 30.5% bounce rate for non-Direct channels, 0% CVR. Zero on-page conversion mechanisms exist. 3 form starts in 90 days across all 30 pages.

**Proposed change:** Add contextual resource download CTAs to service pages, matched to the page's topic. Start with a pilot of the top 5 pages by traffic (2,089 sessions combined = 47% of all service page traffic):

| Pilot Page | Sessions | Matched Resource | Resource CVR |
|---|---|---|---|
| /what-we-do/financial-advisory-consulting | 642 | ASC 606 Revenue Recognition Template | 4.2% |
| /what-we-do/digital-transformation-consulting | 349 | Data Culture Guide | 14.9% |
| /what-we-do/cfo-consulting | 337 | 13-Week Cash Flow Forecast Model | 12.7% |
| /what-we-do/m-and-a-consulting | 280 | Post-Merger Integration Checklist | 6.6% |
| /who-we-serve/cfo | 205 | Quality of Earnings Template | 11.9% |

Each resource already exists, already converts, and is topically relevant to the service page. The CTA block should include: resource title, 1-sentence value prop, and a gated download form (name + email minimum).

For industry pages (phase 2), link to the most relevant case study by industry instead of a resource template. Industry page visitors are more likely responding to "show me you've done this in my vertical" than "give me a generic template."

**Why this should work:** Visitors on service pages are evaluating whether Embark can solve their specific problem. They are mid-funnel: interested enough to explore services, but not ready to talk to sales (otherwise they'd be on /contact). The behavioral data confirms this -- 334 nav clicks show lateral exploration, not conversion intent. The only current next step is the header "Contact Us" button (14 clicks in 90 days = 0.3% click rate). A contextual resource download matches the visitor's current intent (learning and evaluation) rather than forcing a premature conversion action. The resource CTAs also create an email capture point that doesn't exist today, feeding the nurture pipeline.

The pilot approach (5 pages, 47% of traffic) reduces implementation effort while covering the highest-impact pages. If the pilot converts at even 2%, that's ~14 additional leads/month from pages currently generating zero.

**Target metric:** Resource download rate per service page (primary), overall form_submit volume (secondary)
**Audience:** Mid-funnel evaluators exploring specific service capabilities, particularly Organic Search visitors (1,449 sessions, 29.4% bounce)

**Scores:** Impact 5 | Confidence 4 | Ease 4
Impact 5 because this is the largest sized opportunity in the analytics: 30 pages with zero conversion mechanism receiving 4,441 sessions/quarter. Even a modest 2% capture rate on the 5-page pilot adds ~14 leads/month. Confidence 4 because the resources already exist and convert well on their own pages (4.2-14.9% CVR), the structural gap is confirmed (14 CTA clicks and 3 form starts in 90 days), and the behavioral data shows visitors are engaged but have no on-page conversion path. Ease 4 (raised from 3) because the pilot scope reduces from 20 pages to 5, all resources already exist, and the CTA block is a repeatable CMS module.

**What a win proves:** Validates the hypothesis that service page visitors will convert on contextual resource offers. This changes the site's conversion architecture: every content page becomes a lead capture point, not just /contact and /resources. A successful pilot justifies expanding to all 30 pages and building the resource-to-service page mapping for the full site.
**What a loss teaches:** Suggests service page visitors are either too early in their journey (awareness, not consideration) or are evaluating competitively and don't want to exchange information yet. The nav click data pointing to /team and /happy-works suggests trust-building may be more important than content at this stage. The next test would be ungated content (case study summaries, team bios relevant to the service area) that builds trust without requiring email capture.

---

### 6. Service Page Differentiation Injection

**Page:** /what-we-do/financial-advisory-consulting (pilot), then expand to other service pages
**What to test:** Add differentiation-specific content blocks to the highest-traffic service page, replacing generic capability descriptions with Embark-specific proof and competitive positioning.

**Current state:** The Financial Advisory and Consulting page receives 642 sessions/90 days with 36.6% bounce, 88s average session duration, and 7 CTA clicks (all header "Contact Us"). The scorecard analysis flags service sub-pages as drifting to generic copy: "Solving complex business challenges with industry-leading expertise and world-class hospitality." "Industry-leading" is a generic superlative that breaks Embark's own voice rules. The competitive analysis shows 0.50 claim overlap on core services. Service pages read like they could belong to any of the 11 analyzed competitors.

**Baseline:** ~210 sessions/month, 37.0% bounce rate, 0% CVR.

**Proposed change:** Replace generic capability descriptions with differentiated content that a competitor cannot replicate.

> **Before:** "Solving complex business challenges with industry-leading expertise and world-class hospitality"
> **After:** "Big 4 Alumni financial advisors, embedded alongside your team. 96% reduction in reconciliation time for Interstate Batteries. SEC-ready financials in 4 weeks for Atlas Technical Consultants."

Add a "Why Embark" comparison block (traditional firms vs. Embark) similar to the homepage comparison table, adapted for this specific service area.

**Why this should work:** Visitors on service pages are in comparison mode, evaluating Embark against 3-5 similar firms. When every service page says "we help you with complex financial challenges," none stands out. Injecting specific proof (named client outcomes from that service area) and competitive framing (traditional firms vs. Embark) gives the comparison-mode buyer a concrete reason to remember this vendor. The competitive analysis confirms that no analyzed competitor publishes NPS, attrition, or client outcome metrics on service pages.

**Target metric:** Bounce rate and engagement time on the pilot page (primary), downstream /contact or resource download clicks (secondary)
**Audience:** CFOs and finance leaders evaluating financial advisory options

**Scores:** Impact 4 | Confidence 3 | Ease 4
Impact 4 because competitive differentiation on service pages addresses the claim overlap gap (0.50) and the Specificity dimension. Confidence 3 because the differentiators are verified but we're extrapolating that comparison-mode visitors will respond to differentiation on a page with moderate traffic. Ease 4 because this is primarily a copy change with content that already exists in the case studies.

**What a win proves:** Confirms that differentiation injection on service pages changes visitor behavior in the evaluation phase. Successful pilot validates the approach for all 13 service pages and 7 industry pages.
**What a loss teaches:** Indicates that service page visitors are not yet in comparison mode, or that they need a different type of differentiation (process/methodology rather than proof points). Test interactive elements (video testimonials, process walkthroughs) as an alternative differentiation vehicle.

---

### 7. Objection Preemption: "Not a CPA Firm" Reframe

**Page:** /contact (primary), /what-we-do (secondary)
**What to test:** Surface the "not a CPA firm" regulatory constraint as a competitive advantage rather than burying it in footer disclaimers and FAQ answers.

**Current state:** Embark is legally required to state "Embark is not a CPA firm" (Texas State Board of Public Accountancy compliance). This disclaimer appears in the website footer. The competitive analysis identifies two related objections buyers raise: "You're not a CPA firm" and "We need one firm for audit + advisory + tax." The scorecard provides rebuttals for both: "That's our advantage. No audit conflicts. No independence constraints. We advise you without restrictions." and "Your auditor should audit. We should advise. Independence means we work for you, not around regulatory limits." These rebuttals do not appear anywhere on the main site pages.

**Baseline:** /contact: ~1,480 sessions/month, 63.1% bounce, 1.19% CVR. /what-we-do: ~540 sessions/month, 24.6% bounce.

**Proposed change:** Add an "Independence as Advantage" content section on /contact and /what-we-do pages:

> **Before:** Footer: "Embark is not a CPA firm." (defensive, buried)
> **After:** Above the contact form: "Why we don't do audits: No audit conflicts. No independence constraints. We advise you without restrictions. Your auditor should audit. We execute alongside your team with zero regulatory friction."

Additionally, add a brief FAQ-style block addressing the top two objections with the specific rebuttals, placed in the consideration flow before the form.

**Why this should work:** Unanswered objections do not disappear. They become reasons to choose a competitor. When a buyer sees "Embark is not a CPA firm" in the footer without context, they may interpret this as a limitation rather than a design choice. Proactive objection preemption reframes the concern before it solidifies: the constraint becomes a feature. Loss aversion applies in reverse: by articulating what buyers lose by choosing a CPA firm for advisory (audit conflicts, independence constraints, divided attention), Embark turns a defensive disclosure into a competitive wedge.

**Target metric:** contact_us_form_submit rate (primary), /contact bounce rate (secondary)
**Audience:** CFOs and finance leaders who are comparing Embark against Big 4 or CPA advisory firms

**Scores:** Impact 4 | Confidence 4 | Ease 3
Impact 4 because this objection is identified as a primary "when we lose" factor across multiple competitor battle cards. Confidence 4 because the objection is well-documented in competitive research, specific rebuttals exist with verified proof supporting them, and the /contact page has high traffic. Ease 3 because this requires both copy creation and placement decisions across multiple pages, plus potential stakeholder review of the regulatory language.

**What a win proves:** Confirms that proactive objection preemption on high-intent pages reduces form abandonment. The "independence as advantage" framing is validated as a selling point that the sales team can adopt in their conversations.
**What a loss teaches:** Suggests that raising the objection proactively introduces a concern buyers hadn't considered. The "not a CPA firm" framing, even when reframed positively, may plant doubt rather than resolve it. This would indicate the objection is better handled in sales conversations than on the website, and the site should focus on what Embark does rather than what it doesn't.

---

## Explorations

### 8. Happy Works Page: Conversion Path Addition

**Page:** /happy-works
**What to test:** Add a conversion mechanism to the Happy Works page, which currently has strong engagement but no way for visitors to take action.

**Current state:** The /happy-works page receives approximately 117 sessions per month with a 25.3% bounce rate, which is one of the lowest bounce rates on the site. The page showcases Embark's culture philosophy and includes the quantified proof: NPS 93, 9% consultant attrition, 91% client retention, and the revenue growth trajectory from $7M to $149M. Visitors who reach this page are clearly engaged (low bounce, strong dwell time). But there is no CTA, form, or next step on the page.

**Baseline:** ~117 sessions/month, 25.3% bounce rate, 0% CVR.

**Proposed change:** Add a contextual CTA at the bottom of the page: "See what happy consultants deliver. Read our case studies." Link to the case study index or to 2-3 featured case studies. Add a secondary CTA: "Ready to work with us? Book a 15-minute intro call."

**Why this should work:** Visitors who navigate to /happy-works have self-selected into Embark's strongest differentiator (culture proof). They are likely in evaluation mode, comparing Embark's culture claims against competitors. This is a high-intent, high-engagement audience with no conversion path. Adding a contextual next step (case studies that connect culture to client outcomes) maintains the visitor's momentum. The CTA bridges the gap between "I believe these consultants are happy" and "I believe happy consultants will do good work for me."

**Target metric:** CTA click-through rate (primary), downstream case study views and /contact visits (secondary)
**Audience:** Evaluators exploring Embark's culture differentiation

**Scores:** Impact 2 | Confidence 3 | Ease 4
Impact 2 because the page has low traffic (~117 sessions/month), limiting conversion volume regardless of rate improvement. Confidence 3 because the engagement signal is strong (25.3% bounce) but this is a novel test without pattern precedent. Ease 4 because this is adding a CTA block and links, which is straightforward CMS work.

**What a win proves:** Validates that culture-proof engaged visitors will convert when given a path. This supports building a "culture-to-conversion" funnel: paid campaigns driving traffic to /happy-works as a differentiated landing page.
**What a loss teaches:** Indicates that /happy-works visitors are browsing out of curiosity (potential recruits, industry observers, journalists) rather than evaluating as potential clients. The page serves brand awareness, not conversion. Redirect investment to pages where visitors have buyer intent.

---

### 9. Persona-Based Navigation Paths

**Page:** Site-wide navigation
**What to test:** Add use-case or persona-based navigation paths ("For CFOs," "For PE-Backed Companies," "For Companies in Transition") alongside or replacing the current service-based navigation.

**Current state:** Embark serves 4 distinct personas (CFO, COO, CIO/CTO, CHRO/CPO) with different primary challenges and evaluation criteria. The current navigation is organized by service category (/what-we-do, /who-we-serve), which forces each persona to self-filter through service descriptions to find what's relevant. The messaging analysis recommends persona-specific messaging, but the site architecture delivers a one-size-fits-all experience.

**Baseline:** Site-wide bounce rate: 69.5%. Service page group: 31.6% bounce, 0% CVR. Industry page group: 31.6% bounce, 0% CVR.

**Proposed change:** Add a "How We Help" dropdown with persona-based entry points:
- "For CFOs & Finance Leaders" -> Office of the CFO content, case studies featuring CFOs (P21 Solo Brands, P17 Interstate Batteries)
- "For PE-Backed Companies" -> PE/VC advisory services, portfolio company case studies
- "For Companies in Transition" -> M&A advisory, IPO readiness, integration support

Each path leads to a persona-tailored page that reframes Embark's services through that buyer's lens.

**Why this should work:** When a B2B site serves multiple buyer personas, service-based navigation forces each persona to translate features into personal value. Persona-based navigation acts as a shortcut: "For CFOs" immediately signals "this section is about my problems." It reduces navigation effort and increases perceived relevance. The competitive analysis shows no competitor currently offers persona-based navigation, making this a structural differentiation opportunity.

**Target metric:** Navigation engagement (clicks on persona paths), downstream page views per session, and /contact CVR (primary)
**Audience:** All visitors, segmented post-hoc by which persona path they select

**Scores:** Impact 4 | Confidence 3 | Ease 2
Impact 4 because this addresses both the Specificity gap and the structural 0% CVR on service/industry pages by creating relevance-matched pathways. Confidence 3 because the 4 personas are documented but only the CFO persona has strong direct evidence (testimonials from CFO-adjacent roles). Ease 2 because this requires navigation redesign, new page templates, and content creation for each persona path, which involves design and development effort.

**What a win proves:** Validates that Embark's audience self-identifies with persona labels and prefers role-based navigation over service-based navigation. This would reshape the entire site architecture and content strategy around buyer personas.
**What a loss teaches:** Indicates that Embark's visitors either don't identify with the persona labels used, or that the service-based structure is adequate for their evaluation process. Suggests the navigation structure is not the friction point and optimization should focus on within-page content instead.

---

### 10. Segment-Based Hero Personalization

**Page:** Homepage (/)
**What to test:** Serve persona-matched hero copy (headline, subhead, CTA) based on traffic source signals: UTM parameters from paid campaigns, referral source, or ad group targeting.

**Current state:** All visitors see the same homepage hero regardless of who they are or how they arrived. The messaging analysis defines distinct value propositions for each persona: CFOs care about reporting gaps and audit readiness. COOs care about process scaling. CIOs care about system modernization. PE sponsors care about portfolio company performance. But the homepage addresses none of them specifically.

**Baseline:** ~6,700 sessions/month, 59.5% bounce rate. Cross-network drives 9,562 sessions to the site (14.5% of total).

**Proposed change:** Serve different hero headline/subhead combinations based on UTM campaign parameters from paid campaigns. Example:
- UTM campaign contains "cfo" or "finance": "Your finance team needs Big 4 caliber support without the Big 4 price tag. NPS 93."
- UTM campaign contains "pe" or "portfolio": "Financial advisory for PE-backed portfolio companies. From acquisition to exit. 91% client retention."
- Default (organic, direct): "Big 4 Alumni advisors who stay, execute, and care. NPS 93." (the control from Experiment 1)

**Why this should work:** Relevance drives conversion. A CFO evaluating financial advisory options and a PE sponsor looking for portfolio company support evaluate through completely different lenses. Matching the opening message to their frame reduces cognitive distance between "this page exists" and "this page is for me." The paid traffic (Cross-network + Paid Search combined: 11,000 sessions) already carries targeting signals via UTM parameters, making segment detection feasible without new infrastructure.

**Target metric:** Bounce rate by segment (primary), /contact CVR by segment (secondary)
**Audience:** Paid traffic segments identifiable by UTM parameters

**Scores:** Impact 5 | Confidence 2 | Ease 2
Impact 5 because personalization on the highest-traffic page, applied to the largest paid traffic channel, has transformational potential if it works. Confidence 2 because the personas are defined but only the CFO has strong direct evidence, UTM-based targeting depends on campaign discipline (which hasn't been verified), and the current headline hasn't been tested yet (run Experiment 1 first). Ease 2 because this requires a personalization platform or CMS conditional logic, campaign UTM standardization, and cross-team coordination between marketing, paid media, and web development.

**What a win proves:** Confirms that segment-specific messaging produces measurably better outcomes than one-size-fits-all. This validates the investment in a full personalization program, including dynamic content across service pages, case study matching, and persona-specific landing pages.
**What a loss teaches:** Indicates that the homepage serves a "learn about Embark" function where all visitors need the same foundational message before segment-specific details become relevant. Suggests personalization should target deeper pages (service pages, case studies) where visitors have already established category understanding.

---

## Sequencing Rationale

**Start with the homepage.** Experiments 1 (H1 headline), 2 (proof strip), and 5 (CTA language) all target the homepage and can be run in a phased sequence: headline first, then proof strip, then CTA. The headline test is foundational because it establishes whether outcome-oriented language with culture proof outperforms generic positioning. Every downstream experiment assumes this direction. If the headline loses, the messaging strategy shifts to category-clarity-first, which changes the proof strip and CTA approaches. Run the headline test for at least 2-3 weeks before layering on the proof strip.

**Contact page optimization (Experiment 3) runs in parallel.** It targets a different page and a specific audience segment (PMax retargeting traffic), so it doesn't confound with homepage tests. The form completion optimization is time-sensitive because the PMax "Handraisers - Retargeting" campaign is sending ~1,000 mobile sessions/month to /contact with an 88% form abandonment rate -- every month without a fix is wasted retargeting spend. **Prerequisite:** audit the /contact form fields before designing the variant.

**Service page CTAs (Experiment 4) should start after the homepage direction is validated.** If the homepage headline test confirms that proof-forward messaging works, the service page CTAs should emphasize proof-aligned resources. If the headline test reveals that category clarity is more effective, the service page CTAs should lean into explainer content. Start with 3-5 high-traffic service pages as a pilot before expanding to all 20 pages.

**Experiments 6 (differentiation injection) and 7 (objection preemption) require Experiment 1 results.** Both apply messaging principles that the headline test will validate or invalidate. If proof-forward messaging wins on the homepage, inject it into service pages (Experiment 6) and frame objections around proof (Experiment 7). These two can run in parallel with each other since they target different page types.

**Explorations (8, 9, 10) are sequenced by learning value.** Experiment 8 (Happy Works CTA) is low-effort and can run any time. Experiment 9 (persona navigation) should wait until Experiments 1 and 4 reveal which messaging direction works. Experiment 10 (personalization) depends on Experiment 1 establishing a winning baseline and Experiment 9 validating whether persona-based framing resonates.

---

## What's Not Here (and Why)

**Pricing transparency test.** Embark does not have a pricing page, but neither do any of the 11 analyzed competitors. Deal sizes are highly variable (project-based, retainer, interim/fractional). The pricing transparency pattern requires competitive pressure (competitors publishing pricing) to trigger, and that pressure does not exist in this market. Additionally, consulting pricing is legitimately complex: publishing a number without context could anchor unfavorably.

**Form field reduction.** The /contact page uses a form, but without direct observation of the field count and types, a field reduction test would be speculative. If the form has 5+ fields, this becomes a viable Quick Win. Manual site audit recommended.

**Blog content optimization (/research-and-development-accounting).** This page has a shallow_engagement failure mode (81% bounce, 0.86 pages/session) but only 441 sessions over 90 days. The keyword-content mismatch is real but the traffic volume makes optimization low-impact. Not worth a dedicated experiment, but worth a content audit to either improve the page or redirect the URL.

**NPS inconsistency (87 vs 93).** The main site shows an NPS of 87 while HubSpot landing pages show 93 (the confirmed figure). This is not an experiment. Update the main site to 93. Just do it.

**Banned term removal on service pages.** Several service sub-pages use "industry-leading" and other superlative language that violates Embark's own voice guidelines. This is a content hygiene task, not an experiment. Remove the banned terms and replace with specific language. Just do it.

**Multi-step form test.** This requires knowing the current form structure. If the /contact form is a single-page form with 5+ fields, a multi-step form conversion test is a strong candidate. Verify form field count first.

**ROI calculator.** An interactive ROI calculator is a high-value Strategic Bet, but it requires custom engineering and benchmark data that hasn't been confirmed. The evidence strip (Experiment 2) tests whether ROI metrics resonate before investing in the calculator.

**Assessment/diagnostic tool.** A viable Exploration for Embark's 4 personas and multiple segments, but requires significant development effort and persona validation. Wait until Experiment 9 (persona navigation) validates whether visitors self-identify with persona labels before building an assessment tool.

---

## Prerequisites and Data Gaps

### Missing Baseline Data

- **Contact form field count and structure (BLOCKING for Experiment 3).** The form on /contact has not been directly audited for field count, field types, or form completion funnel. GA4 data shows a 4.3x form completion gap between Cross-network (12.1%) and Direct (51.5%) visitors, with 71% of Cross-network traffic arriving on mobile. This makes form audit the top prerequisite. **Action:** Audit the /contact form manually. Count fields, note types (text, dropdown, checkbox), check for required vs. optional fields, and test the form on a mobile device to assess UX friction.
- **Enhanced measurement is disabled.** Scroll, click, and file_download events report zero in the current 90-day period (previously active at 36,708 scroll events, 5,207 click events, 645 file_downloads). This eliminates engagement signal data for all pages and prevents scroll depth analysis for Experiments 1, 2, and 6. **Action:** Re-enable enhanced measurement in GA4 immediately. This is not optional for running CRO experiments, as it provides the engagement data needed to interpret test results.
- **Direct traffic quality.** Direct traffic (54.5% of all sessions) has an 85.2% bounce rate (up from 69.5% prior period). This is anomalous for legitimate direct traffic. Before optimizing the homepage for Direct visitors (Experiment 1), determine whether this traffic is real. **Action:** Check for bot traffic patterns, review referral exclusion settings, audit internal/CMS preview traffic leakage (/_hcms/preview/* accounted for 952 sessions), and investigate whether HubSpot CTA redirects (/cs/c/) are inflating Direct attribution.
- **Ad campaign creative and UTM structure.** Experiment 10 (segment personalization) requires knowledge of current ad messaging and UTM parameter conventions. GA4 data confirms the primary campaign driving /contact traffic is "Performance Max - Handraisers - Retargeting" (3,034 sessions/90 days, 99% of Cross-network). **Action:** Export current Google Ads campaign creatives, review PMax asset groups and audience signals for the Handraisers campaign, and document UTM parameter taxonomy for personalization targeting.

### Context Verification Needed

- **COO, CIO/CTO, and CHRO/CPO persona validation.** Three of four personas are inferred from website service descriptions and job role norms. Only the CFO persona has direct evidence (testimonials from CFO-adjacent roles). This affects Experiments 9 and 10, which depend on persona labels resonating with real visitors. **Action:** Client interviews with actual COO, CIO, and CHRO buyers. Alternatively, review CRM data for buyer role distribution across closed deals.
- **"Right-sized flexibility" value theme proof.** This value theme has Level 2 proof only (single testimonial mentioning pricing flexibility). If used in homepage copy (Experiment 1 variant), the claim lacks the verification depth of other themes. **Action:** Collect 2-3 additional client testimonials referencing engagement flexibility, no-contract model, or pricing accommodation.

### Infrastructure Prerequisites

- **A/B testing platform.** Experiments 1-3 and 5-7 require an A/B testing platform configured on the target pages. The GA4 event data shows `viewed_experiment` events (11,036 in current period) from FunnelEnvy, indicating a testing platform is active. **Verify:** Confirm which testing tool is in use, which pages it covers, and whether it supports the proposed test types.
- **CMS conditional content or personalization tool.** Experiment 10 (segment-based hero personalization) requires the ability to serve different hero content based on UTM parameters or visitor attributes. **Action:** Evaluate whether the current CMS (appears to be HubSpot based on /_hcms/ paths) supports conditional content modules or smart content rules. If not, a personalization platform is needed.
- **Cross-team coordination for paid campaigns.** Experiments 3 and 10 require alignment between the paid media team (ad creative, UTM conventions) and the web/CRO team (landing page copy, testing setup). **Action:** Establish a shared brief for ad-to-page messaging consistency before launching Experiment 3.

---
*Analysis produced by FunnelEnvy | February 2026*
*Based on positioning analysis across 5 research sources, 11 competitors, and 90 days of GA4 analytics data (65,850 sessions)*
