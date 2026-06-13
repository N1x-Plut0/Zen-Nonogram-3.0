# Zen Nonogram · 禅

A calm, paper-and-moss themed nonogram (picross) game. Reveal hidden pictures by
filling grid squares according to the numeric clues on each row and column.

Everything lives in a single self-contained file — **[index.html](index.html)** —
with no build step and no dependencies.

## Run it

Just open `index.html` in any modern browser (double-click it, or drag it into a
browser window). That's it.

> If you prefer serving it over `http://` (handy on some systems), run any static
> server in this folder, e.g. `python -m http.server` and visit
> `http://localhost:8000`.

## Features

- **Level library** — built-in puzzles from 5×5 up to 20×20, in soft multi-colour palettes.
- **Compound puzzles** — solve a set of small tiles that combine into one larger picture.
- **Puzzle editor** — draw your own solutions, pick a size and colours, and save them.
- **Accounts (optional)** — register a local username/password to keep your own saved
  puzzles and solved-progress separate. You can also just play as a guest.
- **Quality-of-life** — click-and-drag fill, auto-cross completed lines, undo/redo
  (Ctrl+Z / Ctrl+Y), and a gentle win celebration.

## How saving works

The game stores everything in your browser via `localStorage` — accounts, custom
puzzles, and which levels you've solved all persist across refreshes on the same
browser. Clearing your browser data will reset it. Nothing is sent to any server.

> Note: accounts are a lightweight local convenience only. Passwords are hashed,
> but this is **not** real security — don't reuse an important password here.

## Project layout

```
Zen-Nonogram/
├── index.html   ← the entire game (HTML + CSS + JS)
└── README.md
```
