# Hemphill Counseling Services — Agent Handoff
## "Ready to Begin" Section Redesign

**Date:** April 1, 2026
**Status:** Planning complete. No code has been written. Next agent picks up at execution.

---

## What Was Decided

The "Ready to Begin" section (the final section of the homepage) needs a full content and layout revision. Carlton and the previous agent worked through every element. Here is what was agreed:

### Drop Entirely
- **"No free consults."** — Gone. No replacement. No softened version.
- **All "no phone calls" language from the website.** — "No phone calls necessary" is now Instagram-only per updated brand guidelines. It should not appear anywhere on the website, including buttons, body copy, or CTAs. The current button labeled "BOOK NOW — NO PHONE CALLS" needs to be replaced.

### CTA Structure — Replace Single Button With Three Paths

The current single "Book Now" button routes to Linktree, which then routes to insurance or self-pay. This is being replaced with direct paths:

| Path | Platform | Audience | Treatment |
|---|---|---|---|
| Using insurance | Headway | Prospective therapy clients | Primary CTA button |
| Self-pay | SimplePractice portal | Prospective therapy clients | Primary CTA button (equal weight to Headway) |
| Supervision / Consultation | Email Carlton directly | Clinicians | Quieter — text link, not a button |

Carlton has the direct URLs for Headway and SimplePractice. The next agent should ask for them before writing any href values.

The contact form (SimplePractice widget) was considered and ruled out for this section. It is built for prospective therapy clients only and would not serve the supervision/consultation audience. Email covers both audiences more cleanly.

### Photo
- Carlton's suit photo should be added to this section.
- This photo is **not currently in the HTML file** — Carlton needs to provide it.
- Placement: somewhere in the section that anchors trust before the booking click. Exact layout TBD based on what works with the new structure.
- Do not use the flannel/bookshelf headshot or the Chicago skyline headshot for this section.

### Step-by-Step Process — Rewrite for Accuracy

The current 1-2-3 steps are inaccurate. The real client-facing sequence is:

1. Choose your path (insurance via Headway, or self-pay via SimplePractice)
2. Enter your information and select an available appointment time
3. You're booked. Carlton receives a notification, confirms, and sends paperwork.

The paperwork packet (GFE if self-pay, Informed Consent, Practice Policies, GAD-7, PHQ-9, biopsychosocial assessment, credit card authorization, AI consent form) is substantial but does not need to be listed on this page. A line like "You'll receive everything you need before your first session" is sufficient. Do not itemize it in the website copy.

### Copy Fixes (Existing Issues to Correct)
- **Grammar error in Step 3:** "We reviews your intake, asks follow-up questions" — fix to "Carlton reviews" or "I review" (confirm voice preference with Carlton)
- **Em dashes in body copy:** Brand guidelines prohibit em dashes. Current body copy contains two. Rewrite to remove them.
- **Redundant second book button:** Currently there is a "BOOK A SESSION" button on the left and a "BOOK NOW — NO PHONE CALLS" button on the right. With the new three-path CTA structure, this redundancy is resolved naturally.

---

## What Is Not Decided Yet

- Exact layout of the redesigned section (photo placement, card vs. no card, etc.)
- Whether the 1-2-3 step format is kept or replaced with something else
- First-person vs. third-person voice in the step descriptions
- Carlton has not yet uploaded the suit photo or the updated HTML file

---

## Files

| File | Status | Notes |
|---|---|---|
| `HCS_Brand_Guidelines.md` | Updated | Section 9 revised — "No phone calls necessary" is now Instagram-only |
| `hemphill-website-v3_1.html` | Not yet uploaded | Carlton will provide; this is the active file to edit |
| Suit photo | Not yet provided | Required before execution |

---

## Next Steps for the Incoming Agent

1. Ask Carlton to upload `hemphill-website-v3_1.html`
2. Ask Carlton to upload the suit photo
3. Ask Carlton for the direct Headway URL and SimplePractice booking URL
4. Confirm first-person vs. third-person voice preference for the step descriptions
5. Propose a layout for the redesigned section before writing code
6. Make surgical edits to the existing HTML file only — do not rebuild from scratch

---

## Standing Project Rules (Do Not Violate)

- **Never rebuild from scratch.** Carlton's strong preference is surgical edits to the existing file.
- The active file is a single-file HTML with base64-encoded images. Keep it that way.
- Carlton pushes to GitHub manually via VS Code terminal. Do not attempt to use Claude Code, gh CLI, or any automated git workflow.
- Netlify auto-deploys from the `main` branch of `github.com/hemphillcounselingservices/hemphill-counseling`.
- A `git-workflow.md` file exists in the project root — load it if Claude Code is ever invoked.

---

## Blog — Separate Initiative, Not Started

Carlton also wants to start a blog. This was flagged at the end of the session but not discussed. It is a separate initiative from the "Ready to Begin" redesign. The incoming agent should address the website section first, then open a separate planning conversation about the blog.
