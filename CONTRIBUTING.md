# How to maintain this résumé

Notes to myself, so future-me doesn't have to rediscover any of this.

## What each file is for

| File | Purpose |
| --- | --- |
| `README.md` | The GitHub profile page. Highlights only — one screen of scrolling. |
| `RESUME.md` | The complete résumé, and the source for the PDF. |
| `PROJECTS.md` | Deep-dives: problem, architecture, trade-offs, retrospective. |
| `resume.json` | [JSON Resume](https://jsonresume.org/schema/) mirror for parsers and AI screeners. |
| `assets/resume.css` | Print styling for the PDF only. GitHub ignores it. |
| `assets/Caleb-Easton-Resume.pdf` | Built by CI on every push that touches `RESUME.md`. Don't edit by hand. |

`RESUME.md` and `resume.json` say the same things in two formats. When one changes, change
the other in the same commit — a stale `resume.json` is worse than none, because the systems
that read it never show you what they found.

## Adding an entry

1. Add the full version to `RESUME.md` (and `PROJECTS.md` if it deserves a write-up).
2. Mirror it into `resume.json`.
3. If it belongs in the highlights, add a condensed version to `README.md`.
4. Push. CI rebuilds the PDF and commits it back.

## Writing bullets that work

The pattern is **action verb → what you built → outcome**:

> Built a scheduling API in FastAPI that cut manual shift assignment from ~3 hours a week to
> under 10 minutes for a 40-person team.

Not:

> Responsible for working on backend development tasks using Python.

Rules worth keeping:

- Past tense, strong verb: Built, Designed, Automated, Migrated, Reduced, Shipped.
- Never start with "Responsible for", "Helped with", "Worked on", or "Assisted".
- Reach for a number wherever one honestly exists — users, time saved, latency, scale, scope.
- One idea per bullet. If it needs "and", it's two bullets.
- Say what *you* did. "The team built" tells a reader nothing about you.

## Rendering the PDF locally

```sh
npx md-to-pdf RESUME.md --stylesheet assets/resume.css
```

Opens as `RESUME.pdf` in the repo root; it's gitignored. If it spills to a second page, the
two fastest fixes are marked `TIGHTEN` in `assets/resume.css`.

## Before applying anywhere

Run through the checklist at the bottom of `RESUME.md`. The one that matters most: no `{{`
left anywhere.
