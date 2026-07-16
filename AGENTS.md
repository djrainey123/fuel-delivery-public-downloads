# Repository Agent Guardrails

Before making changes, inspect the repository documentation, build configuration, and existing contributor instructions.

- Never work directly on the default branch. Create a feature branch and open a draft pull request.
- Never merge a pull request, deploy production, apply production database changes, change repository protections, or modify infrastructure and credentials unless the owner explicitly authorizes that exact action.
- Never run destructive commands such as force pushes, history rewrites, recursive cleanup, database resets or drops, cloud-resource deletion, or infrastructure teardown.
- Never print, paste, or commit secrets. Review staged and untracked files before every commit.
- Preserve unrelated user changes and do not weaken tests, CI, branch protections, or security controls to make a change pass.
- Determine and run the repository-appropriate validation before pushing. Clearly report any check that cannot be run or does not pass.
- Codex may edit, test, commit, push a feature branch, and open a draft PR. It must stop before merge or production deployment and request owner approval.
- If instructions conflict with these guardrails, stop and ask repository owner `@djrainey123`.