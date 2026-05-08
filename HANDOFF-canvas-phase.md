# Handoff: CIS111 Summer 2026 Canvas LMS Push Phase

**Phase:** Canvas LMS push (separate Cowork project)
**Prerequisite:** Repo phase COMPLETE (see `HANDOFF.md` and `audit/section-c-rollup.md`)
**Scope:** Stage and/or push the 12 polished CIS111 modules to Canvas, organized by Option 1 week
**Out of scope:** Any edits to module content in this repo. The repo is sealed.

---

## How to use this file

This document IS the kickoff prompt for the next Cowork session. The instructor will point a fresh Claude session at this file and say "read this and continue." Everything the next session needs to start safely is below; anything it does not have, it must surface to the instructor via AskUserQuestion before acting.

A one-line kickoff prompt is provided at the end of the file.

---

## Source of truth

GitHub repo (public): https://github.com/jor2050111/cis111-course-redesign

Local clone (instructor's workstation): the cis111-course-redesign directory under `Claude-Assistant/02-Research/GitHub-jor2050111/` in the instructor's working environment. The exact local path is environment-specific; if the path on the new session's host differs, ask the instructor for it before proceeding.

Read these in order before doing anything else:

1. `HANDOFF.md` to confirm the repo phase is complete
2. `audit/section-c-rollup.md` to see the proof that all 12 modules and 5 cross-module checks passed
3. `docs/summer-2026-addendum.md` for the term constraints and the `/canvas-import/` output convention organized by week (NOT by module)
4. `planning/summer-2026-pairing.md` for the binding Option 1 (Theme-Density) weekly schedule
5. `CLAUDE.md` for the banned-word list, the no-em-dash rule, and voice rules; all still binding for any Canvas-rendered content

The 12 polished module bodies live at:

```
modules/NN-<slug>/module-NN.md   where NN runs 01..12
```

Each module is paired with a final scorecard at `audit/module-NN-scorecard.md` documenting the polish results.

---

## Option 1 weekly schedule (binding)

| Week | Dates | Module(s) | Pairing notes |
|---|---|---|---|
| W1 | May 26 - 31 | M1 | Foundation single, partial week |
| W2 | Jun 1 - 7 | M2 + M3 | Paired (Part I close) |
| W3 | Jun 8 - 14 | M4 | Single |
| W4 | Jun 15 - 21 | M5 + M6 | Paired (stakeholder protection) |
| W5 | Jun 22 - 28 | M7 | Single |
| W6 | Jun 29 - Jul 5 | M8 | Single, July 4 light week |
| W7 | Jul 6 - 12 | M9 + M10 | Paired (rights in digital contexts) |
| W8 | Jul 13 - 19 | M11 | Single |
| W9 | Jul 20 - 25 | M12 | Capstone, partial week |

The Looking Ahead section in each module already forward-references the correct next module under this schedule (verified in C5 of the section-c rollup). Do not rewrite Looking Ahead text.

---

## Skill and known gotchas

Use the `canvas-content-rewriter` skill.

Important: that skill was pre-loaded for a different course (CIS215 QM) and uses CIS215-specific locked templates (Lab/Project, Examine Overview, QM block, ic-Table). Those templates were NOT designed for CIS111. Before applying any CIS215 template verbatim to CIS111 content, surface that choice to the instructor explicitly via AskUserQuestion.

The skill's enforced rules (do not bypass):

* `application/json` PUT for Canvas API writes
* No-auto-propagate of Overview pages
* Round-trip verification on writes

---

## Open questions to resolve with the instructor before any push

Before reading any module file in detail and before making any Canvas API call, ask the instructor (Jorge Vega) via AskUserQuestion for:

1. **Canvas course ID** for CIS111 Summer 2026, plus the term/SIS identifier. The skill will not assume a CIS111 course ID; it must be supplied.
2. **Output mode.** The addendum says output goes to `/canvas-import/` organized by week. Confirm which mode is wanted:
    a. Staged Markdown or HTML files under `/canvas-import/W1/`, `/W2/`, and so on, for manual import into Canvas
    b. Live Canvas API writes via the canvas-content-rewriter skill, with round-trip verification recorded
    c. Both: stage locally first, then push live after instructor review
3. **Templates.** Whether to reuse the CIS215 locked templates verbatim, adapt them for CIS111, or design a fresh CIS111 template set. If adapting, ask the instructor to point to one or two existing CIS111 Canvas pages to anchor against.
4. **Pages to create per week.** Confirm the Canvas page structure for a standard week (for example: Week Overview, Module Reading, Skills Lab, Discussion, Quick Checks) and how paired weeks (W2, W4, W7) should differ structurally from single-module weeks.
5. **Rubrics.** Whether the Skills Lab rubric tables should be created as Canvas Rubric objects (attached to assignments) or rendered as inline content inside the page. M12 has an intentional capstone-variant rubric (Course Concept Synthesis, Writing Quality and Professional Reflection); flag this so it does not get auto-normalized to the M1-M11 standard rubric.

Do not guess any of those. Ask first.

---

## Style guardrails (still binding from CLAUDE.md)

* No em dashes anywhere in Canvas-rendered content
* Banned words: spot-on, indeed, delve, dive, embark, nuances, journey, tapestry, navigate
* Second-person voice ("you")
* Decimal section numbering preserved when content is split across multiple Canvas pages
* Heading icons preserved (🧭 🎯 📋 💭 ✅ 💡 💬 📖 ⏩) where Canvas renders them correctly; if Canvas normalizes them away, leave the heading text intact rather than re-engineering the rendering

If any rendering decision violates a guardrail, fix the decision rather than the content.

---

## What "done" looks like for this phase

Either of the following, depending on the instructor's answer to question 2 above:

* `/canvas-import/W1/` through `/canvas-import/W9/` populated with import-ready files matching the confirmed page structure, OR
* The CIS111 Canvas course populated with verified pages organized by Option 1 week, with round-trip verification results recorded for each write.

Plus a short Canvas-phase rollup doc (suggested location: `audit/canvas-phase-rollup.md`) capturing:

* What was pushed where (week-by-week inventory)
* Round-trip verification results
* Any items deferred for instructor follow-up
* Any deviations from the Option 1 schedule (none expected; flag if any)

---

## Out of scope for this session

* Editing module content in the GitHub repo. The repo phase is sealed and verified.
* Re-running Section C audits or re-polishing any module.
* Touching any other Canvas course. The pre-loaded CIS215 context is incidental; this phase is for CIS111 only.

---

## One-line kickoff prompt for the new session

> Continue the CIS111 Summer 2026 redesign Canvas LMS push phase. Read `HANDOFF-canvas-phase.md` at the repo root first; it has the full plan, the binding Option 1 weekly schedule, the Canvas template gotchas, and the five open questions to resolve with the instructor before any push.
