# Chore Roulette: 90-second pitch

Built only from what works in `app/index.html` today: add/remove flatmates and chores, the spin wheel
with the "not last week's person" rule, rota saved in localStorage, New week, edge cases, long-name fix,
fair-play notes, winner celebration, Space to spin, Copy to group chat.
Not pitched (cut on purpose): streak leaderboard, dark mode.

**Before you go on stage:** load seed data (3 flatmates, 3 chores: Bins, Dishes, Bathroom), press New week
once so "last week" is filled in, and have the app open full-screen in the browser. Swap the names below
for your seed names.

---

## Speaker notes (about 220 words, 90 seconds)

### 1. Hook (0:00–0:10)
[Slide 1. Speaker A, slow and quiet. Don't click yet.]

"It's 11pm. The bins are overflowing. Again. And everyone swears it's not their turn."

[Pause one beat.]

### 2. Problem (0:10–0:25)
[Click to slide 2.]

"Every flat has this fight. The same person ends up with the bins, and nobody remembers who did what last week.
A rota on the fridge gets ignored. A group chat just becomes the argument."

### 3. Solution + live demo (0:25–1:00)
[Click to slide 3, then switch to the browser tab with the app. Speaker B drives.]

"This is Chore Roulette. Three flatmates, three chores, already in. I press space."

[Press Space. Let the wheel run.]

"Watch the wheel slow down... it lands on Priya for the bins. Now the dishes. See Sam greyed out?
Sam did the dishes last week, so the wheel skips Sam, and says so right here. That's the fairness rule, out in the open."

[Point at the fair-play note under the wheel. Let the remaining chore finish.]

"Refresh the page. The rota is still here. One click copies it to the group chat."

[Refresh. Click Copy. Point at "Copied". Switch back to the slides.]

### 4. How we built it (1:00–1:10)
[Click to slide 4.]

"Built with Claude Code in one sitting. One HTML file, plain JavaScript, no framework. A CLAUDE.md fixed our stack and our palette,
we built one feature per prompt, and project skills ran the planning and this pitch."

### 5. Impact and improvements (1:10–1:20)
[Click to slide 5.]

"Anyone sharing a flat can use it tonight: no sign-up, nothing to install. Next we'd add a chore streak leaderboard and dark mode."

### 6. Ask / close (1:20–1:30)
[Stay on slide 5, or go back to the wheel. Both speakers.]

"Try it with your own flat: [link or QR]. So tonight, nobody argues about the bins. The wheel decides."

---

## 5-slide outline

**Style for every slide** (from `slide-style.md`, matching the app): flat `#FAFAF7` background, no gradient;
`#111111` text; `#E63022` as the one accent. Bold sans-serif headings, plain body text. One line per slide, mostly visual.
No emoji, no purple-blue gradients or glass effects, no stock photos, no filler words.

| # | Title (6 words max) | Visual idea | Speaker note |
|---|---|---|---|
| 1 | **It's 11pm. Whose turn?** | Close-up photo or drawing of an overflowing bin on the flat background; the single red line "Whose turn?" is the only colour. | Part 1: hook. |
| 2 | **Same person. Every week.** | Three chore names (Bins, Dishes, Bathroom) in black; the bins row repeated over four weeks with the same name each time, the repeat marked in red. No other text. | Part 2: problem. |
| 3 | **Live demo** | Mostly empty slide: a thick black-bordered box with the wheel's red slice in it. It only holds the screen while you switch to the browser. | Part 3: demo, then press Space. |
| 4 | **Built with Claude Code** | Screenshot of the `CLAUDE.md` rules (stack, palette, "one feature per prompt") next to a list of the skill names: `hack-plan`, `pitch-story`. One caption line: "One file. No framework." | Part 4: how we built it. |
| 5 | **Next: streaks and dark mode** | Two simple black-outlined boxes, "Chore streaks" and "Dark mode". The closing line, "The wheel decides.", goes in red at the bottom. | Parts 5 and 6: impact, ask and close. |

---

## Criteria check

| Criterion (weight) | What scores it | Line in the script |
|---|---|---|
| Impact (30%) | Relatable problem and the fix | "It's 11pm. The bins are overflowing..." / "The same person ends up with the bins, and nobody remembers who did what last week." / "Anyone sharing a flat can use it tonight." |
| Demo (30%) | Live, clear, under 60 seconds | "I press space... Watch the wheel slow down... Refresh the page. The rota is still here." (35 s, three steps from `PLAN.md`, seed data preloaded) |
| Design (20%) | The wheel is the hero, distinctive look | "Watch the wheel slow down..." (the signature moment) plus the three-colour retro style on every slide |
| Technical (20%) | Fairness rule, persistence, reliable | "Sam did the dishes last week, so the wheel skips Sam, and says so right here." / "Refresh the page. The rota is still here." Edge cases (1 flatmate, no chores, more chores than people) are handled in the code. Say so if a judge asks. |
| Best use of Claude (prize) | Show the workflow, not just the result | "A CLAUDE.md fixed our stack and our palette, we built one feature per prompt, and project skills ran the planning and this pitch." Slide 4 shows the file. |

---

## Backup plan
If the live demo breaks: have a short screen recording of the same three steps ready, or step through
screenshots of the wheel mid-spin, the greyed-out name with its fair-play note, and the rota after a refresh.
