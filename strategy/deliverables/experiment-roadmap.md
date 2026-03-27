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

## Roadmap Summary

| # | Experiment | Page | Tier | I | C | E | ICE |
|---|-----------|------|------|---|---|---|-----|
| 1 | Homepage Clarity Overhaul: Differentiation-Led Messaging + Proof Strip | Homepage (/) | Quick Win | 5 | 4 | 4 | 13 |
| 2 | Contact Form Context Reinforcement | /contact | Quick Win | 4 | 4 | 5 | 13 |
| 3 | Service Page Conversion Injection | /what-we-do/* | Quick Win | 4 | 4 | 4 | 12 |
| 4 | Specificity Injection on Homepage | Homepage (/) | Strategic Bet | 4 | 4 | 5 | 13 |
| 5 | Cross-Network Ad-Message Alignment on Contact Page | /contact | Strategic Bet | 4 | 4 | 3 | 11 |
| 6 | Service Page Differentiation Injection | /what-we-do/* | Strategic Bet | 4 | 3 | 4 | 11 |
| 7 | About Page Proof Hierarchy Restructure | /about | Strategic Bet | 4 | 3 | 4 | 11 |
| 8 | Industry Page Conversion Path + Proof | /who-we-serve/* | Exploration | 3 | 3 | 4 | 10 |
| 9 | Competitive Comparison Page | New page | Exploration | 4 | 3 | 2 | 9 |
| 10 | Resource Content Bridge: Blog-to-Template CTAs | /13-week-cash-flow-*-best-practices and similar | Exploration | 2 | 3 | 5 | 10 |

---

## Quick Wins

### 1. Homepage Clarity Overhaul: Differentiation-Led Messaging + Proof Strip

**Page:** Homepage (/)
**What to test:** Replace the generic headline, subhead, and hero section with differentiation-led messaging anchored in Embark's unique culture proof, combined with a quantified proof strip immediately below the fold.

**Current state:** The homepage leads with a rotating carousel. Slide 1 headline: "High-impact consulting for growing companies." Subhead: "At Embark, we help ambitious businesses scale into their next chapter with strategic guidance and hands-on support." Two CTAs: "What we do" / "Talk to an advisor." Slides 2-3 promote downloadable templates. No quantified proof appears above the fold. The homepage has 20,019 sessions over 90 days with a 59.5% bounce rate and 0% conversion rate.

**Baseline:** 6,673 sessions/mo, 59.5% bounce, 0% CVR (no conversion mechanism on page)
**Test Feasibility:** Cannot estimate (no conversion rate baseline on this page). Use CTA click-through rate or navigation-to-contact as proxy metric. Minimum 7-day run required.

**Proposed change:** Replace the carousel with a static hero. Lead with a differentiation-anchored headline, outcome-oriented subhead, and a proof strip showing NPS 93, 9% attrition, 91% client retention, and 21x revenue growth. Single primary CTA.

> **Before:** "High-impact consulting for growing companies"
> **After:** "Big 4 Alumni advisors who stay, execute, and care"

> **Before subhead:** "At Embark, we help ambitious businesses scale into their next chapter with strategic guidance and hands-on support."
> **After subhead:** "Financial advisory and consulting backed by an NPS of 93, 9% consultant attrition, and 91% client retention. No long contracts. No bloated fees. No revolving door of junior associates."

> **Before proof:** None above the fold
> **After proof strip:** NPS 93 | 9% Attrition | 91% Client Retention | $7M to $149M Revenue | 26 US Offices

**Why this should work:** B2B buyers decide in 3-5 seconds whether a page is relevant. "High-impact consulting for growing companies" forces cognitive work -- it could describe any advisory firm. Embark's actual differentiators (quantified culture proof, hospitality framing) require reading the About page and Happy Works page to discover. Moving the NPS 93 and 9% attrition data to the first scroll eliminates this discovery cost. The carousel compounds the problem: slides 2-3 promote templates, diluting the positioning message at the highest-attention moment. A static hero with proof creates a single, differentiated first impression that no competitor can replicate.

**Target metric:** Primary: CTA click-through rate ("Talk to an advisor" clicks / homepage sessions). Secondary: bounce rate reduction. Tertiary: downstream /contact page visits originating from homepage.
**Audience:** All visitors, with particular importance for new visitors (90% of traffic)

**Scores:** Impact 5 | Confidence 4 | Ease 4
- Impact 5: Homepage is the highest-traffic page (20K sessions/90 days), addresses the scorecard's top opportunity (clarity), and the carousel replacement removes a known conversion-suppressing pattern. Worsening bounce trend (+13.5pp vs prior period) adds urgency.
- Confidence 4: Exact current copy available. Audience-messaging analysis provides specific channel adaptation for the homepage. Full performance baseline exists. Mechanism is well-validated.
- Ease 4: Copy changes plus carousel removal. Requires CMS template edit but no new infrastructure. Proof strip content already exists.

**What a win proves:** Embark's unique culture metrics (NPS, attrition, retention) are the strongest lead message for the homepage. Validates that differentiation-led positioning outperforms generic category language for financial advisory buyers. Informs all downstream page messaging -- if culture proof wins on the homepage, propagate to service pages, LinkedIn ads, and sales collateral.

**What a loss teaches:** Either (a) the target audience values category credibility ("consulting for growing companies") over culture proof, suggesting the brand isn't yet established enough to lead with unconventional positioning, or (b) the specific copy execution failed while the strategy was sound. Check micro-conversion: if proof strip engagement increased but bounces didn't decrease, the headline may need iteration rather than strategy reversal.

---

### 2. Contact Form Context Reinforcement

**Page:** /contact
**What to test:** Add value reinforcement, expectation-setting, and relevant social proof adjacent to the contact form to reduce last-moment abandonment.

**Current state:** The /contact page has 4,439 sessions with a 63.1% bounce rate and 1.17% CVR (contact_us_form_submit). The form fires 52 contact submissions over 90 days. The page has no visible value reinforcement around the form itself -- no reminder of what the visitor gets, no trust signals near the submit button, and no expectation-setting for what happens after submission. The "Talk to an advisor" CTA appears only 15 times in click tracking, suggesting the primary CTA language may not be resonating.

**Baseline:** 1,480 sessions/mo, 63.1% bounce, 1.17% CVR (contact_us_form_submit)
**Test Feasibility:** ~26 weeks at 15% MDE (2 variants, ~7,600 samples/variant). Challenging. Consider micro-conversion metric (form_start rate) for faster signal. 100 conversions/variant requires approximately 12 months at current volume -- route primary metric to form_start for feasibility purposes.

**Proposed change:** Add three reinforcement elements adjacent to the form: (1) A "What to expect" section: "A senior advisor will reach out within one business day to discuss your situation. No sales pitch. No obligation." (2) A relevant client testimonial: "Embark sends the best people, so much so that it makes us think that these people grow on trees." -- Brandon Walls, CPA, VP Controller, Ashford Hospitality Trust. (3) A proof metric strip: NPS 93 | 9% Attrition | 91% Client Retention.

**Why this should work:** At the moment of form submission, the visitor re-evaluates their decision. The /contact page currently asks for information without reinforcing what the visitor receives in return. For enterprise B2B buyers considering a financial advisory engagement, the implicit question is "Is disclosing my contact information worth the potential sales pressure?" Expectation-setting ("no sales pitch, no obligation") and a named client testimonial from a VP Controller address both the uncertainty about post-submission experience and the credibility of the firm. The proof metrics reinforce differentiation at the point of highest commitment.

**Target metric:** Primary: contact_us_form_submit rate. Secondary: form_start rate (leading indicator). Track both to distinguish initiation friction from completion friction.
**Audience:** All /contact visitors, particularly cross-network (paid) traffic which converts at only 0.42% vs direct at 2.24%.

**Scores:** Impact 4 | Confidence 4 | Ease 5
- Impact 4: The /contact page is the only meaningful bottom-of-funnel conversion point. Even modest CVR improvement on 1,480 sessions/mo directly increases qualified leads. Worsening CVR trend (-2.01pp site-wide) adds urgency.
- Confidence 4: Form context reinforcement is a well-validated pattern. Named client testimonials and specific proof points are available. The 5.3x gap between direct and cross-network CVR suggests messaging/trust gaps that reinforcement directly addresses.
- Ease 5: Copy additions adjacent to an existing form. No structural changes. Can be implemented in hours.

**What a win proves:** Post-click trust reinforcement matters for Embark's buyer profile. The proof metrics and client testimonials are effective conversion tools, not just brand assets. Informs proof placement strategy across all high-intent pages.

**What a loss teaches:** The /contact page bounce issue may be primarily traffic quality (particularly the 85.2% bounce from direct traffic) rather than page experience. If form_start improves but form_submit doesn't, the bottleneck is in the form fields themselves, not the surrounding context.

---

### 3. Service Page Conversion Injection

**Page:** /what-we-do/* (13 service pages)
**What to test:** Add contextually relevant conversion elements to service pages that currently have zero conversion paths.

**Current state:** The 13 service pages under /what-we-do/* receive 4,224 sessions over 90 days (1,408/mo) with 0% conversion rate. No form, no CTA to a resource download, no content offer, and no path to /contact is prominently surfaced. These pages describe Embark's offerings but provide no mechanism to capture visitor interest. Opportunity sizing estimates ~22 additional conversions/month if a 3% capture rate is achieved.

**Baseline:** 1,408 sessions/mo, 31.6% bounce, 0.0% CVR
**Test Feasibility:** Cannot estimate (no current CVR baseline). If targeting 3% capture rate: ~4 weeks at 15% MDE. Feasible once a conversion mechanism exists.

**Proposed change:** Add below-the-fold contextual CTAs on each service page linking to a relevant resource download. Match the resource to the service: the M&A consulting page links to the post-merger integration checklist (already converting at 6.44% on its own page); the financial advisory page links to the ASC 606 template; the Office of the CFO page links to the 13-week cash flow template. Each CTA follows the pattern: "[Service-specific pain point]? Download our [resource name]."

> **Before:** Service pages end with no conversion element.
> **After:** "Navigating a post-merger integration? Download our Post-Merger Integration Checklist -- used by finance teams at companies from $50M to $5B in revenue." [Gated download form: name, email, company]

**Why this should work:** Visitors on service pages have demonstrated interest in a specific capability. They're evaluating whether Embark can solve their problem. A contextually matched resource download converts this evaluation intent into a lead capture moment. The resource itself provides value (the visitor gets a useful tool), while the download form captures contact information for nurture. This is not a hard sell -- it's offering the logical next step. The resources already convert at 6.55% when visitors find them directly. The service pages are simply missing the bridge.

**Target metric:** Primary: form_submit rate on service pages (currently 0%). Secondary: downstream contact_us_form_submit within 30 days of resource download.
**Audience:** All service page visitors. Highest priority: /what-we-do/m-and-a-consulting (PE-backed companies in transaction) and /what-we-do/financial-advisory-consulting (635 sessions, highest individual service page traffic).

**Scores:** Impact 4 | Confidence 4 | Ease 4
- Impact 4: 1,408 monthly sessions with zero conversion is a structural gap, not a marginal optimization. The opportunity sizing identifies this as a "large" impact opportunity. Resource downloads are the primary MQL driver for Embark.
- Confidence 4: The resources already convert well on their own pages (12.66% for the cash flow template, 6.44% for the post-merger checklist). Adding a contextual bridge to high-traffic pages is a validated pattern. Full traffic baseline exists.
- Ease 4: Requires adding CTA blocks to CMS templates. Resources and gated forms already exist. Main effort is matching content to pages and creating the CTA copy.

**What a win proves:** Service pages can function as mid-funnel conversion points, not just informational dead-ends. Validates that Embark's resource library is a conversion asset that should be surfaced contextually, not buried in a resource hub. Informs a site-wide strategy of matching content offers to visitor intent by page.

**What a loss teaches:** Service page visitors may have different intent than expected -- perhaps they're researching capabilities rather than evaluating solutions. If CTA impressions are high but clicks are low, the resource match may be wrong. If clicks are adequate but form completions are low, the form itself is the barrier (test form optimization next).

---

## Strategic Bets

### 4. Specificity Injection on Homepage

**Page:** Homepage (/)
**What to test:** Replace generic outcome language in the homepage body copy with specific, quantified results from published case studies.

**Current state:** Below the fold, the homepage uses generic outcome language: "drive real results," "high-impact," "scale into their next chapter." Meanwhile, Embark has 17 published case studies with quantified outcomes -- Interstate Batteries (96% reduction in bank reconciliation time), Atlas Technical Consultants (two years of audited financials prepared in 4 weeks for SEC filing), Solo Brands (successful IPO with three acquisitions integrated). None of these numbers appear anywhere in homepage copy.

**Baseline:** 6,673 sessions/mo, 59.5% bounce, 0% CVR
**Test Feasibility:** Cannot estimate (no CVR on homepage). Use engagement metrics: scroll depth or CTA click-through as proxy.

**Proposed change:** Replace the generic service description tiles with specific proof-anchored tiles. Each tile leads with a quantified case study metric, followed by the service name and a one-line description.

> **Before:** "Turn complex problems into clear solutions. Game plans into growth. That's Embark."
> **After:** "Bank reconciliation: 12 hours to 30 minutes. SEC filing: 4 weeks from a three-way merger. IPO prep: three acquisitions integrated. That's what hands-on consulting looks like."

> **Before service tile:** "Deal Advisory & M&A -- Solving complex business challenges with industry-leading expertise."
> **After service tile:** "Deal Advisory & M&A -- We prepared two years of audited financials in 4 weeks for Atlas Technical's SEC filing after a three-way merger."

**Why this should work:** Specificity signals credibility. The positioning scorecard identifies specificity as the top gap: Embark's outcomes exist in case studies but not in marketing copy. "High-impact consulting" forces the visitor to trust a claim on faith. "12 hours to 30 minutes" is verifiable and memorable. For CFOs and finance leaders evaluating advisory firms, specific operational metrics (time reduction, audit outcomes, process automation) are the proof currency. They're evaluating "can this firm actually deliver?" not "does this firm have nice copy?"

**Target metric:** Primary: CTA click-through rate and engagement with service tiles. Secondary: bounce rate.
**Audience:** All visitors, particularly CFO persona (primary buyer).

**Scores:** Impact 4 | Confidence 4 | Ease 5
- Impact 4: Addresses the scorecard's top gap (specificity). Homepage is highest traffic. But separated from Experiment 1 because this targets body copy, not ATF -- different page zone, different mechanism.
- Confidence 4: Exact case study metrics available from published case studies. Before copy is directly observed. Specificity-over-vagueness is one of the most validated CRO principles.
- Ease 5: Pure copy changes. Swap existing text for case study metrics. No structural or design changes.

**What a win proves:** Quantified case study outcomes are more effective positioning copy than generic aspirational language. Validates that specificity -- not just clarity -- drives engagement for Embark's buyer profile. Creates a playbook: every service page, ad, and sales asset should lead with a specific metric.

**What a loss teaches:** Either the specific metrics chosen don't resonate with the homepage audience (too operational, not strategic enough for C-suite visitors), or the homepage audience is too top-of-funnel for proof to matter yet. Segment by traffic source: if organic visitors respond but paid don't, the issue is awareness-stage mismatch, not content quality.

**Dependency note:** This experiment should run after Experiment 1 (Homepage Clarity Overhaul) wins or loses. The headline sets the positioning frame; specificity in body copy supports it. Running specificity injection under a generic headline tests specificity in a hostile context.

---

### 5. Cross-Network Ad-Message Alignment on Contact Page

**Page:** /contact
**What to test:** Create a paid-traffic variant of the /contact page with headline and context matched to the ad creative that drives cross-network (Google Ads) traffic.

**Current state:** Cross-network (Google Ads) drives 3,084 sessions to /contact over 90 days but converts at only 0.42% CVR vs direct traffic at 2.24% -- a 5.3x gap. This is the second-largest sized opportunity in the performance data (estimated 7-8 additional conversions/month). The contact page likely shows the same generic experience regardless of how the visitor arrived. Ad-to-page messaging mismatch is the most probable explanation for the gap: the ad promises one thing, the page delivers a generic experience.

**Baseline:** 1,028 sessions/mo from cross-network to /contact, 0.42% CVR (cross-network), 2.24% CVR (direct)
**Test Feasibility:** ~18 weeks at 15% MDE targeting cross-network traffic only (2 variants, ~2,100 samples/variant). Extended. Consider unified CVR (form_submit + contact_us_form_submit) for faster signal.

**Proposed change:** For visitors arriving from Google Ads (cross-network/CPC UTM), show a modified contact page: (1) Headline that echoes the ad's promise -- if the ad targets "outsourced CFO" searches, the page headline should be "Talk to an Outsourced CFO Advisor" not the generic contact heading. (2) Reduce or remove full site navigation for paid visitors (single conversion path). (3) Add proof specific to the ad's topic (e.g., if the ad targets M&A, surface the Atlas Technical case study). Scope this variant to paid traffic only using UTM targeting.

**Why this should work:** Paid visitors arrive with a specific expectation set by the ad. Two things break that expectation: the page headline doesn't echo the ad's promise (cognitive dissonance at arrival), and full site navigation offers escape routes before the value proposition lands. The 5.3x CVR gap between direct and cross-network traffic on this page is strong evidence of message mismatch -- direct visitors arrive with intent; paid visitors arrive with an expectation that the page doesn't fulfill.

**Target metric:** Primary: contact_us_form_submit rate for cross-network traffic. Secondary: form_start rate (leading indicator).
**Audience:** Cross-network (Google Ads) visitors to /contact only.

**Scores:** Impact 4 | Confidence 4 | Ease 3
- Impact 4: The opportunity sizing estimates 7-8 additional conversions/month. Cross-network is the highest-converting channel by Key Event CVR (0.23%) but underperforms dramatically on /contact specifically.
- Confidence 4: The 5.3x CVR gap between channels on the same page is strong evidence of a correctable mismatch. Ad-message alignment is a well-validated pattern.
- Ease 3: Requires audience targeting by UTM in the testing platform, creating a variant page (or dynamic content), and understanding the actual ad creative to match. Multiple ad campaigns may need multiple variants.

**What a win proves:** The CVR gap was caused by message mismatch, not traffic quality. Ad-aligned landing experiences work for Embark's paid traffic. Creates a template for all future paid campaigns: dedicated or dynamic landing page variants matched to ad creative.

**What a loss teaches:** The gap may be traffic quality rather than page experience -- cross-network audiences may be less qualified regardless of page messaging. If form_start improves but submit doesn't, the mismatch is in the form, not the page context. If neither metric moves, investigate whether cross-network traffic is fundamentally different in intent (brand awareness vs. lead generation campaigns).

---

### 6. Service Page Differentiation Injection

**Page:** /what-we-do/* (starting with /what-we-do/financial-advisory-consulting, 635 sessions)
**What to test:** Add Embark-specific differentiation blocks to service pages that currently read like generic category descriptions.

**Current state:** Service page copy reads generically: "Solving complex business challenges with industry-leading expertise and world-class hospitality." The word "industry-leading" breaks Embark's own voice rules (no unqualified superlatives). Competitive analysis shows high claim overlap on "strategy + execution" (shared by 6 of 7 direct competitors) and "Office of the CFO" (shared by 5). Service pages could belong to any competitor in the space. Meanwhile, Embark's unique differentiators (NPS 93, 9% attrition, hospitality framing) appear nowhere on these pages.

**Baseline:** 1,408 sessions/mo across services group, 31.6% bounce, 0.0% CVR
**Test Feasibility:** Dependent on Experiment 3 succeeding first (need a conversion mechanism to measure against). If 3% capture rate is achieved from Experiment 3: ~6 weeks at 15% MDE on the combined services group. Feasible.

**Proposed change:** On each service page, add a differentiation block after the service description. The block surfaces: (1) the specific Embark advantage for that service ("Our financial advisors have a 9% attrition rate -- half the Big 4 average. The team assigned to your engagement is the team that finishes it."), (2) a relevant case study metric from that service area, and (3) a comparison point vs. the status quo ("Traditional firms: junior associates learning on the job. Embark: Big 4 Alumni advisors who've done this before.").

> **Before:** "Solving complex business challenges with industry-leading expertise and world-class hospitality."
> **After:** "Financial Advisory from Big 4 Alumni consultants -- with 91% client retention to prove we mean it. When Interstate Batteries needed bank reconciliation overhauled, we reduced processing time from 12 hours to 30 minutes."

**Why this should work:** B2B buyers evaluating service pages are in comparison mode. They're reading 3-5 similar firms' descriptions. When every vendor says "we help you with financial reporting," none stands out. Injecting specific differentiators (9% attrition, named case study outcomes, comparison to traditional firms) gives the comparison-mode buyer a reason to remember Embark. The competitive landscape confirms that Embark's culture proof and hospitality positioning are genuinely unique -- but that uniqueness is invisible on service pages.

**Target metric:** Primary: conversion rate on service pages (post-Experiment 3 CTA implementation). Secondary: time on page and scroll depth as engagement proxies.
**Audience:** All service page visitors. Expected highest impact on visitors from organic search ("financial consulting firm," "CFO advisory services") who are actively comparing providers.

**Scores:** Impact 4 | Confidence 3 | Ease 4
- Impact 4: High claim overlap in competitive landscape means generic copy actively hurts Embark's position. Differentiation blocks address this directly on 1,408 sessions/mo.
- Confidence 3: Strong strategic basis but before copy is inferred (exact service page copy partially available). The mechanism is sound but the specific differentiator-to-service mapping hasn't been tested.
- Ease 4: Copy additions to existing pages. No structural changes. Case study content and proof points already exist.

**What a win proves:** Differentiation-led service page copy outperforms generic category language for financial advisory buyers in evaluation mode. Establishes a template for all 13 service pages.

**What a loss teaches:** Service page visitors may be too early in the funnel for differentiation to matter -- they might be at the "what does this firm do" stage rather than "how is this firm different." If so, focus differentiation on deeper pages (/about, /happy-works) where visitors have already decided the category fits.

---

### 7. About Page Proof Hierarchy Restructure

**Page:** /about
**What to test:** Restructure the About page to lead with quantified proof of capability rather than mission and values statements.

**Current state:** The /about page receives 1,020 sessions over 90 days with a 22.9% bounce rate (strong engagement). The page likely leads with narrative content about Embark's philosophy and mission. Meanwhile, the strongest proof points -- NPS 93, Deloitte Global CEO Barry Salzberg on the board, $7M to $149M revenue growth, 9% attrition -- may be buried below the fold or on separate pages (/happy-works). The About page is the 10th most-visited page on the site.

**Baseline:** 340 sessions/mo, 22.9% bounce, no CVR data for this page
**Test Feasibility:** Cannot estimate (no conversion events tracked on /about). Use downstream metric: /contact page visits originating from /about within the same session.

**Proposed change:** Restructure the About page to lead with a "proof-first" hierarchy: (1) Quantified credentials strip: NPS 93, 9% attrition, 91% retention, 26 offices, $149M revenue. (2) Institutional proof: Barry Salzberg (former Deloitte Global CEO) on board, Parthenon Capital investment. (3) Team credential highlights: Big 4 Alumni background, average years of experience. (4) Then mission/values/culture narrative. Proof first, philosophy second.

**Why this should work:** Visitors reaching the About page are evaluating trust, not seeking inspiration. They're asking "Can this company actually deliver?" Mission statements answer a question nobody on the About page is asking. Leading with proof (NPS 93, board-level institutional credibility, revenue growth trajectory) directly addresses the trust evaluation. Culture narrative and Happy Works philosophy provide context after trust is established. The About page has strong engagement (22.9% bounce, 65s avg duration) -- visitors are reading. The question is whether what they read first builds trust efficiently.

**Target metric:** Primary: downstream /contact page visits originating from /about. Secondary: click-through to /happy-works or /team from /about.
**Audience:** All /about page visitors. Likely includes referred prospects verifying company credibility after a sales conversation.

**Scores:** Impact 4 | Confidence 3 | Ease 4
- Impact 4: The About page is critical for services companies where trust evaluation drives conversion. High engagement (22.9% bounce) means visitors are reading -- the experiment optimizes what they read first. For financial advisory, team and institutional credibility are primary decision factors.
- Confidence 3: About page layout is inferred, not directly confirmed. The proof hierarchy principle is well-established in CRO, but exact current page structure is an assumption. Strong proof points exist.
- Ease 4: Primarily content reordering. Proof points already exist. No new content needed, just restructured presentation.

**What a win proves:** Proof-first positioning on trust evaluation pages accelerates the path to conversion. Validates that Embark's quantified metrics (NPS, attrition, retention) function as effective trust signals, not just marketing claims.

**What a loss teaches:** About page visitors may already be past the trust evaluation stage (perhaps post-sales-call verification where they want the narrative, not the numbers). If engagement metrics stay flat, the page may already be optimized for its actual audience. Segment by referral source to determine if the visitors are pre-sale (need trust) or post-sale (want narrative).

---

## Explorations

### 8. Industry Page Conversion Path + Proof

**Page:** /who-we-serve/* (7 industry pages)
**What to test:** Add industry-matched conversion CTAs and proof points to industry pages that currently have zero conversion paths.

**Current state:** The 7 industry pages under /who-we-serve/* receive 1,277 sessions over 90 days (426/mo) with 0% CVR and 31.6% bounce. Like service pages, these describe Embark's industry coverage without offering any mechanism for content download or lead capture. The copy reads generically: "Supporting high-growth SaaS and tech organizations with specialized guidance" -- no proof, no specificity, no differentiation.

**Baseline:** 426 sessions/mo, 31.6% bounce, 0.0% CVR
**Test Feasibility:** ~8 weeks at 15% MDE if 3% capture rate is achieved (post-CTA injection). Feasible on combined group. Individual industry pages have insufficient traffic for standalone tests.

**Proposed change:** On each industry page, add: (1) an industry-matched case study summary (e.g., energy page gets the Presidio Petroleum case study: "10x well-count increase, 6x headcount growth with only 10 office employees"), (2) a contextual resource download CTA matched to the industry's primary pain point, and (3) industry-relevant client testimonials if available.

**Why this should work:** Industry page visitors have self-selected into a specific vertical. They're asking "Does this firm understand MY industry?" Generic copy answers "we serve many industries." Industry-matched proof (named case studies, vertical-specific metrics) answers the actual question. The combination of proof and a conversion path transforms these pages from informational dead-ends into lead capture points.

**Target metric:** Primary: form_submit rate on industry pages. Secondary: downstream /contact visits from industry pages.
**Audience:** Industry-specific visitors. Highest priority: energy (3 case studies available: Presidio Petroleum, oil & gas E&P, energy sector streamlining) and healthcare (1 case study: leading home healthcare provider).

**Scores:** Impact 3 | Confidence 3 | Ease 4
- Impact 3: Lower traffic than service pages (426/mo vs 1,408/mo). Impact is real but volume-limited.
- Confidence 3: Mechanism is sound but case study matching is incomplete (17 case studies across 15+ industries, but many are anonymized). Only 4 of 17 case studies have named clients. Proof matching to specific industry pages requires verification.
- Ease 4: Same implementation pattern as Experiment 3. Copy additions to existing templates.

**What a win proves:** Industry-matched proof converts better than generic industry descriptions. Creates a template for expanding industry pages with case study content.

**What a loss teaches:** Industry page visitors may be too early in the funnel (browsing, not evaluating). If engagement metrics don't change, these visitors may need an entirely different page structure (diagnostic tool, assessment) rather than a conversion CTA.

---

### 9. Competitive Comparison Page

**Page:** New page (/compare or /why-embark)
**What to test:** Create a transparent comparison page showing Embark vs. top 2-3 competitors on key evaluation criteria.

**Current state:** No comparison or "vs." page exists on Embark's site. The homepage has a "Traditional firms vs. Embark" comparison table that is the most assertive copy on the site, but it compares against a generic archetype, not named competitors. Meanwhile, competitive analysis identifies 7 direct competitors, high claim overlap (0.50 score), and three genuinely unique differentiators (Happy Works, Unmatched Hospitality, revenue growth trajectory) that no competitor can match.

**Baseline:** No existing page. Estimate initial traffic from internal links + potential paid search targeting "[Competitor] alternative" keywords.
**Test Feasibility:** Cannot estimate (new page with no traffic baseline). Pre/post analysis recommended rather than A/B test.

**Proposed change:** Create a comparison page structured around Embark's strengths: (1) lead with dimensions where Embark wins (published culture metrics, hospitality, flexibility), (2) include honest "where they're stronger" sections for credibility, (3) use the competitive positioning data: Embark NPS 93 vs. competitors who publish no satisfaction metrics; Embark 9% attrition vs. Big 4 average of 19%. Target competitors: Riveron (closest Dallas-based peer), CFGI (claims "largest independent"), CrossCountry (most similar culture positioning).

**Why this should work:** B2B buyers actively compare vendors. If Embark doesn't provide a comparison, buyers build their own from competitor websites and review platforms -- where Embark has no control over framing. A comparison page created by Embark controls the evaluation criteria: anchoring on dimensions (quantified culture metrics, published NPS, attrition data) where no competitor has comparable evidence. Honest inclusion of competitor advantages builds credibility. The competitive analysis shows Embark has genuinely unique proof -- the comparison page makes that uniqueness explicit.

**Target metric:** Primary: /contact page visits originating from comparison page. Secondary: time on page and scroll completion.
**Audience:** Mid-to-late funnel evaluators comparing advisory firms. Expected traffic sources: internal links from service pages, organic search for "[competitor] alternative" keywords, paid search.

**Scores:** Impact 4 | Confidence 3 | Ease 2
- Impact 4: B2B evaluation pages can become high-converting assets. Embark has strong, verifiable differentiators that comparison pages are designed to surface.
- Confidence 3: New page creation has higher uncertainty than optimizing existing pages. No baseline traffic. Requires ongoing maintenance as competitors change. Comparison page effectiveness depends on whether Embark's target buyers actually comparison-shop online vs. through referral networks.
- Ease 2: Requires new page creation, content development, competitor research formatting, and ongoing maintenance. Higher effort than optimizing existing pages.

**What a win proves:** Embark's quantified differentiators are compelling in direct comparison. Validates that controlling the comparison frame is valuable for financial advisory buyers. Creates a reusable asset for sales enablement.

**What a loss teaches:** Financial advisory buyers may not use vendor-created comparison pages (preferring third-party sources like G2, Clutch, or peer referrals). If traffic is low, the page exists as a sales enablement tool rather than a marketing conversion asset. Consider distributing the comparison content as a gated PDF instead.

---

### 10. Resource Content Bridge: Blog-to-Template CTAs

**Page:** /13-week-cash-flow-forecast-model-template-best-practices (586 sessions, 52.7% bounce) and similar blog/content pages
**What to test:** Add prominent download CTAs on blog posts that discuss templates Embark already offers as gated resources.

**Current state:** The blog post about the 13-week cash flow template (/13-week-cash-flow-forecast-model-template-best-practices) receives 586 sessions with 52.7% bounce -- but the actual downloadable template lives on a separate page (/resources/13-week-cash-flow-forecast-model-template) that converts at 12.66%. Visitors landing on the blog post may not find the download page. Similarly, the career path guide for Big 4 CPAs (443 sessions, 55.8% bounce) has no visible download gate. The opportunity sizing identifies this as a "small" impact opportunity (~1-2 conversions/month for the cash flow post alone).

**Baseline:** ~200 sessions/mo for cash flow blog post, 52.7% bounce, ~0% CVR
**Test Feasibility:** ~12 weeks at 15% MDE if 5% capture rate is achieved. Extended. Consider aggregating multiple blog posts for statistical power.

**Proposed change:** Add a prominent, contextual download CTA above the fold and inline within the blog post content. Format: "Download the Template: Get our 13-Week Cash Flow Forecast Model -- the same template we use with PE-backed portfolio companies. [Download Now]." Link directly to the gated download form, not to the resource listing page.

**Why this should work:** Visitors reading a blog post about a specific template have demonstrated intent -- they searched for or clicked on content about this exact topic. The conversion path currently requires the visitor to independently navigate to /resources and find the download page. Adding a direct bridge eliminates that navigation friction. The template page already converts at 12.66%, proving the content has value. The blog post is simply missing the bridge.

**Target metric:** Primary: form_submit rate on blog posts with resource bridges. Secondary: template download attribution from blog traffic.
**Audience:** Organic search visitors landing on blog content. Likely finance professionals searching for templates, checklists, and best practices.

**Scores:** Impact 2 | Confidence 3 | Ease 5
- Impact 2: Low traffic per page (~200/mo for the top blog post). Even at high capture rates, absolute conversion volume is small. Aggregate impact across multiple blog posts may be meaningful.
- Confidence 3: The mechanism is straightforward (bridge content to download), but the blog audience may be less qualified than direct template seekers. Capture rate assumption is uncertain.
- Ease 5: Adding a CTA and link to existing blog content. Trivial implementation. Can be deployed in hours across multiple posts.

**What a win proves:** Blog content is an effective top-of-funnel capture mechanism when explicitly bridged to resources. Creates a scalable pattern for all content pages.

**What a loss teaches:** Blog visitors may have a fundamentally different intent (learning, not downloading). If CTA impressions are high but clicks are near zero, the audience mismatch is too large for a CTA to bridge. Consider softer engagement mechanisms (newsletter, webinar invitations) instead.

---

## Sequencing Rationale

**Start with Experiments 1, 2, and 3 in parallel.** These target different pages (homepage, /contact, service pages) and different mechanisms (messaging clarity, trust reinforcement, conversion path creation). Running them simultaneously maximizes learning velocity without measurement interference. All three are high-confidence, high-ease tests that build organizational momentum.

**Experiment 1 (Homepage Clarity Overhaul) sets the positioning direction.** If differentiation-led messaging wins on the homepage, it validates the core strategy that informs Experiments 4, 6, and 7. If it loses, the team should pause and reconsider whether culture-proof positioning resonates with Embark's audience before propagating it to other pages.

**Experiment 4 (Specificity Injection) runs after Experiment 1, same page.** These are separate hypotheses targeting different page zones: Experiment 1 tests the headline/ATF positioning frame, Experiment 4 tests whether quantified case study metrics improve body copy engagement. Experiment 4 should only run after Experiment 1 resolves so the body copy operates under a proven headline.

**Experiment 5 (Ad-Message Alignment) runs after Experiment 2.** Both target /contact but test different mechanisms. Experiment 2 adds universal trust reinforcement. Experiment 5 creates a paid-traffic-specific experience. If Experiment 2 wins, Experiment 5 builds on the improved page experience for a specific audience. If Experiment 2 loses, Experiment 5 still has merit (the gap is channel-specific).

**Experiment 6 (Service Page Differentiation) depends on Experiment 3.** Experiment 3 adds conversion CTAs to service pages. Experiment 6 improves the page content to make those CTAs more effective. Without a conversion mechanism (Experiment 3), Experiment 6 has no metric to optimize against.

**Experiment 7 (About Page Proof Hierarchy) is independent** and can run alongside any other experiment since it targets a separate page.

**Experiments 8, 9, and 10 are Explorations** that run when bandwidth allows, after the Quick Wins and Strategic Bets have produced results. Experiment 9 (Comparison Page) has the longest creation timeline and should begin content development early, even if the launch is deferred.

**Low-traffic page prioritization:** Service pages (/what-we-do/*) support only one concurrent test at current traffic levels (1,408 sessions/mo aggregate). Experiment 3 runs first; Experiment 6 queues behind it. Similarly, industry pages (/who-we-serve/*) with 426 sessions/mo can only support one test at a time.

**Proximity-to-conversion ordering within tiers:** Within the Quick Wins tier, Experiment 2 (contact page, closest to conversion) takes priority over Experiment 1 (homepage, further from conversion) when resources force a choice. Within Strategic Bets, Experiment 5 (contact page variant) takes priority over Experiment 6 (service pages) for the same reason. However, since Experiments 1, 2, and 3 target different pages, they should run in parallel rather than sequenced by proximity.

---

## Cross-Channel Propagation Candidates

These are not scored experiments. They are contingent suggestions that become actionable only if the source experiment wins.

- If **Experiment 1** (Homepage Clarity Overhaul) wins: test the same differentiation-led headline in LinkedIn ads. Rationale: LinkedIn is a primary channel for reaching CFOs at PE-backed companies, and the "Big 4 Alumni advisors who stay, execute, and care" message can be tested as ad copy with the same mechanism (differentiation over category language).
- If **Experiment 1** wins: update the Google Search ad description to match the winning headline. Current search ad description likely uses generic category language. Rationale: ad-to-page message continuity compounds with the homepage win.
- If **Experiment 2** (Contact Form Context Reinforcement) wins: apply the same proof strip and testimonial pattern to email nurture sequences. Rationale: the trust-building mechanism at the point of conversion transfers to the point of re-engagement.
- If **Experiment 4** (Specificity Injection) wins: replace generic outcome language in sales decks and proposals with the winning case study metric format. Rationale: if quantified specificity outperforms aspirational language on the website, it likely outperforms in sales materials for the same audience.
- If **Experiment 6** (Service Page Differentiation) wins: replicate the differentiation block pattern on the Embark partner page (/partners, 517 sessions) and technology pages. Rationale: the same comparison-mode buyer visits partner and technology pages when evaluating implementation capabilities.

---

## What's Not Here (and Why)

**Form field reduction (service/industry pages).** No forms currently exist on service or industry pages (0% CVR, no conversion mechanism). Before testing form optimization, Experiment 3 must first add a form. Form optimization becomes testable only after a baseline conversion rate is established.

**Urgency and scarcity tactics.** Evaluated and suppressed. Embark serves mid-market to enterprise B2B buyers in professional services with sales cycles measured in weeks to months. Enterprise B2B buyers are 34% more likely to abandon when they perceive artificial scarcity, and 40% distrust vendors who rely on fabricated urgency. If genuine scarcity exists (limited client roster, cohort-based onboarding), frame it as a structural reality ("We maintain focused engagements to ensure senior advisor availability") rather than a pressure tactic.

**Personalization (segment-based hero, industry proof matching).** Embark serves 4 distinct personas (CFO, COO, CIO/CTO, CHRO), making personalization theoretically high-impact. However, 53% of personalization implementations harm conversion rates. Before testing personalization: (1) verify segment detection accuracy (UTM structure, reverse IP reliability), (2) confirm distinct messaging exists and has been validated per segment (Experiments 1, 4, 6 should validate base messaging first), (3) ensure traffic per segment supports statistical significance. Personalization amplifies the base experience -- resolve base experience hypotheses (Experiments 1-7) before testing personalization.

**Pricing transparency test.** Embark does not publish pricing, and no pricing page exists. Competitors also lack published pricing (project-based/retainer models with variable deal sizes). Pricing transparency is a legitimate test for SaaS companies with clear tiers, but for professional services with custom engagements ranging from one-time projects to ongoing retainers, publishing pricing requires internal stakeholder alignment and potentially changes the sales model. This is a business decision, not a CRO test.

**Navigation restructuring by persona/use case.** Evaluated but too early. Embark has 4 personas, but only the CFO persona is well-evidenced (4 testimonials from CFO-adjacent roles). COO, CIO, and CHRO personas are inferred from service descriptions with no direct evidence. Testing persona-based navigation without validated persona definitions risks optimizing for segments that don't match actual buyer behavior. Prerequisite: validate non-CFO personas through client interviews or CRM data before investing in navigation restructuring.

**Homepage carousel optimization (rather than replacement).** The carousel itself is the problem, not the slide content. Carousel elements on homepages have consistently underperformed in testing. Slide 2-3 content (template promotions) is better served as a secondary CTA or resource section below the fold, not as a rotating primary message. Experiment 1 replaces the carousel entirely rather than optimizing within a structurally weak pattern.

**Enhanced measurement re-enablement.** Scroll, click, and file_download events dropped to zero in the current period (previously 36,708 scroll events, 5,207 click events). This is a tracking configuration issue, not an experiment. Re-enabling enhanced measurement is a prerequisite action item (see Prerequisites section), not a testable hypothesis.

**Direct traffic investigation.** Direct traffic (54.5% of sessions) has an 85.2% bounce rate, up from 69.5%. This is anomalous and warrants investigation (bot traffic, misconfigured referral exclusions, internal/app traffic). Before optimizing the homepage for direct visitors, determine whether this traffic is real. This is an analytics hygiene task, not a CRO experiment.

**Return visitor login optimization.** Embark is a consulting firm, not a SaaS product. There is no logged-in experience with saved state, personalized dashboards, or streamlined workflows. Making login prominent only lifts revenue when the logged-in experience has genuine value. Without an account experience that justifies login, this pattern does not apply.

**Infeasible experiments (traffic too low for A/B testing):**
- **/happy-works page optimization** -- 352 sessions over 90 days (~117/mo). The Happy Works page has strong engagement (25.3% bounce) but insufficient traffic for A/B testing at any feasible timeline. This page is Embark's strongest positioning asset and deserves attention, but changes should be implemented directly (pre/post analysis) rather than A/B tested. Suggestion: update NPS from stale 87 to confirmed 93, add case study metrics, and monitor engagement metrics pre/post.
- **/research-and-development-accounting** -- 441 sessions, 81.0% bounce, shallow engagement. This page has a keyword-content mismatch (high organic traffic, immediate exits). The fix is editorial (rewrite to match search intent or redirect to a relevant resource), not an A/B test. Pre/post analysis recommended.

---

## If Tests Are Inconclusive

A/B tests produce inconclusive results 41-50% of the time. This is normal, not a failure. Each experiment below has a predefined response for a flat result.

**General protocol for any inconclusive test:**
1. Verify test integrity: check for tracking errors, bot traffic (especially given the anomalous 85.2% direct bounce rate), external events (holidays, PR incidents, product changes) that may have contaminated results.
2. Run the segment analysis specified below. If any segment shows statistical significance, consider deploying the variant as a personalization for that segment only.
3. Check the micro-conversion specified below. If the leading indicator improved but the macro conversion didn't, downstream friction exists. The "next test" recommendation addresses it.
4. If no signal in segments or micro-conversions: follow the "if flat" action below.
5. For experiments on pages with volatile traffic (especially homepage with 54.5% direct traffic): if the test reaches p < 0.15 but not p < 0.05, and the result aligns with the predicted direction, recommend deploying with continued monitoring and re-evaluating at 2x the original sample size. If the effect holds at 2x sample, confirm. If it reverses, revert. This applies only to well-supported hypotheses (Experiments 1-7), not Explorations.
6. Post-deployment validation: for winning variants on the homepage (which receives >30% of traffic from volatile direct sources), run a 30-day pre/post time-series comparison after deployment. Monitor traffic source composition weekly. If the dominant traffic source shifts >20% in volume or composition during validation, extend the window or re-run the test.

### Quick Wins

**Experiment 1: Homepage Clarity Overhaul**
- **Check first:** New vs. returning visitors -- if returning visitors respond but new don't, the differentiation message requires prior brand awareness to land
- **Micro-conversion:** CTA click-through rate ("Talk to an advisor" and "What we do"). If clicks increase but bounce stays flat, the messaging resonated but the post-click experience needs work
- **If segment shows signal:** Deploy differentiation-led hero for the responding segment. Keep the generic version for others while iterating on copy for the non-responding segment
- **If flat across segments:** Iterate bolder. Test a full ATF overhaul: remove the carousel, replace with video testimonial from a named CFO (e.g., Jim Forson: "Every single Embarker has been competent, enthusiastic, passionate"), combine with proof strip. If the headline change alone is flat, the content format may matter more than the copy
- **Leads to:** Experiment 4 (Specificity Injection) if this line is abandoned

**Experiment 2: Contact Form Context Reinforcement**
- **Check first:** Traffic source -- cross-network (paid) vs. direct visitors. If cross-network visitors respond but direct don't, the reinforcement addresses ad-to-page trust gaps
- **Micro-conversion:** form_start rate. If form_start improves but form_submit doesn't, the context helped initiation but the form itself is the remaining barrier
- **If segment shows signal:** Deploy reinforcement for the responding channel. Run Experiment 5 (Ad-Message Alignment) as the next test for non-responding channels
- **If flat across segments:** Move to Experiment 5. The /contact page issue may be message mismatch (channel-specific) rather than trust gaps (universal)
- **Leads to:** Experiment 5 (Cross-Network Ad-Message Alignment)

**Experiment 3: Service Page Conversion Injection**
- **Check first:** Service page type -- compare conversion rates across individual service pages. If M&A consulting converts but Digital Transformation doesn't, the resource match matters more than the CTA placement
- **Micro-conversion:** CTA click-through on service pages (clicks on the resource download CTA)
- **If segment shows signal:** Expand winning service-resource matches. Retire or replace non-converting matches
- **If flat across segments:** The service page audience may be too top-of-funnel for gated content. Test ungated content (blog links, video explainers) instead of forms. Move on to Experiment 6 (Differentiation Injection) which addresses content quality rather than conversion mechanics
- **Leads to:** Experiment 6 (Service Page Differentiation)

### Strategic Bets

**Experiment 4: Specificity Injection on Homepage**
- **Check first:** Organic vs. paid visitors. Organic visitors (research intent) may respond more strongly to specific proof; paid visitors may need the promise-to-proof match from Experiment 5
- **Micro-conversion:** Scroll depth past proof sections, click-through on service tiles
- **If segment shows signal:** Deploy specificity for responding segment. Test different proof types (operational metrics vs. growth metrics vs. named client logos) for the non-responding segment
- **If flat across segments:** Iterate bolder -- replace the entire service tile section with a case study carousel showing before/after metrics. If subtle specificity additions don't move the needle, test a fundamentally different content structure
- **Leads to:** Experiment 6 (Service Page Differentiation) -- propagate specific proof to service pages

**Experiment 5: Cross-Network Ad-Message Alignment**
- **Check first:** Individual ad campaign performance. If Performance Max converts differently than standard search campaigns, the variant needs campaign-specific messaging, not a single paid variant
- **Micro-conversion:** form_start rate for cross-network visitors specifically
- **If segment shows signal:** Create campaign-specific landing page variants (one per ad group or campaign type)
- **If flat across segments:** The CVR gap between direct and cross-network may reflect traffic quality (lower intent from display/discovery placements in Performance Max) rather than message mismatch. Consider splitting Performance Max into separate campaigns for clearer attribution. Move on to Experiment 8 (Industry Page Conversion)
- **Leads to:** Experiment 8 (Industry Page Conversion Path)

**Experiment 6: Service Page Differentiation**
- **Check first:** New vs. returning visitors on service pages. New visitors in comparison mode are the primary target; returning visitors may have already evaluated differentiation
- **Micro-conversion:** Time on page and resource download CTA click-through (from Experiment 3's conversion mechanism)
- **If flat across segments:** The differentiation blocks may not be specific enough to the individual service areas. Test a more radical approach: replace generic service descriptions entirely with case-study-led narratives for each service
- **Leads to:** Experiment 9 (Competitive Comparison Page) -- if on-page differentiation doesn't work, try a dedicated comparison format

**Experiment 7: About Page Proof Hierarchy**
- **Check first:** Referral source. Visitors from /what-we-do/* or /contact (evaluating) vs. visitors from external links (brand research) may have different proof needs
- **Micro-conversion:** Click-through to /contact or /happy-works from /about
- **If flat across segments:** The About page may already be well-optimized for its actual audience (22.9% bounce suggests strong relevance). Move on. The About page's low bounce rate means it's working -- don't fix what isn't broken
- **Leads to:** No direct successor. About page optimization is a standalone test

### Explorations

**Experiment 8: Industry Page Conversion Path**
- **Check first:** Industry page type. Compare conversion rates across energy, healthcare, technology, etc. If energy pages convert (3 available case studies) but others don't, it's a proof availability problem, not a structural one
- **Micro-conversion:** CTA click-through on industry pages
- **If flat across segments:** Move on. Industry pages may serve awareness intent only. Redirect effort to strengthening the resource library with industry-specific content
- **Leads to:** Experiment 9 (Comparison Page) -- if industry-specific proof doesn't convert on Embark's pages, try a comparison format

**Experiment 9: Competitive Comparison Page**
- **Check first:** Traffic source. Organic search visitors (searching "[competitor] alternative") vs. internal navigation visitors have different intent and baseline trust
- **Micro-conversion:** Time on page and /contact visits from comparison page
- **If flat:** The comparison page may need promotion (paid search targeting comparison keywords, internal linking from service pages) before it can generate meaningful traffic. If traffic exists and engagement is strong but downstream conversion is flat, the comparison convinced visitors but the /contact path has friction. Test pre-filling the /contact form context based on the comparison page visit
- **Leads to:** Consider gating the comparison as a downloadable PDF for lead capture

**Experiment 10: Resource Content Bridge**
- **Check first:** Content page type. Compare blog posts about templates vs. blog posts about general topics. If template-adjacent posts convert but general posts don't, expand the pattern narrowly
- **Micro-conversion:** CTA click-through on bridge elements
- **If flat:** Blog visitors may prefer reading to downloading. Move on to other opportunities. The absolute volume (~200 sessions/mo per post) makes this a low-priority optimization
- **Leads to:** No direct successor. This is the lowest-impact experiment in the roadmap

---

## Prerequisites and Data Gaps

### Missing Baseline Data

- **Enhanced measurement disabled.** Scroll, click, and file_download events dropped to zero in the current period. Re-enable enhanced measurement in GA4 immediately. Affected experiments: all (scroll depth data improves confidence in engagement-based metrics), particularly Experiments 4 and 7 where scroll depth is a key proxy metric. **Action:** Re-enable in GA4 Admin > Data Streams > Enhanced Measurement.
- **No conversion tracking on service, industry, team, about, offices, or happy-works pages.** These pages have zero conversion events despite significant traffic (combined ~10,000 sessions/90 days). Affected experiments: 3, 6, 7, 8 (all rely on downstream conversion metrics). **Action:** Implement event tracking for CTA clicks and resource download initiations on these pages. At minimum, track "talk_to_an_advisor_cta_click" on all pages where the CTA appears.
- **Direct traffic quality unknown.** 54.5% of sessions are Direct with 85.2% bounce (up from 69.5%). Before optimizing the homepage (Experiments 1 and 4), determine whether this traffic is real. **Action:** Check for bot traffic patterns, HubSpot internal referral leakage, mobile app WebView traffic, and misconfigured CMS preview traffic. Filter confirmed non-human traffic from analytics.
- **Form completion vs. initiation rates.** form_start (908 events) vs form_submit (544 events) gives a 60% completion rate overall, but per-page breakdown is not available in the current data. Affected experiments: 2, 5 (both optimize the /contact form funnel). **Action:** Set up per-page form_start and form_submit tracking in GA4 to isolate initiation vs. completion friction.
- **No segment-level tracking.** No audience segmentation exists in GA4 for PE-backed portfolio companies (stated primary segment), mid-market vs. enterprise, or industry verticals. Affected experiments: all (segment analysis in the inconclusive protocol requires this data). **Action:** Implement UTM parameter conventions for segment identification in paid campaigns. Consider reverse IP enrichment for organic traffic.

### Context Verification Needed

- **NPS discrepancy.** Main site still shows stale NPS 87 while landing pages and client confirmation say NPS 93. Affected experiments: 1, 2, 4, 7 (all use NPS 93 in proposed copy). **Action:** Update main site to reflect confirmed NPS of 93 before running experiments that reference it. Using the correct number is not an experiment -- it's a fix.
- **About page current layout.** Experiment 7 assumes the About page leads with mission/values narrative. This is inferred from site analysis but not directly confirmed. **Action:** Verify current About page structure before scoping the restructure variant.
- **Service page exact copy.** Some service page copy is available ("Solving complex business challenges with industry-leading expertise"), but exact copy for all 13 service pages is not fully extracted. Affected experiments: 6. **Action:** Capture full copy for all service pages before writing differentiation blocks.
- **Ad creative content.** Experiment 5 requires matching the /contact page to the ad creative. Current ad copy and creative are not in the available context. **Action:** Export current Google Ads campaign copy and creative assets before scoping the ad-aligned variant.

### Infrastructure Prerequisites

- **A/B testing platform with audience targeting.** Experiments 2 (channel-specific analysis), 5 (paid-only variant), and personalization prerequisites require the ability to target test variants by traffic source, device, or audience segment. **Action:** Confirm the current testing platform (FunnelEnvy is referenced in viewed_experiment events) supports UTM-based audience targeting.
- **CMS template flexibility.** Experiments 1 (carousel removal), 3 and 8 (CTA additions to templates), and 7 (content reordering) require CMS changes. **Action:** Confirm HubSpot CMS supports per-page or per-template widget insertion for service and industry page groups.
- **form_submit event reclassification.** form_submit (resource downloads) is not a GA4 Key Event, despite being the primary MQL driver (544 events vs. 53 contact_us_form_submit). This affects all experiments measuring resource download conversion. **Action:** Mark form_submit as a Key Event in GA4 to enable unified conversion reporting.

---
*Analysis produced by FunnelEnvy | 2026-03-20*
*Based on positioning analysis across 5 context sources including company research, competitive landscape, audience messaging, positioning scorecard, and 90-day GA4 performance data (65,850 sessions)*
