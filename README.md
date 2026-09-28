# AIBIRTH 💖🎂

Two separate surprise mini-games that run in any phone browser. Each one is a single
`index.html` file with no app to install and nothing to build.

| Project | Folder | Flow |
|---|---|---|
| 💘 **Valentine** | [`valentine/`](valentine/index.html) | Envelope → catch falling hearts → "Will you be my Valentine?" → love letter |
| 🎂 **Birthday** | [`birthday/`](birthday/index.html) | Envelope → pop the balloons → blow out the candles → birthday card |

## 💘 Valentine

1. **Envelope**: "Hey *name*, someone made you a little surprise…"
2. **Catch my heart**: they drag a basket to catch 💖 (💝 counts double, 💔 takes one away).
3. **"Will you be my Valentine?"**: tapping **No** does nothing except make **Yes** bigger each time 😄
4. **Love letter**: it types itself out, with optional photos and your signature.

## 🎂 Birthday

1. **Envelope**: "Hey *name*, it's your special day…"
2. **Pop the balloons**: they tap the rising 🎈 to pop them (🎁 counts double).
3. **Cake**: they tap the flames, or tap 🎤 and really blow into the phone. Confetti and a *Happy Birthday* tune follow.
4. **Birthday card**: your message types itself out.

## Personalise

Open the project's `index.html` and edit the `CONFIG` block near the top: names, the
letter text, and optional `photos` / `music`. The birthday version also has `age`, which sets the number of candles.

Photos and music go next to the file, for example `valentine/photos/us1.jpg` with
`photos: ["photos/us1.jpg"]`.

## Get a link to send

Any static host works, and each folder gets its own link:

- **Netlify Drop**: drag the `valentine` (or `birthday`) folder onto
  https://app.netlify.com/drop and you get a link instantly.
- **GitHub Pages**: repo **Settings → Pages → Deploy from a branch**. The links will be
  `https://<username>.github.io/AIBIRTH/valentine/` and `…/AIBIRTH/birthday/`.
  (Pages on a *private* repo needs a paid GitHub plan. On a free plan, make the repo public.)

The 🎤 blow feature needs an `https://` link. If the mic isn't allowed, tapping the flames still works.
