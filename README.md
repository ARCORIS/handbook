<div align="center">

# ARCORIS Handbook

**Engineering and documentation operating handbook for the ARCORIS ecosystem.**

[![Start Here](https://img.shields.io/badge/Start-Handbook%20Index-0F766E?style=flat)](docs/index.md)
[![Operating Rules](https://img.shields.io/badge/Scope-Engineering%20%26%20Documentation%20Rules-1D4ED8?style=flat)](https://github.com/ARCORIS/handbook)

[Core Platform](https://github.com/ARCORIS/arcoris) · [Docs](https://github.com/ARCORIS/docs) · [Community](https://github.com/ARCORIS/community) · [Enhancements](https://github.com/ARCORIS/enhancements) · [Examples](https://github.com/ARCORIS/examples)

Policies · Standards · Workflows · Quality Gates · Release · Security · Templates

**Overview:** [Purpose](#purpose) · [Start here](#start-here) · [Intended audiences](#intended-audiences)

**Scope:** [What belongs here](#what-belongs-here) · [What does not belong here](#what-does-not-belong-here) · [Source of truth](#source-of-truth-policy)

**Structure:** [Repository map](#repository-map) · [Section map](#section-map) · [Handbook principles](#handbook-principles)

**Repository:** [Contributing](#contribution-expectations) · [Repository status](#repository-status)

</div>

---

## Purpose

This repository is the **operating handbook** for ARCORIS.

It exists to define how engineering and documentation work should be structured, reviewed, approved, released, and maintained across the ecosystem.

This repository is not public product documentation and it is not a generic policy dump. It is the canonical home for **working rules, standards, workflows, quality gates, and reusable templates**.

## Start here

Use the [Handbook Index](docs/index.md) as the primary entry point for handbook navigation, reading order, and section-based access paths.

The index defines how the handbook should be explored across overview, documentation, engineering, workflow, quality, release, security, incident management, and templates.

## What belongs here

Use this repository for material that defines **how ARCORIS work is done**.

Typical content includes:

- engineering and documentation policies;
- writing, naming, metadata, and diagram standards;
- architecture boundary rules and design guidelines;
- workflow, review, and definition-of-done rules;
- quality gates, testing strategy, reliability, and SLO guidance;
- release, versioning, compatibility, rollback, and deprecation policy;
- security, dependency, secrets, and vulnerability management policy;
- incident response, severity, escalation, postmortem, and runbook standards;
- reusable templates and checklists used by multiple repositories.

## What does not belong here

This repository must not absorb responsibilities that belong elsewhere.

The following should live outside this repository:

- canonical public system explanation, user-facing concepts, and stable architecture narratives;
- governance, roles, ownership, meetings, and community coordination;
- proposal-specific design alternatives, change records, and decision lifecycle tracking;
- runnable examples, environment baselines, demos, and scenario material;
- implementation-near technical documentation that belongs next to source code.

If a rule becomes part of the working model of the ecosystem, it should be captured here. If a topic explains the public system, proposes a change, or demonstrates runtime behavior, it should remain in the repository that owns that responsibility.

## Repository map

ARCORIS uses multiple repositories with different responsibilities. This repository is only one layer of that system.

### Core platform

| Repository | Role |
| --- | --- |
| [Core Platform](https://github.com/ARCORIS/arcoris/blob/main/README.md) | Main code repository for the platform |

### Documentation ecosystem

| Repository | Role |
| --- | --- |
| [Docs](https://github.com/ARCORIS/docs/blob/main/README.md) | Public documentation and canonical system explanation |
| Handbook (this repository) | Engineering and documentation operating rules |
| [Community](https://github.com/ARCORIS/community/blob/main/README.md) | Governance, roles, coordination, and contributor growth |
| [Enhancements](https://github.com/ARCORIS/enhancements/blob/main/README.md) | Major proposals, accepted changes, and decision history |
| [Examples](https://github.com/ARCORIS/examples/blob/main/README.md) | Runnable examples, baselines, demos, and scenario material |

This repository should define operational rules for the ecosystem without taking over the responsibilities of the repositories those rules govern.

## Section map

The handbook is organized into a small set of durable sections.

| Section | Role |
| --- | --- |
| [Overview](docs/overview/index.md) | Mission, scope, glossary, repository boundaries, and source-of-truth rules |
| [Documentation](docs/documentation/index.md) | Documentation standards, writing rules, diagrams, metadata, requirements, and information architecture |
| [Engineering](docs/engineering/index.md) | Engineering principles, architecture boundaries, API design, observability, dependencies, configuration, and performance guidance |
| [Workflow](docs/workflow/index.md) | Contribution flow, branching, commits, reviews, issue triage, planning, and definition of done |
| [Quality](docs/quality/index.md) | Testing strategy, quality gates, reliability rules, SLO/SLI guidance, and failure-injection policy |
| [Release](docs/release/index.md) | Versioning, release, changelog, deprecation, rollback, and compatibility policy |
| [Security](docs/security/index.md) | Security principles, access control, dependency security, secrets, threat modeling, vulnerability management, and release security |
| [Incident Management](docs/incident-management/index.md) | Incident response, severity model, escalation, on-call policy, postmortems, and runbooks |
| [Templates](docs/templates/index.md) | Reusable templates and checklists referenced by handbook standards and processes |

Detailed navigation and reading order should be defined in the [Handbook Index](docs/index.md) and in the section index pages themselves, not in this root README.

## Intended audiences

This repository serves several audiences:

- **maintainers** who define and enforce working rules across repositories;
- **contributors** who need to understand how changes should be prepared and reviewed;
- **documentation authors** who need consistent standards, templates, and lifecycle rules;
- **engineers** who need shared expectations for boundaries, quality, observability, release, and security;
- **reviewers and operators** who need repeatable checklists, policies, and process guidance.

Because these audiences differ, the handbook should prioritize **clarity, actionability, and boundary discipline** over narrative depth.

## Source-of-truth policy

This repository should hold the canonical explanation of the **current operating model** for ARCORIS.

That means:

- active working rules should be documented here;
- shared standards and templates should live here;
- review, release, security, quality, and incident processes should not remain implicit or scattered across repositories;
- adopted operating practices should be updated here when they change.

If a topic exists in multiple forms, the boundary is simple:

- **operating rule, policy, standard, checklist, or template** -> [Handbook](https://github.com/ARCORIS/handbook)
- **stable public system explanation** -> [Docs](https://github.com/ARCORIS/docs)
- **proposed change or decision history** -> [Enhancements](https://github.com/ARCORIS/enhancements)
- **governance and coordination** -> [Community](https://github.com/ARCORIS/community)
- **runnable and demonstrative material** -> [Examples](https://github.com/ARCORIS/examples)
- **implementation-near technical detail** -> [Core Platform](https://github.com/ARCORIS/arcoris)

## Handbook principles

Material in this repository should follow a small set of strict principles:

- **One clear source of truth per operational topic.**
- **Rules must be actionable.** Policies and standards should be usable in real review and implementation work.
- **Stable information architecture.** Prefer durable sections over ad hoc policy sprawl.
- **Boundary discipline.** Do not mix public system explanation, governance, proposals, examples, and code-near technical notes into the handbook.
- **Promotion of adopted practice.** Once a working rule is accepted, it should be reflected here explicitly.
- **Templates support standards.** Reusable templates and checklists should reinforce handbook rules rather than compete with them.
- **Docs-as-code rigor.** Handbook content should be reviewable, versioned, traceable, and maintainable like source code.

## Contribution expectations

A good change in this repository usually does one or more of the following:

- clarifies a policy, standard, boundary, or lifecycle rule;
- improves the precision or usability of a shared process;
- reduces ambiguity between repositories and document types;
- strengthens reviewability through checklists, templates, or clearer acceptance criteria;
- aligns written rules with the operating model actually used by the ecosystem;
- removes stale, conflicting, duplicated, or underspecified guidance.

Changes should not move public architecture explanation, governance material, proposal records, runnable examples, or implementation-near technical documentation into this repository.

## Repository status

This repository currently defines the operating boundaries, shared standards, and process surface for ARCORIS.

The repository structure already reflects the major domains of handbook responsibility, with `mkdocs.yml` for site structure and `lychee.toml` for link-check configuration at the root.

As the handbook evolves, section index pages, review discipline, and repository automation should continue to reinforce this repository’s role as the canonical home for ecosystem working rules.
