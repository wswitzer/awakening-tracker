# Domain Documentation

This is a single-context repository.

- Canonical domain vocabulary lives in root `CONTEXT.md`.
- Durable, hard-to-reverse architectural decisions live under `docs/adr/`.
- `CONTEXT.md` is a glossary, not an implementation plan or scratchpad.
- Agents must read the relevant domain terms and ADRs before changing behavior that depends on them.

Create ADRs sparingly: only for decisions that are hard to reverse, surprising without context, and the result of a real trade-off.
