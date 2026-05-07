# Polish Task: Module 5 (Whistleblowing and Accountability)

**Module:** 05-whistleblowing-and-accountability
**Working file:** `modules/05-whistleblowing-and-accountability/module-05.md`
**Branch:** `polish/module-05`
**Output scorecard:** `/audit/module-05-scorecard.md`
**Authority for stop-condition:** `rubrics/redesign-acceptance.md`

---

## Why Module 5 First

Module 5 is the chosen first target for the polish loop because:

* Currently 7,253 words. Target band 5,500-6,500. This will exercise the trim-without-losing-substance pattern.
* Two CLO mappings (V and VII), so the rubric's CLO traceability check is non-trivial but not overwhelming.
* Mid-course module. Forward and backward references exist but are not at the boundary edges.
* Existing AI touchpoint is the 2021 Frances Haugen case. Currency check (B2) will require adding a 2025-2026 reference.

If the loop works on Module 5, it will work on the others.

---

## Pre-Flight

```bash
# From repo root
git checkout main
git pull
git checkout -b polish/module-05
mkdir -p audit
```

---

## Reading Order (Once, At Start of Session)

1. `CLAUDE.md` (project standards, voice, banned words, MLO format)
2. `docs/summer-2026-addendum.md` (term constraints, length targets)
3. `rubrics/redesign-acceptance.md` (the loop authority)
4. `docs/style-guide.md` (referenced from rubric criteria B7)
5. `docs/CIS111_CLOs.md` (CLO V and CLO VII full text for traceability)
6. `templates/module-template.md` (structural reference)
7. `modules/05-whistleblowing-and-accountability/module-05.md` (the file being refined)

---

## Workflow

### Step 1: Mechanical Audit (Section A)

Run all of Section A's mechanical checks against `module-05.md`. Report results in this order, with raw counts:

* A1 Em-Dash Count
* A2 Banned-Word Count (word-boundary match)
* A3 Word Count (current vs. target band 5,500-6,500)
* A4 Heading Icon Compliance
* A5 List Bullet Style (asterisks only, no hyphens)
* A6 MLO Format Compliance
* A7 Decimal Section Numbering

Output preliminary results to `/audit/module-05-scorecard.md` with FAIL items listed but not yet fixed.

### Step 2: Mechanical Fixes

For each FAIL in Section A, apply the appropriate fix:

* **A1 (em dashes):** Replace each with comma, colon, parentheses, or sentence split based on context. Do not substitute hyphen.
* **A2 (banned words):** Replace each with a context-appropriate alternative.
* **A3 (word count, this is the big one):** Trim from current 7,253 to a target of 6,000 (middle of band). Approach:
    * Identify repetitive paragraphs. Consolidate.
    * Cut tangential historical context unless it directly serves an MLO.
    * Tighten over-explained transitions and meta-commentary.
    * **Preserve in full:**
        * All case studies and stakeholder analyses
        * All Quick Checks
        * The Skills Lab and its rubric
        * The Discussion Prompt
        * MLO statements
        * The Frances Haugen narrative hook (it works)
    * **Trim aggressively in:**
        * Introductory paragraphs that restate the module purpose
        * "As you can see" or "in summary" connective tissue between sections
        * Repeated definitions of terms already defined earlier
* **A4-A7:** Apply mechanical fixes per CLAUDE.md and the rubric.

After mechanical fixes, re-run Section A. All items must PASS before proceeding.

**Commit checkpoint after Section A passes:**

```
git add modules/05-whistleblowing-and-accountability/module-05.md audit/module-05-scorecard.md
git commit -m "polish(module-05): mechanical pass (trim, banned-word check, format compliance)"
```

### Step 3: Judgment Audit (Section B)

Run all of Section B's judgment checks. For each, output one-sentence evidence (the reasoning, not just PASS/FAIL).

* B1 Schedule Consistency
* B2 AI-2026 Currency (Module 5 will likely fail B2 because the existing AI reference points to 2021; add a 2025-2026 touchpoint)
* B3 Skills Lab Rubric Vocabulary Consistency
* B4 Discussion Prompt Quality
* B5 Case Study Stakeholder Coverage
* B6 CLO Alignment Traceable (verify CLO V and CLO VII are both addressed in body content, not just referenced in MLOs)
* B7 Voice Consistency
* B8 Looking Ahead Forward Reference (currently points to Module 6; this will need updating after pairing decision lands, but for this polish pass, leave as-is and note in scorecard that B8 is provisionally PASS pending pairing)

### Step 4: Judgment Revisions

For each FAIL in Section B, revise the relevant section. Apply skills in this order:

1. `instructional-content-writing` skill for any structural or pedagogical revision
2. `humanizing-text` skill as a final pass to remove AI-flavored phrasing

Specifically for B2 (AI currency), suggested approach:

* Add a 2025-2026 touchpoint somewhere in section 5.4 (Practical Guidance) or 5.5 (Skills Lab)
* Possible angle: AI-driven internal compliance and HR-monitoring tools that can flag pre-whistleblowing patterns of behavior. The ethical question is whether such tools enable or suppress whistleblowing.
* Frame the student as an orchestrator who must verify AI compliance-tool outputs, not as a passive consumer of AI flags

After revisions, re-run Section B. If all PASS, proceed to Step 5. If any FAIL, increment the revision pass counter.

**Commit checkpoint after Section B passes:**

```
git add modules/05-whistleblowing-and-accountability/module-05.md audit/module-05-scorecard.md
git commit -m "polish(module-05): judgment pass (AI-2026 currency, voice, CLO alignment)"
```

### Step 5: Iteration Limit

* Maximum 3 revision passes total across Sections A and B
* If after 3 passes any criterion still fails, halt and write halt notes to the scorecard
* Request instructor review

### Step 6: Final Scorecard and Commit

* Update `/audit/module-05-scorecard.md` with final PASS/FAIL per criterion using the template at the end of the rubric file
* Add a Notes section explaining any non-trivial revision decisions (especially anything trimmed that was substantive)
* Final commit:

```
git add audit/module-05-scorecard.md
git commit -m "polish(module-05): final scorecard, all rubric checks pass"
```

* Do not merge to main automatically. Branch is ready for PR review.

---

## Stop Conditions

* Stop when all Section A and Section B criteria pass for `module-05.md` on a single pass
* OR stop after 3 revision passes regardless of result
* Do not proceed to other modules. This task is module-05 only.

---

## What This Task Does NOT Do

* Does not run Section C (cross-module). Section C runs after all 12 modules pass individually.
* Does not modify other modules.
* Does not modify `CLAUDE.md`, the addendum, the rubric, or the templates.
* Does not pick a pairing.
* Does not push to GitHub remote (instructor will push after PR review).
* Does not update Looking Ahead's specific module reference (waits for pairing decision).

---

## Task System Setup

Per CLAUDE.md, use the Tasks system. Create at minimum:

* Task: Read context files (rubric, addendum, CLAUDE.md, style-guide, CLOs, module-05.md)
* Task: Run Section A mechanical audit
* Task: Apply Section A fixes (depends on previous)
* Task: Re-run Section A to verify (depends on previous)
* Task: Commit Section A checkpoint
* Task: Run Section B judgment audit
* Task: Apply Section B revisions (depends on previous, may iterate)
* Task: Re-run Section B to verify
* Task: Commit Section B checkpoint
* Task: Write final scorecard and commit

Mark each Task done before moving to the next. If a revision pass is triggered, create new Tasks for that pass rather than reopening completed ones.

---

## Expected Output

1. Modified `modules/05-whistleblowing-and-accountability/module-05.md` (trimmed from ~7,250 words to ~6,000, with 2025-2026 AI touchpoint added)
2. New `/audit/module-05-scorecard.md` with all rubric criteria reported
3. Two or three commits on `polish/module-05` branch
4. Branch ready for instructor PR review

---

## Reusing This Task for Other Modules

When Module 5 is complete and reviewed, this task spec can be cloned for other modules. Search-and-replace:

* `module-05` with the target module identifier (e.g., `module-06`)
* `Whistleblowing and Accountability` with the target module title
* The Module 5 specific notes (Frances Haugen, CLO V/VII, current word count) with the target module's equivalents
* The "Why Module 5 First" section can be removed for follow-on runs

Save the cloned spec as `/planning/tasks/polish-module-NN.md` before invoking.
