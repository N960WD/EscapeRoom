# Everything and Nothing

A two-player, pass-and-play card game for adult couples (18+). It runs entirely offline in any modern browser on a phone, tablet or laptop. There are no points and no winner.

## How to play
1. Before the first card, agree on your limits and a stop word. At setup, choose how many passes each player gets (1–3).
2. Players take turns tapping any numbered card. Each number can be played only once.
3. Each player has their own set list of cards, which is never shuffled. Whichever number a player taps, the next card on their list comes up, so the activities build in the planned order. Each player has 10 cards (20 in total).
4. The card flips and splits into two half-cards, each with a 2–4 word clue. **A** is always the gentler pick and **B** the bolder one.
5. The player picks one clue, and it flips to reveal the activity. "You" is the player who picked the card; the other player's name is filled in automatically.
6. **Done** or **Stop** (either player, any time) ends the activity, and it's the next player's turn.
7. **Pass** skips that card, and the same player picks again to get the next card on their list. If a player's list runs out, the other player keeps going until their list is done. With no passes left, the player does the activity (or someone calls Stop).
8. The game ends when every card on both lists has been played.

**Supply list:** scarf or soft tie, blindfold, ice, a drink, massage oil, lube, towels, and a playlist.

## Running it offline
- **Laptop:** copy the `everything-and-nothing` folder and double-click `index.html`.
- **Phone / tablet:** open the page once from any web server (for example GitHub Pages), then use *Add to Home Screen*. The included service worker caches the game so it works in airplane mode after that.

The game saves itself on the device, so a refresh or accidental close won't lose your place.

## Customizing the cards
Tap **Edit Cards** on the start screen or in the ☰ menu. Cards come up in exactly the order written:

```
# Player 1
## Round 1: Warm-Up
Card title | Clue A | Activity A | Clue B | Activity B
...
# Player 2
## Round 1: Warm-Up
...
```

Write `{you}` wherever the other player's name should appear. The board shows one number per card, up to 40 in total. You can also edit `DEFAULT_DECK` near the top of the script in `index.html`.
