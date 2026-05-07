# CIS111 Summer 2026 Term Addendum

**Status:** Active for the May 26 to July 30, 2026 online term
**Authority:** Layers on top of CLAUDE.md. Where this addendum specifies something, it overrides the general guidance in CLAUDE.md for the summer 2026 term only.
**Scope:** This file aligns the existing 12-module repo with a specific summer term. It does not replace CLAUDE.md, the style guide, or the module template.

---

## Term Calendar

* **Term start:** Tuesday, May 26, 2026
* **Term end:** Thursday, July 30, 2026
* **Total term span:** 9 weeks and 3 days
* **Instructional period:** 8 weeks and 5 days
* **Finals period:** Final week of the term, reserved for capstone submission and final reflection only. No new instructional content delivered in finals week.
* **Holidays and observances within the term window:**
    * Memorial Day (Monday, May 25, 2026): falls one day before term start
    * Independence Day (Saturday, July 4, 2026): falls within Week 6, expect reduced student availability that weekend

## Module-to-Week Mapping

The repo contains 12 modules. The instructional period is 8 weeks and 5 days. A pairing decision is required because 12 modules will not fit one-per-week into the instructional period.

The pairing options are produced by a separate planning task and selected by the instructor. Once selected, record the final pairing in `/planning/summer-2026-pairing.md` and reference that file from this section.

**Constraints any pairing must satisfy:**

* Every module from the existing 12 must be covered. No module is dropped.
* Module 12 (Capstone) is the final instructional module. Final assessment may extend into finals week, but no new content is introduced after the last full instructional week.
* Week 6 carries reduced load because the July 4 holiday falls inside it. Avoid scheduling a paired-module week in Week 6.
* CLO coverage remains complete. The CLO-to-Module table in CLAUDE.md is binding.
* Paired modules in a single week share a thematic Part where possible (Part I, II, III, or IV per the existing module-structure.md).

**Scheduling math:**

The instructional period of 8 weeks 5 days = 9 academic week-slots, with Weeks 1 and 9 being partial 6-day weeks. For 12 modules in 9 week-slots:

* **3 pairs + 6 singles** = 12 modules in 9 weeks (tightest fit, no buffer)
* **4 pairs + 4 singles** = 12 modules in 8 weeks (1 buffer week reserved for capstone development)
* **5 pairs + 2 singles** = 12 modules in 7 weeks (2 buffer weeks reserved for capstone and review)

The planning task at `/planning/tasks/generate-pairing-options.md` produces a concrete version of each option for instructor review.

---

## Weekly Cadence

* **Asynchronous-first delivery.** No required synchronous sessions. Optional synchronous office hours announced separately.
* **Submission days:**
    * Discussion initial post: Friday, 11:59 PM Phoenix time
    * Peer responses, Quick Checks, Skills Lab: Sunday, 11:59 PM Phoenix time
* **Time zone reference:** Arizona uses Mountain Standard Time year-round (no daylight saving observance). All deadlines stated in Phoenix local time.
* **Feedback turnaround target:** Within 72 hours of submission.
* **Student weekly load target:** 8 to 12 hours per week (reading, activities, discussion, Skills Lab). Paired-module weeks may approach the upper bound. Standard single-module weeks land in the middle of the range. Week 6 lands at the lower bound because of the holiday.
* **Finals week:** No new content. Capstone submission and final reflection only.

---

## Module Length Targets for Summer Term

The original CLAUDE.md guidance allows variable length. For an 8-week 5-day term, length normalization matters because student capacity is constrained. Apply these targets during the polish pass:

* **Standard module:** 5,500 to 6,500 words of body content (excluding Skills Lab rubric tables and Further Reading lists)
* **Capstone (Module 12):** 6,500 to 7,500 words is acceptable due to integration scope
* **Module 1 exception:** May land as low as 5,000 words. It is the foundation module, and a shorter onboarding module is pedagogically defensible for Week 1.

**Current state at audit (word counts of `module-N.md` body):**

| Module | Current Words | Action Required |
|--------|--------------|-----------------|
| 01 | 5,097 | None (within Module 1 exception) |
| 02 | 5,317 | Light expansion to 5,500+ |
| 03 | 5,720 | None (in band) |
| 04 | 5,601 | None (in band) |
| 05 | 7,253 | Trim to 6,000-6,500 |
| 06 | 8,050 | Trim to 6,000-6,500 |
| 07 | 7,791 | Trim to 6,000-6,500 |
| 08 | 8,174 | Trim to 6,000-6,500 |
| 09 | 6,520 | None (at upper bound) |
| 10 | 6,357 | None (in band) |
| 11 | 8,515 | Trim to 6,000-6,500 |
| 12 | 6,936 | None (in capstone band) |

When trimming, preserve case studies and core ethical analysis. Cut repetition, tangential historical context, and over-explained transitions.

---

## AI-2026 Currency Pass

Module 3 anchors AI ethics. Every other module includes at least one AI touchpoint per the existing module-structure.md design. During the polish pass, verify each AI touchpoint for currency:

* No AI references frozen to events older than 2024 unless explicitly framed as historical context
* At least one current 2025 to 2026 AI ethics touchpoint per module
* AI references frame students as orchestrators and verifiers, not passive consumers, consistent with the program's stance on AI integration

---

## Skills Lab Rubric Alignment

The current module template uses a 5-point rubric across 4 criteria (Ethical Analysis, Stakeholder Consideration, Evidence and Reasoning, Writing Quality). For summer 2026, retain this structure with one alignment update: the level vocabulary (Mastery, Proficiency, Developing, Emerging, Not Evident) and criterion descriptors should match across all 12 modules. Where individual modules use slightly different language for the same level, normalize to the master template.

---

## Hand-Off to Canvas LMS Phase

This repo phase ends when the redesign acceptance rubric passes for all modules and the pairing decision is recorded. The Canvas LMS push is a separate project, handled in Cowork using the canvas-content-rewriter skill.

Output for that hand-off goes to `/canvas-import/` organized by week (matching the selected pairing), not by module. The Canvas push phase is out of scope for this addendum.

---

## What This Addendum Does Not Change

* CLAUDE.md voice, structure, MLO, decimal numbering, and heading icon rules remain authoritative
* Style guide remains authoritative for inclusive language, terminology, and formatting
* Module template remains the structural reference for every module
* CLO-to-Module mapping in CLAUDE.md remains binding
* Banned-word rules and the no-em-dash rule remain binding (the polish pass enforces them)

---

## Authority Hierarchy for the Summer Term

When in conflict, apply in this order:

1. CLAUDE.md banned-word and no-em-dash rules (always binding)
2. CLAUDE.md voice, structure, and MLO requirements
3. This summer-2026 addendum
4. docs/style-guide.md
5. templates/module-template.md
6. Original module content
