# 🧩 Memory Puzzle

A simple, dependency-free memory (tile-matching) puzzle game. Flip two
tiles at a time, find every matching pair, and try to beat your best
move count and time. Built with plain HTML, CSS, and JavaScript — no
frameworks, no build step, no dependencies.

## Play it

Just open `index.html` in any browser — or enable **GitHub Pages** on
this repo (Settings → Pages → deploy from the `main` branch) to play it
at `https://<your-username>.github.io/memory-puzzle/`.

## Features

- Two difficulty levels: 4×4 (8 pairs) and 6×6 (18 pairs)
- Move counter and live timer
- Smooth 3D card-flip animation
- Keyboard-accessible (tab to a tile, press Enter/Space to flip)
- Respects `prefers-reduced-motion`
- Fully responsive — works on mobile and desktop
- Zero dependencies — a single self-contained `index.html`

## How to play

1. Click **New Game**, or pick a difficulty (4×4 or 6×6).
2. Click any tile to flip it face-up.
3. Click a second tile — if the symbols match, both stay face-up; if not,
   they flip back after a moment.
4. Match every pair to win. Your move count and time are shown at the top.

## Project structure

```
memory-puzzle/
├── index.html      # the entire game — markup, styles, and logic
├── .gitignore
└── README.md
```

## Customizing

- **Symbols:** edit the `SYMBOL_SETS` object in the `<script>` section of
  `index.html` to swap the emoji used for tile faces.
- **Grid sizes:** add another entry to `SYMBOL_SETS` and a matching button
  in the `.difficulty` group to add more board sizes.
- **Colors:** all colors are defined as CSS custom properties at the top
  of the `<style>` block (`--teal-deep`, `--mustard`, `--coral`, etc.).

## License

MIT — feel free to use, modify, and share.
