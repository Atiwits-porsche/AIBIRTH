# AIBIRTH 💖

A surprise Valentine + Birthday mini-game that runs in any phone browser. It's a single
`index.html` file with no app to install and nothing to build.

## What the recipient sees

1. **Envelope**: "Hey *name*, someone made you a little surprise…"
2. **Catch my heart**: they drag a basket to catch falling 💖 (💝 counts double, 💔 takes one away).
3. **Birthday cake**: they tap the flames to blow out the candles, or tap 🎤 and really blow
   into the phone. Confetti and a *Happy Birthday* tune follow.
4. **"Will you be my Valentine?"**: the **No** button runs away and the **Yes** button keeps growing 😄
5. **Love letter**: it types itself out, with optional photos, a signature and a "More love" confetti button.

## Personalise it

Open `index.html` and edit the `CONFIG` block near the top:

```js
toName: "My Love",     // their name
fromName: "Me",        // your name
age: 25,               // candles on the cake
heartsToWin: 14,
question: "Will you be my Valentine?",
letter: [ "...", "..." ],        // your message, one line per paragraph
photos: ["photos/us1.jpg"],      // optional: add images to a photos/ folder
music: "music/our-song.mp3",     // optional: add an mp3 to a music/ folder
```

## Get a link to send

Any static host works. Pick one:

- **GitHub Pages**: repo **Settings → Pages → Deploy from a branch → `main` / root**.
  The link will be `https://<username>.github.io/AIBIRTH/`.
  (GitHub Pages on a *private* repo needs a paid GitHub plan. On a free plan, make the repo public.)
- **Netlify Drop**: drag the project folder onto https://app.netlify.com/drop and you get
  a link instantly.

The 🎤 blow feature needs an `https://` link, which both options give you.
If the mic isn't allowed, tapping the flames still works.

## Test locally

Open `index.html` in a browser. To test on your phone over Wi-Fi, run
`python3 -m http.server` and open `http://<your-computer-ip>:8000`.
