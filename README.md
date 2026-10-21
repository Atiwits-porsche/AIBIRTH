# AIBIRTH 💖🎂

Two separate surprise mini-games that run in any phone browser. Each one is a single
HTML file with no app to install and nothing to build.

| Project | Folder | Games on the map | Final surprise |
|---|---|---|---|
| 💘 **Valentine** | [`valentine/`](valentine/valentine.html) | Catch my heart · Find the pairs · Secret scratch card · Cupid's Arrow · Photo puzzle | "Will you be my Valentine?" → love letter |
| 🎂 **Birthday** | [`birthday/`](birthday/birthday.html) | Pop the balloons · Find the gift · Unwrap the gift · Cake Stacker · Spin the Wheel | Blow out the candles → birthday card |

## How it works

After the envelope, a **game map** shows all 5 games. They can be played in any order. Each finished
game lights up a ❤️ (Valentine) or ⭐ (Birthday), and the final surprise unlocks when all 5 are done.
A ← button in each game goes back to the map. In every Valentine game, a **Kiss me 💋** button
skips just that game (it counts as finished) and goes back to the map. Progress is remembered if the page is closed, and
**Replay** on the last screen starts over.

## 💘 Valentine games

- **Catch my heart**: drag a basket to catch 💖 (💝 counts double, 💔 takes one away).
- **Find the pairs**: flip cards to match 6 pairs (💖 🌹 💌 🍫 🧸 💍).
- **Secret scratch card**: rub the card to reveal your message (`secret`).
- **Cupid's Arrow**: tap to shoot arrows straight up and hit 5 flying hearts.
- **Photo puzzle**: slide the pieces back into place (3×3). Uses `puzzlePhoto`, or a heart picture with their name.
- **Final**: "Will you be my Valentine?" (No does nothing, Yes grows) → the love letter.

## 🎂 Birthday games

- **Pop the balloons**: tap the rising 🎈 (🎁 counts double).
- **Find the gift**: a 🎁 hides under one of 3 party hats, the hats shuffle, and they tap the right one. 3 rounds, each faster.
- **Unwrap the gift**: tap the present 8 times to reveal `giftMessage`.
- **Cake Stacker**: tap to drop sliding cake layers; whatever hangs over the edge falls off. Stack 8 to win.
- **Spin the Wheel**: spin for a prize from `wheelPrizes`. Set `wheelWinner` to a number to always land on that prize (0 = first).
- **Final**: blow out the candles (tap, or 🎤 blow into the phone) → the birthday card.

## Personalise

Open `valentine/valentine.html` or `birthday/birthday.html` and edit the `CONFIG` block near the top: names, the
letter text, and optional `photos` / `music`. Valentine also has `secret` and `puzzlePhoto`; Birthday has `age`
(number of candles), `giftMessage`, `wheelPrizes` and `wheelWinner`.

Photos and music go next to the file, for example `valentine/photos/us1.jpg` with
`photos: ["photos/us1.jpg"]`.

## Get a link to send

Any static host works, and each folder gets its own link:

- **Netlify Drop**: drag the `valentine` (or `birthday`) folder onto
  https://app.netlify.com/drop and send the link it gives you, for example
  `https://your-site.netlify.app/`.
- **GitHub Pages**: repo **Settings → Pages → Deploy from a branch**. The links will be
  `https://<username>.github.io/AIBIRTH/valentine/` and `…/AIBIRTH/birthday/`.
  (Pages on a *private* repo needs a paid GitHub plan. On a free plan, make the repo public.)

Each folder has a tiny `index.html` that jumps straight to the game, which keeps the
links short. The long form (`…/valentine/valentine.html`) works too.

The 🎤 blow feature needs an `https://` link. If the mic isn't allowed, tapping the flames still works.
