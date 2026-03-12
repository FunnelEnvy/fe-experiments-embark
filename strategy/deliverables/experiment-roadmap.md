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
| 1 | Objection Preemption: Independence as Advantage | /contact, /what-we-do/* | Quick Win | 3 | 4 | 4 | 11 |
| 2 | Team Page: Evaluation-Stage Conversion Path | /team/* | Quick Win | 3 | 4 | 5 | 12 |
| 3 | Offices Page: Local Advisor Contact Path | /offices | Quick Win | 2 | 3 | 5 | 10 |
| 4 | Homepage Hero: Differentiation-Led Messaging with Proof | / | Strategic Bet | 5 | 4 | 3 | 12 |
| 5 | Contact Page: Paid Traffic Message Alignment | /contact | Strategic Bet | 4 | 4 | 3 | 11 |
| 6 | Service Page Differentiation with Contextual Conversion Paths | /what-we-do/* | Strategic Bet | 4 | 3 | 3 | 10 |
| 7 | Industry Page: Vertical-Specific Proof and Conversion Paths | /who-we-serve/* | Strategic Bet | 3 | 3 | 3 | 9 |
| 8 | Returning Visitor Differentiated Experience | Site-wide | Exploration | 3 | 3 | 2 | 8 |
| 9 | Blog Content: Organic Entry Point Capture | Root-level blog posts | Exploration | 2 | 3 | 3 | 8 |
| 10 | Segment-Based Hero Personalization | / | Exploration | 4 | 2 | 1 | 7 |
| 11 | Persona-Based Navigation Paths | Site-wide navigation | Exploration | 4 | 2 | 1 | 7 |
| 12 | Finance Function Readiness Assessment | New page | Exploration | 3 | 2 | 2 | 7 |

---

## Quick Wins

### 1. Objection Preemption: Independence as Advantage

**Page:** /contact and /what-we-do/financial-advisory-consulting
**What to test:** Proactively reframe Embark's non-CPA status as a buyer advantage on high-intent pages, rather than leaving it as a footer disclaimer.

**Current state:** "Embark is not a CPA firm" appears only as a disclaimer in the website footer. The contact page and service pages make no proactive mention of why independence from audit and tax work benefits the buyer. The objection cheat sheet has a strong rebuttal ("No audit conflicts. No independence constraints. We advise you without restrictions."), but this messaging is not surfaced anywhere on the website. Buyers who notice the disclaimer or recognize that Embark is not a CPA firm receive no reframing context. The competitive landscape identifies a missing rebuttal for the "We need a one-stop-shop for audit + advisory + tax" objection, which is Embark's most structural positioning challenge against CPA/advisory combo firms (Cherry Bekaert, Baker Tilly, RSM, Forvis Mazars).
**Baseline:** /contact: 1,480 sessions/mo, 63.1% bounce, 1.19% CVR. /what-we-do/financial-advisory-consulting: 212 sessions/mo, 37.0% bounce, 0% CVR.
**Test Feasibility:** ~7 weeks at 15% MDE on /contact using engagement rate (2 variants, ~1,214 samples/variant). Extended. Consider form_start as micro-conversion for faster signal.
**Proposed change:** Add an "Independence is our advantage" content block on the /contact page (above or adjacent to the form) and on /what-we-do/financial-advisory-consulting. Content reframes the non-CPA status positively: why advisory independence means unrestricted counsel without audit conflicts.

> **Before:** Footer disclaimer: "Embark is not a CPA firm." No proactive reframing on any page.
> **After:** Content block on /contact: "Why independence matters. Your auditor should audit. We should advise. Because we don't perform audits or tax work, we advise you without the independence constraints that limit CPA firms who audit and advise the same client. No conflicts. No restrictions. Just unrestricted advisory from Big 4 Alumni who chose consulting."

**Why this should work:** Unanswered objections don't disappear. They become reasons to choose a competitor. Buyers evaluating Embark alongside CPA/advisory combo firms will notice the non-CPA status. Without proactive reframing, the buyer defaults to "they can't do audits" as a limitation rather than "they can advise without restrictions" as a benefit. Preemptive reframing addresses the concern at the moment of highest intent (contact page), converting what looks like a weakness into a differentiator.

**Target metric:** Form start rate on /contact, secondary: contact_us_form_submit rate
**Audience:** All /contact and service page visitors, particularly those arriving from competitive search terms

**Scores:** Impact 3 | Confidence 4 | Ease 4
Impact 3: Addresses a specific subset of visitors who have this concern, not all visitors. Meaningful for those it affects, but not universal. Confidence 4: The objection is well-documented across competitive analysis and client intake. Strong rebuttal copy exists. Behavioral principle (loss aversion in reverse: show what buyer loses choosing a conflicted advisor) is well-established. Ease 4: Adding a content block to existing pages. Copy is already drafted in the objection cheat sheet. No structural changes required.

**What a win proves:** Proactive objection handling on high-intent pages influences conversion. Validates expanding this approach to other objections ("How do we know we'll get senior people?" and "Aren't you just a staffing agency?").
**What a loss teaches:** Visitors may not carry this objection to the contact page, or the reframe may not be strong enough to overcome it. Would suggest the objection is better handled in sales conversation than web copy, or that the reframe needs customer-attributed proof (a testimonial from someone who initially had the same concern).

---

### 2. Team Page: Evaluation-Stage Conversion Path

**Page:** /team and /team/*
**What to test:** Add a contextual conversion mechanism to the team pages, capturing buyers who are actively evaluating Embark's people.

**Current state:** The /team page group receives 4,217 sessions per 90 days (1,406 sessions/mo) with the strongest engagement metrics on the entire site: 25.4% bounce rate, 74.6% engagement rate, and 107s average engagement time. Individual team member pages (e.g., /team/paul-allen at 412 sessions, 40.5% bounce) show visitors are drilling into specific people. /team is also a significant entry page: 1,577 landing sessions per 90 days with 38.0% bounce and 62.0% engagement rate. Despite this, the team page group has a 0% conversion rate. No CTA, no form, no path to contact exists on any team page. Visitors who are deep in evaluation mode -- actively researching the specific people they'd work with -- have no way to take the next step without navigating to /contact independently.
**Baseline:** 1,406 sessions/mo (group), 25.4% bounce, 0% CVR. 107s avg engagement time.
**Test Feasibility:** ~3 weeks at 15% MDE (2 variants, ~1,045 samples/variant) using engagement rate. CTA click-through rate can be measured as a new baseline. Feasible.
**Proposed change:** Add a contextual CTA to the team page and individual team member pages. Options: (1) "Work with our team" button linking to /contact with team context pre-populated, (2) inline "Talk to an advisor" CTA positioned after the team grid or at the bottom of individual bios, (3) a brief reinforcement line adjacent to the CTA: "Big 4 Alumni advisors with an NPS of 93. The people you see here are the people who show up."

> **Before:** Team grid with headshots, names, and titles. No conversion mechanism. Visitors must independently navigate to /contact.
> **After:** Same team grid plus: "These are the advisors who show up. Big 4 Alumni with 9% attrition -- half the industry average. [Talk to an advisor]" positioned below the team grid. On individual bio pages: "Want to work with [Name]'s team? [Get in touch]" below the bio.

**Why this should work:** Visitors browsing the team page are in evaluation mode. They're answering the question "who are these people and can I trust them?" The 107s average engagement time and 74.6% engagement rate confirm genuine interest, not casual browsing. These are among the most engaged visitors on the entire site. Adding a conversion mechanism at the moment they've finished evaluating (bottom of team grid, bottom of individual bio) captures intent at peak confidence. The proof reinforcement (NPS 93, 9% attrition) provides the final push: "these people stay, and clients love working with them."

**Target metric:** CTA click-through rate (new), secondary: /contact page visits from /team/*, form_start rate on /contact for team-referral sessions
**Audience:** All /team and /team/* visitors

**Scores:** Impact 3 | Confidence 4 | Ease 5
Impact 3: Adds a conversion path to a high-engagement page group (1,406 sessions/mo), but these visitors are mid-funnel (evaluating people) not bottom-funnel (ready to buy). Incremental lead capture, not transformational. Confidence 4: Behavioral signal is unambiguous: 107s engagement and 74.6% engagement rate mean visitors are genuinely interested. The only question is whether adding a CTA captures that interest or if these visitors already find /contact on their own. GA4 shows pages/session of 1.15 on /team, suggesting most visitors don't navigate further. Ease 5: Adding a CTA block with existing copy to a page template. No structural changes. Minimal development effort.

**What a win proves:** High-engagement evaluation pages generate leads when given a conversion mechanism. Validates adding CTAs to other high-engagement, zero-conversion pages (/about at 1,020 sessions, /partners at 517 sessions, /offices at 1,850 sessions).
**What a loss teaches:** Team page visitors may be a different audience than buyers (recruiters, job seekers, competitors). The high engagement may reflect research behavior rather than purchase intent. Would suggest analyzing team page traffic sources to identify what proportion is buyer vs. non-buyer.

---

### 3. Offices Page: Local Advisor Contact Path

**Page:** /offices
**What to test:** Add a location-specific conversion mechanism to the offices page, converting local-presence validation into contact intent.

**Current state:** The /offices page receives 1,850 sessions per 90 days (617 sessions/mo) with 29.4% bounce, 70.6% engagement rate, and 106s average engagement time. It also serves as an entry page for 832 landing sessions with 48.7% bounce and 51.3% engagement rate. Embark has 26 US offices, and this page is a consideration-stage destination for buyers evaluating whether Embark has local coverage for their needs. Despite strong engagement metrics, the page has 0% conversion rate. No CTA or contact mechanism exists. Visitors who confirm Embark has a local presence must independently navigate to /contact, losing the location context.
**Baseline:** 617 sessions/mo, 29.4% bounce, 0% CVR. 106s avg engagement time.
**Test Feasibility:** ~5 weeks at 15% MDE (2 variants, ~1,045 samples/variant) using engagement rate. Pre/post is a viable alternative given the lower traffic volume. Borderline feasible for A/B; pre/post recommended.
**Proposed change:** Add a "Contact your local advisor" or "Find your nearest advisor" CTA to the offices page. Option A: a single prominent CTA linking to /contact. Option B: per-office contact links or a form that captures the visitor's location of interest alongside their contact information. Include proof reinforcement: "26 offices. Local advisors. National reach."

> **Before:** Office listings with locations. No conversion mechanism. Visitors confirming local presence must navigate to /contact independently.
> **After:** Office listings plus: "Ready to connect with a local advisor? [Contact your nearest office]" with optional location selection that pre-populates the contact form. Reinforcement: "26 US offices. The advisor who shows up is the advisor who stays."

**Why this should work:** Visitors checking office locations are answering a specific buying question: "Can this firm serve us locally?" The 106s engagement time suggests they're carefully reviewing locations, not just glancing. Once a visitor confirms local availability, the next natural step is "talk to someone there." Without a CTA, the page answers the location question but drops the visitor before capturing intent. The location context is also valuable for sales routing -- knowing which office the visitor is interested in makes the follow-up more relevant.

**Target metric:** CTA click-through rate (new), secondary: /contact page visits from /offices, form_start rate
**Audience:** All /offices visitors

**Scores:** Impact 2 | Confidence 3 | Ease 5
Impact 2: 617 sessions/mo is moderate traffic, and the conversion potential depends on what proportion of visitors are buyers vs. job seekers or other audiences. The page doesn't have enough traffic to drive a large absolute number of conversions. Confidence 3: Engagement metrics confirm visitor interest, but the audience mix is uncertain. Some portion of office page traffic may be job seekers checking locations rather than buyers evaluating coverage. Ease 5: Adding a CTA to a single page with existing infrastructure. Trivial implementation.

**What a win proves:** Consideration-stage pages with strong engagement generate leads when given a contextual conversion path. Validates the broader pattern of adding CTAs to high-engagement, zero-conversion pages across the site.
**What a loss teaches:** Office page visitors may not be buyers, or the location-to-contact journey may already happen organically (visitors navigate to /contact after /offices without needing a CTA). Would suggest audience analysis of /offices traffic sources before further investment.

---

## Strategic Bets

### 4. Homepage Hero: Differentiation-Led Messaging with Proof

**Page:** /
**What to test:** Replace the generic carousel hero with a static, differentiation-led hero section that leads with Embark's unique positioning and proof, replacing aspirational language with specific claims backed by quantified evidence.

**Current state:** The homepage hero is a three-slide carousel. Slide 1 uses the headline "High-impact consulting for growing companies" with the subhead "At Embark, we help ambitious businesses scale into their next chapter with strategic guidance and hands-on support." Slides 2 and 3 promote downloadable templates (controller transition template, external audit preparation guide). CTAs are "What we do" and "Talk to an advisor." None of Embark's structural differentiators (NPS 93, 9% attrition, 91% client retention, Happy Works, Big 4 Alumni talent) appear above the fold. The carousel dilutes the first impression by rotating between positioning and resource promotions. The content offers in slides 2-3 are not driving conversion: the homepage has 0% CVR despite the carousel templates being visible to all 6,673 monthly visitors.
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

**Why this should work:** B2B buyers decide within 3-5 seconds whether a page is relevant. The current headline ("High-impact consulting for growing companies") is category language that any advisory firm could use. It forces visitors to do cognitive work to figure out what makes Embark different. The proposed version leads with Embark's strongest differentiator (Big 4 Alumni who stay) and immediately backs it with proof no competitor can match (NPS 93, 9% attrition). The carousel currently spreads attention across three slides, two of which promote templates rather than positioning -- and those templates aren't converting anyway (0% homepage CVR despite prominent placement). A static hero eliminates this dilution and focuses the first impression on the message most likely to reduce bounce: "this company is different, and here's the proof." The positioning scorecard identifies Clarity as the top opportunity and Specificity as the top gap. This experiment addresses both simultaneously.

**Target metric:** Engagement rate (inverse of bounce), secondary: /contact page visits from homepage, "Talk to an advisor" CTA click rate
**Audience:** All homepage visitors

**Scores:** Impact 5 | Confidence 4 | Ease 3
Impact 5: Highest-traffic page (6,673/mo), worsening bounce trend (+13.5pp), and addresses both the top gap (specificity) and top opportunity (clarity) from the positioning scorecard. A win here changes the entire site's conversion trajectory. Confidence 4: "Before" copy is exact text from the website. "After" copy adapts directly from the positioning statement and channel adaptations. GA4 data confirms worsening bounce trend. Traffic adequacy is high. Capped at 4 (no evidence module calibration data). Ease 3: Requires carousel removal, layout restructuring for static hero, proof strip creation, and CTA consolidation. More than a copy swap. Moderate development effort.

**What a win proves:** Differentiation-led, proof-backed messaging resonates more than generic aspirational copy. Validates extending this approach to service pages (Experiment #6) and informs the content of personalized hero variants (Experiment #10).
**What a loss teaches:** Visitors may value the aspiration-first framing ("growing companies," "next chapter"), or the proof metrics may not carry meaning for visitors unfamiliar with NPS or attrition benchmarks. Would suggest testing proof-first (case studies above fold) separately from differentiation-first (headline change) to isolate which element failed.

---

### 5. Contact Page: Paid Traffic Message Alignment

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

### 6. Service Page Differentiation with Contextual Conversion Paths

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
Impact 4: 1,408 sessions/mo with zero conversion represents a major structural opportunity. Performance profile sizes this as "large" impact: ~22 additional conversions/month at a conservative 3% capture rate (combined with industry pages). The current state is complete conversion absence. Confidence 3: Trigger conditions confirmed (generic copy, 0% CVR, case studies available), but "before" copy is described from messaging gap analysis rather than exact page text. Competitive landscape confidence is 2, limiting certainty about differentiation effectiveness. Ease 3: Requires content creation for differentiation blocks and case study cards across multiple pages, plus resource CTA integration. Can be templated, but still requires per-page adaptation.

**What a win proves:** Service page visitors respond to differentiation content and will convert on contextual resource offers. Validates the broader strategy of turning service pages from brochures into conversion-capable assets. Directly informs Experiment #7 (industry pages).
**What a loss teaches:** The conversion gap on service pages may be intent-based (visitors come to learn about capabilities, not to engage yet), or the generic copy may not be the conversion blocker (page structure or CTA placement could be). Would suggest testing CTA placement and offer type independently from content changes.

---

### 7. Industry Page: Vertical-Specific Proof and Conversion Paths

**Page:** /who-we-serve/* (7 industry sub-pages)
**What to test:** Add industry-specific case study proof and contextual conversion CTAs to industry pages, converting a zero-conversion page group into an active lead capture mechanism.

**Current state:** The 7 industry sub-pages under /who-we-serve/* collectively receive 1,277 sessions per 90 days (426 sessions/mo) with a group conversion rate of 0%. The /who-we-serve hub page itself gets 382 sessions with 22.5% bounce and 77.5% engagement rate, indicating strong interest in industry-specific content. Like service pages, no conversion mechanism exists on any industry page. Embark serves 19 industries with specific buying triggers per vertical (PE-backed companies: audit readiness + M&A complexity; energy: ESG compliance + commodity accounting; healthcare: regulatory compliance + revenue cycle). The competitive landscape identifies ESG advisory from a non-CPA firm as unclaimed white space. None of the 17 published case studies with quantified outcomes are surfaced on industry pages.
**Baseline:** 426 sessions/mo (group), 31.6% bounce, 0% CVR. /who-we-serve hub: 382 sessions, 22.5% bounce, 77.5% engagement. Individual industry page traffic is below 100 sessions/mo each.
**Test Feasibility:** Cannot estimate (no conversion rate baseline). Group-level engagement metrics are feasible but slow at 426 sessions/mo. Pre/post recommended for individual pages.
**Proposed change:** For the top 2-3 industry pages by traffic, add: (1) an industry-specific pain statement tied to a buying trigger (e.g., energy: "ESG reporting compliance deadline approaching. Commodity accounting complexity growing."), (2) a named case study from that vertical with a quantified outcome, (3) an industry-contextual CTA (not a generic template download but a vertical-relevant offer: e.g., "See how we prepared Atlas Technical's SEC filing in 4 weeks" or "Download: Post-Merger Integration Checklist for PE Portfolio Companies").

> **Before (/who-we-serve/[industry]):** Generic industry description. No case studies. No conversion CTA. No differentiation from competitors who claim the same verticals.
> **After (energy example):** "Big 4 Alumni advisors with deep energy sector experience. ESG reporting readiness, commodity accounting, and operational finance for oil & gas, renewables, and infrastructure." + Named case study card + "Talk to an energy sector advisor" CTA.

**Why this should work:** Industry page visitors arrive with a vertical-specific lens. A CFO at a PE-backed energy company evaluating advisors cares that Embark has energy experience, not just general consulting credentials. Generic industry pages force buyers to infer relevance ("do they actually know our sector?"). Industry-specific proof eliminates this inference step. The competitive landscape shows most competitors claim broad industry coverage without vertical-specific proof -- Embark's named case studies across 15+ industries are a genuine differentiation advantage that isn't deployed. Additionally, the /who-we-serve hub's 77.5% engagement rate signals that visitors arriving at industry content are engaged and evaluating.

**Target metric:** Resource CTA click-through rate (new), secondary: engagement rate, /contact page visits from industry pages
**Audience:** Industry page visitors, particularly those arriving from industry-specific search queries or paid campaigns

**Scores:** Impact 3 | Confidence 3 | Ease 3
Impact 3: 426 sessions/mo is moderate traffic, and individual page volumes are too low for per-page testing. Combined with service pages (Experiment #6), the total zero-conversion opportunity is 1,834 sessions/mo. Industry pages contribute the smaller share. Confidence 3: The structural gap (0% CVR, no conversion path) is confirmed. The mechanism (proof + CTA) is the same as Experiment #6, applied to a different page group. Capped at 3 because individual industry page content hasn't been reviewed, and case study-to-industry mapping may require new content. Ease 3: Same templated approach as service pages, but requires industry-specific case study matching and potentially new case study cards for industries where quantified outcomes aren't yet published.

**What a win proves:** Industry-framed visitors convert on vertical-specific proof and CTAs. Validates investing in deeper industry content (dedicated landing pages, industry-specific resources) and informs whether Embark should lead with industry expertise or service capability in paid campaigns.
**What a loss teaches:** Industry page visitors may be too early in their journey to convert (browsing sectors rather than evaluating a specific advisor). Or the industry pages may attract informational traffic (students, journalists, competitors) rather than buyers. Would suggest traffic source analysis of industry pages before further investment.

---

## Explorations

### 8. Returning Visitor Differentiated Experience

**Page:** Site-wide
**What to test:** Serve a differentiated experience to returning visitors, recognizing their familiarity with Embark and accelerating them toward conversion instead of repeating the same first-visit messaging.

**Current state:** Returning visitors represent 9.4% of traffic (6,104 sessions per 90 days) but convert at 2.5x the rate of new visitors (2.06% vs. 0.83% unified CVR). They spend 4.2x longer on site (245s vs. 58s) and bounce 18pp less (52.7% vs. 70.4%). Despite this significantly higher intent, returning visitors see the exact same homepage, service pages, and CTAs as first-time visitors. The site's 90% new-visitor composition means all messaging is calibrated for first impressions, not for visitors who already know what Embark does and are returning to take action. Both new and returning CVRs declined from the prior period (new: 2.83% to 0.83%, returning: 4.59% to 2.06%), but returning visitors remain the highest-converting identifiable segment.
**Baseline:** 2,035 returning sessions/mo, 52.7% bounce, 2.06% unified CVR, 245s avg engagement.
**Test Feasibility:** ~4 weeks at 15% MDE (2 variants, ~1,045 samples/variant) using engagement rate on returning segment. Requires audience segmentation in testing platform (new vs. returning cookie). Feasible if platform supports it.
**Proposed change:** For identified returning visitors (via cookie or GA4 user state), modify the homepage experience: (1) skip the positioning pitch and lead with a direct CTA: "Welcome back. Ready to talk to an advisor?", (2) surface case study proof instead of generic value props (they already know the value props), (3) optionally show a "What's new" element if there's recent content (new case study, new resource). On /contact, returning visitors see simplified form reinforcement: "You've been here before. Here's what happens next: a 15-minute call, no obligation."

> **Before:** All visitors see the same homepage and /contact experience regardless of visit history.
> **After (returning visitor):** Homepage hero: "Welcome back. Our Big 4 Alumni advisors are ready when you are. [Talk to an advisor]" + latest case study card + "Since your last visit: [new resource or case study]". /contact: "You've been researching. Let's talk. A 15-minute call with a senior advisor to discuss your specific situation."

**Why this should work:** A returning visitor has already answered "what does this company do?" Their questions are now "should I engage?" and "how do I start?" Repeating the positioning pitch wastes their higher intent. B2B buying cycles often involve 3-7 website visits before a conversion event. By the second or third visit, the visitor needs acceleration, not re-education. The 2.5x conversion rate gap proves returning visitors are fundamentally different from new ones. Tailoring the experience to their stage should widen this gap further.

**Target metric:** Returning visitor engagement rate, secondary: returning visitor contact_us_form_submit rate, returning-to-new CVR ratio
**Audience:** Returning visitors (identified by cookie/user state), all pages but primarily homepage and /contact

**Scores:** Impact 3 | Confidence 3 | Ease 2
Impact 3: 2,035 sessions/mo is a meaningful segment, and the 2.06% baseline CVR provides room for improvement. Lifting returning CVR from 2.06% to 3% would add ~2 additional contact form completions per month. Not transformational in absolute terms, but validates a high-leverage pattern. Confidence 3: The returning-visitor intent signal is strong (2.5x CVR, 4.2x engagement time). The mechanism (differentiated messaging by visit stage) is well-established in B2B. Capped at 3 because: (a) returning visitor composition is unknown (could be employees, partners, or repeat job seekers, not just buyers), (b) the prior-period CVR decline affected returning visitors too, suggesting external factors beyond messaging. Ease 2: Requires visitor identification (new vs. returning) in the testing platform, conditional content rendering, and creation of returning-visitor variants for homepage and /contact. More complex than a simple copy swap.

**What a win proves:** Visit-stage personalization materially improves conversion for returning visitors. Validates investing in a multi-visit journey model (first visit = positioning, second visit = proof, third visit = conversion acceleration) and informs the personalization infrastructure needed for Experiment #10.
**What a loss teaches:** Returning visitors may already be converting at their natural ceiling, or the "returning" segment may be contaminated with non-buyer traffic (employees, partners, job seekers returning to check listings). Would suggest decomposing returning traffic by landing page to isolate the buyer subset before further personalization investment.

---

### 9. Blog Content: Organic Entry Point Capture

**Page:** Root-level blog posts (/research-and-development-accounting, /methods-for-a-summary-of-misstatements-*, and similar)
**What to test:** Add contextual service CTAs and resource offers to high-traffic blog posts that currently serve as organic entry points with no conversion path.

**Current state:** Several root-level blog posts attract meaningful organic traffic but have zero conversion mechanisms. /research-and-development-accounting receives 441 sessions with 81.0% bounce and is the only page flagged for shallow_engagement (0.86 pages/session, 19.0% engagement rate) -- visitors arrive from organic search, don't find what they need, and immediately leave. /methods-for-a-summary-of-misstatements-iron-curtain-vs.-rollover-approach receives 272 sessions with 55.5% bounce. These pages bring visitors who are searching for specific accounting topics that map directly to Embark's service expertise, but the content provides no bridge to Embark's advisory offerings. The career path guide (/resources/guides/the-career-path-guide-for-big-4-cpas at 443 sessions, 55.8% bounce) is in the Resources group but converts at ~0% while the group average is 6.55%.
**Baseline:** Combined ~1,200 sessions/90 days across root-level blog content. /research-and-development-accounting: 441 sessions, 81% bounce, shallow_engagement. /methods-for-misstatements: 272 sessions, 55.5% bounce. Career path guide: 443 sessions, 55.8% bounce, ~0% CVR.
**Test Feasibility:** Individual page traffic is too low for A/B testing. Pre/post recommended with group-level measurement. Can instrument CTA clicks as a new baseline metric across all blog pages simultaneously.
**Proposed change:** For blog posts with >200 sessions/90 days, add: (1) a contextual service CTA that maps the blog topic to an Embark capability (e.g., R&D accounting post: "Need help with R&D accounting treatment? Our Big 4 Alumni FARS advisors handle complex technical accounting."), (2) a relevant resource download link (e.g., R&D accounting post: link to ASC 606 template or similar), (3) a brief Embark positioning line that connects the educational content to advisory value.

> **Before (/research-and-development-accounting):** Blog content about R&D accounting methods. No CTA. No link to Embark's services. No resource offer. Visitors arrive from organic search and leave.
> **After:** Same blog content plus: sidebar or end-of-article CTA: "Complex accounting treatments like R&D capitalization require hands-on expertise. Our FARS advisors have helped companies like Interstate Batteries reduce reconciliation time by 96%. [Talk to a FARS advisor]" + "Download: ASC 606 Revenue Recognition Template" link.

**Why this should work:** Blog visitors arrive with a specific technical question. They're often mid-level accounting professionals (controllers, VPs of finance) who influence or make advisory hiring decisions. The current content answers their question but gives them no reason to think of Embark as anything other than a blog. Adding a contextual CTA that connects the blog topic to Embark's service capability plants a seed: "the people who wrote this article also do this as a service." The R&D accounting page's 81% bounce and shallow_engagement flag suggest the current content may not even answer the visitor's question well -- adding richer content alongside a service CTA addresses both the content gap and the conversion gap.

**Target metric:** CTA click-through rate (new), secondary: resource download rate, /contact page visits from blog content
**Audience:** Organic search visitors landing on root-level blog posts

**Scores:** Impact 2 | Confidence 3 | Ease 3
Impact 2: Individual blog pages have low traffic (200-450 sessions each), and the visitor profile skews informational rather than transactional. Conversion rates on blog CTAs in B2B are typically 0.5-2%, yielding 1-3 conversions/month across all blog pages combined. Confidence 3: The organic traffic is confirmed and the topic-to-service mapping is straightforward. The shallow_engagement flag on /research-and-development-accounting confirms a content gap that a CTA alone won't fix, but adding service context alongside content improvement is a reasonable combined approach. Ease 3: Requires per-post CTA creation with topic-to-service mapping. Can be templated, but each post needs a relevant service link and resource offer. Moderate content effort across multiple pages.

**What a win proves:** Organic blog traffic can be converted into advisory leads through contextual service CTAs. Validates investing in a content strategy that deliberately creates blog content as top-of-funnel entry points for specific service lines.
**What a loss teaches:** Blog visitors may be too early in their journey (informational search, not evaluative) to respond to advisory CTAs. Or the blog content itself may need to be substantially improved before any CTA is effective (the shallow_engagement flag suggests content quality issues). Would suggest improving the content first and testing CTAs second.

---

### 10. Segment-Based Hero Personalization

**Page:** /
**What to test:** Serve persona-matched hero messaging (headline, subhead, CTA) to different visitor segments based on traffic source signals, testing whether relevance-driven personalization outperforms a single best message.

**Current state:** All homepage visitors see the same hero regardless of their role, industry, or stage in the buying process. Embark serves four distinct personas (CFO, COO, CIO/CTO, CHRO/CPO) with different primary challenges, but the homepage speaks to none of them specifically. The persona messaging grid has detailed per-persona lead messages that have never been deployed.
**Baseline:** 6,673 sessions/mo, 59.5% bounce, 0% CVR
**Test Feasibility:** Depends on segment identification accuracy and per-segment traffic volume. With 4 segments and ~1,668 sessions/mo each (if evenly distributed), individual segment testing requires larger effect sizes or longer durations. Consider starting with 2 segments (CFO vs. all others).
**Proposed change:** For visitors identifiable by UTM parameters, paid campaign source, or referral path, serve a hero variant matched to their likely persona. CFO-segment visitors see: "Your finance team is stretched. Our Big 4 Alumni advisors close the gap." COO-segment visitors see operations-focused messaging. Unidentifiable visitors see the baseline hero from Experiment #4.

> **Before:** Single hero for all visitors: "High-impact consulting for growing companies" (or whatever wins from Experiment #4)
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

### 11. Persona-Based Navigation Paths

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

### 12. Finance Function Readiness Assessment

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
**What a loss teaches:** Professional services buyers may prefer human qualification over self-service tools, or the assessment may feel too generic to be useful. Would suggest the classification problem is better solved by persona-based navigation (Experiment #11) than by an interactive tool.

---

## Sequencing Rationale

The roadmap starts with three Quick Wins to build organizational confidence in testing and establish baseline conversion data on currently zero-converting pages. Experiment #1 (Objection Preemption) tests whether proactively addressing the non-CPA objection influences conversion on high-intent pages, teaching Embark how to handle their most structural positioning challenge in web copy. Experiments #2 (Team Page) and #3 (Offices Page) add conversion mechanisms to high-engagement pages that currently capture zero leads. These are low-risk, high-ease implementations that establish whether evaluation-stage pages generate leads when given the opportunity. They also produce baseline CTA click-through data that informs what conversion rates to expect when adding CTAs to service and industry pages (Experiments #6 and #7).

The Strategic Bets build on Quick Win learnings. Experiment #4 (Homepage Hero Overhaul) is the highest-impact test in the roadmap. It should run after Quick Wins establish testing process and internal buy-in, because a carousel removal and above-fold restructuring requires broader stakeholder alignment than adding a content block. If the hero overhaul wins, it validates differentiation-led messaging as Embark's web strategy, informing every downstream experiment. If it loses, the loss interpretation drives a fundamentally different direction: either the differentiation-led framing is wrong, or the proof metrics don't resonate, both of which reshape subsequent tests. Experiment #5 (Contact Page Paid Alignment) can run in parallel with #4 since it targets different traffic on a different page. Experiment #6 (Service Page Differentiation) should run after the homepage messaging is validated so it can extend the proven approach, rather than guessing which messaging direction to take. Experiment #7 (Industry Pages) follows the same template as #6 and should run concurrently or immediately after, applying service page learnings to vertical-specific content.

The Explorations are sequenced by dependency and infrastructure requirements. Experiment #8 (Returning Visitor Experience) can run once audience segmentation exists in the testing platform, which is also a prerequisite for Experiment #5. Experiment #9 (Blog Content) is independent and can run at any time via pre/post measurement, but has the lowest impact ceiling. Experiment #10 (Segment Personalization) only makes sense after Experiment #4 proves which baseline messaging works. You need a validated default before you can test whether persona-specific variants outperform it. Experiment #11 (Persona Navigation) is the most structural change in the roadmap and should only proceed if Experiment #6 reveals persona-specific engagement patterns on service pages. Experiment #12 (Assessment Tool) is the longest build and should wait until positioning fundamentals are validated across the site.

Cross-tier dependencies: Quick Win results (#2, #3) establish baseline CTA conversion rates for zero-converting pages, directly informing the conversion projections for #6 and #7. Experiment #4's result informs both #6 (messaging direction) and #10 (baseline for personalization). Experiment #1 is independent of other experiments and its learning (does proactive objection handling work in web copy?) applies broadly. Experiment #8 (returning visitors) shares infrastructure requirements with #5 (audience targeting in testing platform).

---

## What's Not Here (and Why)

### Patterns Evaluated and Excluded

**Homepage content offer for unready visitors.** Evaluated and rejected. The hypothesis was to add a mid-funnel content download offer to the homepage for visitors not ready to "Talk to an advisor." However, the homepage carousel already promotes downloadable templates in slides 2 and 3 (controller transition template, external audit preparation guide). These are content offers prominently placed above the fold, and they are not converting: the homepage has 0% CVR despite the carousel templates being visible to all 6,673 monthly visitors. Adding another content offer to a page where content offers are already failing is not a valid hypothesis. The real question is why the existing content offers don't convert, which is addressed by Experiment #4 (replacing the carousel entirely with differentiation-led messaging).

**Pricing transparency.** Embark's pricing model is inherently variable: project-based, retainer, interim, and fractional engagements with scope-dependent pricing. No public pricing page exists. Competitors in this space also don't publish pricing. For project-based consulting where deal sizes depend on engagement scope, duration, and team composition, publishing price ranges risks either scaring qualified prospects (high anchor) or attracting unqualified ones (low anchor). Not recommended until competitive dynamics change.

**Form field reduction.** The current field count on the /contact form could not be confirmed from available context. If the form has 5+ fields, reducing to name, email, and company is a strong test. Recommendation: audit the /contact form structure, then evaluate. Session recording analysis would provide baseline drop-off data by field.

**Long-form vs. short-form page testing.** Page scroll depth and content length could not be confirmed. Enhanced measurement (scroll events) is currently disabled, so the baseline data needed to evaluate this pattern does not exist.

**Value-before-commitment sequencing.** Embark sells consulting services, which are inherently difficult to "preview" before commitment. Unlike SaaS products with interactive demos, consulting value is demonstrated through credentials and case studies. The assessment tool (Experiment #12) is the closest applicable variant of this pattern.

**Comparison-mode intervention.** GA4 data shows pages/session averaging 1.06-1.37, indicating most visitors view 1-2 pages per session. No significant deep-browsing segment exists that would benefit from session-depth-triggered offers.

### Patterns Skipped Due to Missing Data

**CTA click-through optimization and element engagement drop-off.** No element-level interaction data is available. Enhanced measurement (click events) has been disabled. Re-enabling would unlock CTA click-through analysis and carousel engagement decay data, enabling two additional experiment patterns.

**Form optimization (field reduction and multi-step).** Form field count, structure, and per-field abandonment data are unknown. A site audit or session recording analysis would provide the baseline needed to evaluate these patterns.

### Infeasible at Current Traffic

**Happy Works page: Is the existing form converting, and can it convert better?** The /happy-works page (352 sessions per 90 days, ~117 sessions/mo, 25.3% bounce, 107s avg engagement) is one of the most engaging pages on the site. It houses Embark's strongest differentiator (Happy Works philosophy with NPS 93, 9% attrition, revenue growth trajectory) and has a form at the bottom of the page. The performance profile does not include conversion data for this page, so it is unknown whether the form generates any submissions. The testable question is whether culture-page visitors who are deeply engaged (107s avg, low bounce) can be converted through form optimization, contextual proof placement, or a different offer framing. At 117 sessions/mo, A/B testing is impractical. Suggested approach: first, instrument the form to confirm whether it fires form_submit or a dedicated event, and measure current conversion rate. If the form is converting, optimize via pre/post. If it is not, test a different offer framing (e.g., "See how Happy Works translates to client outcomes" with a case study CTA instead of or alongside the form) via pre/post analysis over 60-90 days.

### Just-Do-It Fixes (Not Experiments)

These items should be implemented directly. They are not hypotheses requiring A/B testing because the correct action is clear:

- **Update NPS from 87 to 93 on the main site.** HubSpot landing pages already show the confirmed figure. The main site displays a stale number.
- **Re-enable enhanced measurement in GA4.** Scroll, click, and file_download events dropped to zero in the current period. This data is essential for engagement analysis across all experiments.
- **Add a download CTA to /13-week-cash-flow-forecast-model-template-best-practices.** This blog post (586 sessions/mo, 52.7% bounce) discusses a template that has a dedicated download page converting at 12.66%. Visitors likely can't find the actual download. Add a prominent link.
- **Gate the career path guide for Big 4 CPAs.** /resources/guides/the-career-path-guide-for-big-4-cpas (443 sessions, 55.8% bounce) sits in the Resources group (6.55% avg CVR) but converts at ~0%. Unlike template pages with download gates, this guide has no visible conversion mechanism. Add an email gate consistent with other resource pages.
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
- **Non-CFO personas are inferred.** COO, CIO/CTO, and CHRO persona definitions are based on website service descriptions and job norms, not buyer interviews or sales data. Affects: Experiments #10 (Segment Personalization) and #11 (Persona Navigation), where persona accuracy directly determines messaging relevance. Action: interview 2-3 buyers in non-CFO roles to validate or revise persona definitions.
- **"Right-sized flexibility" value theme has weak proof.** Only Level 2 testimonial evidence supports this theme. Multiple competitors offer similar engagement flexibility. Affects: any experiment using flexibility as a differentiating claim. Action: collect engagement model data (average project duration, contract structure statistics, cost comparisons to Big 4 alternatives).
- **Competitive landscape confidence is 2.** Limited by single-page extractions for several competitors (Accordion, CFGI, Opportune, Forvis Mazars) and no pricing data across competitors. Affects: Experiment #6 (Service Page Differentiation), where differentiation effectiveness depends on competitive accuracy. Action: deeper competitive research on Riveron, Accordion, and CFGI service positioning and pricing signals.
- **Team page audience composition unknown.** /team receives 4,217 sessions/90 days with high engagement, but the visitor mix (buyers vs. job seekers vs. competitors vs. employees) is unknown. Affects: Experiment #2 (Team Page Conversion Path) -- if most visitors are non-buyers, the conversion opportunity is smaller than the traffic suggests. Action: analyze /team traffic by source/medium and cross-reference with /careers traffic patterns to estimate buyer proportion.

### Infrastructure Prerequisites

- **Audience targeting in testing platform.** Required for Experiment #5 (paid traffic variant on /contact), Experiment #8 (returning visitor experience), and Experiment #10 (segment-based hero personalization). Experiments need the ability to serve different page variants based on UTM parameters, campaign source, referral path, or visitor state (new vs. returning). Action: verify whether the current testing platform supports UTM-based, source-based, and cookie-based audience targeting.
- **Personalization infrastructure.** Required for Experiment #10 (dynamic hero content by visitor segment). Experiment needs the CMS or testing platform to support conditional content blocks. Action: evaluate whether existing CMS or FunnelEnvy's testing infrastructure can deliver dynamic hero content by visitor segment without custom development.
- **CMS navigation flexibility.** Required for Experiment #11 (persona navigation paths). The navigation restructuring requires the CMS to support adding role-based entries without major template changes. Action: assess CMS navigation capabilities and estimate development effort for adding persona-based navigation.

---
*Analysis produced by FunnelEnvy | 2026-03-12 (revised)*
*Based on positioning analysis across 5 context sources and GA4 behavioral data (65,850 sessions, 90 days)*
