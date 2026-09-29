# Everything and Nothing

A two-player, pass-and-play activity card game. It runs entirely offline in any modern browser on a phone, tablet or laptop. There are no points and no winner.

## How to play
1. Players take turns tapping a numbered card (1–30). Each card can be played only once.
2. The card flips and splits into two half-cards, each with a 2–4 word clue.
3. The player picks one clue, and it flips to reveal the activity: something they do, something they do for or to the other player, or something the other player does for them.
4. **Done**: the activity is finished and it's the next player's turn.
5. **Stop**: either player can call stop at any time. The activity ends and it's the next player's turn.
6. **Pass**: each player has 3. Passing uses up the card, and the same player picks a new card. With no passes left, the player must do the activity (or someone calls Stop).
7. The game ends when all 30 cards have been played.

## Running it offline
- **Laptop:** copy the `everything-and-nothing` folder and double-click `index.html`.
- **Phone / tablet:** open the page once from any web server (for example GitHub Pages), then use *Add to Home Screen*. The included service worker caches the game so it works in airplane mode after that.

The game saves itself on the device, so a refresh or accidental close won't lose your place.

## Customizing the cards
Tap **Edit Cards** on the start screen or in the ☰ menu. Put one activity on each line as `Clue | Activity`. Use `{me}` for the player who picked the card and `{you}` for the other player. Each new game randomly deals 60 activities onto the 30 cards. You can also edit `DEFAULT_DECK` near the top of the script in `index.html`.
