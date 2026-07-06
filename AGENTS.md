# AGENTS.md — AI-Assisted Web Development Course

## Repository type

Static HTML course site. No build system, no package.json, no runtime dependencies. Open `index.html` in a browser.

## Teaching workspace structure (per `SKILL.md`)

| Path | Purpose |
|------|---------|
| `MISSION.md` | Learner's goal — grounds all teaching decisions |
| `RESOURCES.md` | Curated knowledge sources and communities |
| `NOTES.md` | Scratchpad for user preferences and working notes |
| `index.html` | Course landing page (theme toggle, phases overview) |
| `lessons/` | Lesson HTML files (`0001-<name>.html` through `0060-<name>.html`) |
| `reference/` | Cheatsheet/glossary HTML files (NOT in `lessons/reference/`) |
| `assets/style.css` | Shared stylesheet with dark/light theme |
| `assets/lessons-data.js` | **Single source of truth** — `window.LESSONS` array used by sidebar and nav |
| `assets/sidebar.js` | Auto-builds sidebar from `window.LESSONS` |
| `assets/lesson-nav.js` | Auto-builds prev/next buttons from `window.LESSONS` |
| `sequence-tracker/` | Progress tracking (`overview.json`, `lesson-plan.md`) |
| `learning-records/` | ADR-style records of what the learner demonstrated |

## Lesson numbering and phase mapping

```
Phase 0 (AI Tools):         0001–0006
Phase 1 (MySQL):            0007–0013
Phase 2 (Laravel):          0014–0023
Phase 3 (Next.js):          0024–0032
Phase 4 (API Integration):  0033–0038
Phase 5 (Auth & Security):  0039–0045
Phase 6 (Testing):          0046–0051
Phase 7 (Deployment):       0052–0056
Phase 8 (Capstone):         0057–0060
```

## Adding a new lesson

Update **all three** sources or nav/sidebar will break:

1. `assets/lessons-data.js` — add entry to `window.LESSONS` array at correct position. The `file` field must NOT include a `lessons/` prefix.
2. `sequence-tracker/overview.json` — add entry with status, phase, topics.
3. `sequence-tracker/lesson-plan.md` — add row in the correct phase table.

## Lesson file conventions

- Filename: `XXXX-<kebab-case-name>.html` — the `XXXX` prefix is parsed by `sidebar.js` and `lesson-nav.js` to identify the current lesson via `filename.split('-')[0]`.
- Script load order (in `<body>`): `lessons-data.js` → `sidebar.js` → `lesson-nav.js`.
- Every lesson must include:
  - `<link rel="stylesheet" href="../assets/style.css">`
  - Theme toggle inline `<script>` in `<head>` reading `localStorage`
  - Theme toggle button with `class="theme-toggle"` and `id="themeToggle"`
  - `<div class="lesson-nav"></div>` for prev/next buttons
  - Quiz with 3 questions, correct answers set in `checkQuiz()` function
  - `<div class="project">` for the mini-project
- Content language: Taglish (mixed Tagalog and English).
- Reference files go in `reference/` — NOT in `lessons/reference/` (a common mistake).
- Reference files should use `../assets/style.css` for the CSS path.
- `index.html` must link the first lesson at `lessons/0001-intro-ai-assisted-development.html`.

## Content source

The course outline in `ai-web-development.md` is the authoritative guide — all lesson topics, order, and structure derive from it.

## Theme toggle

Dark/light mode is persisted to `localStorage` key `"theme"`. The anti-flash script runs inline in `<head>`:
```html
<script>if (localStorage.getItem("theme") === "dark") document.documentElement.setAttribute("data-theme", "dark");</script>
```

## Key gotchas

- `sidebar.js` and `lesson-nav.js` derive the base directory from `window.location.pathname`, so links work at any page depth automatically as long as `file` values omit directory prefixes.
- The `sequence-tracker/overview.json` `file` fields also omit directory prefixes.
- Do NOT add sidebar/nav scripts to `index.html` or reference files — they are not lessons.
- No ports, servers, or `npm install` needed. Open files directly in a browser.
