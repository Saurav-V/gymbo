# Gymbo

A personal gym log, built as a Progressive Web App (PWA). Aesthetics inspired by GMUNK's HUD designs for the film Oblivion (2013). It runs in the browser, installs to an Android home screen like a normal app, and works offline. There's no app store, account or server: it is hosted on GitHub Pages and your data stays on your phone.

**Live app:** https://saurav-v.github.io/gymbo/

## Features

- **Routines:** build routines, reorder exercises and routines by dragging, and give each routine a colour.
- **Workouts:** log sets with weight and reps, and see what you did last time next to each set. You can also:
  - mark sets as warm-ups and add notes per exercise;
  - reorder or replace exercises mid-workout;
  - use a count-up rest timer.
- **Deload mode:** sets weights to 75%, rounded to the nearest 2.5 kg, without affecting your "Previous" values or records.
- **Records:** celebrates a new heaviest weight or best set volume, and marks past workouts that set records.
- **Exercise library:** a built-in exercise bank with muscle-group images and how-to steps, plus your own custom exercises. Search works by name, equipment or muscle.
- **Weekly targets:** a glyph on the Home screen tracks sessions, duration and volume against your goals (weeks run Monday to Sunday).
- **Backup and export:** save a backup file and import it again, and download your stats as a CSV.
- **Haptics:** short vibrations on key actions, which you can switch off.

## Install on your phone

1. Open the live app link in Chrome (or Firefox) on Android.
2. Choose **Add to Home screen** or **Install app** from the browser menu.

## Your data

Everything is stored in the browser's local storage on your device. The app asks the browser to keep that storage persistent, but clearing site data or uninstalling the browser will still erase it. Use **Save backup** on the Profile screen regularly.

## Project structure

```
index.html            The whole app: markup, styles and script
sw.js                 Service worker: offline caching
manifest.webmanifest  App name, colours and icons for installing
icons/                App icons and favicon
muscles/              Muscle-group images used in the exercise picker and info pages
```
