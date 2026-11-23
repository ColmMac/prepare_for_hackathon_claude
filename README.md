# Claude Code Hackathon Toolkit

**Claude Builder Club @ UoE, Workshop 1**

A skeleton you tailor in the workshop, then reuse at every hackathon:
raw idea → working prototype → winning pitch.

## Quick start
```bash
git clone https://github.com/ZekiKam/cbc-workshop1
cd cbc-workshop1
claude
```
Log in with your **Claude Pro account**. Choose the Claude account option, not an API key, so you don't use your API credits.

> Can't see `.claude/`? Folders starting with a dot are hidden. Mac Finder: **Cmd+Shift+.** · Terminal: `ls -a`

## What's inside
```
cbc-workshop1/
├── CLAUDE.md              ← the rules Claude reads every session (tailor it)
├── BRIEF.md               ← the hackathon problem + judging criteria (swap per hackathon)
├── PLAN.md                ← YOUR plan: pick a Design, then /hack-plan fills in the rest
├── app/index.html         ← empty: you build the app here, one feature at a time
├── pitch/                 ← /pitch-story writes your pitch here
├── secrets/               ← fake keys, blocked by .claude/settings.json
└── .claude/
    ├── settings.json      ← permission rules: deny secrets/
    └── skills/
        ├── hack-plan/     ← fills in PLAN.md (MVP, cut list, demo path)
        ├── pitch-story/   ← 90-sec pitch + 5-slide outline
        ├── demo-check/    ← go/no-go, plus checks YOU add
        └── readme-writer/ ← empty: YOU write this skill
```

## Your workshop checklist
- [ ] **1. Tailor CLAUDE.md:** add one rule of your own under "Our team's rules".
- [ ] **2. Pick your design:** open `PLAN.md` and tick one option in each Design group.
- [ ] **3. Plan:** press Shift+Tab until you're in plan mode, then run `/hack-plan`. Read the plan it writes.
- [ ] **4. Build one feature at a time:** send `Build MVP feature 1 from PLAN.md`.
      **Open `app/index.html` in your browser and check it before you move on.** Then run `/clear` and ask for feature 2.
- [ ] **5. Write your own skill:** create `.claude/skills/readme-writer/SKILL.md`, then run `/clear` and say `write our README`.
- [ ] **6. Add your own checks:** open `.claude/skills/demo-check/SKILL.md` and fill in "Our team's extra checks".
- [ ] **7. Pitch:** run `/pitch-story`, then `/demo-check`. Aim for a GO.

Stuck? The finished version is in [cbc-workshop1-solutions](https://github.com/ZekiKam/cbc-workshop1-solutions): compare your files with it, or copy across the step you're on.

## Reuse it at your next hackathon
- Replace `BRIEF.md` with the real brief and judging criteria.
- Reset `PLAN.md` to its headings, and change the stack in `CLAUDE.md` to fit your team.
- Use the skills everywhere: `cp -r .claude/skills/* ~/.claude/skills/`

## Learn more
- [Claude Code docs](https://code.claude.com/docs/en/overview)
- [Claude Code in Action](https://anthropic.skilljar.com/claude-code-in-action/)
- [Introduction to Agent Skills](https://academy.claude.com/courses/introduction-to-agent-skills)
