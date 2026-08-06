# Matt Pocock Skills

Upstream: `mattpocock/skills`

Pinned upstream commit observed during bootstrap: `2ab958093e83e0ec752e6c1c5932da465bf23e0c`

Promoted upstream plugin version observed during bootstrap: `1.2.0`

Pinned `skills` installer version: `1.5.20`

## Installation

The canonical reproducible bootstrap is `.github/workflows/bootstrap-matt-pocock-skills.yml`. It clones the upstream repository, checks out the exact pinned commit, and installs the exact promoted skill set using the pinned installer version.

For a local equivalent, use the same pinned source checkout and run:

```bash
npx skills@1.5.20 add /path/to/pinned/mattpocock-skills \
  --agent codex --copy --yes \
  --skill <each promoted skill listed by the bootstrap workflow>
```

Do not replace the pinned source or installer with `latest` in a reproducibility-sensitive workflow.

The repo-local installation is intentional: skills are versioned with this project and may later be adapted where the research harness needs stricter scientific behavior.

The `setup-matt-pocock-skills` repository configuration is:

- Issue tracker: GitHub Issues for `wswitzer/awakening-tracker`
- Domain layout: single-context (`CONTEXT.md` + `docs/adr/`)
- Root agent instructions: `AGENTS.md`
- Default triage labels: `needs-triage`, `needs-info`, `ready-for-agent`, `ready-for-human`, `wontfix`

The concrete setup files are under `docs/agents/`.

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

Do not silently update upstream skills or the installer during an in-progress confirmatory research protocol. Either can alter agent behavior and therefore affect reproducibility. Record the previous and new upstream versions/commits and installer version, run harness regression evals, and promote the update deliberately.
