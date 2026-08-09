# CLAUDE.md

Résumé repo. Renders at github.com/CalebEaston. Branch is `master` — never `main`.

## Files & sync

- `README.md` — profile page. Highlights only; one screen. Projects before Experience.
- `RESUME.md` — full résumé; source for the CI-built PDF. One page rendered.
- `PROJECTS.md` — deep-dives (problem → architecture → trade-offs → retrospective).
- `resume.json` — JSON Resume v1 mirror. **Any content change to RESUME.md updates resume.json in the same commit.** README.md gets the condensed version only if it's a highlight.
- `assets/Caleb-Easton-Resume.pdf` — CI-built (on pushes touching RESUME.md, resume.css, or the workflow). Never edit by hand.
- `.ignored/` — gitignored scratch. Drafts and notes go here, never in tracked files.

## Format contract (agents parse this — do not break it)

- Keep the "Note for AI agents and recruiters" blockquotes. Update them if structure changes.
- Reverse-chronological everywhere. Entries: `### Name — one-liner`, bold title/date line, `**Stack:** A · B · C`, then bullets. `·` separators, `MM/YYYY` dates.
- Heading hierarchy is the parse tree: `##` sections, `###` entries. No skipped levels, no decorative headings, no HTML layout tables, no images-as-text.
- `{{PLACEHOLDER}}` marks unfinished content. Never invent facts to fill one; ask or leave it. Before any "done": `grep -r '{{' --exclude-dir=.ignored .` returns nothing.

## Bullet rules

- Past-tense action verb → what → outcome. Number, name, or concrete result in ≥half.
- Banned openers: "Responsible for", "Helped with", "Worked on", "Assisted".
- One idea per bullet. Claims must be defensible in an interview — never inflate.
- Every project links to something a stranger can open.

## Ops

- PDF must stay one page: tighten via the two `TIGHTEN` markers in `assets/resume.css`.
- Never delete/recreate this repo (profile-README namespace risk). If the profile README stops rendering: owner clicks "Share to profile" on the repo page.
