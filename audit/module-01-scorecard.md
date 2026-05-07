# Module 1 Scorecard

**Date:** 2026-05-07
**Revision Pass:** 1
**Overall Status:** PASS

## Section A: Mechanical

* A1 Em-Dash Count: PASS (count: 0)
* A2 Banned Words: PASS (matches: 0; none of spot-on, indeed, delve, dive, embark, nuances, journey, tapestry, navigate detected)
* A3 Word Count: PASS (count: 5,523, target: Module 1 exception allows 5,000-5,800; pre-polish was 5,111, expanded to 5,523 via B2 additions) — Module 1 exception applies
* A4 Heading Icons: PASS (Module Overview 🧭, Learning Objectives 🎯, Think About It 1.1/1.2/1.3 🧠, Quick Check 1.1/1.2/1.3/1.4 ✅, Case Study 1.1 📋, Summary and Retrieval 💡, Discussion Prompt 💬, Further Reading 📖, Looking Ahead ⏩; Skills Lab 1.5 carries no icon as required)
* A5 List Bullets: PASS (no hyphen bullets; all asterisks)
* A6 MLO Format: PASS (3 of 3 MLOs match `MLO-N.X (Bloom's): **Verb...** *(CLO X)*` format; all three reference CLO I, consistent with the CLO-to-Module table in CLAUDE.md)
* A7 Section Numbering: PASS (1.1-1.7 sequential; 1.5 Skills Lab, 1.6 Summary, 1.7 Discussion)

## Section B: Judgment

* B1 Schedule Consistency: PASS — Module Overview Estimated Time is 4-5 hours, appropriate for a standard single module; M1 is alone in W1 (May 26-31 partial week) under Option 1, so the standard load estimate is correct and the lighter onboarding posture is consistent with the addendum.
* B2 AI-2026 Currency: PASS — New subsection "The Frameworks in the Age of AI" added in §1.4 (121 words) introduces the orchestrator-verifier stance with EU AI Act (February 2025 enforcement phase-in) and 2024-2025 ACM/IEEE guidance as anchors; Discussion Prompt updated to span 2023-2025 events including the EU AI Act enforcement context; orchestrator-verifier term defined in Key Terms with 2024-2025 ACM/IEEE citation; Key Concepts bullet in §1.6 reinforces the AI application of all four frameworks.
* B3 Rubric Vocabulary: PASS — Skills Lab 1A rubric uses Mastery (5), Proficiency (4), Developing (3), Emerging (2), Not Evident (1) across 5 criteria (Stakeholder Analysis, Ethical Framework Application, Module Concept Application, Recommendation Quality, Writing and Professionalism), matching the cross-module standard.
* B4 Discussion Prompt Quality: PASS — Prompt requires students to take and defend a position on whether a dedicated AI ethics team is an ethical obligation for companies that deploy AI systems, referencing at least one framework from the module, and addressing the strongest counterargument using a different framework; framework reference and structured peer engagement are explicitly required.
* B5 Case Study Stakeholders: PASS — Case Study 1.1 (Campus Wi-Fi Tracking Debate) presents 4 stakeholder groups with genuinely competing interests (Dr. Reyes/safety, Marcus/privacy and freedom, Janet/security and data risk, Prof. Ochoa/academic freedom); no obvious correct answer because the safety benefit is real but the privacy and chilling-effect concerns are equally real and framework-dependent.
* B6 CLO Alignment: PASS — CLO I (Compare and contrast ethical theories and apply them to technology scenarios) is traced through all four content sections: §1.1 introduces morals/ethics/laws distinction (MLO-1.1 Understand), §1.2 covers utilitarianism and deontology, §1.3 covers virtue ethics and social contract theory, §1.4 applies all four to IT decisions including AI orchestration (MLO-1.2 Apply, MLO-1.3 Analyze); all three MLOs reference CLO I correctly.
* B7 Voice Consistency: PASS — Second-person ("you") sustained throughout all content sections including the new AI touchpoint subsection ("When you deploy or configure an AI system, you are not a passive user"); no academic passive voice; no moralizing; the new subsection uses direct, action-oriented phrasing consistent with the cross-module standard established in M3 and M5.
* B8 Looking Ahead: PASS — Looking Ahead correctly forward-references Module 2 (professional and corporate settings, corporate culture, codes of conduct, pressures on good people); under selected Option 1, M1 is in W1 and M2+M3 are paired in W2, so forward-referencing M2 is accurate per the binding schedule.

## Notes

**Module 1 word-count exception applies.** Pre-polish count was 5,111 (within the Module 1 exception of 5,000-5,800). Post-polish count is 5,523 after the B2 AI touchpoint additions. No trim was required or performed. The addendum explicitly designates M1 as the foundation module with a lighter onboarding posture; the polish pass adds substance without padding.

**B2 additions: placement rationale.** The AI touchpoint was placed at the end of §1.4 (Applying Ethical Frameworks to IT Decisions) as a new subsection "The Frameworks in the Age of AI." This location is pedagogically correct: students have just seen the four frameworks compared in a table and applied to a real case study. The subsection shows them one more application domain (AI orchestration) before moving to the Skills Lab. The orchestrator-verifier term is introduced here, defined in Key Terms, and echoed in the Key Concepts summary — a three-point anchoring pattern that matches the M3 approach.

**Orchestrator-verifier as a foundation, not an anchor.** M1 introduces the orchestrator-verifier term lightly (one new subsection, one Key Terms entry, one Key Concepts echo). M3 is the AI anchor that elaborates the full governance framework. This is the correct progression: M1 plants the term so it is not new when M3 develops it. Each subsequent module applies it to a specific domain (whistleblowing in M5, clinical AI in M6, etc.). M1's job is to show that the four ethical frameworks are the *reasoning tools* for the orchestrator-verifier role, not to explain the role in depth.

**Discussion Prompt update.** The pre-polish prompt referenced only 2023 events. The updated prompt spans 2023-2025 and adds the EU AI Act enforcement context (February 2025 phase-in), which ties directly to the AI touchpoint in §1.4 and gives the prompt a 2025-2026 hook that satisfies B2 in a second location.

**M1 as exemplar for tone and structure.** Per the rubric's B7 note that "voice is consistent and conforms to docs/style-guide.md" and that "tone matches Module 1 sample," this module is the cross-module tone reference. The pre-polish module already met that standard: direct second-person voice, no moralizing, accessible language, no academic passive voice. The post-polish additions maintain that standard in the new subsection and updated prompt. Future polish passes on M2-M12 should reference M1's voice as the benchmark.

**B8 forward reference confirmed.** Looking Ahead points to M2. Under Option 1 (selected 2026-05-07), M1 is solo in W1 and M2+M3 are paired in W2. Pointing to M2 is accurate and does not need to enumerate both M2 and M3; students will see the W2 pairing in the course calendar.

**Section C (cross-module) deferral.** Per the rubric, Section C runs after all 12 modules pass A and B individually. This scorecard reports A and B only.

**Branch state.** `polish/module-01` contains three commits ahead of main:
1. `polish(module-01): mechanical pass (format compliance)` — all Section A checks PASS; B2 additions and Discussion Prompt update were already staged before the first commit, so they appear here (consistent with M3 precedent noted in module-03-scorecard.md)
2. `polish(module-01): judgment pass (AI-2026 currency, voice, CLO alignment)` — all Section B checks PASS on first pass; scorecard initial draft included
3. `polish(module-01): final scorecard, all rubric checks pass` — this file with final notes, branch state updated
