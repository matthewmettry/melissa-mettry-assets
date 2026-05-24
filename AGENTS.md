# AGENTS.md - Melissa Mettry Assets

This repository stores public assets and lightweight workflow files for the Melissa Mettry Instagram pipeline.

## Source Of Truth

- Linear is the task source of truth.
- GitHub is the code review and merge source of truth.
- Work from one Linear issue at a time.

## Branches

- Use the Linear-generated branch name when available.
- Use one branch per Linear issue by default.
- Do not mix unrelated issues into this repo just because the file change is small.

## Scope

- Do not change published post assets unless the Linear issue explicitly asks for it.
- Treat `post-*` folders and `dashboard/dashboard-data.json` as user-facing output.
- Preserve unrelated local changes and generated files.

## Pull Requests

PR titles should start with the Linear issue ID, for example:

`LIN-28: Prove Linear-to-agent-to-PR pilot`

PR bodies must include:

- Linear issue link
- Acceptance criteria checklist
- Files changed
- Verification performed
- Risks or follow-up issues

## Verification

For documentation-only changes, verify with:

```powershell
git status --short
```

For asset changes, also verify the changed files render or load as expected before moving the Linear issue to Done.

## Handoff

Before finishing, add a Linear comment with:

- Branch or PR link
- What changed
- Verification evidence
- Any blocker or decision needed
