# Planning Task: Generate Summer 2026 Pairing Options

**Owner:** Instructor (decision)
**Executor:** Claude Code (option generation only, no decision)
**Output file:** `/planning/summer-2026-pairing.md`

---

## Goal

Generate exactly three concrete pairing options for fitting the existing 12 CIS111 modules into the 9 academic week-slots of the summer 2026 instructional period. Output a decision-ready document for instructor review.

**Critical constraint:** Do not pick an option. Do not modify modules. Do not modify the addendum.

---

## Reading List (Read In This Order)

1. `CLAUDE.md` (project standards, including the CLO-to-Module table)
2. `docs/summer-2026-addendum.md` (term constraints, holiday calendar, pairing rules)
3. `docs/module-structure.md` (existing thematic Parts and module rationale)
4. `docs/CIS111_CLOs.md` (full CLO list for cross-checking coverage)
5. For each of the 12 modules, read only the front-matter:
    * Module title (H1)
    * The 2-3 paragraph narrative introduction
    * Module Overview block (time, prerequisites, CLOs)
    * MLOs
    * The H2 headings of the main content sections (read the headings, skim the body)

The full module bodies are not required for this task. Front-matter and section headings give enough signal for thematic and CLO-density decisions.

---

## Scheduling Math (Authoritative)

The instructional period is 8 weeks 5 days = 61 days = 9 academic week-slots:

| Week | Dates | Days | Notes |
|------|-------|------|-------|
| 1 | May 26 - May 31 | 6 (Tue-Sun) | Partial start, term-launch onboarding |
| 2 | Jun 1 - Jun 7 | 7 | Standard |
| 3 | Jun 8 - Jun 14 | 7 | Standard |
| 4 | Jun 15 - Jun 21 | 7 | Standard |
| 5 | Jun 22 - Jun 28 | 7 | Standard |
| 6 | Jun 29 - Jul 5 | 7 | Reduced load (July 4 holiday) |
| 7 | Jul 6 - Jul 12 | 7 | Standard |
| 8 | Jul 13 - Jul 19 | 7 | Standard |
| 9 | Jul 20 - Jul 25 | 6 | Partial (final instructional days) |
| Finals | Jul 26 - Jul 30 | 5 | No new content |

Module-fit math for 12 modules in 9 week-slots:

* **3 pairs + 6 singles** = 12 modules in 9 weeks (tightest fit, no buffer)
* **4 pairs + 4 singles** = 12 modules in 8 weeks (1 buffer week reserved for capstone development)
* **5 pairs + 2 singles** = 12 modules in 7 weeks (2 buffer weeks reserved for capstone and review)

These three fit-counts are the basis for the three options.

---

## Constraints (From Addendum, Binding)

* All 12 modules covered. No module dropped.
* Module 12 (Capstone) is the final instructional module.
* Week 6 is light-load (July 4 holiday). Do not schedule a paired-module week in Week 6.
* CLO coverage remains complete per the CLO-to-Module table in CLAUDE.md.
* Paired modules in a single week share a thematic Part where possible (Parts I-IV per module-structure.md).
* Module 1 may stand alone in Week 1 as foundation (encouraged but not required).

---

## Generation Heuristics

Each option uses a different strategy and a different fit-count to maximize differentiation:

### Option 1: "Theme-Density"
* **Strategy:** Pair within Parts to maintain thematic coherence
* **Fit:** 3 pairs + 6 singles (9-week tight fit)
* **Pairs to consider:** M2+M3 (Professional + Corporate Ethics, Part I); M5+M6 (Whistleblowing + Healthcare, both stakeholder-protection in Part II); M9+M10 (IP + Free Speech/Privacy, both rights-based in Parts III-IV)
* **Trade-off:** Best thematic flow. Tightest week-by-week density. No capstone buffer.

### Option 2: "Length-Balance"
* **Strategy:** Pair shortest with longest to even out weekly student load post-polish
* **Fit:** 3 pairs + 6 singles (9-week tight fit)
* **Pairs to consider:** Pair the lightest standalone with the heaviest standalone (after polish-pass word counts are forecast). Use the post-polish target of 5,500-6,500 per module to estimate weekly load.
* **Trade-off:** Smoothest student workload. May break thematic flow.

### Option 3: "Capstone-Buffer"
* **Strategy:** Use 4 pairs to free up Week 9 for capstone-only development
* **Fit:** 4 pairs + 4 singles (8-week content + 1 buffer)
* **Pairs to consider:** Concentrate pairing in Weeks 2-5 to build a capstone-development runway in Weeks 8-9. Module 12 still anchors the final week, but Week 9 becomes capstone-focused with no new module content.
* **Trade-off:** Strongest capstone preparation. Tighter early term. More pairs total.

If a fourth option emerges naturally during analysis (for example, a "5 pairs + 2 singles" option that maximizes capstone runway), document it as an Honorable Mention with the same structure but mark it as not part of the primary three.

---

## Required Output Structure

Create `/planning/summer-2026-pairing.md` with this structure:

```markdown
# CIS111 Summer 2026 Pairing Options

**Generated:** YYYY-MM-DD
**Status:** Awaiting instructor selection
**Term:** May 26 - July 30, 2026 (8 weeks 5 days instructional + 5 days finals)

## Summary Comparison

| Option | Strategy | Pairs | Singles | Buffer | Best For |
|--------|----------|-------|---------|--------|----------|
| 1 | Theme-Density | 3 | 6 | 0 | Instructor who values thematic flow |
| 2 | Length-Balance | 3 | 6 | 0 | Instructor who values even weekly load |
| 3 | Capstone-Buffer | 4 | 4 | 1 wk | Instructor who values capstone runway |

## Option 1: [Descriptive Name]

### Strategy
[One sentence]

### Pairing Decisions
For each pair, include: modules paired, rationale, combined CLOs, combined post-polish word count estimate.

### Week-by-Week Schedule
| Week | Dates | Module(s) | Theme | CLOs | Notes |
|------|-------|-----------|-------|------|-------|
| 1 | May 26 - 31 | ... | ... | ... | Partial week, onboarding |
| 2 | Jun 1 - 7 | ... | ... | ... | ... |
| ... | ... | ... | ... | ... | ... |
| 9 | Jul 20 - 25 | ... | ... | ... | Partial |

### Strengths
* [Bullet 1]
* [Bullet 2]
* [Bullet 3]

### Risks and Compromises
* [Bullet 1]
* [Bullet 2]
* [Bullet 3]

### Capstone Foreshadowing Pattern
[One paragraph: when does Module 12 work begin to be visible to students]

### Pair Justification Test
For each pair, answer in one paragraph: Why these two and not other combinations?

[Repeat sections for Option 2 and Option 3]

## Cross-Option CLO Coverage Verification

| CLO | Option 1 Module(s) | Option 2 Module(s) | Option 3 Module(s) | Coverage Confirmed |
|-----|--------------------|--------------------|--------------------|--------------------|
| I | ... | ... | ... | YES/NO |
| ... | ... | ... | ... | ... |

## Recommendation Note

This document presents three options without recommending one. Selection is an instructor decision based on cohort, prior experience teaching summer terms, and capstone scope.
```

---

## Acceptance Criteria

The planning document is complete when:

* Three distinct options are presented (not minor variations of one)
* Each option includes a complete week-by-week schedule with actual dates from the table above
* Each pair has explicit rationale (thematic, length, or capstone-runway)
* CLO coverage is verified complete for each option in the cross-option table
* Trade-offs are clearly stated for each option
* No option is presented as recommended

---

## Stop Conditions

* Stop after `/planning/summer-2026-pairing.md` is created
* Do not modify any module files
* Do not modify `CLAUDE.md`, the addendum, or the rubric
* Do not pick an option
* Wait for instructor selection before any downstream task runs

---

## Task System Setup

Per CLAUDE.md, use the Tasks system. Create at minimum:

* Task: Read context files (CLAUDE.md, addendum, module-structure, CLOs, module front-matter)
* Task: Generate Option 1 (Theme-Density)
* Task: Generate Option 2 (Length-Balance)
* Task: Generate Option 3 (Capstone-Buffer)
* Task: Cross-option CLO coverage verification
* Task: Assemble final document

Each generation task may be done in parallel after the read-context task completes.
