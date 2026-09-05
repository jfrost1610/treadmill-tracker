# treadmill-tracker

A single-page web app for building and running incline treadmill walk routines. Set up a sequence of stages — incline %, speed, and duration — and it cycles through them automatically with a countdown timer and an audio cue at each transition.

**Live app:** https://jfrost1610.github.io/treadmill-tracker/

## Features

- Build a routine from any number of stages (incline, speed, minutes)
- Visual elevation/terrain profile of the whole routine, with the active stage highlighted
- Auto-advancing timer with a chime on each stage change and a preview of what's next
- Pause, resume, and reset controls
- mph / km/h toggle
- Routine is saved automatically in the browser (`localStorage`) so it's there next time
- No build step, no dependencies — a single `index.html` file

## Using it on iPhone

1. Open the live app link above in **Safari**
2. Tap the **Share** icon
3. Tap **Add to Home Screen**

It'll launch full-screen from your home screen like a native app.

## Notes / limitations

- Routine data is stored per-browser (`localStorage`), so it won't sync across devices — each device/browser keeps its own saved routine
- iOS does not allow web apps to vibrate, and the timer pauses if the screen locks or the app is backgrounded — keep the screen on and the app in the foreground during a session
- This repo is public, which is required for free GitHub Pages hosting

## Local development

No build step required. Just open `index.html` directly in a browser, or serve it with any static file server.
