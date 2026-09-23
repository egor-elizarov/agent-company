# Bootstrap and repository instructions

This file governs work inside agent-company. Read `README.md` for its human-facing
purpose. Apply the working conventions in `templates/AGENTS.md` to your own work;
its `PROJECT.md` default concerns consuming projects. This repository's scope is
recorded here and in README, not in `templates/PROJECT.md`.

## Bootstrap contract

Bootstrap creates or adapts a target project's AI foundation. It authorizes
instructions, project context, and selected skills, not product implementation.
Never copy this root AGENTS.md into a consuming project. Use
`templates/AGENTS.md` as the portable source instead.

The target must work without this checkout or its Git history. Do not add links,
symlinks, or instructions requiring access to agent-company. Do not record the
source revision or introduce version/update metadata by default.

## Inspect and choose

1. Establish the target directory and project purpose from the request and
   available context. Ask only for missing information that affects setup.
   Prefer a target outside this checkout to avoid inherited maintenance rules;
   if the requested location would inherit them, resolve that location with the
   human before setup.
2. Inspect the target before writing: applicable instructions (including parent
   and nested scopes), README, current project context, existing skills, and
   relevant local changes. If a supposedly new target contains useful material,
   follow the existing-project procedure below.
3. Choose the minimal set of skills justified by known project needs. The human
   may explicitly request all skills, no skills, or specific skills. Do not copy
   every available skill merely because it exists. Read selected SKILL.md files
   to confirm their scope; no skills is a valid outcome. Check that the intended
   agent environment supports their format; report unresolved compatibility.
4. Explain consequential context and skill choices before writing. Reuse the
   setup authorization for routine additive changes. Surface consequential
   conflicts for human decision; do not silently replace local policy.

## New project

- Create target AGENTS.md by adapting `templates/AGENTS.md` to the project.
- Populate PROJECT.md from `templates/PROJECT.md` with known facts, actual human
  decisions, and relevant unknowns. Remove template guidance and omit unused
  sections. Do not invent requirements, approvals, verification results, or an
  application scaffold.
- Add selected skills and complete the verification and handoff below.

## Existing project

- Preserve useful AGENTS.md content and applicable instruction scopes. Merge only
  missing, relevant conventions from `templates/AGENTS.md`; recognize equivalent
  wording instead of appending duplicates. Create AGENTS.md only if needed.
- Reuse an existing project-context entry point when suitable and designate its
  target-local path in AGENTS.md. Preserve the project's brief and authoritative
  documents; link them rather than duplicating their contents. Create PROJECT.md
  only when no suitable entry point exists, and add only missing context.
- Preserve local edits, decisions, historical evidence, and unrelated files. Do
  not rewrite goals or reorganize application code as part of adoption.
- Inspect skill-name collisions. Leave identical skills unchanged; preserve
  modified or different same-name skills and compare them before proposing a
  replacement. Ask for a decision when the collision has consequential effects.
- Repeated adoption should add only what is still missing, without duplicate
  rules, context documents, or skill copies.

## Skills and attribution

Copy selected complete folders from `.agents/skills/` into the target's
`.agents/skills/`, preserving SKILL.md names and scope. Skills provide methods;
project context provides facts and approvals. Available role != required role !=
workflow stage. Inputs do not require running another skill first. Do not run
selected skills as a side effect of copying them.

Preserve applicable LICENSE and NOTICE material locally with copied content,
using the target's existing third-party notice convention when available. Do not
replace the target's own license or imply it licenses the whole target project.
Attribution does not require source-revision tracking or access to this checkout.

## Verify and hand off

Review the target changes for preserved instructions, duplicates, unresolved
conflicts, valid local context links, and complete selected skill folders. Check
that the resulting instructions contain no agent-company maintenance context or
source-checkout dependencies. Distinguish static checks from actual agent-runtime
verification; do not claim discovery or execution that was not tested.

Report what was created, adapted, or preserved; selected skills and reasons;
verification and limits; and any material open decision. Tell the human to open
the target directory and start a fresh agent session there, reading its AGENTS.md
and designated context entry point. Stop after foundation setup; do not begin
product implementation or automatically progress to another role.

## Maintaining this repository

This is an experimental foundation extracted from one project. Cross-project
portability and effectiveness remain unproven. Keep revisions grounded in observed
use, and keep portable conventions in templates rather than this local contract.
The five skills are optional product, content, interface design, critique, and
owner-feedback methods; they do not supply implementation or operational roles.

Do not introduce an installer, CLI, orchestrator, registry, workflow engine,
automatic routing, or a mandatory pipeline. Review changes for consistency across
README, bootstrap instructions, and portable templates. Preserve skill scope and
avoid turning available capabilities into required stages.
