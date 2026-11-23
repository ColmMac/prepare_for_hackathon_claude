# Hackathon Toolkit (CBC Workshop 1)

Claude reads this file at the start of every session. It sets the rules for this project.
Swap `BRIEF.md` to reuse the toolkit at any hackathon.

## What we're building
Read `@BRIEF.md` for the problem, the judging criteria and the sponsor prizes.
After `/hack-plan` has run, `PLAN.md` is the source of truth for scope.

## Tech stack (do not change without asking)
- ONE file: `app/index.html` with inline `<style>` and `<script>`.
- Vanilla HTML, CSS and JavaScript only. No frameworks, no npm, no build step, no CDNs.
- Data is saved in `localStorage`. No backend, no login, no database, no API keys.
- It must work by double-clicking `app/index.html`.

## How to work
- Build the demo path first: the 3 steps a judge will see in the demo. Polish comes later.
- Build one feature at a time. After each one, tell me how to check it in the browser.
- Keep changes small. If a feature needs more than ~150 new lines, propose a smaller version first.
- Ask before adding any dependency, file or folder outside `app/`, `pitch/` and `PLAN.md`.
- If something in `PLAN.md` is on the cut list, don't build it unless I say so.

## Design rules (no AI slop)
- Choose a palette of 1 background, 1 ink and 1 accent colour, and use it everywhere.
- Avoid purple-blue gradients, glassmorphism, emoji as icons, and generic "Welcome to X" hero text.
- Use real copy written for flatmates, not lorem ipsum or marketing filler.
- Use a clear type scale: one display font for headings and one body font.
- It must work on a phone screen (360px wide).

## Off limits
- Never read or edit anything in `secrets/`.

## Our team's rules
<!-- Workshop step: add one rule of your own below, e.g. "Explain each change in one sentence" -->
-
