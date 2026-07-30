# CipherScale

A standalone browser prototype for a timed multiplayer word-guessing party game.

## Run it

Open `index.html` in any modern browser. No server, installation, or internet connection is required.

For a local web server instead:

```bash
python3 -m http.server 8080
```

Then visit `http://localhost:8080`.

## Prototype features

- One human player plus 1–7 configurable bot opponents
- Easy, normal, and hard bot behavior
- 3–2–1 countdown followed by a locked 5-second input window
- Speed-based scoring for correct guesses
- No penalty for wrong guesses
- Point penalties for blank or repeated answers
- Circular player layout with a CSS-drawn cyan lizard host
- Responsive noir interface, sound effects, round log, and final leaderboard

## Future online version

The core game state can later be moved to a server-authoritative WebSocket backend. The browser would send only locked guesses, while the server controls countdowns, word selection, scoring, reconnects, rooms, and anti-cheat checks.
