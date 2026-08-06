# Matt Pocock Skills

Upstream: `mattpocock/skills`

Pinned upstream commit observed during bootstrap: `2ab958093e83e0ec752e6c1c5932da465bf23e0c`

Promoted upstream plugin version observed during bootstrap: `1.2.0`

## Installation

Install repo-local copies from the repository root with:

```bash
npx skills@latest add mattpocock/skills
```

The repo-local installation is intentional: skills should be versioned with this project and may be adapted where the research harness needs stricter scientific behavior.

After installation, run the `setup-matt-pocock-skills` skill once for this repository and preserve the following configuration:

- Issue tracker: GitHub Issues for `wswitzer/awakening-tracker`
- Domain layout: single-context (`CONTEXT.md` + `docs/adr/`)
- Root agent instructions: `AGENTS.md`
- Default triage labels: `needs-triage`, `needs-info`, `ready-for-agent`, `ready-for-human`, `wontfix`

## Skills expected to be used by this project

- `wayfinder` — multi-session uncertain decision spaces
- `research` — primary-source evidence gathering
- `domain-modeling` — maintain canonical research/harness language
- `to-spec` — convert understood decisions into implementation specifications
- `to-tickets` — produce dependency-aware tracer-bullet issues
- `implement` — execute bounded issues
- `tdd` — behavior-first implementation where applicable
- `diagnosing-bugs` — systematic failure diagnosis
- `code-review` — independent implementation review
- `handoff` — preserve context across agent-session boundaries
- `writing-great-skills` — author project-specific scientific-agent skills

## Update policy

Do not silently update upstream skills during an in-progress confirmatory research protocol. Skill updates can alter agent behavior and therefore may affect reproducibility. Record the previous and new upstream versions/commits, run harness regression evals, and promote the update deliberately.
