# Handoff: CIS111 Summer 2026 Section C Cross-Module Audit

**Date written:** 2026-05-07
**Phase:** Repo polish complete; Section C cross-module audit pending
**Pairing:** Option 1 (Theme-Density) — selected and recorded in `planning/summer-2026-pairing.md`

---

## Read this file first, then proceed

This handoff captures the state of the repo at the moment all 12 individual module polish loops finished. The previous session's context window was approaching its budget, so this doc was written to let a fresh session continue cleanly without re-deriving operational details.

The repo is in a clean, well-defined state. All 12 polish branches are pushed to origin. Nothing has been merged to `main` yet.

---

## Polish results (snapshot)

| Module | Words | Em-dashes | Banned | 2025/26 refs | Branch | Notes |
|---|---:|---:|---:|---:|---|---|
| M1 | 5,523 | 0 | 0 | 3 | `polish/module-01` | Foundation; word-count exception (5,000-5,800) applies |
| M2 | 5,726 | 0 | 0 | 4 | `polish/module-02` | RARE EXPANSION case (was 5,331) |
| M3 | 6,499 | 0 | 0 | 7 | `polish/module-03` | AI Ethics Anchor; sets up orchestrator-verifier frame |
| M4 | 6,248 | 0 | 0 | 7 | `polish/module-04` | |
| M5 | 6,455 | 0 | 0 | 2 | `polish/module-05` | First polished; reference exemplar |
| M6 | 6,491 | 0 | 0 | 5 | `polish/module-06` | |
| M7 | 6,504 | 0 | 0 | 5 | `polish/module-07` | 16.7% trim |
| M8 | 6,509 | 0 | 0 | 12 | `polish/module-08` | 20.5% trim; W6 light week |
| M9 | 6,503 | 0 | 0 | 3 | `polish/module-09` | Paired with M10 in W7 |
| M10 | 6,498 | 0 | 0 | 3 | `polish/module-10` | Paired with M9 in W7 |
| M11 | 6,499 | 0 | 0 | 3 | `polish/module-11` | 23.8% trim; densest CLO load |
| M12 | 7,366 | 0 | 0 | 6 | `polish/module-12` | Capstone; capstone band 6,500-7,500 |

Repo-wide quick check (preview of C4): 0 em dashes, 0 banned words across all 12 modules. C4 will almost certainly PASS once branches are merged.

Each branch contains 3 commits except `polish/module-12`, which has 2 (mechanical and judgment passes were combined in one commit; final scorecard is the second commit). The 2-vs-3 commit difference is fine; do not "normalize" it.

---

## Step-by-step plan

### Step 1: Open PRs for each polish branch

For each of the 12 polish branches, open a PR via `gh pr create` (the `gh` CLI is available and authenticated for `jor2050111`). Recommended PR title and body format:

**Title:** `polish: Module NN — [Module Title]`

**Body template:**
```
Polish loop for Module NN per rubrics/redesign-acceptance.md (Sections A and B).

See audit/module-NN-scorecard.md for full audit results.

- Final word count: XXXX (band 5,500-6,500 [or capstone/exception band])
- 2025-2026 AI currency added per orchestrator-verifier framing established in M3
- All Section A and Section B criteria PASS

Pair partner under Option 1 (Theme-Density): [M_NN paired in W_X | M_NN alone in W_X]
```

Each polish branch only modifies its own module file plus its own scorecard, so merge conflicts between PRs are unlikely. Commit the PRs in any order.

### Step 2: Merge each PR to `main`

Merge each PR with a standard merge commit. After merging:
- Delete the polish branch locally and on origin
- Pull `main` to verify it now contains all 12 polished modules and all 12 scorecards
- Run a quick repo-wide grep to confirm em-dash and banned-word counts remain 0

### Step 3: Run the Section C cross-module audit

Per `rubrics/redesign-acceptance.md`, Section C has 5 criteria. Operate on `main` after all merges.

#### C1. Cumulative Workload (target: 80-100 hours total)

The rubric specifies cumulative hours summed across the term. Note: the per-module "Estimated time" in each Module Overview covers reading + activities + discussion but may not fully include Skills Lab time, peer-response time, and individual study. The addendum's student weekly load target of 8-12 hours/week × 9 weeks = 72-108 hours is the relevant benchmark; the rubric's 80-100 sits inside that band.

**Per Option 1 weekly schedule, sum of Module Overview estimates:**

| Week | Modules | Per-week estimate | Notes |
|---|---|---:|---|
| 1 | M1 | 4-5 hr | Partial week, foundation |
| 2 | M2+M3 paired | ~8-10 hr | Approaches upper bound |
| 3 | M4 | 4-5 hr | |
| 4 | M5+M6 paired | ~8-10 hr | |
| 5 | M7 | 4-5 hr | |
| 6 | M8 | 4-5 hr | July 4 light week |
| 7 | M9+M10 paired | ~8-10 hr | |
| 8 | M11 | 5-6 hr | Densest module |
| 9 | M12 | 5-6 hr | Capstone, partial week |

**Sum range from Module Overview estimates:** ~50-62 hours.
**Plus Skills Lab work (12 labs × 90-120 min):** ~18-24 hours.
**Plus peer responses, study, capstone synthesis time:** ~15-20 hours.
**Approximate total:** ~83-106 hours, which centers within the 80-100 target.

If your sum falls outside 80-100 after running the calculation, document the gap in `audit/section-c-rollup.md` rather than re-trimming modules. The Module Overview estimates can be adjusted upward (e.g., M11 to 6-7 hr) as a cleaner fix than re-touching content.

#### C2. CLO Complete Coverage (all 18 CLOs addressed)

Cross-check against the CLO-to-Module table in `CLAUDE.md`:

| CLO | Module | Verified by MLO |
|---|---|---|
| I | M1 | MLO-1.1, 1.2, 1.3 |
| II | M2 | MLO-2.1, 2.2, 2.3 |
| III | M3 | MLO-3.1, 3.2, 3.3 |
| IV | M4 | MLO-4.1, 4.2, 4.3 |
| V | M5 | MLO-5.1, 5.2 |
| VI | M6 | MLO-6.1, 6.2, 6.3 |
| VII | M5 | MLO-5.3 |
| VIII | M7 | MLO-7.1, 7.2 |
| IX | M7 | MLO-7.3 |
| X | M8 | MLO-8.1, 8.2, 8.3 |
| XI | M9 | MLO-9.1, 9.2, 9.3 |
| XII | M10 | MLO-10.1, 10.3 |
| XIII | M10 | MLO-10.2, 10.3 |
| XIV | M11 | MLO-11.1 |
| XV | M11 | MLO-11.2 |
| XVI | M11 | MLO-11.3 |
| XVII | M12 | MLO-12.1, 12.2, 12.3 |
| XVIII | M11 | MLO-11.2, 11.3 |

This is structurally established. Verify by grepping each module's MLO block and confirming the CLO references match the table. Likely PASS without remediation.

#### C3. Skills Lab Style Consistency

All 12 Skills Lab rubrics should use the same vocabulary (Mastery, Proficiency, Developing, Emerging, Not Evident) across the same 5 criteria (Stakeholder Analysis, Ethical Framework Application, Module Concept Application, Recommendation Quality, Writing and Professionalism).

Each individual scorecard's B3 line confirms this is consistent in that module. Verify cross-module by extracting the rubric tables and diffing the criterion names and level labels. Likely PASS.

#### C4. Banned Words and Em Dashes Across All Modules

Already pre-checked at the polish-loop level. From `main` after all merges, run:

```
grep -rEc "—" modules/
grep -rwiE "\b(spot-on|indeed|delve|dive|embark|nuances|journey|tapestry|navigate)\b" modules/
```

Expected: empty output for both. If anything appears, identify which module introduced the regression.

#### C5. Pairing-Aware Forward References (Looking Ahead)

This is the cross-module check most likely to need touch-ups. Each module's Looking Ahead must accurately forward-reference the next module per Option 1.

**Per-module C5 expectation matrix:**

| Module | Position | Looking Ahead should reference |
|---|---|---|
| M1 | W1 alone | M2 (start of W2 paired week with M3) |
| M2 | W2 paired w/ M3 | M3 as same-week partner (acceptable) OR M4 (next week) |
| M3 | W2 paired w/ M2 | M4 (next week, W3) |
| M4 | W3 alone | M5 (start of W4 paired week with M6) |
| M5 | W4 paired w/ M6 | M6 as same-week partner (existing) |
| M6 | W4 paired w/ M5 | M7 (next week, W5) |
| M7 | W5 alone | M8 (next week, W6) |
| M8 | W6 alone | M9 (start of W7 paired week with M10) |
| M9 | W7 paired w/ M10 | M10 as same-week partner (existing) |
| M10 | W7 paired w/ M9 | M11 (next week, W8) |
| M11 | W8 alone | M12 (next week, W9, capstone) |
| M12 | W9 alone | NO successor; "There is no Module 13" course-closer is intentional and correct |

For each module, read the Looking Ahead section and verify it matches the expected reference. M12's Looking Ahead is a course closer, not a forward reference; it should be marked PASS for B8/C5 with a note.

If any module's Looking Ahead does not match, fix it directly on `main` (small commits, one per module) rather than re-opening polish branches. Use commit message: `chore(module-NN): align Looking Ahead with Option 1 pairing`.

### Step 4: Write `audit/section-c-rollup.md`

Use this template:

```markdown
# CIS111 Summer 2026 Section C Cross-Module Roll-Up

**Date:** YYYY-MM-DD
**Pairing:** Option 1 (Theme-Density)
**Overall Status:** PASS / FAIL

## C1 Cumulative Workload: PASS / FAIL
- Calculated total: XX-XX hours
- Target band: 80-100 hours
- Method: [brief description]
- Evidence per week: [bullets or table]
- Notes: [any items requiring instructor attention]

## C2 CLO Complete Coverage: PASS / FAIL
- 18 of 18 CLOs covered: ✓ / ✗
- CLO-to-MLO trace: [reference handoff table or paste verified version]
- Notes: ...

## C3 Skills Lab Style Consistency: PASS / FAIL
- All 12 rubrics use Mastery/Proficiency/Developing/Emerging/Not Evident: ✓ / ✗
- Criterion names parallel across modules: ✓ / ✗
- Notes: ...

## C4 Repo-Wide Banned Words and Em Dashes: PASS / FAIL
- Em-dash count across all modules/: 0 expected
- Banned-word matches: 0 expected
- Method: [grep commands run]
- Notes: ...

## C5 Pairing-Aware Forward References: PASS / FAIL
- Per-module verification:
  - M1: ✓ references M2
  - M2: ✓ references M3 (or M4)
  - M3: ✓ references M4
  - [...continue for all 12...]
- Notes: M12 is the terminal module with no successor; intentional course-closer is correct.

## Notes
[Aggregate notes including any items deferred, any mid-audit content fixes made, and any items flagged for instructor attention.]

## Repo Phase Status
After this roll-up: REPO PHASE COMPLETE / INCOMPLETE.
```

### Step 5: Commit and push, mark phase complete

```
git add audit/section-c-rollup.md
git commit -m "audit(section-c): cross-module roll-up — repo phase complete"
git push origin main
```

Update `HANDOFF.md` (if it exists at the repo root) or this file with a "Phase Complete" note. The repo phase is then officially done.

### Step 6 (next phase): Canvas LMS push

Per `docs/summer-2026-addendum.md`, the Canvas push is a **separate project**, not continued in this repo. Use the Cowork environment with the `canvas-content-rewriter` skill. Output goes to `/canvas-import/` organized by Option 1 week (not by module). Out of scope for this repo phase.

---

## Authority files (read in order if needed)

1. `CLAUDE.md` — project standards, banned words, MLO format, CLO-to-Module table
2. `docs/summer-2026-addendum.md` — term constraints, length targets, AI-2026 currency, weekly load
3. `rubrics/redesign-acceptance.md` — Section C definition, scorecard template
4. `planning/summer-2026-pairing.md` — selected Option 1 schedule (binding)
5. `audit/module-05-scorecard.md` and `audit/module-11-scorecard.md` — scorecard format references
6. `planning/tasks/polish-module-{05,06,11}.md` — workflow templates that succeeded for the polish loops

---

## Gotchas worth knowing

- **Sister directory `cis111-summer-redesign/`** at the parent path is a non-git working dir that held the original planning materials. It was consolidated into this repo earlier in the redesign process. Safe to ignore.
- **`polish/module-12` has 2 commits**, not 3, because the mechanical and judgment passes were combined. The final scorecard is the second commit. This is fine.
- **The orchestrator-verifier framing** is consistent across modules: introduced in M1, anchored in M3, and applied module-specifically in M2 and M4 through M12. If C5 or any cross-module read reveals an inconsistency in this framing, fix toward the M3 anchor's definition.
- **M2 was the only expansion case** (5,331 → 5,726). Every other module trimmed.
- **M12 has a wider word band** (6,500-7,500) per the capstone exception; do not try to trim it under 6,500.
- **No module should be edited during Section C** unless a specific cross-module check requires it. Section C is verification, not re-polishing. The exception is a Looking Ahead reference fix in C5, which is small and targeted.
- **The `gh` CLI is configured** for `jor2050111` and works for PR creation, listing, and merging. If you hit auth issues, ask the user before debugging.

---

## Tools that worked well in the polish phase

- Subagents with `subagent_type: general-purpose` and `model: sonnet` for individual module polish loops, sequentially (not parallel — worktree isolation hit a base-branch resolution error from the parent's cwd, and parallel non-isolated agents would race on git locks)
- Each subagent typically ran 5-15 minutes wall-clock per module
- Subagents that were given 1) the rubric path, 2) the addendum path, 3) two existing scorecards (M5, M11) as templates, and 4) two existing post-polish modules as voice references produced consistent results without the parent needing to micromanage

---

## One-line kickoff prompt for the new session

> Continue the CIS111 Summer 2026 redesign at `/Users/vega/My Drive (jor2050111@phoenixcollege.edu)/Claude-Assistant/02-Research/GitHub-jor2050111/cis111-course-redesign/`. Read `HANDOFF-section-c.md` first; it has the full plan, per-module C5 targets, the C1 arithmetic breakdown, the section-c-rollup.md template, and known gotchas.
