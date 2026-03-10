# Handoff: Copy Phase Skill Improvements

> **Purpose:** Improve the landing page generator's Phase 2 (Copy Agent) based on a real-world comparison between AI-generated copy and a human-written draft for the same campaign.
>
> **Skill files to modify:**
> - `/home/david/.claude/skills/landing-page-generator/phases/copy.md` (primary target)
> - `/home/david/.claude/skills/landing-page-generator/agent-header.md` (if changes affect shared rules)
>
> **Do not modify:** The brief phase, design phase, QA phase, SKILL.md, or any campaign deliverables.

---

## What happened

We ran the full landing page generator pipeline for Embark's interim CFO paid search campaign. Phase 1 (Brief) produced a solid brief with 5 pillars, 12 proof points, objection handling, form strategy, and compliance rules. Phase 2 (Copy) consumed the brief and generated `copy.md`.

Separately, a human wrote a draft for the same page. We compared them.

The AI-generated copy (Draft A) won on proof density, message match, conversion architecture, objection handling, and compliance. The human draft (Draft B) surfaced three structural patterns the copy skill doesn't currently teach.

---

## Findings: What the skill gets right

These are working well and should not be changed:

1. **Proof density requirement.** The self-check requiring proof in 4+ sections produced copy with named clients, quoted humans, and quantified outcomes in 7 of 9 sections. The human draft had 3 stats and zero named proof. This is a major differentiator.

2. **Single CTA discipline.** The rule "same CTA text appears in exactly 3 locations" prevented the dual-CTA mistake the human draft made ("Talk to a Senior Advisor" + "Learn more").

3. **Message match instruction.** "If the brief has a [GAP] on ad copy, write headlines that message-match the target keywords directly" produced a hero that mirrors the search query exactly.

4. **FAQ/objection section.** The copy phase's requirement to include proof in every FAQ answer produced significantly stronger objection handling than the human draft (which had none).

5. **Compliance self-check.** Caught banned terms, em dashes, and disclaimer requirements that the human draft missed.

---

## Findings: What the skill is missing

These are patterns the human draft got right that the current copy.md instructions don't teach. Each finding includes the specific change needed.

### Finding 1: No problem-agitation section between logo bar and pillar cards

**The gap:** The current section order goes: Hero > Social Proof Bar > Problem/Solution Cards. There is no dedicated problem-agitation beat. The copy jumps from "trust us" (logo bar) to "here's how we solve it" (cards) without first making the buyer feel the weight of their problem.

**What the human draft did better:** Draft B included a full paragraph between the hero and the pillar section:

> "Executive turnover, unexpected departures, or sudden strain on the finance team can disrupt closes, reporting accuracy, audit readiness, and cash management within weeks. Permanent hiring for senior finance roles often takes months. During that time, small breakdowns compound quickly, and boards and investors rarely tolerate prolonged instability."

This agitation paragraph makes the buyer feel the cost of inaction before presenting the solution. The AI-generated copy went straight to solution cards.

**Recommended change to copy.md:**

Add a new section between Section 2 (Social Proof Bar) and Section 3 (Problem/Solution Cards):

```
**Section 2.5: Problem Agitation**
- 2-3 sentences that name the buyer's current situation and make the cost of inaction concrete.
- Frame the problem in time terms: what happens in weeks, not years. Urgency, not catastrophe.
- Do NOT introduce the solution here. This section is pain only.
- Tone: empathetic urgency, not fear-based. "This is what's happening" not "you're in trouble."
- Source: buyer trigger events and emotional state from the brief's Audience section.
- This section has no proof points. It's pure empathy and problem naming.
```

Renumber subsequent sections accordingly (Problem/Solution Cards becomes Section 4, etc.).

---

### Finding 2: No confidentiality signal anywhere in the copy

**The gap:** The current copy.md instructions never mention confidentiality, discretion, or privacy as a copy element. For high-stakes B2B services (interim executive placement, M&A advisory, audit remediation), the buyer often needs reassurance that the conversation itself is private. A CEO dealing with a CFO departure doesn't want that information broadcast.

**What the human draft did better:** Draft B's final CTA block included "Confidential conversations" as a reassurance bullet. The AI-generated copy had no confidentiality signal anywhere.

**Recommended change to copy.md:**

Add to the Lightbox Form Copy section:

```
- Micro-copy should include a confidentiality signal when the brief's service line involves:
  executive transitions, leadership changes, M&A, audit issues, compliance remediation,
  or any situation the buyer might not want publicly known.
- Examples: "Confidential. No obligation." / "This conversation stays between us."
- Place below the submit button, adjacent to the "what happens next" micro-copy.
```

Also add to the self-check:

```
- [ ] If service involves executive transitions or sensitive situations: confidentiality signal present in form copy
```

---

### Finding 3: Hero lacks a scannable value prop summary (checkmarks/bullets)

**The gap:** The current hero instructions produce: headline, subheadline, CTA button, social proof line. For paid search traffic that scans in 2-3 seconds, there's no quick-scan element that summarizes the top 3 value props in a glanceable format.

**What the human draft did better:** Draft B included three checkmark bullets below the subheadline:

```
Immediate coverage for critical finance roles
Senior operators who execute, not just advise
Interim CFO leadership ready within days
```

These give the scanner three reasons to stay before they've read a single paragraph.

**Recommended change to copy.md:**

Add to Section 1 (Hero), after the subheadline instruction:

```
- Hero value bullets (3 max): Short, scannable statements that summarize the top 3 reasons
  to stay on this page. One line each. No periods. Front-load the differentiator.
  - Source from the brief's page pillars: extract the core promise of each top pillar.
  - These are NOT the pillar card headlines repeated. They are compressed value signals.
  - Format: checkmark, bullet, or plain list depending on design system.
  - Example: "Big 4 Alumni operators, not staffing temps" / "Deployed in days, not months" /
    "NPS 93 client satisfaction"
```

---

### Finding 4: "How It Works" section produces generic copy

**The gap:** The current instruction says "3 steps: clear, numbered, action-oriented. Keep each step to 1-2 sentences." The AI-generated output was:

> 1. Tell us what you need. A 15-minute call...
> 2. We match you with an operator. Big 4 Alumni...
> 3. They start working. Your interim leader embeds...

This is generic enough to describe any consulting firm. No step includes a differentiating detail specific to the company or service.

**Recommended change to copy.md:**

Replace the How It Works instruction with:

```
**Section 6: How It Works**
- Include by default (not optional). Buyers comparing providers need to understand the process.
- 3 steps: clear, numbered, action-oriented.
- CRITICAL: Each step must include one differentiating detail that a competitor could not
  say. Generic process steps ("tell us what you need, we'll match you, they start") add
  no value. Differentiate by naming:
  - Matching criteria (e.g., "matched by industry, complexity, and situation type")
  - Speed commitment (e.g., "initial candidates within 48 hours")
  - Credential filter (e.g., "every candidate has 10+ years and Big 4 background")
  - Process artifact (e.g., "you receive a transition plan before day one")
- If the brief doesn't contain differentiating process details, flag as [GAP] and ask the
  human rather than generating generic steps.
```

---

### Finding 5: No ad copy generation guidance

**The gap:** The brief for this campaign noted "Ad copy not yet written. Ads will be created to match LP messaging. Copy Agent should produce recommended ad headlines and descriptions that echo the hero." The copy agent did produce ad copy, but the copy.md skill file has no instructions for this. The agent improvised correctly, but without guardrails.

**Recommended change to copy.md:**

Add a new output section after Post-Submit Flow Copy:

```
**Recommended Ad Copy (conditional)**
- Include only when the brief's ad copy field is marked as "not yet written" or similar.
- Purpose: Give the ads team headlines and descriptions that message-match the LP hero,
  so ad-to-page continuity is guaranteed.
- Format: RSA (Responsive Search Ad) compatible.
  - 6-8 headlines (max 30 characters each)
  - 3-4 descriptions (max 90 characters each)
- Rules:
  - At least 2 headlines must include the primary target keyword verbatim.
  - At least 1 headline must include a proof metric (NPS, attrition rate, etc.).
  - Descriptions should name: trigger event, speed/credential, and proof point.
  - All ad copy must pass the same compliance checks as page copy (banned terms,
    regulatory constraints).
```

---

### Finding 6: Stat contextualization is not required

**The gap:** The self-check requires proof points but doesn't require that stats be contextualized. The human draft stated "NPS 93" and "91% consultant retention" without any benchmark. The AI-generated copy added "The consulting industry average is 27" next to NPS 93, which makes the number land. But this happened by chance, not by instruction.

**Recommended change to copy.md:**

Add to Section 4 (Quantified Proof):

```
- Every stat must include context that tells the reader why the number matters.
  A number without context is wallpaper.
  - Good: "NPS 93. The consulting industry average is 27."
  - Good: "9% consultant attrition. Half the Big 4 average."
  - Bad: "NPS 93." (So what?)
  - Bad: "91% client retention." (Is that good? Compared to what?)
- If a benchmark is available in the proof points library or context files, use it.
- If no benchmark exists, contextualize with a concrete comparison:
  time saved, dollars avoided, or what the number means for the buyer's daily experience.
```

---

### Finding 7: Problem/Solution cards hardcoded to 3

**The gap:** Section 3 says "3 cards from the brief's Page Pillars." But briefs may have more or fewer pillars. The Embark brief had 5 pillars (user explicitly chose to keep all 5). The copy agent wrote all 5, overriding the instruction. This was the right call, but it happened despite the instruction, not because of it.

**Recommended change to copy.md:**

Replace:
```
- 3 cards from the brief's Page Pillars.
```

With:
```
- One card per pillar from the brief. Default is 3 pillars. If the brief contains
  more (up to 5), write all of them. If more than 5, recommend consolidation and
  flag to the human.
- Design note: if more than 3 cards, note in the output that the design phase should
  use a layout that accommodates the count (e.g., 3+2 grid, scrolling cards, or
  alternating full-width sections for 4-5 pillars).
```

---

## Summary of all changes

| # | File | Section | Change Type |
|---|------|---------|------------|
| 1 | copy.md | Section order | Add Section 2.5: Problem Agitation between logo bar and pillar cards |
| 2 | copy.md | Lightbox Form Copy + Self-Check | Add confidentiality signal for sensitive service lines |
| 3 | copy.md | Section 1: Hero | Add hero value bullets (3 scannable statements) |
| 4 | copy.md | Section 6: How It Works | Require differentiating details per step; make non-optional |
| 5 | copy.md | New section: Recommended Ad Copy | Add conditional ad copy generation when ads aren't written yet |
| 6 | copy.md | Section 4: Quantified Proof | Require stat contextualization with benchmarks |
| 7 | copy.md | Section 3: Problem/Solution Cards | Support variable pillar count (3-5) instead of hardcoded 3 |

---

## Implementation notes

- Changes 1-7 are all to `phases/copy.md`. No changes needed to `agent-header.md`.
- The section renumbering from Change 1 (inserting Section 2.5) will cascade: current sections 3-9 become 4-10. Update all internal references.
- Change 4 makes "How It Works" non-optional. If this is too aggressive, keep it optional but add the differentiation requirement for when it IS included.
- Change 5 is conditional (only fires when brief says ads aren't written). Low risk.
- None of these changes affect the brief phase, design phase, or QA phase.
- After making changes, the self-check list should be updated to reflect the new section count and new checks (confidentiality, stat context).
