# Awakening Tracker Agent Instructions

This repository is a scientific research system first and a software project second. Agents must preserve methodological rigor, provenance, reproducibility, and the ability to falsify the project's central hypothesis.

## Required reading

Before material work, read:

1. `RESEARCH_CONSTITUTION.md`
2. `CONTEXT.md`
3. Relevant ADRs under `docs/adr/`
4. Relevant issue and its blockers
5. Relevant repo-local skills under `.agents/skills/`

## Agent skills

### Issue tracker

Work is tracked in GitHub Issues for `wswitzer/awakening-tracker`. See `docs/agents/issue-tracker.md`.

### Triage labels

Use the canonical triage vocabulary described in `docs/agents/triage-labels.md` when available.

### Domain docs

This is a single-context repository. Domain terminology lives in root `CONTEXT.md`; durable architectural decisions live in `docs/adr/`. See `docs/agents/domain.md`.

## Operating rules

- Never assume spiritual awakening is increasing. Treat increase, decrease, null, mixed, and alternative-explanation outcomes as legitimate.
- Distinguish observation, derived measure, statistical inference, and interpretation.
- Never alter a frozen research protocol because of observed result direction.
- Prefer primary sources and retain machine-resolvable provenance for material claims.
- Missing or uncertain data must remain visibly missing or uncertain unless an explicit protocol defines imputation.
- Counterevidence must be preserved and surfaced.
- Scientific/governance rules outrank implementation convenience.
- Work in bounded, verifiable increments. Do not mark work complete until acceptance criteria and relevant checks pass.
- Record reusable failures as evals rather than merely adding more prose instructions.
- Reflection may propose harness improvements; the proposing model may not unilaterally credit or promote its own improvement.
- New methodology discovered after outcome exposure must create a new explicit protocol version; preserve the prior analysis.
- Use fresh-context adversarial review for major research milestones.

## Matt Pocock skills

Repo-local copies of the relevant Matt Pocock skills belong under `.agents/skills/`. Use them according to their own `SKILL.md` instructions. The project pins the upstream source in `docs/agents/matt-pocock-skills.md`.

Default routing:

- uncertain multi-session decision space -> `wayfinder`
- external evidence gathering -> `research`
- terminology and domain boundaries -> `domain-modeling`
- convert understood work into a specification -> `to-spec`
- break approved work into dependency-aware tracer bullets -> `to-tickets`
- implementation -> `implement`, with `tdd` and `code-review` as appropriate
- context boundary -> `handoff`
- authoring or improving project-specific skills -> `writing-great-skills`
