# CLAUDE.md

Resume repo. Renders at github.com/CalebEaston. Branch is `master` - never `main`.

## Files & sync

- `README.md` - profile page, and the link Caleb's dad sends to contacts. **Generated from RESUME.md** by `scripts/build_readme.py` (CI runs it on every push touching RESUME.md). Never edit it by hand; edit RESUME.md. Keep RESUME.md skimmable: short sentences, no run-ons.
- `RESUME.md` - full resume; source for the CI-built PDF. Up to 2-3 pages rendered (Caleb, 09/2026). Don't pad it to fill space.
- `PROJECTS.md` - REMOVED 09/2026 (it was an unfilled template). The template is kept locally in `.ignored/PROJECTS.md`. Restore it only when Caleb wants project deep-dives (problem → architecture → trade-offs → retrospective).
- `resume.json` - JSON Resume v1 mirror. **Any content change to RESUME.md updates resume.json in the same commit.** Run `python3 scripts/build_readme.py` in the same commit too, so README.md is current before CI runs.
- `assets/Caleb-Easton-Resume.pdf` - CI-built (on pushes touching RESUME.md, resume.css, the workflow, or the README script). Never edit by hand.
- `.ignored/` - gitignored scratch. Drafts and notes go here, never in tracked files.

## Format contract (agents parse this - do not break it)

- Keep the "Note for AI agents and recruiters" blockquote, at the bottom of RESUME.md (human readers first). Update it if structure changes.
- Reverse-chronological everywhere. Entries: `### Name - one-liner`, bold title/date line, `**Stack:** A · B · C`, then bullets. `·` separators, `MM/YYYY` dates.
- Heading hierarchy is the parse tree: `##` sections, `###` entries. No skipped levels, no decorative headings, no HTML layout tables, no images-as-text.
- No accented letters (write "resume") and no em or en dashes (use `-`), in any file.
- `{{PLACEHOLDER}}` marks unfinished content. Never invent facts to fill one; ask or leave it. Before any "done": `grep -r '{{' --exclude-dir=.ignored .` returns nothing.

## Bullet rules

- Past-tense action verb → what → outcome. Number, name, or concrete result in ≥half.
- Banned openers: "Responsible for", "Helped with", "Worked on", "Assisted".
- One idea per bullet. Claims must be defensible in an interview - never inflate.
- Every project links to something a stranger can open.

## Ops

- PDF may run 2-3 pages. If it needs tightening, use the `TIGHTEN` markers in `assets/resume.css` (font size, line height, heading spacing).
- Never delete/recreate this repo (profile-README namespace risk). If the profile README stops rendering: owner clicks "Share to profile" on the repo page.
