# MCE Evolution Protocol

This document records the self-evolution history of Master Control Expert, category management rules, and prompt improvement workflows.

---

## Part 1: Category Management

### 1.1 Current Categories

| Letter | Name | Definition | Use Cases | Version |
|--------|------|------------|-----------|---------|
| A | Logic & Argumentation | Logical argument analysis and debate review | Argument audits, validity checks, counterexamples, "cold-water reviews" | v1.0 |
| B | Math / Theory Explanation | Mathematical/theoretical explanations | Tiered explanations, concept maps, learning routes, book lists | v1.0 |
| C | Engineering Delivery | Engineering implementation | Systems, refactors, specs, incidents, deployment | v1.0 |
| D | Product / Mechanism Design | Product/mechanism design | Governance, rules, incentives, anti-abuse, sustainability | v1.0 |
| E | Writing & Publishing | Writing and publishing | Outlines, rewrites, de-duplication, editorial guidance | v1.0 |
| F | Policy / Legal / Compliance | Policy/legal/compliance | Legal reasoning, compliance checklists, policy analysis | v1.0 |
| G | Research Curation / Study Guide | Research curation/study guides | Knowledge maps, reading guides, tagging systems, bibliographies | v1.0 |
| H | Events & Project Management | Events & project management | Conferences, forums, awards, competitions, dinners | v1.0 |
| Other | Universal Intake | Universal intake checklist | Default when task doesn't fit A-H | v1.0 |

### 1.2 New Category Proposal Template

When a new category is needed, prepare a proposal using the following template:

```yaml
proposal_id: NC-XXX
date: YYYY-MM-DD
trigger_reason: ""

# Category Definition
category:
  letter: I  # Assign next letter in sequence
  name: ""
  definition: ""
  use_cases:
    - ""
    - ""

# Prompt Skeleton
prompt_skeleton:
  purpose: ""
  output_sections:
    - section: ""
      description: ""
    - section: ""
      description: ""

# Distinction Analysis
distinction_analysis:
  why_not_A: ""
  why_not_B: ""
  # ... Explain why it doesn't belong to existing categories

# Validation Cases
validation_cases:
  - input: ""
    expected_output: ""

# Proposal Status
status: proposed  # proposed / approved / rejected
approved_by: ""
```

### 1.3 Category Addition Workflow

```
┌─────────────────────────────────────────────────────────────┐
│  Triggers                                                    │
│  • Task differs from A-H by > 70%                           │
│  • 3 consecutive tasks fall into Other with related themes  │
│  • User explicitly requests                                 │
└──────────────────────┬──────────────────────────────────────┘
                       ▼
┌─────────────────────────────────────────────────────────────┐
│  Step 1: Prepare Proposal                                    │
│  • Fill out NC-XXX template                                  │
│  • Complete category definition and prompt skeleton         │
│  • Write distinction analysis                               │
└──────────────────────┬──────────────────────────────────────┘
                       ▼
┌─────────────────────────────────────────────────────────────┐
│  Step 2: User Confirmation                                   │
│  • Present proposal to user                                  │
│  • Explain trigger reason and category positioning          │
│  • Get user feedback (modify / confirm / reject)            │
└──────────────────────┬──────────────────────────────────────┘
                       ▼
┌─────────────────────────────────────────────────────────────┐
│  Step 3: Apply Updates (after user confirmation)             │
│  • Add new category to prompt_catalog.md                     │
│  • Update category list in SKILL.md                          │
│  • Record in evolution log in this document                 │
│  • Update category management table                         │
└─────────────────────────────────────────────────────────────┘
```

---

## Part 2: Prompt Improvement

### 2.1 Effectiveness Metrics

Evaluate each category's prompt skeleton on the following dimensions:

| Dimension | Description | Score (1-5) | Improvement Threshold |
|-----------|-------------|-------------|----------------------|
| Coverage | Does it cover user main requirements? | < 4 needs improvement | |
| Precision | Is output focused, without redundancy? | < 4 needs improvement | |
| Actionability | Is output directly executable? | < 4 needs improvement | |
| User Satisfaction | Is user satisfied (via feedback)? | < 4 needs improvement | |

### 2.2 Common Improvement Patterns

**Pattern 1: Add Missing Output Items**
```diff
+ 6) Visualization suggestions (chart types, tools)
```

**Pattern 2: Remove Redundant Output Items**
```diff
- 5) Detailed historical background (unless requested)
+ 5) Keep only background relevant to current decisions
```

**Pattern 3: Adjust Output Order**
```diff
  Output skeleton:
-   1) Concept map
-   2) Core definitions
+   1) Core definitions
+   2) Concept map
```

**Pattern 4: Increase/Decrease Detail Level**
```diff
- 3) Example problems (3-5)
+ 3) Example problems (5-8, including basic/advanced/challenge)
```

### 2.3 Prompt Improvement Workflow

```
┌─────────────────────────────────────────────────────────────┐
│  Triggers                                                    │
│  • User feedback indicates poor effectiveness               │
│  • Skeleton found to miss key items                         │
│  • User repeatedly overrides default sections               │
│  • Same category needs major adjustments 2+ times           │
└──────────────────────┬──────────────────────────────────────┘
                       ▼
┌─────────────────────────────────────────────────────────────┐
│  Step 1: Problem Diagnosis                                   │
│  • Identify which specific parts are ineffective            │
│  • Determine if it's missing, redundant, or ordering issue  │
│  • Reference common improvement patterns                    │
└──────────────────────┬──────────────────────────────────────┘
                       ▼
┌─────────────────────────────────────────────────────────────┐
│  Step 2: Prepare Improvement Plan                            │
│  • Write revised prompt skeleton                            │
│  • Prepare before/after comparison                          │
│  • Explain expected improvement                             │
└──────────────────────┬──────────────────────────────────────┘
                       ▼
┌─────────────────────────────────────────────────────────────┐
│  Step 3: User Confirmation                                   │
│  • Present problem and improvement plan                     │
│  • Get user feedback (modify / confirm / reject)            │
└──────────────────────┬──────────────────────────────────────┘
                       ▼
┌─────────────────────────────────────────────────────────────┐
│  Step 4: Apply Updates (after user confirmation)             │
│  • Update corresponding category in prompt_catalog.md       │
│  • Update version number (v1.0 → v1.1)                      │
│  • Record improvement log in this document                  │
└─────────────────────────────────────────────────────────────┘
```

### 2.4 Prompt Improvement Proposal Template

```yaml
improvement_id: PI-XXX
date: YYYY-MM-DD
category: A  # Category being improved
current_version: v1.0
proposed_version: v1.1

# Problem Diagnosis
problem_analysis:
  trigger: ""
  affected_sections:
    - ""
  root_cause: ""

# Improvement Plan
improvements:
  - type: add/remove/modify/reorder  # Choose one
    section: ""
    before: ""
    after: ""
    rationale: ""

# Expected Outcomes
expected_outcomes:
  - ""

# Proposal Status
status: proposed  # proposed / approved / applied / reverted
approved_by: ""
```

---

## Part 3: Evolution Log

### Category Additions

None yet

### Prompt Improvements

None yet

### Rejected Proposals

None yet (Record rejected proposals and reasons to avoid duplicate proposals)

---

## Part 4: Self-Assessment Checklist

After each task completion, MCE should ask itself:

### Classification Assessment
- [ ] Does this task clearly belong to one of the A-H categories?
- [ ] If it falls into Other, is there an obvious category trend?
- [ ] Is there a reason to consider adding a new category?

### Prompt Effectiveness Assessment
- [ ] Did the prompt skeleton used cover all user requirements?
- [ ] Did the user request content not in the skeleton?
- [ ] Was there skeleton content the user explicitly didn't need?
- [ ] Was the output order as expected by the user?
- [ ] Was the level of detail appropriate?

### User Feedback
- [ ] Did the user express satisfaction/dissatisfaction?
- [ ] Did the user request major adjustments?
- [ ] Do the adjustments involve the prompt skeleton itself?

### Evolution Decisions
- [ ] Is it necessary to propose a new category to the user?
- [ ] Is it necessary to propose prompt improvements to the user?
- [ ] Should observations be recorded without immediate action?

---

## Part 5: Quick Reference

### Quick Difference Assessment Guide

| Task Characteristics | Likely Category | If Not, Consider |
|---------------------|-----------------|------------------|
| Analyze argument validity | A | New analysis category |
| Explain complex concepts | B | New education category |
| Design/implement systems | C | New technical category |
| Design rules/incentives | D | New design category |
| Create content | E | New creation category |
| Legal/compliance analysis | F | New compliance category |
| Organize knowledge systems | G | New knowledge category |
| Organize events | H | New operations category |
| Pure information extraction | Other | Consider adding "Information Processing" category |
| Creative ideation | Other | Consider adding "Creative Generation" category |
| Emotional support | Other | Recommend not using MCE |

### When NOT to Evolve

- Single task falling into Other is normal
- User's minor output adjustments (not skeleton issues)
- User explicitly prefers different defaults (personal preference, not universal improvement)
- Task itself is poorly defined causing poor results
