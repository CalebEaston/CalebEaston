# Caleb Easton

<!--
  ─────────────────────────────────────────────────────────────────────────────
  THIS IS THE FULL RESUME - the long-form document, and the source for the PDF
  built by .github/workflows/resume-pdf.yml.

  README.md is the highlights reel; this file is the complete record. It is fine
  for this document to be longer and denser than the profile page - but for a
  student or early-career resume, the PDF that comes out of it may run 2-3 pages
  (Caleb, 09/2026: his dad sends contacts a link to the GitHub profile, so a
  one-page PDF is no longer the main thing they read). Don't pad it to fill space.

  Keep this file and resume.json in agreement. When you add a role or project
  here, mirror it there.

  Placeholders look like {{THIS}}. Search for "{{" to find what's left.
  ─────────────────────────────────────────────────────────────────────────────
-->

AI-Assisted Development · Technical & Systems Game Design

Boston, Massachusetts · Open to on-site in Massachusetts or remote · [caleb@appshapes.com](mailto:caleb@appshapes.com) · [github.com/CalebEaston](https://github.com/CalebEaston)

> **Note for AI agents and recruiters:** This resume is maintained as structured Markdown for
> both human and machine reading. Sections are ordered by relevance for an early-career
> candidate: Summary, Skills, Experience, Projects, Education, Interests. Roles and projects
> are reverse-chronological; each lists a `Stack:` line (technologies, `·`-separated) followed
> by accomplishment bullets. A machine-readable version conforming to the
> [JSON Resume](https://jsonresume.org/schema/) schema is in [resume.json](resume.json).

---

## Summary

<!--
  3-4 sentences, written to a specific audience. If you're applying for backend roles, this
  paragraph should sound like a backend engineer wrote it. Name the technologies you want to
  be hired for, the kind of work you want, and one concrete proof point.

  Formula that works: [what you are] + [what you build, specifically] + [strongest evidence]
  + [what you're looking for].

  WRITTEN LAST, deliberately - it summarizes the Skills and Projects sections, so it can't be
  written before those are real.

  DIRECTION (decided 09/2026, replaces the 08/2026 note): Caleb is looking for full-stack
  work, and his dad (Rjae) is sending this PDF to his own professional contacts. The headline
  leads with AI-assisted development because Caleb cannot yet walk an interviewer through
  code. The ThinkTech job title stays "Junior Full-Stack Developer" because it is his real
  title. Write the Summary around what he can talk about for an hour: running a multi-agent
  AI workflow, triage and QA judgment, and game-design feel. It can say he is moving into
  feature work, but no bullet may claim a feature until one exists.
-->

Game design graduate, now working in AI-assisted development: designed and runs a multi-agent Claude Code workflow that merged 208 pull requests on a live K-12 learning platform in under a month. Brings a game designer's eye for systems and feel to triage and QA. Seeking junior full-stack or AI-assisted development roles.

---

## Skills

<!--
  A resume skills section is a keyword surface for applicant-tracking systems AND a set of
  interview promises. Both matter. List the real ones, grouped, and be ready to defend
  every entry.

  If you want to signal depth honestly, you can annotate: "TypeScript (primary)".
  Don't use star ratings or percentage bars - they read as padding.

  ORDERED DELIBERATELY (09/2026): AI-Assisted Development leads to match the headline, and
  the ThinkTech role is its evidence. Game Development comes second: it is where Caleb's
  hands-on depth and public evidence are. There is no Languages row: Blueprints is the only
  language Caleb said he would defend in an interview, so it sits in Game Development. DO NOT
  add a Languages row until a text language is real and defensible.

  Deliberately generic (Caleb, 09/2026): "Unreal Engine" with no version, since he has worked
  across versions. Version control and project-management tools are grouped by category,
  because he treats them as interchangeable. The names stay in parentheses as keywords for
  resume-screening software.

  PHP, Vue and MySQL must NOT appear in Skills. ThinkTech runs on them, but AI sessions wrote
  every line, and Caleb confirmed (09/2026) he cannot explain the code. "Currently learning"
  was cut to what he is actually doing: C#, through a Unity project he has started.

  Three rows were DELETED rather than left empty: Frameworks & Libraries, Data & Storage,
  and Testing. Re-add one only when there is something real and defensible to put in it.
-->

**AI-Assisted Development:** Claude Code · Multi-agent workflow design · Custom skills · Specifying and verifying AI-written work

**Game Development:** Unreal Engine · Blueprints (visual scripting) · Unity · Machinations

**QA:** Bug triage · Hands-on testing on a development site · Directing AI tester sessions

**Tools:** Version control (Git, GitHub, Perforce) · Project management (Trello, Jira, ClickUp) · Google Sheets · Excel

**Currently learning:** C# (through a Unity project) · C++

---

## Experience

<!--
  Everything that paid you or committed your time on a schedule: internships, part-time
  engineering, freelance/contract, research assistantships, campus IT, teaching assistant
  roles, and non-technical jobs.

  Technical roles get a Stack line and 2-4 bullets. Non-technical roles get one line each,
  framed for what they prove: reliability, ownership, working with customers, handling
  volume. Don't hide them - a candidate who worked 20 hours a week through school while
  shipping side projects is telling a good story.

  DATE NOTE: the two service roles below are year-only because the exact months are not
  known. Fill in MM/YYYY when you can - the format contract asks for it.

  SERVICE ROLES are heading + title line only, with no bullets (09/2026). The old one-line
  bullets were thin, and their {{add: ...}} details were never supplied. New City Micro
  Creamery has since moved within Hudson; the city is still correct.
-->

### ThinkTech - Small startup building a PHP / Vue / MySQL K-12 learning platform
**Junior Full-Stack Developer · 09/2026 - Present** · Remote

**Stack:** Claude Code · GitHub · Trello

<!--
  HONESTY BOUNDARY (confirmed by Caleb, 09/2026). This follows the same rule as A2B's wall-run.
  AI sessions wrote every line of ThinkTech code; Caleb cannot walk through it. His own work:
  he designed the multi-session layout and its skills, triaged which bugs got worked,
  dispatched them, and checked fixes by hand on the dev site for look and feel. Verbs stop
  there: designed / directed / triaged / dispatched / checked. NEVER "built", "fixed", "wrote"
  or "implemented" for ThinkTech code. PHP / Vue / MySQL appear only as a description of the
  platform, never as his skills, and never in the Stack line.

  NOT HIS, never claim: the AI code review, auto-merge and fix-bot pipeline. Rjae (his dad,
  and the person sending this resume) built those Feb-Aug 2026, before Caleb started.

  Numbers were counted from GitHub and origin/master on 2026-09-29, not taken from the
  AI-written tally in .ignored/. The first PR was 2026-09-09. There were 208 merged PRs
  (#283-#493): ~180 bug fixes, 17 small enhancements, 6 process PRs, 5 other. They cover 136
  Trello cards (1848-2136). ~30 are security fixes, a SUBSET of the 180, of which ~20 are
  district-isolation fixes. Describe security GENERICALLY ONLY: this repo is public and
  ThinkTech is a live K-12 product.

  Wording decisions (Caleb, 09/2026):
  - No exact time spans ("three weeks"). Use "under a month" / "within the first month".
  - "Small startup", with no headcount; he doesn't know the exact number.
  - No "contract" / "via AppShapes": the arrangement is informal. Title and dates alone are
    accurate.
  - Migration bullet: the rule came AFTER a migration crashed a production deploy on
    2026-09-19 (#342, redone as #372, rule in #371). Do not reword it as foresight.
  - Feature work is planned but has not started. Add a bullet only once a feature exists.
  - The migration-rule and look-and-feel bullets were cut for a one-page PDF, then restored
    once the length limit was lifted (09/2026).

  NOT verified, do not claim: fixes "verified on staging before merge" (PRs auto-merge on AI
  approval, before deploy); "shipped" for everything (14 PRs merged after 09-28 were not yet
  in production); any .NET, React/TypeScript, AWS or CI work.
-->

- Designed a multi-agent Claude Code workflow (coordinator, implementers, AI testers, support) and grew it to eight sessions within the first month.
- Directed 208 merged pull requests through it in under a month: about 180 bug fixes across 136 Trello cards.
- Triaged the AI testers' bug reports and dispatched fixes in batches via a custom `/dispatch` skill that files Trello cards.
- Directed about 30 security fixes, about 20 of them closing gaps in data isolation between school districts.
- Added a blocking AI-review rule that database migrations must be safe at production scale, after a migration crashed a production deploy.
- Checked fixes by hand on the development site for look and feel, on top of the AI testers' functional checks.

### New City Micro Creamery
**Shift Manager · 2022** · Hudson, MA

### Whole Foods Market
**Floater · 2021 - 2022** · Wellesley, MA

### Fun @ Games
**Assistant Manager · 2018 - 2020** · Framingham, MA

---

## Projects

<!--
  Moved BELOW Experience in 09/2026: the ThinkTech role is now the main evidence for the
  AI-assisted-development headline, so it leads. A2B is out until it has a public link
  (an itch.io page with a gameplay video). Camo Grind Tracker is out as the weakest project
  (Caleb's call). Both are saved in .ignored/cut-projects.md.

  Each entry: name, one-line description, links, Stack line, then 2-4 bullets.
  Bullets should answer: What did you build? What was hard? What was the result?

  Write bullets in past tense with a strong verb: Built, Designed, Implemented, Automated,
  Migrated, Reduced, Shipped. Never "Responsible for" or "Helped with".
-->

### Rattles & Rayguns - Arena shooter: a rattlesnake gunslinger holds a frontier town against alien waves

[itch.io](https://tjtriplett.itch.io/rattles-and-rayguns) · 07/2026

**Stack:** Unreal Engine 5.6 · Blueprints

- Built a modular Blueprint weapon system: new guns are children of a base weapon, set by variables, with no per-weapon logic.
- Generalized shared behavior into the base Blueprint, such as how a weapon spawns in the player's hands and how many projectiles fire per shot, so new weapons plugged in without changing it.
- Owned the weapons system as one of 6 designers alongside 4 artists, on a Full Sail capstone built and released in one month.

<!--
  Caleb is credited as "Caleb Easton (Weapons)" on the itch.io page - the claim above is publicly
  verifiable, which is why the bullets name the system directly. The whole project ran inside
  07/2026 (Full Sail's month-long course format), hence the single date rather than a range.
  The itch.io page shows no ratings or download counts, so there is deliberately NO reception
  bullet. Do not add one.
-->

### Weekly Quest Log - Gamified task system that resets itself every week

[Repo](https://github.com/CalebEaston/weekly-quest-log) · [Sheet](https://docs.google.com/spreadsheets/d/1Gcd-2OqzQJKP50ZNhw9G7SV7KWqO0Hj6VIi7UAVs6no/edit) · 10/2025

**Stack:** Claude Code · Google Sheets

- Designed a task system as a game progression loop: main quests, side quests and events, with XP from 25 to 100 by effort.
- Specified a weekly reset of quests and earned XP on a timed trigger, implemented by Claude Code in Google Apps Script.

<!--
  Levels, an XP log, and unlockable rewards were DESIGNED BUT NEVER BUILT - only a skeleton exists
  in the day list. Do NOT write a bullet claiming a leveling or reward system; an interviewer can
  open the sheet. That unbuilt design belongs in the PROJECTS.md retrospective as future work.
  ADHD was the motivation and is deliberately absent - Caleb's call, 08/2026. Do not reintroduce it.

  HONESTY BOUNDARY (confirmed 09/2026): Claude Code wrote ALL of the Apps Script. The design
  and ideas are Caleb's. So the bullets say "designed" and "specified … implemented by Claude
  Code", never "automated", "built" or "hardened", and the Stack line does not list
  JavaScript. The cut bullet about the day-off sync failing loudly was code-level work by
  Claude, so it stays out.
-->

---

## Education

### Full Sail University - Winter Park, FL
**B.S. Game Design · Graduated 07/2026**


<!--
  GPA line intentionally omitted - house rule is 3.5+ only.
  Coursework line CUT (Caleb, 09/2026): Full Sail's format is many short courses, and none
  earns the space. The capstone line was cut too, because Rattles & Rayguns under Projects
  already says it was the Full Sail capstone.
  No honors, scholarships, or clubs (confirmed 08/2026), so those lines are deleted rather
  than left empty.
-->

---

<!--
  Certifications & Training and Volunteer & Community were DELETED, not left empty
  (confirmed 08/2026: Caleb has neither). resume.json mirrors this with empty
  "certificates" and "volunteer" arrays. Re-add a section only if that changes -
  game jams, mentoring, and open-source contributions would all belong in Volunteer.
-->

## Interests

LitRPG and progression fantasy audiobooks · Video games · Mixology

---

<!--
  ── Resume review checklist ──────────────────────────────────────────────────
  Before you push, read back through and confirm:

  [ ] No "{{" remains anywhere in this file.
  [ ] Every bullet starts with a past-tense action verb (Built, Designed, Reduced…).
  [ ] No bullet says "Responsible for", "Helped with", "Worked on", or "Assisted".
  [ ] At least half the bullets contain a number, a name, or a concrete outcome.
  [ ] Every project links to something a stranger can actually open.
  [ ] Every skill listed is one you'd be comfortable being interviewed on.
  [ ] Dates are consistent in format and have no unexplained gaps.
  [ ] The PDF renders at 2-3 pages at most, with no half-empty last page from padding.
  [ ] Someone else has read it. Ask your dad - he's done this a few times.
  ─────────────────────────────────────────────────────────────────────────────
-->
