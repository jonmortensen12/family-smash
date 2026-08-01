# Family Smash

A local-multiplayer fighting game. Five fighters, seven stages, playable in any
browser and installable to a phone home screen.

## Files

| File | What it is |
| --- | --- |
| `index.html` | The whole game. Faces, sounds and stages are all embedded. |
| `manifest.webmanifest` | Tells the phone the name, icon and that it opens fullscreen. |
| `sw.js` | Service worker. Makes it installable and playable with no signal. |
| `icon-192.png` / `icon-512.png` | Home screen icons. |

All four support files must sit in the **same folder** as `index.html`.

## Putting it on GitHub

1. Go to <https://github.com/new>. Name the repository `family-smash`.
   Leave it **Public** — GitHub Pages needs public on a free account.
   Don't add a README (this file is one). Click **Create repository**.
2. On the new empty repo page, click **uploading an existing file**.
   Drag in all five files. Click **Commit changes**.
3. Go to **Settings → Pages**.
   Under *Build and deployment*, set Source to **Deploy from a branch**,
   branch to **main**, folder to **/ (root)**. Click **Save**.
4. Wait about a minute, then refresh the Pages settings screen. It will show
   the live address:

   ```
   https://<your-username>.github.io/family-smash/
   ```

## Installing it

- **iPhone / iPad** — open the address in **Safari** (not Chrome; only Safari
  can install to the home screen on iOS). Tap Share, then **Add to Home
  Screen**. It launches fullscreen with no browser bars.
- **Android** — open in Chrome, tap the ⋮ menu, then **Install app**.
- **Computer** — just visit the address. Chrome and Edge show an install
  icon at the right of the address bar if you want it as a desktop app.

## Updating it later

Replace `index.html` in the repo (drag a new one onto the file list, or use
**Add file → Upload files**) and commit. The service worker checks the network
first, so the new version appears on the next load. If a phone ever seems
stuck on an old build, close the app fully and reopen it.

## Controls

**Gamepad** — left stick moves, up on the stick jumps. Cross jump, Square
attack, Circle special, Triangle grab, R1 shield, L1 smash, Options menu.

**Two players on one keyboard** — in the menu set one slot to *Keys: WASD* and
the other to *Keys: arrows*.

| | WASD side | Arrows side |
| --- | --- | --- |
| Move / jump / duck | A D · W · S | ← → · ↑ · ↓ |
| Attack | F | . |
| Special | G | / |
| Grab | T | ; |
| Smash | R | , |
| Shield | H | ' |

**One player on a keyboard** — *Keyboard*: A/D move, W jump, S fast-fall,
J attack, K special, U grab, I smash, L shield, arrow keys act as the c-stick.
Esc opens the menu.
