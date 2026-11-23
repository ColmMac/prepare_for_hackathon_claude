---
name: hack-plan
description: Turns a hackathon brief into a scoped build plan (MVP, cut list, demo path, timeline) saved as PLAN.md. Use at the start of a hackathon, or when the user asks to plan, scope or prioritise what to build.
allowed-tools: Read, Write, Glob
---

# Hackathon planner

You help a small team decide what to build in a short, fixed time. The plan should be
small enough to finish, because a working demo beats a half-built vision.

## Steps
1. Read `BRIEF.md` and `CLAUDE.md`. If the brief is missing, ask the user to paste it.
2. Ask how much build time is left, if they haven't said. Assume 60 minutes if they don't know.
3. Work out what scores points. Rank the judging criteria by weight, and note which sponsor prizes are realistic.
4. Write `PLAN.md` using the structure in [plan-template.md](plan-template.md). Rules:
   - The **demo path** is exactly 3 steps a judge will see, and every MVP feature must serve it.
   - The **MVP** has at most 4 features, each small enough to build in one prompt.
   - The **cut list** names the ideas you're deliberately not building, so nobody builds them by accident.
   - The **timeline** leaves the last 15% of the time for the pitch and a demo rehearsal.
   - Respect the tech stack in `CLAUDE.md`. Never plan anything that needs a new dependency.
5. Finish with a 3-line summary in chat, followed by the first prompt the user should send to start building.

Keep the plan under one screen. Teams don't read long plans at 3 AM.
