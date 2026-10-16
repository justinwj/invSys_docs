# invSys documentation agent instructions

These instructions apply to this documentation repository. Read the shared
instructions in `../invSys_fork/AGENTS.md` before editing; they define architectural
precedence, the required specification/plan/handoff read order, evidence handling,
and the handoff policy for both repositories. Resolve pointers within this
repository; do not select a specification, plan or handoff by timestamp.

## GitHub contribution workflow

The user confirmed this workflow on 2026-10-16; it persists across chats:

- Pull upstream changes from `soetrain/invSys_docs`, branch `main`, using remote
  `origin`. The sibling code repository pulls from `soetrain/invSys_fork`.
- Publish feature branches to the authenticated contributor's corresponding
  `justinwj` repository using remote `fork`, then create or update a PR targeting
  **soetrain's matching repository, branch `main`**. These fork pushes and PRs are
  authorized parts of this workflow. A branch push alone is not completion.
- Preserve local work and merge fetched `origin/main` into the active feature
  branch when needed. Do not rebase published history, force-push or discard
  divergent local-only commits. Local `main` tracks `origin/main`.
- The GitHub CLI default repository is `soetrain/invSys_docs` here and
  `soetrain/invSys_fork` in the code repository. Default pushes go to `fork`;
  feature branches may track their published fork branch. An unqualified pull on
  such a branch does not necessarily pull soetrain's latest `main`.
- Incomplete work stays in a draft PR with its open gates stated. Soetrain
  reviews/merges, then pulls from his own account. Do not merge, enable auto-merge
  or push directly to soetrain `main` without separate explicit instructions.
- Before ending, verify the upstream PR base/head and published commit, review
  Git status, and report the PR links or an actual blocker.
