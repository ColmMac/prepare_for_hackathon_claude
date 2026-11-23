# Claude Code Hackathon Toolkit

**Claude Builder Club @ UoE, Workshop 1**

Win hackathons with Claude: from raw idea to working prototype to winning pitch.
Clone this repo into any hackathon, swap `BRIEF.md`, and go.

## Quick start
```bash
git clone https://github.com/ZekiKam/cbc-workshop1
cd cbc-workshop1
claude
```
Log in with your **Claude Pro account**. Choose the Claude account option, not an API key, so you don't use your API credits.

## What's inside
```
cbc-workshop1/
├── CLAUDE.md              ← rules Claude reads every session (stack, scope, design)
├── BRIEF.md               ← the hackathon problem + judging criteria (swap per hackathon)
├── app/index.html         ← you build the app here (one file, no install)
├── pitch/                 ← /pitch-story writes your pitch here
├── secrets/               ← fake keys, blocked by .claude/settings.json (guardrails demo)
├── solutions/             ← the finished readme-writer skill, if you fall behind
├── demo/                  ← the hooks demo (instructor)
└── .claude/
    ├── settings.json      ← permission rules: deny secrets/
    └── skills/
        ├── hack-plan/     ← brief → PLAN.md (MVP, cut list, demo path)
        ├── pitch-story/   ← 90-sec pitch + 5-slide outline
        ├── demo-check/    ← go/no-go before judging
        └── readme-writer/ ← YOU write this one in the workshop
```

## Workshop steps
1. **Plan:** press Shift+Tab until you reach plan mode, then type `/hack-plan`.
2. **Build:** switch modes with Shift+Tab, then ask for MVP feature 1 from `PLAN.md`. Open `app/index.html` in your browser after each feature. Run `/clear` between features.
3. **Write a skill:** create `.claude/skills/readme-writer/SKILL.md`, then say "write our README".
4. **Pitch:** run `/pitch-story`, then `/demo-check`.

Fallen behind? Run `git checkout mvp-done` to get a working app, then carry on from step 3.

## Use it at your next hackathon
- Replace `BRIEF.md` with the real brief and judging criteria.
- Edit the tech stack in `CLAUDE.md` to match your team.
- To use the skills in every project, copy them: `cp -r .claude/skills/* ~/.claude/skills/`

## Learn more
- [Claude Code docs](https://code.claude.com/docs/en/overview)
- [Claude Code in Action](https://anthropic.skilljar.com/claude-code-in-action/)
- [Introduction to Agent Skills](https://academy.claude.com/courses/introduction-to-agent-skills)
