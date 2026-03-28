# Hemphill Counseling Services — Agent Handoff Summary

## Project Overview
Carlton Hemphill is building a single-file HTML website for **Hemphill Counseling Services**. The site needs to be professional, credible, and work reliably across devices. The active file is `hemphill-website-v3_1.html`.

---

## Current State

### Infrastructure
- **GitHub repo**: `github.com/hemphillcounselingservices/hemphill-counseling` (exists)
- **Netlify**: Connected to the GitHub repo (auto-deploys on push to `main`)
- **Local project path**: `C:\Users\carlt\OneDrive\Documents\Claude\Projects\Website`

### Git Status (as of this handoff)
- Branch: `main` only (two orphaned Claude Code branches were deleted this session)
- Worktrees: Root only — clean
- One orphaned folder remains at `.claude\worktrees\naughty-heisenberg` that could not be deleted because a process had it locked. Carlton is restarting his computer to release the lock and will delete it manually after restart.

### HTML File
- The current working file `hemphill-website-v3_1.html` is **local only** — it has NOT been pushed to GitHub yet
- The GitHub repo contains an outdated version of the site
- Next step after cleanup: upload the current HTML file, verify it, then push to GitHub so Netlify deploys the correct version

---

## Workflow (Agreed Upon)
**GitHub + Netlify auto-deploy** is the chosen long-term workflow:
1. Edit file (in Claude chat or Claude Code)
2. Commit to `main`
3. Push to `main`
4. Netlify auto-deploys

### Critical Rules for Claude Code
A file called `git-workflow.md` has been created and should be placed in the project root. Carlton loads it at the start of every Claude Code session by saying:
> "Read git-workflow.md and follow those rules for this session."

Key rules in that file:
- No branches, no worktrees, no PRs, no `gh` CLI
- All commits go directly to `main`
- Push pattern: `git add` → `git commit` → `git push origin main`

---

## What Went Wrong Previously
- Claude Code defaulted to a team-developer workflow: creating branches, worktrees, and pull requests
- The `gh` CLI was not installed, causing `command not found` errors
- This created nested/orphaned worktrees and branches that had to be manually cleaned up
- Framer was attempted earlier and abandoned due to layout/responsiveness failures at breakpoints
- GitHub was previously ruled out due to these issues but has now been reinstated as the correct approach with proper configuration

---

## Site Assets
- Logo
- Two headshots:
  - Flannel/bookshelf photo → hero section
  - Chicago skyline photo → about section
- Two credential badges: NCC and BC-TMH
- Images are embedded as base64 in the HTML for a self-contained single file

## Features In Progress / Planned
- Base64-encoded images embedded directly in HTML
- Responsive breakpoints at 1200 / 900 / 600px
- Mobile hamburger menu
- Looping insurance company name ticker (Aetna, Cigna, etc.)

---

## Carlton's Preferences
- **Never rebuild the whole site for minor changes** — surgical edits to the existing file only
- Works directly in Claude chat (not Claude Code) for most edits
- Deploys via Netlify drag-and-drop OR GitHub push (now that the workflow is clean)
- Prefers self-contained single HTML files over multi-file setups
- Wants durable long-term solutions discussed before diving into fixes

---

## Immediate Next Steps
1. Carlton restarts computer and deletes `.claude\worktrees\naughty-heisenberg` manually
2. Carlton uploads `hemphill-website-v3_1.html` to Claude chat
3. Agent verifies file is in good shape
4. Carlton pushes the file to the `main` branch on GitHub (via GitHub website or terminal)
5. Confirm Netlify deploys correctly
6. Resume planned feature work (images, responsive breakpoints, hamburger menu, ticker)
