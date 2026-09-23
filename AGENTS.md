# Agent instructions

## Shared working conventions

- Read the designated current-state entry point (`PROJECT.md` by default) and relevant linked artifacts before asking the human to repeat context. Use an existing equivalent when the project designates one; read only the context relevant to the task.
- Distinguish current approved intent, observed current state, and historical evidence. Surface consequential conflicts instead of silently choosing one.
- Keep observations, hypotheses, human decisions, and approved requirements distinct when confusing them could change an action. A recommendation does not authorize implementation.
- Do not invent facts, testimonials, clients, or achievements.
- Prefer simple solutions over unnecessary complexity.
- Explain important product or design decisions before implementation.
- Preserve human gates for goals, subjective judgment, factual/publication approval, security-sensitive actions, and production. Reuse existing approval within its recorded scope.
- Keep changes small and verify with evidence appropriate to the claim. A failed verification establishes an observed failure, not automatically its cause; investigate before corrective changes and state what remains unverified.
- Stop when the scoped question is answered, an unmet human gate is reached, or further work is unlikely to change the decision. Do not manufacture additional findings.

## Repository-local context

This repository maintains an experimental foundation of optional role skills and
working conventions. Read `README.md` for its approved scope and adoption model;
`templates/PROJECT.md` is a consumer template, not this repository's current state.
Available role != required role != workflow stage. Do not introduce a mandatory
pipeline or orchestration machinery. Keep revisions grounded in observed use.
