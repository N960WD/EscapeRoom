# Everything and Nothing

A two-player, pass-and-play card game for adult couples (18+). It runs entirely offline in any modern browser on a phone, tablet or laptop. There are no points and no winner.

## How to play
1. Take turns tapping any numbered card. Each number can only be played once.
2. The card first shows its title for 5 seconds so you can read it aloud. Then it flips and splits into two halves, each with a short clue. **A** is always the gentler pick, **B** the bolder one.
3. Choose one clue — it flips to reveal the activity. "You" means the player who picked the card.
4. **Pass** — each player has a set number of passes (chosen at the start). Tap **Pass** as soon as the card flips, or after you've revealed the activity. If you choose to pass, the other player goes next. Tap a player's name to see how many passes they have left.
5. **Stop** — either player can say "stop" out loud at any time and the game ends (☰ → **End Game** in the app).
6. The game ends when every card has been played. No points, no winner. Just fun.

Behind the scenes, each player has their own fixed list of cards: whichever number they tap, the next card on their list comes up. If one player's list runs out first, the other player takes the remaining turns.

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
