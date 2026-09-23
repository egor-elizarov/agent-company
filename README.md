# agent-company v0.1

An experimental foundation for human-directed, agent-assisted project work:
shared working conventions, a current-state template, and five optional skills.
It was extracted from one completed project. Cross-project portability, reduced
total effort, and superiority over one agent changing roles remain unproven.

**Available role != required role != workflow stage.**

The starter library provides capabilities, not a prescribed team or sequence.
Use only roles relevant to the current problem. Ordinary work does not require a
packaged role. The human still selects work and makes consequential decisions.

## Adopt manually

1. Merge the **Shared working conventions** section of [AGENTS.md](AGENTS.md)
   into your project's instructions. Preserve existing local instructions; do not
   copy the repository-local maintenance section.
2. Copy [templates/PROJECT.md](templates/PROJECT.md) to your project's `PROJECT.md`
   and fill in the relevant sections. Alternatively, designate an existing
   equivalent in your AGENTS.md. Keep project-specific paths there.
3. Copy only the needed skill folders from `.agents/skills/` into the same location
   in your project. Preserve their `SKILL.md` names and scope. Use an environment
   that supports this skill format; these files do not install an agent runtime.
4. Record the source revision in your project so later updates can be reviewed
   deliberately. There is no automatic synchronization. Preserve applicable
   [license](LICENSE) and [attribution](NOTICE) material when redistributing.

## Current state and historical evidence

`PROJECT.md` is a short entry point, not a duplicate specification or task database.
Link to the current brief, approved requirements, artifacts, and verification
commands rather than copying their contents. Identify approved intent separately
from observed state, with dates or versions where relevant.

Keep historical feedback and reviews tied to the artifact or version assessed.
Preserve original observations and link later decisions or resolutions. A later
successful check does not rewrite an earlier failure. An agent may record a human
decision but must not promote its own recommendation into approval.

Update the entry point when authorized work changes consequential state. A
read-only task can propose an update in its handoff without writing it. Do not
create empty histories or additional documents merely to satisfy a template.

## Optional role library

| Skill | Demonstrated responsibility |
| --- | --- |
| [product-design](.agents/skills/product-design/SKILL.md) | Product/UX goals, journeys, priorities, and material open questions. |
| [content-design](.agents/skills/content-design/SKILL.md) | Website copy grounded in sources, attribution, and publication boundaries. |
| [interface-design](.agents/skills/interface-design/SKILL.md) | Web/interface visual direction, responsive behavior, and accessibility criteria. |
| [interface-critique](.agents/skills/interface-critique/SKILL.md) | Evidence-based critique of visual/interface direction; no universal review mandate. |
| [user-feedback](.agents/skills/user-feedback/SKILL.md) | Owner feedback on an experienced artifact, distinct from target-user research. |

The interface names clarify scope; they do not broaden the original visual roles.
Skills describe methods. Project artifacts supply facts, goals, approvals, and
current state. One skill's input does not require running another skill first.

## Short invocations

Supply the role, bounded question, output destination, and any exceptional limits.
Standing instructions supply the context-reading behavior. Examples are independent:

- “Use product-design to propose the smallest useful first version. Write to
  `docs/product-direction.md`. No implementation.”
- “Use interface-critique to review the current candidate. Report findings only.”
- “Use user-feedback for candidate 1; record the completed checkpoint in the
  designated feedback artifact.”

End a task with the result or artifact, evidence and limitations, and any material
human decision still needed. Do not automatically start another role.

## Human gates

Keep goals/scope decisions, subjective judgment, factual/publication approval,
security-sensitive authorization, and production/publication authorization explicit
when relevant. These are not mandatory checkpoints for every task. Reuse approval
within its recorded scope; changing roles does not require approval again, and
technical success does not expand authorization.

## Verification and limits

Instructions establish evidence standards. Project-specific scripts and CI enforce
concrete invariants; git preserves changes and release identities; external checks
establish actual service behavior. Do not substitute a document review for evidence
from the system involved. A failed check establishes a failure, not its cause;
investigation may justify no corrective change.

v0.1 contains no orchestrator, automatic routing, workflow engine, installer, role
registry, mandatory pipeline, deployment conventions, or automatic retries.
Implementation, release, infrastructure, security, and generic review skills are
not included. Test this foundation through a different project before expanding it.

## Origin

Agent Company grew out of the EGTEC project, where specialized AI roles were
used to take a real product from initial exploration through implementation
and release.

v0.1 extracts the practices that proved useful in that experiment into a small,
reusable starting point. It is intentionally experimental and will evolve as
those practices are tested across different projects.
