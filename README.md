# Vasen 4 kuollut

A guessing game built from Microsoft's Finnish support page for Edge Game
Assist, where every game title was run through a machine translator. You
get the mangled Finnish title ("Vasen 4 kuollut 2", "Kuppipää", "Nössöt
aallot") and have to name the real game.

Play it at <https://lambdakilo.github.io/vasen-4-kuollut/>.

## How a round works

- Pick 10, 20 or all 108 titles.
- Type the English name of the game. Letter case, punctuation, spaces and
  accents are ignored, but the words and numbers have to match, so
  "red dead redemption 2" is right and "rdr2" is not.
- A correct answer without hints is worth 4 points. Hints unlock in order,
  director, release year, then genre, and each one costs a point.
- Three wrong guesses or giving up reveals the answer for 0 points, together
  with a note on what the translator got wrong.

## Source

The titles come from the Finnish version of [Games Enhanced for Microsoft
Edge Game Assist](https://support.microsoft.com/fi-fi/edge/enhanced-games-for-microsoft-edge-game-assist),
with the English names taken from the en-US version of the same page. Only
titles the translator actually changed are included. The hint facts come
from each game's Wikipedia infobox.

## Files

The whole site is `index.html`, a single page with no build step and no
dependencies beyond Google Fonts. GitHub Pages serves it from the root of
`main`; `.nojekyll` keeps Jekyll out of the way.
