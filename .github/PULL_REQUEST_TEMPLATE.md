<!--
Comply54 PR template · standard: comply-ci/docs/ai/pr-conventions.md · write in English.
Keep it tight; every line should earn its place. The checklist is an accountability record:
tick a box only when it is true, and give a one-line reason for any you leave unchecked.
-->

<!-- Lead: 2-4 sentences. The problem and why it matters now. The story, not a changelog. -->

Closes #

## What changed
<!-- Concrete changes as a short list; group by area if large. -->
-

## Validation
<!-- Proof, not "trust me": commands run + what you saw, screenshots for UI, tests added.
     State what you could not test, and why. -->
-

## Risk & rollback
<!-- Blast radius if this is wrong, and the exact way back: config flip, revert PR, or
     the rollback workflow. Every PR has one, even if "low risk, revert this PR". -->
-

## Config & infra
<!-- Anything outside the code needed for this to work or be safe: env / GitHub Actions
     variables, secrets, DB migrations, dashboard settings, IAM, feature flags.
     Say who applies it and in which environment. "None" if none. -->
-

## Scope & follow-ups
<!-- What this deliberately does NOT do, and deferred work with issue links. -->
-

---
<!-- Accountability checklist. Tick only what is true; a one-line reason for anything unchecked. -->
- [ ] Tests added or updated (or a one-line reason none)
- [ ] Docs / `CLAUDE.md` updated if behaviour or commands changed
- [ ] Config & infra above applied, or listed for the reviewer to apply
- [ ] Targets `dev` (`main` is promotion merges only)
- [ ] Rollback path stated above
- [ ] CI green (or a one-line reason the repo has none)
- [ ] Security-sensitive paths (auth, RLS policies, DB migrations, document visibility) — none, or named here and proven safe in Validation
- [ ] Hard rules hold: RLS stays on; non-validated documents never public — enforced by the DB trigger + deploy gate; prove it above if this PR touches either
- [ ] AI-assisted changes reviewed and tested by hand
