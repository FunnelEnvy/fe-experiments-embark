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
| 1 | Homepage H1: Outcome Language with Culture Proof | / | Quick Win | 5 | 4 | 5 | 14 |
| 2 | Homepage Proof Strip: Case Study Metrics Above Fold | / | Quick Win | 4 | 4 | 4 | 12 |
| 3 | Contact Page: Ad-to-Page Messaging Alignment | /contact | Quick Win | 4 | 4 | 4 | 12 |
| 4 | Service Pages: Contextual Resource CTAs | /what-we-do/* | Strategic Bet | 5 | 4 | 3 | 12 |
| 5 | Homepage CTA: Specific Action Language | / | Quick Win | 4 | 4 | 5 | 13 |
| 6 | Service Page Differentiation Injection | /what-we-do/financial-advisory-consulting | Strategic Bet | 4 | 3 | 4 | 11 |
| 7 | Objection Preemption: "Not a CPA Firm" Reframe | /contact, /what-we-do | Strategic Bet | 4 | 4 | 3 | 11 |
| 8 | Happy Works Page: Conversion Path Addition | /happy-works | Exploration | 2 | 3 | 4 | 9 |
| 9 | Persona-Based Navigation Paths | Site-wide navigation | Exploration | 4 | 3 | 2 | 9 |
| 10 | Segment-Based Hero Personalization | / | Exploration | 5 | 2 | 2 | 9 |

---

## Quick Wins

### 1. Homepage H1: Outcome Language with Culture Proof

**Page:** Homepage (/)
**What to test:** Replace the generic homepage headline with a differentiated, outcome-oriented headline that surfaces Embark's unique culture proof.

**Current state:** The homepage H1 reads "High-impact consulting for growing companies." This is a line any advisory firm could use. The subhead ("At Embark, we help ambitious businesses scale into their next chapter with strategic guidance and hands-on support") reinforces generic positioning. The homepage carousel rotates between this positioning slide and two resource promotions (an accounting template and an audit preparation guide), which further dilutes the first impression.

**Baseline:** ~6,700 sessions/month, 59.5% bounce rate, 0% conversion rate. Direct traffic (11,438 sessions) bounces at 74.5% vs Organic Search at 37.5%.

**Proposed change:** Replace the carousel with a single, static hero. Lead with a headline that communicates Embark's actual differentiation: the combination of Big 4 Alumni talent and a culture that retains them.

> **Before:** "High-impact consulting for growing companies"
> **After:** "Big 4 Alumni advisors who stay, execute, and care. NPS 93."

The subhead shifts from aspiration to proof:

> **Before:** "At Embark, we help ambitious businesses scale into their next chapter with strategic guidance and hands-on support."
> **After:** "9% consultant attrition. 91% client retention. 26 offices. We deploy senior financial advisors and stay until the work is done."

**Why this should work:** B2B buyers scanning above the fold decide in 3-5 seconds whether a page is relevant. "High-impact consulting" forces the visitor to do cognitive work: what kind of consulting? For whom? The proposed headline self-qualifies financial advisory buyers immediately and communicates something no competitor can claim (NPS 93). The static hero also eliminates the carousel, which currently cycles away from the positioning message within seconds to promote downloadable templates. Removing the carousel increases the dwell time on the core value proposition.

**Target metric:** Bounce rate (primary), scroll depth and /contact click-through (secondary)
**Audience:** All visitors, with particular importance for Direct traffic where the 74.5% bounce rate indicates first-impression failure

**Scores:** Impact 5 | Confidence 4 | Ease 5
Impact 5 because this is the highest-traffic page on the site (20K sessions/90 days) and the scorecard identifies Clarity as the top opportunity. Homepage bounce worsened 13.5pp vs the prior period. Confidence 4 because the before state is exact copy from the website, the after copy is adapted from the messaging analysis's channel adaptations, and traffic adequacy is high. Ease 5 because this is a text change in the CMS hero module.

**What a win proves:** Validates that Embark's culture proof (NPS, attrition, retention) is a stronger lead message than generic category language. This would inform all downstream pages, ad copy, and sales collateral: lead with the numbers, not the aspiration.
**What a loss teaches:** Suggests visitors scanning the homepage respond more to broad category framing than specific proof claims. This would indicate Embark's brand awareness is too low to lead with metrics (visitors need to understand what the company does before they care how well it does it). Pivot to testing a "category clarity first, proof second" hierarchy.

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

### 3. Contact Page: Ad-to-Page Messaging Alignment

**Page:** /contact
**What to test:** Align contact page headline and supporting copy with the messaging visitors see in paid ad campaigns (Cross-network/Google Ads).

**Current state:** Cross-network campaigns (Google Ads Performance Max, Demand Gen) drive 3,084 sessions to /contact over 90 days but convert at only 0.42% (unified CVR). Direct traffic to the same page converts at 2.24%, a 5.3x gap. This is the largest conversion gap identified in the analytics, and the /contact page is the single bottom-of-funnel conversion point for the entire site (98% of contact form submissions happen here).

**Baseline:** ~1,480 sessions/month, 63.1% bounce rate, 1.19% CVR (form_submit). Cross-network bounce is higher than Direct on this page.

**Proposed change:** Add a dynamic or A/B-tested headline on /contact that echoes the value proposition from paid campaigns. If Cross-network ads reference financial advisory, audit readiness, or CFO services, the contact page should reinforce that language rather than presenting a generic "Contact Us" experience.

> **Before:** Generic contact form with no value reinforcement specific to the ad source
> **After:** "Ready to close the gap in your finance function? Talk to an advisor who's done it for companies like yours." Add a contextual proof point near the form: "91% of clients stay with Embark year over year."

**Why this should work:** Paid visitors arrive with a specific expectation set by the ad creative. When the landing page doesn't reinforce that expectation, there's a cognitive mismatch: "Did I click the right link?" The 5.3x CVR gap between Direct (visitors who sought out the site intentionally) and Cross-network (visitors responding to ad messaging) is a textbook ad-to-page alignment failure. Matching contact page language to ad messaging reduces the expectation gap and maintains the visitor's momentum from ad click to form submission.

**Target metric:** form_submit rate on /contact for Cross-network traffic (primary), overall /contact CVR (secondary)
**Audience:** Paid traffic visitors arriving via Google Ads campaigns

**Scores:** Impact 4 | Confidence 4 | Ease 4
Impact 4 because the opportunity sizing estimates 7-8 additional conversions per month from closing this gap, and contact form submissions are the bottom-of-funnel action. Confidence 4 because the source-page mismatch data is specific and the gap is large enough to produce a measurable result. Ease 4 because this is primarily a copy change with an optional proof element, though coordinating with ad campaign messaging requires cross-team alignment.

**What a win proves:** Validates that the paid-to-page messaging gap is the primary conversion barrier for paid traffic. This learning applies to every future landing page built for paid campaigns: match the promise.
**What a loss teaches:** Suggests the conversion gap is not a messaging problem but a traffic quality problem (Cross-network campaigns may be targeting low-intent audiences). Investigate campaign targeting and audience quality before further page optimization.

---

### 5. Homepage CTA: Specific Action Language

**Page:** Homepage (/)
**What to test:** Replace vague CTA language with specific, expectation-setting action language.

**Current state:** The homepage has two CTAs: "What we do" (navigational, sends visitors to services overview) and "Talk to an advisor" (conversion intent). "Talk to an advisor" recorded only 15 clicks in 90 days across the entire site. "What we do" is navigational, not conversion-oriented. Neither CTA communicates what happens next or reduces the fear of unknown commitment.

**Baseline:** ~6,700 sessions/month. "Talk to an advisor" CTA: 15 clicks in 90 days (0.02% click rate). 0% homepage conversion rate.

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

**Page:** /what-we-do/* and /who-we-serve/* (20 pages total)
**What to test:** Add contextual resource download CTAs to service and industry pages, which currently have zero conversion mechanism.

**Current state:** Service pages (/what-we-do/*) receive 4,224 sessions per 90 days across 13 pages. Industry pages (/who-we-serve/*) receive 1,277 sessions across 7 pages. Combined: 5,501 sessions per quarter with a 0% conversion rate. These pages describe Embark's offerings but provide no mechanism for content download, newsletter signup, or any lead capture. Meanwhile, the /resources section converts at 6.55% with existing templates and guides.

**Baseline:** ~1,834 combined monthly sessions, 31.6% bounce rate, 0% CVR. This is the largest sized opportunity in the analytics: an estimated 22 additional conversions per month if a 3% capture rate is achieved with a 0.4 conservatism factor.

**Proposed change:** Add contextual resource download CTAs to each service page, matched to the page's topic. Examples:
- /what-we-do/m-and-a-consulting: "Download our Post-Merger Integration Checklist" (the checklist already exists and converts at 6.44% on its own page)
- /what-we-do/financial-advisory-consulting: "Get the ASC 606 Revenue Recognition Template"
- /what-we-do/cfo-consulting: "Download the 13-Week Cash Flow Forecast Model"
- /who-we-serve/pe-vc: "See how we helped Solo Brands complete their IPO" (case study link)

For industry pages, link to the most relevant case study by industry.

**Why this should work:** Visitors on service pages are evaluating whether Embark can solve their specific problem. They are mid-funnel: interested enough to explore services, but not ready to talk to sales (otherwise they'd be on /contact). Right now, the only next step available is "Talk to an advisor," which requires a commitment jump. A contextual resource download matches the visitor's current intent (learning and evaluation) rather than forcing a premature conversion action. The resource CTAs also create an email capture point that doesn't exist today, feeding the nurture pipeline.

**Target metric:** Resource download rate per service page (primary), overall form_submit volume (secondary)
**Audience:** Mid-funnel evaluators exploring specific service capabilities

**Scores:** Impact 5 | Confidence 4 | Ease 3
Impact 5 because this is the largest pre-sized opportunity (22 est. monthly conversions), addresses 1,834 monthly sessions with zero current conversion, and the performance data tags it as a "large" impact opportunity. Worsening site-wide CVR trend adds urgency. Confidence 4 because the resources already exist and convert well (6.55% group CVR proves the content works), and the structural gap is confirmed by analytics. Ease 3 because this requires adding CTA blocks to 20 pages and selecting the right resource for each, which is moderate design/content effort even though the resources themselves exist.

**What a win proves:** Validates the hypothesis that service page visitors will convert on contextual resource offers. This changes the site's conversion architecture: every content page becomes a lead capture point, not just /contact and /resources.
**What a loss teaches:** Suggests service page visitors are either too early in their journey (awareness, not consideration) or are evaluating competitively and don't want to exchange information yet. The next test would be ungated content offers (case study summaries, comparison data) that build consideration without requiring email capture.

---

### 6. Service Page Differentiation Injection

**Page:** /what-we-do/financial-advisory-consulting (pilot), then expand to other service pages
**What to test:** Add differentiation-specific content blocks to the highest-traffic service page, replacing generic capability descriptions with Embark-specific proof and competitive positioning.

**Current state:** The Financial Advisory and Consulting page receives 635 sessions/90 days with 37% bounce. The scorecard analysis flags service sub-pages as drifting to generic copy: "Solving complex business challenges with industry-leading expertise and world-class hospitality." "Industry-leading" is a generic superlative that breaks Embark's own voice rules. The competitive analysis shows 0.50 claim overlap on core services. Service pages read like they could belong to any of the 11 analyzed competitors.

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

**Contact page optimization (Experiment 3) runs in parallel.** It targets a different page and a specific audience segment (paid traffic), so it doesn't confound with homepage tests. The ad-to-page alignment test is also time-sensitive because the Cross-network conversion gap represents an ongoing waste of paid media budget.

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

- **Contact form field count and structure.** The form on /contact has not been directly audited for field count, field types, or form completion funnel. This prevents evaluation of form field reduction and multi-step form conversion experiments. **Action:** Audit the /contact form manually. Count fields, note types (text, dropdown, checkbox), and check for required vs. optional fields.
- **Enhanced measurement is disabled.** Scroll, click, and file_download events report zero in the current 90-day period (previously active at 36,708 scroll events, 5,207 click events, 645 file_downloads). This eliminates engagement signal data for all pages and prevents scroll depth analysis for Experiments 1, 2, and 6. **Action:** Re-enable enhanced measurement in GA4 immediately. This is not optional for running CRO experiments, as it provides the engagement data needed to interpret test results.
- **Direct traffic quality.** Direct traffic (54.5% of all sessions) has an 85.2% bounce rate (up from 69.5% prior period). This is anomalous for legitimate direct traffic. Before optimizing the homepage for Direct visitors (Experiment 1), determine whether this traffic is real. **Action:** Check for bot traffic patterns, review referral exclusion settings, audit internal/CMS preview traffic leakage (/_hcms/preview/* accounted for 952 sessions), and investigate whether HubSpot CTA redirects (/cs/c/) are inflating Direct attribution.
- **Ad campaign creative and UTM structure.** Experiments 3 (ad-to-page alignment) and 10 (segment personalization) require knowledge of current ad messaging and UTM parameter conventions. **Action:** Export current Google Ads campaign creatives and UTM parameter taxonomy.

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
