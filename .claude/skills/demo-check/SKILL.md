---
name: demo-check
description: Runs a pre-demo readiness check for a hackathon project and writes a go/no-go checklist. Use when the user asks if they are ready to demo or present, or wants a final check before judging.
allowed-tools: Read, Glob, Grep
---

# Demo check

Goal: nothing surprises you on stage.

## Steps
1. Read `PLAN.md` (the demo path) and `app/index.html`.
2. Walk through the demo path in the code, and flag anything that could break live:
   - an empty state (no flatmates or chores yet): does the app crash or look broken?
   - console errors, unfinished TODOs, or placeholder text
   - anything that needs the internet
   - layout at phone width (360px)
3. Print this checklist in chat, marking each item ✅, ⚠️ or ❌ with a one-line reason:
   - [ ] The demo path works from a fresh page load
   - [ ] Demo data is pre-filled, or quick to add
   - [ ] It works offline (no network needed)
   - [ ] Nothing in the UI says TODO or lorem ipsum
   - [ ] There's a backup: a screen recording or screenshots of the demo
   - [ ] The pitch script exists (`pitch/pitch.md`)
   - [ ] Who talks and who clicks has been agreed
4. Finish with **GO** or **NO-GO**, plus the single most important fix if it's a NO-GO.

Don't edit any files. This skill only reports.
