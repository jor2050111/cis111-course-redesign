# Polish Task: Module 6 (Healthcare IT Ethics)

**Module:** 06-healthcare-it-ethics
**Working file:** `modules/06-healthcare-it-ethics/module-06.md`
**Branch:** `polish/module-06`
**Output scorecard:** `/audit/module-06-scorecard.md`
**Authority for stop-condition:** `rubrics/redesign-acceptance.md`

---

## Why Module 6 Next

Module 6 is the second polish target because:

* It is M5's same-week pairing partner under the selected Option 1 (Theme-Density), Week 4. Polishing M5 and M6 in close succession keeps the paired week thematically synchronized.
* Currently 8,064 words. Target band 5,500-6,500. The trim is heavier than M5's (about 22% reduction vs M5's 11%), exercising the trim-without-losing-substance pattern at scale.
* One CLO mapping (CLO VI), so the rubric's CLO traceability check is straightforward.
* The module already has an AI Touchpoint on AI-assisted diagnostics and clinical AI bias, but contains zero 2025/2026 date references at audit time, so B2 will fail and require a current touchpoint addition.
* Strong cross-references with M5 (HIPAA appears in M5's Skills Lab MedVault scenario; M6 is where HIPAA is taught in depth). Polishing M6 right after M5 lets cross-references be tuned in real time.

---

## Pre-Flight

```bash
# From repo root
git checkout main
git pull
git checkout -b polish/module-06
mkdir -p audit
```

---

## Reading Order (Once, At Start of Session)

1. `CLAUDE.md` (project standards, voice, banned words, MLO format)
2. `docs/summer-2026-addendum.md` (term constraints, length targets, AI-2026 currency requirement)
3. `planning/summer-2026-pairing.md` (Option 1 selected; M5+M6 paired in W4)
4. `rubrics/redesign-acceptance.md` (the loop authority)
5. `docs/style-guide.md` (referenced from rubric criteria B7)
6. `docs/CIS111_CLOs.md` (CLO VI full text for traceability)
7. `templates/module-template.md` (structural reference)
8. `modules/06-healthcare-it-ethics/module-06.md` (the file being refined)
9. `audit/module-05-scorecard.md` (reference: the recently completed pair partner)

---

## Workflow

### Step 1: Mechanical Audit (Section A)

Run all of Section A's mechanical checks against `module-06.md`. Report results in this order with raw counts:

* A1 Em-Dash Count
* A2 Banned-Word Count (word-boundary match)
* A3 Word Count (current vs. target band 5,500-6,500)
* A4 Heading Icon Compliance
* A5 List Bullet Style (asterisks only)
* A6 MLO Format Compliance
* A7 Decimal Section Numbering

Output preliminary results to `/audit/module-06-scorecard.md` with FAIL items listed but not yet fixed.

### Step 2: Mechanical Fixes

For each FAIL in Section A, apply the appropriate fix:

* **A1 (em dashes):** Replace each with comma, colon, parentheses, or sentence split based on context.
* **A2 (banned words):** Replace each with a context-appropriate alternative.
* **A3 (word count, the big one):** Trim from ~8,064 to ~6,000-6,250 (mid-band, with headroom for any B2 add). Approach:
    * Identify repetitive paragraphs. Consolidate.
    * Cut tangential historical context unless it serves an MLO.
    * Tighten over-explained transitions and meta-commentary.
    * **Preserve in full:**
        * All case studies and stakeholder analyses
        * All Quick Checks
        * The Skills Lab scenario and rubric
        * The Discussion Prompt
        * MLO statements
        * The opening narrative hook
    * **Trim aggressively in:**
        * Introductory paragraphs that restate the module purpose
        * Connective tissue between sections ("As you can see...", "In summary...")
        * Repeated definitions of terms already defined earlier
        * Long historical or regulatory backstories that exceed pedagogical need
* **A4-A7:** Apply mechanical fixes per CLAUDE.md and the rubric.

After mechanical fixes, re-run Section A. All items must PASS before proceeding.

**Commit checkpoint after Section A passes:**

```
git add modules/06-healthcare-it-ethics/module-06.md audit/module-06-scorecard.md
git commit -m "polish(module-06): mechanical pass (trim, banned-word check, format compliance)"
```

### Step 3: Judgment Audit (Section B)

Run all Section B checks. For each, output one-sentence evidence.

* B1 Schedule Consistency (note: M6 is paired with M5 in W4; Module Overview should still target 4-5 hours for the M6 module on its own; the addendum says paired weeks may approach the upper student-load bound but each module remains its own pedagogical unit)
* B2 AI-2026 Currency (M6 will likely fail B2 because there are no 2025-2026 dated AI references; add a current touchpoint)
* B3 Skills Lab Rubric Vocabulary Consistency
* B4 Discussion Prompt Quality
* B5 Case Study Stakeholder Coverage
* B6 CLO Alignment Traceable (verify CLO VI is addressed in body content, not just MLOs)
* B7 Voice Consistency
* B8 Looking Ahead Forward Reference (Option 1 selected: M6 followed by M7 in W5; verify the existing forward reference points to M7 and update if not)

### Step 4: Judgment Revisions

For each FAIL in Section B, revise the relevant section. Apply skills:

1. `instructional-content-writing` for any structural or pedagogical revision
2. `humanizing-text` as a final pass to remove AI-flavored phrasing

Specifically for B2 (AI currency), suggested approach:

* Add a 2025-2026 touchpoint in section 6.4 (AI in Healthcare) covering one or more of:
    * FDA's evolving guidance on AI/ML-enabled medical devices and the 2024-2025 final framework on Predetermined Change Control Plans for adaptive AI
    * EU AI Act high-risk classification of medical AI and its 2025 phase-in
    * 2025-2026 published cases of clinical AI bias, particularly in dermatology and radiology models trained on demographically narrow data
    * AI scribing and ambient documentation tools rapidly deployed in 2024-2025 and the consent/PHI questions they raise
* Frame the student as orchestrator-verifier of clinical AI outputs, not passive consumer
* Connect the addition explicitly to the module's existing CLO VI body content

After revisions, re-run Section B. If all PASS, proceed to Step 5. If any FAIL, increment the revision pass counter.

**Commit checkpoint after Section B passes:**

```
git add modules/06-healthcare-it-ethics/module-06.md audit/module-06-scorecard.md
git commit -m "polish(module-06): judgment pass (AI-2026 currency, voice, CLO alignment)"
```

### Step 5: Iteration Limit

* Maximum 3 revision passes total across Sections A and B
* If after 3 passes any criterion still fails, halt and write halt notes to the scorecard
* Request instructor review

### Step 6: Final Scorecard and Commit

* Update `/audit/module-06-scorecard.md` with final PASS/FAIL per criterion
* Add a Notes section explaining any non-trivial revision decisions
* Final commit:

```
git add audit/module-06-scorecard.md
git commit -m "polish(module-06): final scorecard, all rubric checks pass"
```

* Do not merge to main automatically. Branch is ready for PR review.

---

## Stop Conditions

* Stop when all Section A and Section B criteria pass for `module-06.md` on a single pass
* OR stop after 3 revision passes regardless of result
* Do not proceed to other modules. This task is module-06 only.

---

## What This Task Does NOT Do

* Does not run Section C (cross-module). Section C runs after all 12 modules pass individually.
* Does not modify other modules.
* Does not modify `CLAUDE.md`, the addendum, the rubric, the templates, or the pairing selection.
* Does not push to GitHub remote (instructor will push after PR review).

---

## Expected Output

1. Modified `modules/06-healthcare-it-ethics/module-06.md` (trimmed from ~8,064 to ~6,250 words, with 2025-2026 AI touchpoint added)
2. New `/audit/module-06-scorecard.md` with all rubric criteria reported
3. Two or three commits on `polish/module-06` branch
4. Branch ready for instructor PR review
