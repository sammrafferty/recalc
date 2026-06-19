# recalc — Excel reps for analysts

A Monkeytype-style practice arena for Excel fluency, built for investment banking
analysts. Open it, get 60 seconds of real reps, feel sharper, close it. One file,
no install, keyboard-first.

## Run it

Double-click **`index.html`**. That's it — it runs offline in any modern browser.

(Optional, for a localhost URL: `python -m http.server 5188 --directory .` then open
http://localhost:5188/)

## Two disciplines

- **Sprint** — type real banker formulas at speed. A generative engine builds endless,
  realistic drills: `SUMIFS`, `XLOOKUP`, `INDEX/MATCH`, `IFERROR`, mixed `$` anchoring,
  cross-sheet refs (`'Balance Sheet'!$F$5`), and live model lines (growth, margin,
  EBITDA, tax, CAGR, discount factors). Stop-on-error: a wrong paren matters in a model.
- **Navigate** — drive an Excel-like grid with the keyboard: arrows, `Ctrl+arrow` to leap
  data edges, `Shift` / `Ctrl+Shift` range selection, and the `F4` anchor cycle.

## The loop

| Action | Key |
| --- | --- |
| Start a run | just start typing (or any arrow in Navigate) |
| Restart, same settings | `Tab` |
| Back to menu / abort | `Esc` |
| Fix a mistake | `Backspace` |
| Run it back (results screen) | `Tab` or `Enter` |

## Results

WPM (Monkeytype-style), accuracy, consistency, a WPM-over-time graph with miss markers,
a **weak-keys** breakdown (learn that you fumble `$ ( ,`), per-formula speed, personal
bests, and a run-history sparkline. Navigate reports tasks/min and keystroke efficiency.

## Settings

Category · difficulty · time/count modes. Four themes (`excel`, `amber`, `slate`,
`paper`) and an optional keypress sound, top-right. Everything persists locally.

Single-file vanilla JS/CSS. No dependencies, no build, no network.
