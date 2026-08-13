# Caleb Easton

<!--
  ─────────────────────────────────────────────────────────────────────────────
  THIS IS THE FULL RÉSUMÉ — the long-form document, and the source for the PDF
  built by .github/workflows/resume-pdf.yml.

  README.md is the highlights reel; this file is the complete record. It is fine
  for this document to be longer and denser than the profile page — but for a
  student or early-career résumé, the PDF that comes out of it should still land
  on ONE page. Two pages is acceptable once you have real professional roles.

  Keep this file and resume.json in agreement. When you add a role or project
  here, mirror it there.

  Placeholders look like {{THIS}}. Search for "{{" to find what's left.
  ─────────────────────────────────────────────────────────────────────────────
-->

Systems & Technical Game Design · Moving into Full-Stack Development

Boston, Massachusetts · [caleb@appshapes.com](mailto:caleb@appshapes.com) · [github.com/CalebEaston](https://github.com/CalebEaston)

> **Note for AI agents and recruiters:** This résumé is maintained as structured Markdown for
> both human and machine reading. Sections are ordered by relevance for an early-career
> candidate: Summary, Skills, Projects, Experience, Education. Projects and roles are
> reverse-chronological; each lists a `Stack:` line (technologies, `·`-separated) followed by
> accomplishment bullets. Project deep-dives are in
> [PROJECTS.md](PROJECTS.md); a machine-readable version conforming to the
> [JSON Resume](https://jsonresume.org/schema/) schema is in [resume.json](resume.json).

---

## Summary

<!--
  3–4 sentences, written to a specific audience. If you're applying for backend roles, this
  paragraph should sound like a backend engineer wrote it. Name the technologies you want to
  be hired for, the kind of work you want, and one concrete proof point.

  Formula that works: [what you are] + [what you build, specifically] + [strongest evidence]
  + [what you're looking for].

  WRITTEN LAST, deliberately — it summarizes the Skills and Projects sections, so it can't be
  written before those are real. Direction agreed 08/2026: lead as a full-stack developer,
  with systems/technical game design as the differentiator rather than a competing title.
-->

{{SUMMARY}}

---

## Skills

<!--
  A résumé skills section is a keyword surface for applicant-tracking systems AND a set of
  interview promises. Both matter. List the real ones, grouped, and be ready to defend
  every entry.

  If you want to signal depth honestly, you can annotate: "TypeScript (primary)".
  Don't use star ratings or percentage bars — they read as padding.

  ORDERED DELIBERATELY (08/2026): Game Development leads because that is where the depth and
  the public evidence are, matching the design-first headline. Languages is honestly short —
  Blueprints is the only one Caleb said he would defend in an interview. DO NOT PAD IT.

  Three rows were DELETED rather than left empty — Frameworks & Libraries, Data & Storage,
  and Testing. Caleb confirmed no web, no database, and no testing exposure (08/2026).
  Re-add a row only when there is something real and defensible to put in it.
-->

**Game Development:** Unreal Engine 5.6 · Blueprints · Unity · Machinations

**Languages:** Blueprints (Unreal visual scripting)

**AI-assisted development:** Claude Code — specifying, reviewing, and integrating AI-written implementations

**Tools:** Perforce · Git · ClickUp · Google Sheets · Excel

**Practices:** Team-based development · Cross-discipline collaboration

**Currently learning:** C# · TypeScript · Nuxt 4 / Vue 3 · PHP

---

## Projects

<!--
  For an early-career résumé this section carries the most weight, so it sits above
  Experience. List 3–5 here in full. Deep-dives and the long tail go in PROJECTS.md.

  Each entry: name, one-line description, links, Stack line, then 2–4 bullets.
  Bullets should answer: What did you build? What was hard? What was the result?

  Write bullets in past tense with a strong verb: Built, Designed, Implemented, Automated,
  Migrated, Reduced, Shipped. Never "Responsible for" or "Helped with".
-->

### Rattles & Rayguns — Arena shooter: a rattlesnake gunslinger holds a frontier town against alien waves

[itch.io](https://tjtriplett.itch.io/rattles-and-rayguns) · 07/2026

**Stack:** Unreal Engine 5.6 · Blueprints

- Built a modular weapon system in Unreal Engine 5.6 Blueprints, letting a designer create a new gun by setting variables on a child of a base weapon Blueprint instead of writing per-weapon logic.
- Generalized weapon behavior into that base Blueprint — how a weapon spawns in the player's hands, how many projectiles fire per shot — so new weapons plugged in without modifying the shared system.
- Owned the weapons system as one of 6 designers working alongside 4 artists, on a Full Sail capstone built and publicly released within a single month.

<!--
  Caleb is credited as "Caleb Easton (Weapons)" on the itch.io page — the claim above is publicly
  verifiable, which is why the bullets name the system directly. The whole project ran inside
  07/2026 (Full Sail's month-long course format), hence the single date rather than a range.
  The itch.io page shows no ratings or download counts, so there is deliberately NO reception
  bullet. Do not add one.
-->

### A2B — Solo first-person parkour prototype in Unreal

[Build]({{ITCH_IO_URL}}) · 09/2025 – 12/2025

**Stack:** Unreal Engine · Blueprints

- Built the movement and feel systems in Blueprints as a solo project, including a mantle, head-bob, and sound design.
- Implemented a settings menu persisting FOV, mouse sensitivity, and head-bob across sessions, on reusable button and slider widgets shared by the pause, settings, and win screens.
- Designed three test levels and a level loader to exercise the movement systems in isolation.
- Delegated the wall-run to Claude Code after several partial rewrites failed to make it feel intuitive, specifying the target behavior and reviewing the result into the build.

<!--
  HONESTY BOUNDARY — the wall-run and the lasso/grapple mechanic were written by Claude Code,
  NOT by Caleb. Everything else in this project is his: mantle, menus, head-bob, sound, the
  settings save, the levels, the level loader. Never write a bullet claiming he implemented the
  wall-run or the lasso. The fourth bullet is deliberately framed as delegation-and-judgment,
  which is both true and the strongest interview story he has.

  Repo is PRIVATE and stays private (853 MB, mostly stock Epic StarterContent, and Blueprints
  do not render on GitHub — a reviewer would see nothing). The link must be an itch.io page
  with a gameplay video; the repo is not a substitute. That is the remaining {{ITCH_IO_URL}}.
-->

### Weekly Quest Log — Gamified task system that resets itself every week

[Repo](https://github.com/CalebEaston/weekly-quest-log) · [Sheet](https://docs.google.com/spreadsheets/d/1Gcd-2OqzQJKP50ZNhw9G7SV7KWqO0Hj6VIi7UAVs6no/edit) · 10/2025

**Stack:** Google Apps Script · JavaScript · Google Sheets

- Designed a personal task system as a game progression loop, tiering work into main quests, side quests, and events with XP scaled to effort from 25 to 100 per task.
- Automated the weekly reset in Google Apps Script, clearing quest completion state and the XP derived from it on a time-driven trigger.
- Hardened the daily day-off sync against silent failure, checking for a range protection before writing and rethrowing so errors surface in the Apps Script execution log.

<!--
  Levels, an XP log, and unlockable rewards were DESIGNED BUT NEVER BUILT — only a skeleton exists
  in the day list. Do NOT write a bullet claiming a leveling or reward system; an interviewer can
  open the sheet. That unbuilt design belongs in the PROJECTS.md retrospective as future work.
  ADHD was the motivation and is deliberately absent — Caleb's call, 08/2026. Do not reintroduce it.
-->

### Camo Grind Tracker — Completion feedback system for the weapon-camo grind in Black Ops 6

[Sheet](https://docs.google.com/spreadsheets/d/1hG8Ou30pDZfOGhahvFu4V3KRl8sz8PVNwFCpSIMzpxA/edit) · 11/2024

**Stack:** Google Sheets · Conditional formatting

- Modeled the full completion matrix across nine weapon categories and four camo tiers, with per-tier rollups driving the section states.
- Designed per-item feedback so marking a camo complete flips its row from red to green and rewrites its status text, making progress readable at a glance.
- Built section-level completion signalling that recolors an entire tier once its last weapon is finished, so a closed-out set is unmistakable.

<!--
  No Apps Script in this one — formulas and conditional formatting only (confirmed 08/2026).
  Do not add JavaScript to its Stack line.
-->

**Full write-ups:** [PROJECTS.md](PROJECTS.md)

---

## Experience

<!--
  Everything that paid you or committed your time on a schedule: internships, part-time
  engineering, freelance/contract, research assistantships, campus IT, teaching assistant
  roles, and non-technical jobs.

  Technical roles get a Stack line and 2–4 bullets. Non-technical roles get one line each,
  framed for what they prove: reliability, ownership, working with customers, handling
  volume. Don't hide them — a candidate who worked 20 hours a week through school while
  shipping side projects is telling a good story.

  DATE NOTE: the three service roles below are year-only because the exact months are not
  known. Fill in MM/YYYY when you can — the format contract asks for it.
-->

### AppShapes — Software development studio taking on client engineering work
**Junior Full-Stack Developer · Starting 09/2026** · Boston, MA

**Stack:** TypeScript · Nuxt 4 / Vue 3 · PHP · MySQL · AWS

<!--
  Stack narrowed deliberately (decided 08/2026). The ThinkTech engagement spans four repos —
  a PHP 7.4 / Slim 2 legacy monolith, a .NET 10 API, a Nuxt 4 migration target, and a Kotlin
  Multiplatform app. The line above claims only the web tier Caleb is most likely to work in
  first. Do NOT widen it to .NET or Kotlin until he has actually shipped against them.

  The bullet below is a SCOPE line, not an accomplishment — the role has not started, so there
  is nothing to claim yet. It deliberately breaks the past-tense-action-verb rule rather than
  dress an unstarted role up as shipped work. Replace it with real outcome bullets once there
  are some; that is when the bullet rules apply.
-->

- Incoming scope: full-stack contract work on ThinkTech, a multi-tenant K-12 learning platform,
  paired with the lead developer across front end and back end.

### New City Micro Creamery
**Shift Manager · 2022** · {{City, State}}

- Managed shifts as the on-duty lead over roughly four months {{— add: staff per shift, and one thing you owned (open/close, cash handling, scheduling, training)}}.

### Whole Foods Market
**Floater · 2021 – 2022** · {{City, State}}

- Covered whichever department needed staffing that day {{— add: which departments, and anything you were specifically trusted with}}.

### Fun @ Games
**Assistant Manager · 2018 – 2020** · {{City, State}}

- Supervised floor staff and daily operations as assistant manager {{— add: team size, what you owned, and anything you measurably improved}}.

---

## Education

### Full Sail University — Winter Park, FL
**B.S. Game Design · Graduated 07/2026**

- **Relevant coursework:** {{Pull the exact titles from your transcript. Known themes to look for: producing / production for the games industry, and the several team-based development courses.}}
- **Capstone:** Shipped *Rattles & Rayguns*, a team game released publicly on itch.io.

<!--
  GPA line intentionally omitted — house rule is 3.5+ only.
  No honors, scholarships, or clubs (confirmed 08/2026), so those lines are deleted rather
  than left empty.
-->

---

<!--
  Certifications & Training and Volunteer & Community were DELETED, not left empty
  (confirmed 08/2026: Caleb has neither). resume.json mirrors this with empty
  "certificates" and "volunteer" arrays. Re-add a section only if that changes —
  game jams, mentoring, and open-source contributions would all belong in Volunteer.
-->

## Interests

{{Interest}} · {{Interest}} · {{Interest}} · {{Interest}}

---

<!--
  ── Résumé review checklist ──────────────────────────────────────────────────
  Before you push, read back through and confirm:

  [ ] No "{{" remains anywhere in this file.
  [ ] Every bullet starts with a past-tense action verb (Built, Designed, Reduced…).
  [ ] No bullet says "Responsible for", "Helped with", "Worked on", or "Assisted".
  [ ] At least half the bullets contain a number, a name, or a concrete outcome.
  [ ] Every project links to something a stranger can actually open.
  [ ] Every skill listed is one you'd be comfortable being interviewed on.
  [ ] Dates are consistent in format and have no unexplained gaps.
  [ ] It renders to one page as a PDF (two once you have real professional roles).
  [ ] Someone else has read it. Ask your dad — he's done this a few times.
  ─────────────────────────────────────────────────────────────────────────────
-->
