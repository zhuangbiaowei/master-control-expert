# Master Control Expert (MCE)

A structured task processing framework for Claude Code. MCE transforms any request into executable, governed workflows.

## Overview

Master Control Expert (MCE) is a task classification and execution framework that helps Claude Code efficiently handle various types of tasks. Through standardized processes and prompt templates, MCE ensures every task receives systematic, high-quality processing.

## Core Workflow

```
Receive Task → Intake → Classify → Plan → Deliver
```

### Four-Step Method

1. **Intake** - Collect necessary information using the universal checklist
2. **Classify** - Categorize the task into A-H categories
3. **Control** - Output control summary and definition of done
4. **Execute** - Apply corresponding prompt templates and produce concrete deliverables

## Task Categories (A-H)

| Category | Name | Use Cases |
|----------|------|-----------|
| A | Logic & Argumentation | Argument audits, validity checks, counterexamples, "cold-water reviews" |
| B | Math / Theory Explanation | Tiered explanations, concept maps, learning routes, book lists |
| C | Engineering Delivery | Systems, refactors, specs, incidents, deployment |
| D | Product / Mechanism Design | Governance, rules, incentives, anti-abuse, sustainability |
| E | Writing & Publishing | Outlines, rewrites, de-duplication, editorial guidance |
| F | Policy / Legal / Compliance | Legal reasoning, compliance checklists, policy analysis |
| G | Research Curation / Study Guide | Knowledge maps, reading guides, tagging systems, bibliographies |
| H | Events & Project Management | Conferences, forums, awards, competitions, dinners |

## File Structure

```
master-control-expert/
├── SKILL.md                    # Skill definition file (for Claude Code)
├── README.md                   # This file (Chinese)
├── README.en.md                # English version
└── playbook/                   # Playbook directory
    ├── intake_checklist.md     # Universal intake checklist
    ├── prompt_catalog.md       # A-H category prompt skeletons
    ├── control_plan.md         # Control plan template
    ├── decision_log.md         # Decision log
    ├── runbook.md              # Runbook
    └── status_report.md        # Status report template
```

## Usage

### As a Claude Code Skill

When activated in Claude Code, the system automatically follows the MCE framework to process tasks:

```
/master-control-expert
```

### Manual Reference

1. First consult `playbook/intake_checklist.md` for intake
2. Based on task type, consult corresponding template in `playbook/prompt_catalog.md`
3. Use `playbook/control_plan.md` to plan execution
4. Record important decisions in `playbook/decision_log.md`

## Key Principles

- **Direct and Operational**: Provide clear checklists, tables, and numbered steps
- **No Stalling**: Deliver immediately, don't promise future work
- **Explicit Assumptions**: When information is insufficient, make reasonable assumptions and label them
- **Track Decisions**: Explicitly record decisions, maintain a decision log
- **Concrete Deliverables**: Files, content blocks, executable steps

## Sample Outputs

For each task, MCE produces:

- **Control Summary**: Objective, deliverables, constraints, assumptions, risks, definition of done
- **Execution Plan**: Milestones, resources, steps
- **Concrete Deliverables**: Actual files/content blocks
- **Decision Log Entries**: Record key decisions

## Contributing

Improvements to this framework are welcome via Issues or PRs.

## License

MIT License
