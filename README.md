# recalc — Excel reps for analysts

A Monkeytype-style practice arena for Excel fluency, built for investment banking
analysts. Open it, get 60 seconds of real reps, feel sharper, close it. One file,
no install, keyboard-first.

## Run it

Double-click **`index.html`**. That's it — it runs offline in any modern browser.

(Optional, for a localhost URL: `python -m http.server 5188 --directory .` then open
http://localhost:5188/)

## Build — the main loop

**Build** trains the real analyst muscle: constructing a formula by *typing fragments
and selecting references live in a mini-workbook* — Excel "point mode", not transcription.

A generated scaffold shows the target (e.g. `=SUMIFS($H$16:$H$21, $F$16:$F$21, "South")`).
You reproduce it by:

1. **Type** the function and punctuation: `=SUMIFS(`
2. **Point** to the first reference — arrow over the grid, `Ctrl+Arrow` to leap data
   edges, `Shift` / `Ctrl+Shift+Arrow` to extend a range. The reference fills in live.
3. **Anchor** it — `F4` cycles `A1 → $A$1 → A$1 → $A1`. The scaffold shows the `$` you owe.
4. **Lock** it — type the next `,` or `)` (just like Excel, the delimiter accepts the
   reference and types itself), then keep going.
5. **Enter** to finish.

The workbook is a small but real-feeling model — years across the top, a revenue → EBITDA
build, an assumptions block (the `$`-anchor targets), and a comps/lookup table. References
in the scaffold point at actual coordinates, so the rep is pure movement + selection +
anchoring, never a finance word problem. Categories: `sums`, `model`, `anchor`, `lookups`,
`logic`.

## Also included

- **Sprint** — pure typing speed. A generative engine builds endless banker formulas
  (`SUMIFS`, `XLOOKUP`, `INDEX/MATCH`, mixed `$`, cross-sheet refs, live model lines).
  **Excel-style function autocomplete** is built in: type a few letters and a dropdown of
  matching functions appears (the real ~230-function library); `↑`/`↓` to pick, `Tab` to
  insert up to the `(`. Case-insensitive; `Enter` auto-closes trailing `)`. Toggle with `fx`.
- **Warmup** — isolated grid drills: go-to, jump, range select, and the `F4` anchor cycle.
  A quick way to loosen up the movement and selection gestures before a Build session.

## The loop

| Action | Key |
| --- | --- |
| Start a run | just start typing ( `=` ) |
| Point to a reference | arrows · `Ctrl+Arrow` leaps data edges |
| Extend to a range | `Shift+Arrow` · `Ctrl+Shift+Arrow` |
| Anchor the reference | `F4` |
| Lock the reference | type the next `,` or `)` — or `Tab` |
| Fix a mistake | `Backspace` |
| Restart, same settings | `Tab` |
| Back to menu / abort | `Esc` |
| Run it back (results screen) | `Tab` or `Enter` |

## Results

Build scores what matters for the rep: **formulas/min**, **accuracy**, **ref + anchor
accuracy** (references locked correctly first try — right range *and* right `$`),
**keystroke efficiency** (par ÷ your keys — rewards `Ctrl+Arrow` leaps over tapping),
**rework**, completion time, slowest constructs, and most-fumbled keys. Type WPM is kept
as a secondary stat. Sprint reports Monkeytype-style WPM / consistency / weak keys; Warmup
reports tasks/min and efficiency. Personal bests and a run-history sparkline persist locally.

## Settings

Category · time/count modes. Four themes (`excel`, `amber`, `slate`, `paper`) and an
optional keypress sound, top-right. Everything persists locally.

Single-file vanilla JS/CSS. No dependencies, no build, no network.
