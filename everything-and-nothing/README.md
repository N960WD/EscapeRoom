# Everything and Nothing

A two-player, pass-and-play card game for adult couples (18+). It runs entirely offline in any modern browser on a phone, tablet or laptop. There are no points and no winner.

## How to play
1. Before the first card, agree on your limits and a stop word. At setup, choose how many passes each player gets (1–3).
2. Players take turns tapping a numbered card. Each card can be played only once.
3. The 30 cards come in three rounds: **Warm-Up** (1–14), **Heat** (15–23) and **Main Event** (24–30). Cards are shuffled within each round, and the next round unlocks when the current one is finished.
4. The card flips and splits into two half-cards, each with a 2–4 word clue. **A** is always the gentler pick and **B** the bolder one.
5. The player picks one clue, and it flips to reveal the activity. "You" is the player who picked the card; the other player's name is filled in automatically.
6. **Done** or **Stop** (either player, any time) ends the activity, and it's the next player's turn.
7. **Pass** uses up the card, and the same player picks a new card. With no passes left, the player does the activity (or someone calls Stop).
8. The game ends when all 30 cards have been played.

**Supply list:** scarf or soft tie, blindfold, toy, ice, a drink, massage oil, massage candle, lube, towels, a playlist, and a mirror.

## Running it offline
- **Laptop:** copy the `everything-and-nothing` folder and double-click `index.html`.
- **Phone / tablet:** open the page once from any web server (for example GitHub Pages), then use *Add to Home Screen*. The included service worker caches the game so it works in airplane mode after that.

The game saves itself on the device, so a refresh or accidental close won't lose your place.

## Customizing the cards
Tap **Edit Cards** on the start screen or in the ☰ menu. A line starting with `#` begins a round (for example `# Round 2: Heat`). Every other line is one card:

```
Card title | Clue A | Activity A | Clue B | Activity B
```

Write `{you}` wherever the other player's name should appear. The board holds exactly 30 cards. You can also edit `DEFAULT_DECK` near the top of the script in `index.html`.
