# CLAUDE.md

Guidance for Claude Code when working in this repository.

## What this is

`hwargacki1.github.io` — Harrison Wargacki's personal website, published via GitHub Pages.
It's a general personal-brand site (not tied to a specific job search or class assignment),
served from the root of the `main` branch with no build step.

## Structure

- The site is a **single page**: `index.html`. Keep it that way — don't split content into
  additional `.html` pages unless explicitly asked to.
- **No frameworks or build tools.** Plain HTML/CSS/JS only — no React, no bundlers, no npm
  dependencies, no Jekyll config beyond what GitHub Pages does automatically. Everything
  (styles, scripts) stays inline in `index.html`, self-contained.
- `.claude/skills/github-pages/` is a vendored skill folder, not part of the site. It's
  listed in `.gitignore` and should stay untracked.

## Content: keep it resume-accurate

Site content (About, Experience, Education, Skills, etc.) must always match Harrison's
**current resume** — facts and wording should stay accurate to it, not embellished or
invented. When asked to update the site's content:

1. Find the most recent resume file first — check the Desktop and the
   `OneDrive - Xavier University` folder for files matching `*resume*`/`*cv*`, and use
   whichever has the latest modification time. There has been more than one resume file
   present at once; don't assume a fixed filename or location.
2. Rewrite site copy from that resume's actual content. It's fine to restyle the *tone*
   (e.g. punchier headline phrasing) as long as the underlying facts, titles, dates, and
   scope match the resume exactly.
3. If the resume and the live site disagree, treat the resume as the source of truth.

## Publishing workflow

**Always ask before committing or pushing.** Make edits locally and show/describe them,
then confirm with Harrison before running `git add`/`git commit`/`git push`. Don't publish
automatically as a side effect of an edit request — a request to change the site is not by
itself permission to make it live.

The `github-pages` skill (`.claude/skills/github-pages/`) handles the git/GitHub mechanics
(saving, publishing, checking deploy/build status, troubleshooting 404s, etc.) — use it for
that work, but the ask-first rule above still applies before any push.

## Design

The current design is an Apple.com-style layout: full-bleed dark hero, alternating
light/dark full-width sections, system font stack, pill-tag skill/coursework lists, and
scroll-reveal animations. This is **not a locked-in design system** — it's the current look,
and it's fine to propose or make different visual directions if asked. Don't assume future
requests must preserve this exact style unless told to keep it consistent.
