# Steady Workout Tracker (PWA)

A mobile-first, installable workout planner and log. It runs without a framework or build step.

## Features
- Start Strength A, Gym Conditioning B, or Strength B C sessions.
- Tick exercises, record weights/resistance and reps, add duration and notes.
- Monthly calendar with planned and completed workouts.
- Edit a plan on any date, including moving or removing a planned workout.
- Six-week upcoming plan and weekly/completed session counts.
- Local browser storage and JSON export/import backup.
- Offline app shell via service worker.

## Run locally
A PWA service worker requires `localhost` or HTTPS. From this directory run:

```sh
python3 -m http.server 8000
```

Then open `http://localhost:8000` on the same device. For phone installation, host this folder on an HTTPS static host (for example GitHub Pages, Netlify, or Cloudflare Pages), then open the HTTPS URL in Chrome on Android and choose **Install app** or **Add to Home screen**.

## Data and privacy
Workout records are stored in `localStorage` in the browser on the device. They are not synced across devices. Use **Plan → Export backup** regularly, and before clearing browser data or switching phones.

## Notes
- Default schedule: Monday A, Wednesday B, Saturday C.
- The app does not send notifications or sync to a server.
