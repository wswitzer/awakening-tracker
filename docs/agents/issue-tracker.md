# Issue Tracker

This repository uses GitHub Issues in `wswitzer/awakening-tracker` as the canonical work tracker.

## Rules

- Agent-ready implementation work is represented as GitHub issues.
- Issues produced by `to-tickets` declare blockers explicitly.
- Work the frontier: only start an issue whose blockers are complete.
- Do not triage issues created by `to-tickets`; they are already structured for agents.
- PRs are not an independent request surface unless this file is deliberately changed later.

## Wayfinding operations

For `wayfinder`, use a top-level map issue plus linked decision issues. Until native sub-issue/blocking operations are available to the active GitHub tool, record parent and blocking relationships explicitly in issue bodies and keep the roadmap/map issue as the low-resolution index.
