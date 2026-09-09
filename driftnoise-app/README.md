# Drift Noise (PWA)

This folder is a complete, working web app. Once it's hosted on any HTTPS
URL, people can open it on iPhone or Android and add it to their home
screen — it launches full-screen with an icon, no browser chrome, and
plays offline after the first load.

## What's inside
- `index.html` — the player (tap-to-play, sleep timer, volume)
- `drift-noise.mp3` — your 18-minute seamless loop, engineered for sleep
- `manifest.json` — tells the phone this is installable, sets icon/name
- `sw.js` — service worker, caches everything for offline playback
- `icon-192.png` / `icon-512.png` — home screen icons

## Fastest way to get this live (free, ~2 minutes)

**Option A — Netlify Drop (no account needed for a quick test link)**
1. Go to https://app.netlify.com/drop
2. Drag this whole folder onto the page
3. You get a live URL immediately (e.g. `random-name.netlify.app`)

**Option B — GitHub Pages (free, permanent, your own URL)**
1. Create a new GitHub repo, upload these files to it
2. Repo Settings → Pages → Deploy from branch → `main` / root
3. Your app is live at `https://yourusername.github.io/reponame/`

## Installing it on a phone
- **iPhone:** open the URL in Safari → Share icon → "Add to Home Screen"
- **Android:** open the URL in Chrome → menu (⋮) → "Add to Home screen" /
  "Install app"

Once installed, it behaves like a native app: its own icon, full-screen,
no address bar, and it keeps playing with the phone locked (standard iOS/
Android audio-session behavior — no extra code needed).

## Going further (native App Store / Play Store listing)
This same code can be wrapped with **Capacitor** or **React Native** to
produce a real `.ipa` / `.apk` for store submission. That path needs:
- An Apple Developer account ($99/yr) + a Mac with Xcode, for iOS
- A Google Play Developer account ($25 one-time), for Android
- Store assets: screenshots, a privacy policy URL, app description

Happy to build that wrapped version and walk through the submission
checklist when you're ready to go that route.
