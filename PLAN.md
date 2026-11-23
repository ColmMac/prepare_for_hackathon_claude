# PLAN: Chore Roulette

**One-liner:** Flatmates can spin a wheel to share out the week's chores so that nobody gets stuck with the bins twice in a row.

## Design
**Vibe**
- [x] Retro arcade: dark background, neon accent, blocky headings
  (on our light palette: blocky monospace headings, thick black borders, chunky shadows, red as the "neon")

**Palette (background / ink / accent)**
- [x] White `#FAFAF7` / Black `#111111` / Signal red `#E63022`

**Fonts**
- [x] Monospace headings + system sans body

**Signature moment**
- [x] A big spinning wheel with a satisfying slow-down

**Must look good on**
- [x] Laptop

## Demo path (what judges see, in order)
1. Add 3 flatmates and 3 chores (Bins, Dishes, Bathroom) in a few seconds.
2. Hit SPIN: the big wheel slows down and lands on a name for each chore; last week's person for that chore is greyed out and skipped.
3. Refresh the page: this week's rota (and last week's) is still there.

## MVP (build in this order, one feature per prompt)
- [x] 1. Page layout in the chosen design: header, Flatmates + Chores input panels, big wheel area, rota table. Static, placeholder data, palette + fonts as CSS variables.
- [x] 2. Add/remove flatmates and chores, saved to localStorage; wheel slices redraw from the flatmate list.
- [x] 3. SPIN: wheel animates with ease-out slow-down and assigns each chore in turn, never to whoever had it last week (if possible); results fill the rota table.
- [x] 4. Rota persistence + "New week" button (current rota becomes last week), plus edge cases: <2 flatmates, no chores, more chores than people.

## Next features (build in this order, one feature per prompt)
- [x] 5. Long-name fix: wheel label font shrinks so names up to 20 characters fit inside their slice.
- [x] 6. Fair-play note: after each chore's spin, show "<name> skipped for <chore>: did it last week" under the wheel, and keep the notes listed once the rota is set.
- [x] 7. Landing celebration: when the wheel stops, the winning slice flashes red and the winner's name pops up big under the pointer.
- [x] 8. Space bar to spin: pressing Space (when not typing in an input) triggers SPIN.
- [x] 9. Copy to group chat: button copies this week's rota as plain text ("Bins: Priya" per line) to the clipboard, with a "Copied" confirmation.

## Cut list (not building, on purpose)
- Chore streak leaderboard
- Dark mode
- Phone/projector layouts, sound effects, accounts or syncing between phones, editing past weeks

## Points strategy
| Criterion | Weight | How we score it |
|---|---|---|
| Impact | 30% | Open the pitch with the bins argument everyone's had; fairness rule is visible on screen |
| Demo | 30% | 3-step path under 60s, rehearsed; seed data ready so nothing is typed slowly |
| Design | 20% | The wheel is the hero; strict 3-colour palette, blocky arcade type, no generic hero text |
| Technical | 20% | Survives refresh; handles 1 flatmate, 0 chores, more chores than people without breaking |
| Sponsor: Best use of Claude | prize | Realistic: show CLAUDE.md rules, `/hack-plan` skill, one-feature-per-prompt workflow |

## Timeline (45 min)
| Time | Goal |
|---|---|
| 0–8 | Feature 1: layout |
| 8–18 | Feature 2: add flatmates/chores + save |
| 18–30 | Feature 3: spinning wheel + fair assignment |
| 30–38 | Feature 4: rota persistence, new week, edge cases |
| 38–45 | Pitch + one full demo rehearsal (last 15%) |
