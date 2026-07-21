# Beyonder's Regimen — Install Guide

This is a Progressive Web App (PWA). It's a real, installable app icon on your
phone's home screen — works offline, no App Store needed. But browsers only
allow installing from a live web address (not directly from files on your
computer), so you need to host these files somewhere first. Two easy options:

## Option A — Netlify Drop (easiest, ~1 minute, free)
1. Go to https://app.netlify.com/drop on your computer.
2. Drag the whole `pwa` folder (this folder) onto the page.
3. Netlify gives you a live URL like `https://random-name-123.netlify.app`.
4. Open that URL on your phone's browser.
5. **iPhone (Safari):** tap the Share icon → "Add to Home Screen."
   **Android (Chrome):** tap the ⋮ menu → "Install app" (or you'll see an
   install banner pop up automatically — just tap "Install").
6. The app icon now lives on your home screen and opens full-screen, like
   any other app.

## Option B — GitHub Pages (free, a bit more setup)
1. Create a new GitHub repository and upload all files in this folder.
2. In the repo settings, enable GitHub Pages (serve from the main branch).
3. GitHub gives you a URL like `https://yourname.github.io/repo-name/`.
4. Open that URL on your phone and follow step 5 above.

## What's in this folder
- `index.html` — the entire app (self-contained, no build step needed)
- `manifest.json` — tells the phone this is an installable app (icon, name, colors)
- `sw.js` — service worker, caches the app so it works with no signal
- `icon-192.png` / `icon-512.png` — app icons

## Your progress
Everything you check off is saved directly on your phone (in the browser's
local storage), so it persists between sessions automatically. It does not
sync between devices — if you install it on a second phone, that copy starts
fresh. There's nothing to log in to or set up.
