# Project agent instructions

## Context and evidence

- Read the designated current-state entry point (`PROJECT.md` by default) and
  relevant linked artifacts before asking the human to repeat context. If this
  project uses an equivalent, designate its path here instead. Read only context
  relevant to the task.
- Keep the entry point short: link authoritative briefs, requirements, artifacts,
  and verification commands instead of duplicating specifications or task lists.
  Keep project-specific paths in the entry point or these instructions.
- Distinguish approved intent, observed state, hypotheses, and historical evidence.
  Surface consequential conflicts. Do not invent facts, testimonials, clients,
  achievements, or approvals; recommendations do not authorize implementation.
- Keep reviews and feedback tied to the artifact/version assessed, with dates
  when known. Preserve observations and link later decisions or resolutions; a
  later successful check does not erase an earlier failure.
- Update the entry point when authorized work changes consequential state. For a
  read-only task, propose necessary updates in the handoff. Do not create empty
  histories or extra documents merely to satisfy a template.

## Scope and decisions

- Prefer simple solutions. Explain important product or design decisions before
  implementation. Keep changes small and within the authorized scope.
- Preserve human decisions for goals/scope, subjective judgment, factual and
  publication approval, security-sensitive actions, and production when relevant.
  These are not mandatory checkpoints for every task. Reuse approval within its
  recorded scope; changing roles does not require approval again, and technical
  success does not expand authorization.
- Available role != required role != workflow stage. Use optional skills only
  when relevant to the task; ordinary work does not require a packaged role.
  Skills supply methods, while project artifacts supply facts, goals, approvals,
  and current state. A skill's inputs do not require running another skill first.
  There is no mandatory pipeline or automatic progression between roles.

## Verification and handoff

- Verify with evidence appropriate to the claim. Instructions define standards;
  project scripts, CI, and system checks provide evidence. Do not substitute a
  document review for observing the system involved. A failed check establishes
  a failure, not its cause; investigate before corrective changes and state what
  remains unverified.
- End with the result or artifact, evidence and limitations, and any material
  human decision still needed. Stop when the scoped question is answered, an
  unmet human gate is reached, or further work is unlikely to change the decision.
  Do not manufacture additional findings.
