# Git Workflow Instructions

## Core Rule
All changes go directly to `main`. No exceptions.

## What This Means
- Do not create new branches
- Do not create worktrees
- Do not open pull requests
- Do not use the `gh` CLI
- Do not use `git checkout -b` or any branch creation command

## Every Edit Follows This Pattern
1. Make the edit
2. `git add` the changed file(s)
3. `git commit -m "description of change"`
4. `git push origin main`
5. Done

## On Session Start
Before making any edits, confirm:
- Remote origin is pointed at `github.com/hemphillcounselingservices/hemphill-counseling`
- Active branch is `main`
- No orphaned worktrees exist (`git worktree list` should show only the root)

If orphaned worktrees are found, remove them with `git worktree remove` before proceeding.

## If a Push Is Rejected
Do not create a branch. Instead:
1. Run `git pull origin main --rebase`
2. Then push again

## Never Do These
- `gh pr create`
- `git checkout -b`
- `git worktree add`
- Any command that creates a parallel version of the project
