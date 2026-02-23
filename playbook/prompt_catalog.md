# Prompt Catalog (A–H)

Use the Universal Intake first, then apply the category skeleton below.

Each category includes:
- **Version**: Current version of the prompt skeleton
- **Last Updated**: When the skeleton was last modified
- **Effectiveness Score**: Self-assessed coverage (1-5, updated after improvements)
- **Output skeleton**: The actual prompt structure

---

## A. Logic & Argumentation

**Version**: v1.0
**Last Updated**: 2024-01-15
**Effectiveness Score**: 4/5

Use for: argument audits, validity, counterexamples, "cold-water review".

Output skeleton:
1) Conclusion: conditions of validity (necessary/sufficient)
2) Premises: explicit vs implicit
3) Inference chain: shortest valid chain (premise → derivation → conclusion)
4) Vulnerabilities & counterexamples: at least 3 strongest
5) Repairs: strengthen premises / add constraints / define terms
6) Verification: measurable observations/experiments/metrics
Style: formal, testable, minimal rhetoric.

**Evaluation Criteria**:
- [ ] All premises identified?
- [ ] At least 3 counterexamples provided?
- [ ] Repairs are actionable?

---

## B. Math / Theory Explanation

**Version**: v1.0
**Last Updated**: 2024-01-15
**Effectiveness Score**: 4/5

Use for: tiered explanations, concept maps, learning routes, book lists.

Output skeleton:
- Layer 1: high-school intuition (≤300 words, analogies)
- Layer 2: undergraduate (definitions + examples + common pitfalls)
- Layer 3: research intro (key results, main approaches, open problems)
Then:
1) Concept map (10–20 bullets)
2) Example problems / thought experiments (3–5)
3) Study plan (4–8 weeks; readings + practice)
4) Resources (intro/advanced; why each)

**Evaluation Criteria**:
- [ ] Each layer builds on previous?
- [ ] Concept map covers key relationships?
- [ ] Study plan is time-bounded and actionable?

---

## C. Engineering Delivery (Architecture/Implementation/Debugging)

**Version**: v1.0
**Last Updated**: 2024-01-15
**Effectiveness Score**: 4/5

Use for: systems, refactors, specs, incidents, deployment.

Output skeleton:
1) Architecture overview (components, dataflow, interfaces, deps)
2) Key decisions (rationale + alternatives)
3) Milestones (MVP → V1 → V2; deliverables each)
4) Failure modes & observability (logs/metrics/alerts; rollback)
5) Minimal runnable example (pseudo-code / tree / config)
6) Docs list (exact paths)
Debug mode:
- Top 5 likely causes → verification steps → fixes → prevent recurrence.

**Evaluation Criteria**:
- [ ] Architecture is implementable?
- [ ] Milestones have clear deliverables?
- [ ] Failure modes include mitigation?

---

## D. Product / Mechanism Design (Community/Standards/Governance/Incentives)

**Version**: v1.0
**Last Updated**: 2024-01-15
**Effectiveness Score**: 4/5

Use for: governance, rules, incentives, anti-abuse, sustainability.

Output skeleton:
1) Roles & incentives model (user/contributor/maintainer/reviewer/platform)
2) Rules (submission/review/versioning/disputes/enforcement)
3) Incentives (short/long term; monetary/reputation/opportunity; anti-gaming)
4) Cold start path (first 100 supply; first 1000 demand)
5) Risk register (failure modes + mitigations)
6) Metrics (north star + moat + risk metrics)

**Evaluation Criteria**:
- [ ] All key roles identified?
- [ ] Incentives aligned and anti-gaming considered?
- [ ] Cold start path is concrete?

---

## E. Writing & Publishing (Article/Book/Report/Talk)

**Version**: v1.0
**Last Updated**: 2024-01-15
**Effectiveness Score**: 4/5

Use for: outlines, rewrites, de-duplication, editorial guidance.

Output skeleton:
1) Structured outline (with intent per section)
2) Information allocation (word ratio; key arguments placement)
3) De-dup plan (repeats → merge plan)
4) Rewrite draft (strictly following constraints)
5) Chapter-by-chapter edit guide (keep/cut/add + why)

**Evaluation Criteria**:
- [ ] Outline has clear intent per section?
- [ ] Word allocation matches importance?
- [ ] Edit guide is actionable?

---

## F. Policy / Legal / Compliance

**Version**: v1.0
**Last Updated**: 2024-01-15
**Effectiveness Score**: 4/5

Use for: legal reasoning, compliance checklists, policy analysis, thesis structure.

Output skeleton:
1) Issue list
2) Normative basis framework (statutes/principles/cases/practice)
3) Legal reasoning (elements → facts → subsumption → conclusion)
4) Risks & mitigations (operational)
5) Deliverable text (format specified; citation-ready language)

**Evaluation Criteria**:
- [ ] All relevant issues identified?
- [ ] Legal reasoning chain is valid?
- [ ] Deliverable is ready for use?

---

## G. Research Curation / Study Guide

**Version**: v1.0
**Last Updated**: 2024-01-15
**Effectiveness Score**: 4/5

Use for: knowledge maps, reading guides, tagging systems, bibliographies.

Output skeleton:
1) Key concepts table (definition → misconception → related)
2) Sources list (primary/authoritative surveys/courses/tools)
3) Reading guide (stages: intro → understanding → critique → application)
4) Knowledge map (hierarchy or nodes/edges)
5) Tag system (dimensions → labels → rules → examples)

**Evaluation Criteria**:
- [ ] Concepts clarify misconceptions?
- [ ] Sources are authoritative and categorized?
- [ ] Tag system is usable?

---

## H. Events & Project Management

**Version**: v1.0
**Last Updated**: 2024-01-15
**Effectiveness Score**: 4/5

Use for: conferences, forums, awards, competitions, dinners.

Output skeleton:
1) Quantified goal breakdown
2) Agenda (timed; host cues)
3) Roles & responsibilities (RACI)
4) Materials checklist (KV, handbook, badges, stage, livestream)
5) Risk plans (no-show, overtime, PR, technical failure)
6) Post-event deliverables (press kit, minutes, data review)

**Evaluation Criteria**:
- [ ] Goals are measurable?
- [ ] Agenda includes timing and cues?
- [ ] Risk plans are comprehensive?

---

## Other. Universal Intake

**Version**: v1.0
**Last Updated**: 2024-01-15
**Effectiveness Score**: N/A (fallback)

When task doesn't fit A-H, use `playbook/intake_checklist.md` as the universal schema.

**Trigger for Evolution**:
- If this category is used 3+ times in a row with related themes, consider proposing a new category.
