---
schema: performance-profile
schema_version: "2.0"
generated_by: ga4-audit
last_updated: 2026-02-24
last_updated_by: ga4-audit
confidence: 3

company: Embark
property_id: "342047065"
property_name: "Embark With Us - GA4"
date_range:
  start: "2025-11-27"
  end: "2026-02-23"
days: 90

total_sessions: 65850
total_users: 50500
device_mobile_pct: 26

top_pages:
  - path: "/"
    sessions: 20019
    bounce_rate: 59.5
    pages_per_session: 1.06
    avg_engagement_sec: 49
    failure_mode: null
  - path: "/contact"
    sessions: 4439
    bounce_rate: 63.1
    pages_per_session: 1.09
    avg_engagement_sec: 40
    failure_mode: null
  - path: "/careers/listings"
    sessions: 4413
    bounce_rate: 36.4
    pages_per_session: 1.02
    avg_engagement_sec: 121
    failure_mode: null
  - path: "/cs/c/"
    sessions: 3987
    bounce_rate: 98.0
    pages_per_session: 1.02
    avg_engagement_sec: 1
    failure_mode: null
  - path: "/team"
    sessions: 3459
    bounce_rate: 23.0
    pages_per_session: 1.15
    avg_engagement_sec: 107
    failure_mode: null

conversion_events:
  - name: form_submit
    count: 544
    classification: "heuristic"
  - name: contact_us_form_submit
    count: 53
    classification: "KEY EVENT"
  - name: newsletter_subscription
    count: 4
    classification: "heuristic"

primary_conversion_event: form_submit
primary_conversion_rate: 0.83

top_channels:
  - channel: Direct
    sessions: 35896
    bounce_rate: 85.2
  - channel: Organic Search
    sessions: 14029
    bounce_rate: 46.1
  - channel: Cross-network
    sessions: 9562
    bounce_rate: 57.1

source_page_mismatches:
  - page: "/"
    better_channel: "Organic Search"
    worse_channel: "Direct"
    gap_type: "bounce"
    better_value: 37.5
    worse_value: 74.5
  - page: "/careers/overview"
    better_channel: "Organic Social"
    worse_channel: "Direct"
    gap_type: "bounce"
    better_value: 31.9
    worse_value: 73.2
  - page: "/careers/listings"
    better_channel: "Organic Social"
    worse_channel: "Cross-network"
    gap_type: "bounce"
    better_value: 53.9
    worse_value: 78.3
  - page: "/contact"
    better_channel: "Direct"
    worse_channel: "Cross-network"
    gap_type: "conversion"
    better_value: 2.24
    worse_value: 0.42

new_vs_returning:
  new_sessions_pct: 90
  new_conversion_rate: 0.83
  returning_conversion_rate: 2.06
  returning_to_new_ratio: 0.11
  signal: acquisition_heavy

page_groups:
  - group: "Homepage"
    url_pattern: "/"
    monthly_sessions: 6673
    conversion_rate: 0.0
    bounce_rate: 59.5
    page_count: 1
  - group: "Careers"
    url_pattern: "/careers/*"
    monthly_sessions: 2584
    conversion_rate: 0.12
    bounce_rate: 29.4
    page_count: 2
  - group: "Services"
    url_pattern: "/what-we-do/*"
    monthly_sessions: 1408
    conversion_rate: 0.0
    bounce_rate: 31.6
    page_count: 13
  - group: "Team"
    url_pattern: "/team/*"
    monthly_sessions: 1406
    conversion_rate: 0.0
    bounce_rate: 25.4
    page_count: 3
  - group: "Contact"
    url_pattern: "/contact"
    monthly_sessions: 1480
    conversion_rate: 1.17
    bounce_rate: 63.1
    page_count: 1
  - group: "Resources"
    url_pattern: "/resources/*"
    monthly_sessions: 1288
    conversion_rate: 6.55
    bounce_rate: 39.2
    page_count: 9
  - group: "Industries"
    url_pattern: "/who-we-serve/*"
    monthly_sessions: 426
    conversion_rate: 0.0
    bounce_rate: 31.6
    page_count: 7

top_opportunities:
  - page: "/what-we-do/* + /who-we-serve/*"
    issue: "Service/industry pages have zero conversion path"
    formula_type: "Traffic Reallocation"
    current_metric: "0% CVR"
    target_metric: "3% capture rate"
    monthly_sessions: 1834
    estimated_monthly_impact: "large"
    action_category: "structural"
    sizing_note: "Conservatism factor 0.4, capture rate 0.03 applied. Assumes CTA addition to resource downloads. Estimate: ~22 additional conversions/month."
  - page: "/contact"
    issue: "Cross-network traffic converts at <20% of Direct rate"
    formula_type: "CVR Improvement"
    current_metric: "0.42% CVR (Cross-network)"
    target_metric: "2.24% CVR (Direct)"
    monthly_sessions: 1028
    estimated_monthly_impact: "medium"
    action_category: "messaging"
    sizing_note: "Conservatism factor 0.4. Ad-to-page messaging alignment gap likely. Estimate: ~7-8 additional conversions/month."
  - page: "/"
    issue: "Direct traffic bounces at 74.5% vs Organic Search at 37.5%"
    formula_type: "Bounce Reduction"
    current_metric: "74.5% bounce (Direct)"
    target_metric: "37.5% bounce (Organic Search)"
    monthly_sessions: 3813
    estimated_monthly_impact: "small"
    action_category: "messaging"
    sizing_note: "Conservatism factor 0.4, recovery rate 0.15. Low downstream CVR limits impact. Estimate: ~1-2 additional conversions/month. Investigate Direct traffic quality first."

traffic_adequacy: high
sampling_applied: false

comparison_period:
  start: "2025-08-29"
  end: "2025-11-26"

trends:
  sessions_change_pct: -24.8
  primary_cvr_change_pp: -2.01
  bounce_rate_change_pp: 9.0
  mobile_bounce_change_pp: 16.2

l0_available: true
l0_confidence: 4
---

## Property Overview

**Property:** Embark With Us - GA4 (properties/342047065)
**Account:** Embarkwithus (accounts/58335900)
**Industry:** Finance
**Date range:** 2025-11-27 to 2026-02-23 (90 days)
**Comparison period:** 2025-08-29 to 2025-11-26 (90 days)
**Timezone:** America/Chicago
**Currency:** USD

65,850 sessions from approximately 50,500 users over 90 days. No sampling detected. Traffic adequacy is high (>10K sessions).

**Data quality notes:** Three enhanced measurement events (scroll, click, file_download) recorded zero events in the current period despite significant volume in the prior period (36,708 scroll, 5,207 click, 645 file_download). Enhanced measurement was likely disabled during the current period. The /cs/c/ path (3,987 sessions, 98% bounce, 0.9s avg duration) is a HubSpot CTA tracking redirect, not a user-facing page. It inflates session counts and bounce rate. The (not set) landing page bucket (3,396 sessions, 97.9% bounce) and /_hcms/preview/* pages (952 sessions, ~100% bounce) are internal/system traffic.

---

## Page Performance

### Top Pages

| Page | Sessions | Users | Bounce Rate | Engagement Rate | Avg Duration (s) | Pages/Session | Failure Mode |
|------|----------|-------|-------------|-----------------|-------------------|---------------|--------------|
| / | 20,019 | 15,508 | 59.5% | 40.5% | 49 | 1.06 | null |
| /contact | 4,439 | 3,876 | 63.1% | 36.9% | 40 | 1.09 | null |
| /careers/listings | 4,413 | 2,683 | 36.4% | 63.6% | 121 | 1.02 | null |
| /cs/c/ | 3,987 | 4,071 | 98.0% | 2.0% | 1 | 1.02 | null |
| /team | 3,459 | 2,459 | 23.0% | 77.0% | 107 | 1.15 | null |
| /careers/overview | 3,339 | 2,611 | 20.2% | 79.8% | 28 | 1.10 | null |
| /offices | 1,850 | 1,281 | 29.4% | 70.6% | 106 | 1.00 | null |
| /what-we-do | 1,614 | 1,248 | 24.6% | 75.4% | 93 | 1.08 | null |
| /resources/post-merger-integration-checklist | 1,257 | 1,036 | 39.7% | 60.3% | 87 | 1.13 | null |
| /about | 1,020 | 802 | 22.9% | 77.1% | 65 | 1.12 | null |
| /resources/asc-606-revenue-recognition-template | 757 | 646 | 46.5% | 53.5% | 73 | 1.08 | null |
| /what-we-do/financial-advisory-consulting | 635 | 489 | 37.0% | 63.0% | 89 | 1.02 | null |
| /13-week-cash-flow-forecast-model-template-best-practices | 586 | 425 | 52.7% | 47.3% | 45 | 0.82 | null |
| /partners | 517 | 437 | 23.8% | 76.2% | 78 | 1.04 | null |
| /resources/guides/the-career-path-guide-for-big-4-cpas | 443 | 333 | 55.8% | 44.2% | 82 | 0.95 | null |
| /research-and-development-accounting | 441 | 394 | 81.0% | 19.0% | 46 | 0.86 | shallow_engagement |
| /resources | 438 | 302 | 24.7% | 75.3% | 133 | 1.37 | null |
| /team/paul-allen | 412 | 313 | 40.5% | 59.5% | 67 | 0.98 | null |
| /resources/13-week-cash-flow-forecast-model-template | 403 | 359 | 25.3% | 74.7% | 122 | 1.07 | null |
| /who-we-serve | 382 | 312 | 22.5% | 77.5% | 67 | 1.10 | null |

Site-wide averages: 1.34 pages/session, 69.5% bounce rate.

Failure mode thresholds: shallow_engagement = pages/session < 1.005 AND bounce > 79.5%. deep_engagement = pages/session > 2.01 AND CVR < 50% of site average.

Only /research-and-development-accounting qualifies for shallow_engagement (0.86 pages/session, 81.0% bounce). This page has high organic traffic but visitors leave immediately, suggesting a keyword-content mismatch.

### High-Bounce Pages (>50% bounce, >100 sessions)

| Page | Sessions | Bounce Rate | Engagement Rate | Notes |
|------|----------|-------------|-----------------|-------|
| /cs/c/ | 3,987 | 98.0% | 2.0% | HubSpot CTA tracking redirect. Not a user page. |
| /research-and-development-accounting | 441 | 81.0% | 19.0% | shallow_engagement. Keyword-content mismatch. |
| /contact | 4,439 | 63.1% | 36.9% | Primary conversion page. High bounce for a contact form. |
| / | 20,019 | 59.5% | 40.5% | Homepage. Worsened from 46.0% previous period (+13.5pp). |
| /resources/guides/the-career-path-guide-for-big-4-cpas | 443 | 55.8% | 44.2% | Content guide with no visible resource download conversion. |
| /methods-for-a-summary-of-misstatements-iron-curtain-vs.-rollover-approach | 272 | 55.5% | 44.5% | Blog content. No conversion path. |
| /13-week-cash-flow-forecast-model-template-best-practices | 586 | 52.7% | 47.3% | Blog post about the template. Users may not find the actual download. |

### Page Group Performance

| Group | URL Pattern | Pages | Sessions | Weighted Bounce | Weighted Engagement | Conversions (form_submit) | Group CVR |
|-------|-------------|-------|----------|-----------------|---------------------|---------------------------|-----------|
| Homepage | / | 1 | 20,019 | 59.5% | 40.5% | 0 | 0.00% |
| Careers | /careers/* | 2 | 7,752 | 29.4% | 70.6% | 9 | 0.12% |
| Services | /what-we-do/* | 13 | 4,224 | 31.6% | 68.4% | 0 | 0.00% |
| Team | /team/* | 3 | 4,217 | 25.4% | 74.6% | 0 | 0.00% |
| Contact | /contact | 1 | 4,439 | 63.1% | 36.9% | 53 | 1.19% |
| Resources | /resources/* | 9 | 3,864 | 39.2% | 60.8% | 253 | 6.55% |
| Offices | /offices | 1 | 1,850 | 29.4% | 70.6% | 0 | 0.00% |
| Industries | /who-we-serve/* | 7 | 1,277 | 31.6% | 68.4% | 0 | 0.00% |
| News | /news/* | 2 | 470 | 55.5% | 44.5% | 0 | 0.00% |
| Long Tail | various | many | ~17,738 | varies | varies | varies | varies |

Long Tail represents 26.9% of sessions, which exceeds the 10% threshold. This includes /cs/c/ (3,987 sessions), /_hcms/* (952), standalone blog posts at root level, /about (1,020), /partners (517), /happy-works (352), /privacy-policy (105), and 2,376+ additional low-traffic pages.

**Structural observation:** Services (/what-we-do) and Industries (/who-we-serve) groups have 0% CVR compared to Resources at 6.55%. Combined 5,501 sessions/90 days with no conversion path is a strategic opportunity. These pages describe Embark's offerings but provide no mechanism for content download or lead capture.

### Underperforming Pages (conversion rate <50% of group average)

Service and industry pages are not flagged individually because the entire groups convert at 0%, which is a structural gap rather than per-page underperformance. See Opportunity Sizing for impact estimates.

Within the Resources group (avg CVR 6.55%, threshold <3.28%, >200 sessions):

| Page | Group | Sessions | Page CVR | Group Avg CVR | Gap |
|------|-------|----------|----------|---------------|-----|
| /resources/guides/the-career-path-guide-for-big-4-cpas | Resources | 443 | ~0% | 6.55% | -6.55pp |
| /resources (hub) | Resources | 438 | ~0% | 6.55% | -6.55pp |

The career path guide receives significant organic traffic but has no visible download gate, unlike template pages. The /resources hub page functions as a listing/navigation page, not a download destination.

---

## Conversion Events

### Event Inventory

| Event | Count (Current) | Count (Previous) | Change | Classification | Notes |
|-------|-----------------|-------------------|--------|----------------|-------|
| form_submit | 544 | 2,483 | -78% | heuristic (conversion) | Tracks resource/content downloads. Primary MQL driver. Also fires on event registration forms. |
| contact_us_form_submit | 53 | 166 | -68% | KEY EVENT | GA4 Key Event. Fires on contact form. Previous period includes event RSVPs. |
| newsletter_subscription | 4 | 17 | -76% | heuristic (conversion) | Very low volume. |
| viewed_experiment | 11,036 | 19,504 | -43% | engagement | FunnelEnvy experiment tracking. |
| nav_dropdown_open | 5,526 | 10,048 | -45% | engagement | Navigation interaction. |
| nav_link_click | 2,204 | 3,860 | -43% | engagement | Navigation interaction. |
| form_start | 908 | 3,395 | -73% | engagement | Form interaction start. Drop mirrors form_submit decline. |
| hero_download_click | 551 | 619 | -11% | engagement | Resource download CTA click. |
| sales_optin_checkbox | 474 | 408 | +16% | engagement | Checkbox interaction during form fill. |
| slide_navigation | 388 | 91 | +327% | engagement | Hero carousel interaction. |
| cta_click | 345 | 1,067 | -68% | engagement | Generic CTA click tracking. |
| scroll | 0 | 36,708 | -100% | engagement | **Enhanced measurement disabled.** |
| click | 0 | 5,207 | -100% | engagement | **Enhanced measurement disabled.** |
| file_download | 0 | 645 | -100% | engagement | **Enhanced measurement disabled.** |
| talk_to_an_advisor_cta_click | 15 | 17 | -12% | engagement | Maps to L0 "Talk to an advisor" CTA. |
| get_in_touch_click | 10 | 4 | +150% | engagement | Contact intent signal. |
| invitee_event_type_page | 6 | 0 | new | engagement | Calendly integration. |
| filter_interaction | 4 | 0 | new | engagement | Resource filtering. |
| resource_click | 4 | 0 | new | engagement | Resource interaction. |
| trackOptanonEvent | 3 | 0 | new | engagement | Cookie consent. |

### Per-Page Conversion Funnels

**form_submit (resource downloads + event registrations)**

| Page | Sessions | Conversions | CVR |
|------|----------|-------------|-----|
| /resources/post-merger-integration-checklist | 1,257 | 81 | 6.44% |
| /resources/13-week-cash-flow-forecast-model-template | 403 | 51 | 12.66% |
| /contact | 4,439 | 53 | 1.19% |
| /resources/asc-606-revenue-recognition-template | 757 | 33 | 4.36% |
| /resources/quality-of-earnings-template | ~250 | 27 | ~10.80% |
| /resources/asc-842-lease-classification-template | ~200 | 20 | ~10.00% |
| /resources/accounting-close-checklist | ~200 | 17 | ~8.50% |

Note: The 53 form_submit events on /contact likely overlap with 52 contact_us_form_submit events (same form, two event names).

Previous period context: Event registration pages drove 665+ form_submit events (Nashville Healthcare Roundtable: 272, Bentonville CPE Day: 139, Biotechs Pickleball: 81, October Breakfast: 77, Holiday Party: 64, Dinner with Mo: 32). These events ended, which accounts for a significant portion of the 78% form_submit decline. Excluding event registrations: core resource downloads fell from ~1,818 to ~515 (-72%).

**contact_us_form_submit (KEY EVENT)**

| Page | Sessions | Conversions | CVR |
|------|----------|-------------|-----|
| /contact | 4,439 | 52 | 1.17% |
| /audit-facilitation-consulting | ~50 | 1 | ~2.00% |

Effectively a single-page conversion event. 98% of contact_us_form_submit events occur on /contact.

Site-wide CVR: 53 / 65,850 = 0.08%

### Missing Tracking Gaps

- Enhanced measurement disabled: scroll, click, file_download events report 0 in current period
- No service-specific conversion tracking: all leads funnel through /contact form or resource downloads
- No segment-specific tracking for PE-backed portfolio companies (L0's stated primary segment)
- /offices pages (1,850 sessions) have 0 conversion events despite being a consideration-stage page
- Blog content at root level (e.g., /research-and-development-accounting, /methods-for-*) has no conversion tracking

---

## Channel Performance

### By Channel Group

| Channel | Sessions | % of Total | Bounce Rate | Engagement Rate | Key Event Conv | Key Event CVR |
|---------|----------|------------|-------------|-----------------|----------------|---------------|
| Direct | 35,896 | 54.5% | 85.2% | 14.8% | 16 | 0.04% |
| Organic Search | 14,029 | 21.3% | 46.1% | 53.9% | 7 | 0.05% |
| Cross-network | 9,562 | 14.5% | 57.1% | 42.9% | 22 | 0.23% |
| Referral | 1,822 | 2.8% | 47.6% | 52.4% | 3 | 0.16% |
| Organic Social | 1,746 | 2.7% | 47.3% | 52.7% | 0 | 0.00% |
| Paid Search | 1,432 | 2.2% | 47.2% | 52.8% | 4 | 0.28% |
| Unassigned | 714 | 1.1% | 91.3% | 8.7% | 1 | 0.14% |
| Email | 615 | 0.9% | 54.0% | 46.0% | 0 | 0.00% |
| Paid Social | 141 | 0.2% | 48.2% | 51.8% | 0 | 0.00% |
| Paid Other | 74 | 0.1% | 87.8% | 12.2% | 0 | 0.00% |
| Display | 0 | 0.0% | -- | -- | 0 | -- |

Note: Key Event counts only include contact_us_form_submit. form_submit (resource downloads) is not a GA4 Key Event and requires the enrichment data below for unified conversion attribution.

**Channel observations:**
- Direct traffic dominates at 54.5% with an alarming 85.2% bounce rate (up from 69.5% previous period). This is anomalous for legitimate direct traffic and warrants investigation (bot traffic, misconfigured referral exclusions, or app/internal traffic).
- Cross-network (Google Ads) is the highest-converting channel by Key Event CVR (0.23%) despite being third by volume.
- Paid Search converts at 0.28% (highest Key Event CVR) but has relatively low volume (1,432 sessions).
- Display dropped to 0 sessions (was 230 in previous period).

### Top Sources

| Source/Medium | Channel | Sessions | Bounce Rate | Key Event Conv |
|---------------|---------|----------|-------------|----------------|
| (direct) / (none) | Direct | 35,896 | 85.2% | 16 |
| google / organic | Organic Search | 12,010 | 46.3% | 4 |
| google / cpc | Cross-network | 9,475 | 57.1% | 22 |
| bing / organic | Organic Search | 1,456 | 46.4% | 3 |
| google / cpc | Paid Search | 1,430 | 47.2% | 4 |
| linkedin.com / referral | Organic Social | 1,041 | 50.0% | 0 |
| (not set) / (not set) | Unassigned | 593 | 99.5% | 1 |
| embarkwithus.wd1.myworkdayjobs.com / referral | Referral | 355 | 45.1% | 0 |
| linkedin / social | Organic Social | 349 | 38.7% | 0 |
| email / email | Email | 304 | 53.3% | 0 |
| hs_automation / email | Email | 177 | 50.3% | 0 |
| chatgpt.com / referral | Referral | 133 | 43.6% | 1 |
| hs_email / email | Email | 131 | 59.5% | 0 |

Note: google/cpc appears under both Cross-network and Paid Search. Cross-network campaigns (Performance Max, Demand Gen) are categorized separately from standard search campaigns.

ChatGPT referral traffic (133 sessions) is notable as an emerging referral source with 43.6% bounce rate (better than site average).

---

## Device & User Segment Performance

### Device Breakdown

| Device | Sessions | % of Total | Bounce Rate | Engagement Rate | Avg Duration (s) | Pages/Session | Key Event CVR |
|--------|----------|------------|-------------|-----------------|-------------------|---------------|---------------|
| Desktop | 48,012 | 72.9% | 69.2% | 30.8% | 82 | 1.37 | 0.06% |
| Mobile | 17,329 | 26.3% | 70.5% | 29.5% | 49 | 1.27 | 0.14% |
| Tablet | 505 | 0.8% | 63.6% | 36.4% | 46 | 1.16 | 0.00% |

Previous period: Desktop 72,264 sessions (61.8% bounce), Mobile 14,912 sessions (54.3% bounce).

### Mobile vs Desktop Gap

| Metric | Desktop | Mobile | Gap | Significance |
|--------|---------|--------|-----|--------------|
| Bounce Rate | 69.2% | 70.5% | +1.3pp | Low |
| Key Event CVR | 0.06% | 0.14% | +133% (mobile higher) | Medium |
| Avg Duration | 82s | 49s | -33s | Low |
| Pages/Session | 1.37 | 1.27 | -0.10 | Low |

Mobile actually converts at a higher Key Event rate than desktop (0.14% vs 0.06%). In the previous period, mobile Key Event CVR was 0.82% (123 conversions) vs desktop at 0.06% (43 conversions). The high previous-period mobile conversion count was driven by event registration RSVPs (Nashville Healthcare Roundtable, etc.) completed on mobile devices.

[WORSENING] Mobile bounce rate increased from 54.3% to 70.5% (+16.2pp). Desktop bounce increased from 61.8% to 69.2% (+7.4pp). Both worsened, but mobile deteriorated faster.

### New vs Returning

| Segment | Sessions | % of Total | Bounce Rate | Engagement Rate | Avg Duration (s) | Unified CVR |
|---------|----------|------------|-------------|-----------------|-------------------|-------------|
| New | 57,120 | 87.8% | 70.4% | 29.6% | 58 | 0.83% |
| Returning | 6,104 | 9.4% | 52.7% | 47.3% | 245 | 2.06% |
| (not set) | 1,906 | 2.9% | 99.3% | 0.7% | 6 | 0.00% |

Unified CVR includes KEY EVENT conversions + form_submit + newsletter_subscription.

Returning:New ratio: 0.11 (6,104 returning / 57,120 new)
Signal: **acquisition_heavy**

This is a new-visitor-dominated property. Returning visitors convert at 2.5x the rate of new visitors (2.06% vs 0.83%), spend 4.2x longer (245s vs 58s), and bounce 18pp less (52.7% vs 70.4%).

Previous period: New CVR 2.83%, Returning CVR 4.59%. Both segments declined significantly. [WORSENING]

The returning-visitor bounce rate of 52.7% (up from 49.5%) suggests reasonable but declining engagement for repeat visitors. The acquisition_heavy signal reflects high paid media volume bringing first-time visitors rather than weak retention.

---

## Landing Page Performance

### Top Entry Pages

| Landing Page | Sessions | % of Entries | Bounce Rate | Engagement Rate | Key Event CVR |
|--------------|----------|--------------|-------------|-----------------|---------------|
| / | 18,442 | 28.0% | 60.7% | 39.3% | 0.11% |
| /cs/c | 3,995 | 6.1% | 97.9% | 2.1% | 0.00% |
| /contact | 3,741 | 5.7% | 72.3% | 27.7% | 0.37% |
| (not set) | 3,396 | 5.2% | 97.9% | 2.1% | 0.18% |
| /careers/listings | 1,781 | 2.7% | 65.5% | 34.5% | 0.00% |
| /team | 1,577 | 2.4% | 38.0% | 62.0% | 0.00% |
| /careers/overview | 1,553 | 2.4% | 39.9% | 60.1% | 0.00% |
| /resources/post-merger-integration-checklist | 1,058 | 1.6% | 42.0% | 58.0% | 0.09% |
| /offices | 832 | 1.3% | 48.7% | 51.3% | 0.00% |
| /resources/asc-606-revenue-recognition-template | 641 | 1.0% | 50.9% | 49.1% | 0.31% |
| /_hcms/preview/template | 639 | 1.0% | 100.0% | 0.0% | 0.00% |
| /what-we-do | 637 | 1.0% | 44.7% | 55.3% | 0.00% |
| /13-week-cash-flow-forecast-model-template-best-practices | 449 | 0.7% | 56.1% | 43.9% | 0.00% |
| /resources/guides/the-career-path-guide-for-big-4-cpas | 395 | 0.6% | 52.2% | 47.8% | 0.00% |
| /about | 365 | 0.6% | 49.0% | 51.0% | 0.27% |

### High-Bounce Entry Points (>55% bounce, top 20)

| Landing Page | Sessions | Bounce Rate | Top Source | Notes |
|--------------|----------|-------------|-----------|-------|
| /cs/c | 3,995 | 97.9% | Direct | HubSpot CTA tracking redirect. Exclude from analysis. |
| (not set) | 3,396 | 97.9% | Organic Search | Unresolved landing pages. Tracking configuration issue. |
| /_hcms/preview/template | 639 | 100.0% | Direct | Internal CMS preview. |
| /news | 245 | 83.3% | Direct | News listing page. Most traffic from Direct (226 sessions, 87.2% bounce). |
| /contact | 3,741 | 72.3% | Cross-network | Primary conversion page. 82% of landing sessions from Cross-network (3,084). |
| /what-we-do/financial-advisory-consulting | 276 | 71.7% | Direct / Cross-network | Core service page. Both channels bounce >80%. |
| /careers/listings | 1,781 | 65.5% | Organic Search | Career listings. Bounce varies by channel (Organic Social 53.9% vs Cross-network 78.3%). |
| / | 18,442 | 60.7% | Direct | Homepage. Direct traffic (11,438 sessions) bounces at 74.5%. |
| /13-week-cash-flow-forecast-model-template-best-practices | 449 | 56.1% | Cross-network | Blog post about template. Users may not find the download page. |

### Source x Landing Page Mismatches

| Landing Page | Better Channel | Worse Channel | Metric | Better Value | Worse Value | Gap |
|--------------|---------------|---------------|--------|-------------|-------------|-----|
| / | Organic Search | Direct | Bounce | 37.5% | 74.5% | 37.0pp |
| /careers/overview | Organic Social | Direct | Bounce | 31.9% | 73.2% | 41.3pp |
| /careers/listings | Organic Social | Cross-network | Bounce | 53.9% | 78.3% | 24.4pp |
| /contact | Direct | Cross-network | Bounce | 87.6% | 71.8% | 15.8pp |
| /contact | Direct | Cross-network | Conversion | 2.24% | 0.42% | <50% ratio |

The homepage mismatch (37.0pp bounce gap between Organic Search and Direct) is the largest. 11,438 Direct sessions at 74.5% bounce vs 4,305 Organic Search sessions at 37.5% bounce suggests either low-quality Direct traffic (bots, misattributed) or that organic visitors have clearer intent.

The /contact conversion mismatch is critical: Cross-network drives 3,084 sessions to /contact but converts at only 0.42% (unified) vs Direct at 2.24%. The paid campaign messaging likely doesn't align with the contact page experience. Cross-network accounts for 82% of /contact landing sessions.

---

## Opportunity Sizing

| Page | Issue | Formula | Impact Bucket | Action Category | Note |
|------|-------|---------|---------------|-----------------|------|
| /what-we-do/* + /who-we-serve/* | Service/industry pages: 0% CVR, no conversion path | Traffic Reallocation | **large** | structural | Conservatism 0.4, capture rate 0.03. ~1,834 monthly sessions with zero conversion mechanism. Adding resource download CTAs or content offers could yield ~22 additional conversions/month. |
| /contact | Cross-network CVR (0.42%) vs Direct CVR (2.24%) | CVR Improvement | **medium** | messaging | Conservatism 0.4. ~1,028 monthly Cross-network sessions to /contact. Ad-to-page messaging alignment gap. Estimate: ~7-8 additional conversions/month. |
| / | Direct traffic bounces at 74.5% vs Organic Search at 37.5% | Bounce Reduction | **small** | messaging | Conservatism 0.4, recovery rate 0.15. ~3,813 monthly Direct sessions. Low downstream CVR limits impact (~1-2 conversions/month). Investigate Direct traffic quality before optimizing. |
| /13-week-cash-flow-*-best-practices | Blog post at 56.1% bounce with no link to download page | Bounce Reduction | **small** | ux | Conservatism 0.4, recovery rate 0.10. ~150 monthly sessions. Users searching for the template land on the blog post instead of the download page. Adding a prominent download CTA could capture 1-2 conversions/month. |

---

## Key Metrics Summary

### Strengths

- **Resources group converts at 6.55% CVR** - template download pages (/resources/post-merger-integration-checklist at 6.44%, /resources/13-week-cash-flow-forecast-model-template at 12.66%) demonstrate strong content-to-MQL conversion when visitors reach the right page
- **Paid Search + Cross-network drive highest Key Event CVRs** - Paid Search at 0.28% and Cross-network at 0.23% outperform organic channels on contact form conversion, validating paid investment
- **Team and career pages show strong engagement** - /team at 23.0% bounce and /careers/overview at 20.2% bounce with 107s and 28s avg duration indicate these sections serve visitor intent well

### Weaknesses [WORSENING]

- **Site-wide bounce rate increased 9.0pp** (60.5% to 69.5%) with mobile bounce increasing 16.2pp (54.3% to 70.5%). Every device category worsened.
- **Sessions declined 24.8%** (87,582 to 65,850). Traffic is down across most channels.
- **Primary conversion rate (form_submit) collapsed from 2.84% to 0.83%** (-2.01pp, -71%). Even excluding event registrations, core resource downloads fell 72%.
- **Direct traffic (54.5% of all sessions) has 85.2% bounce rate** - up from 69.5% previous period. This anomalous pattern suggests bot traffic, tracking misconfiguration, or misattributed sessions.
- **Enhanced measurement disabled** - scroll, click, and file_download events dropped to zero, eliminating engagement signal data.

### Experiment Opportunities

- **Add conversion paths to service and industry pages** - 1,834 monthly sessions across /what-we-do/* and /who-we-serve/* with zero conversion mechanism. Adding contextual resource download CTAs (e.g., "Download our M&A Integration Checklist" on /what-we-do/m-and-a-consulting) is the highest-impact structural opportunity. Impact bucket: large.
- **Align paid campaign messaging with /contact page** - Cross-network sends 3,084 sessions/90 days to /contact at 0.42% CVR vs Direct at 2.24%. Test: match contact page headline/copy to ad creative messaging. Impact bucket: medium.
- **Investigate and clean Direct traffic** - 85.2% bounce on 35,896 sessions is not normal Direct behavior. Before optimizing the homepage, determine whether this traffic is real. Check for: bot traffic, HubSpot/internal referral leakage, mobile app WebView traffic, misconfigured CMS preview traffic.
- **Bridge blog content to resource downloads** - Pages like /13-week-cash-flow-forecast-model-template-best-practices (586 sessions, 52.7% bounce) discuss templates that have dedicated download pages. Adding a prominent download CTA could convert existing traffic.
- **Re-enable enhanced measurement** - scroll, click, and file_download data is essential for understanding engagement patterns on pages without explicit conversion events.

### Data Gaps

- Enhanced measurement (scroll, click, file_download) disabled in current period
- /cs/c/ tracking redirect inflates session count and bounce rate (~3,987 sessions/90 days, 6% of total)
- No segment-level tracking for L0-stated target segments (PE-backed, mid-market, enterprise)
- form_submit event captures both resource downloads AND event registrations indiscriminately
- No GA4 Key Event designation for form_submit (resource downloads), despite being the primary MQL driver
- (not set) landing page bucket contains 3,396 sessions (5.2%) indicating tracking gaps

---

## L0 Enrichment Notes

L0 consumed: company-identity.md (confidence: 4, generated by positioning-framework)

### Product-Line Grouping Overrides

L0's 6 core services map to /what-we-do/* pages:
- /what-we-do/financial-advisory-consulting -> Financial Reporting & Advisory (FARS)
- /what-we-do/cfo-consulting -> Office of the CFO
- /what-we-do/digital-transformation-consulting -> Digital Transformation
- /what-we-do/m-and-a-consulting -> Deal Advisory & M&A
- /what-we-do/pe-vc-portco-advisory -> PE/VC Portfolio Company Advisory
- /what-we-do/data-analytics-services -> Data Analytics & Automation

All 6 service pages have 0% conversion rate. No service-specific lead capture mechanism exists.

### Funnel Stage Mapping

| Stage | Events | Pages |
|-------|--------|-------|
| Top of Funnel (Awareness) | page_view, hero_download_click | /what-we-do/*, /who-we-serve/*, blog content |
| Mid Funnel (Consideration) | form_submit (resource download), resource_click | /resources/* template pages |
| Bottom of Funnel (Intent) | talk_to_an_advisor_cta_click, get_in_touch_click, contact_us_form_submit | /contact |

L0 states the primary CTA is "Talk to an advisor" but talk_to_an_advisor_cta_click only recorded 15 events in the current period. The "Talk to an advisor" CTA appears to be underperforming as a conversion mechanism relative to resource downloads.

### Tracking Gaps vs L0

- L0 states PE-backed portfolio companies as a primary target segment, but no audience segmentation exists in GA4 to measure segment-specific performance
- L0 mentions 26 US offices, but /offices pages (1,850 sessions) have no conversion tracking despite being a consideration-stage page for in-market buyers
- L0 lists 19 industry verticals served; /who-we-serve/* has 7 industry pages visible in top 50 but none have conversion paths
- L0 references "Happy Works" philosophy as a differentiator; /happy-works page (352 sessions, 25.3% bounce) shows good engagement but no conversion mechanism
