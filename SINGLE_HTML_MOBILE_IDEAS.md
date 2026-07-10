# Single HTML File, Mobile-First — Brainstorm

Self-contained (inline CSS/JS, no build step, no server) apps that work great as one `.html` file on a phone.

## Utility Tools
1. **Tip & Bill Splitter** - calculator with slider, saves last split via localStorage
2. **Unit Converter** - length/weight/temp/currency, offline-capable
3. **QR Code Generator** - canvas-based, no external API
4. **Countdown/Timer/Stopwatch** - laps, vibration on finish
5. **Random Picker/Spinner Wheel** - names, decisions, canvas animation
6. **Color Picker & Palette Generator** - eyedropper, export hex codes
7. **Text Diff Checker** - paste two texts, highlight differences
8. **QR/Barcode Scanner** - via `getUserMedia` camera API

## Trackers & Loggers
9. **Habit Tracker Grid** - tap-to-check calendar, localStorage streaks
10. **Water Intake Tracker** - tap glass icons, daily reset
11. **Expense Logger** - quick-add entries, category totals, localStorage
12. **Mood Journal** - emoji picker + note, saved chronologically
13. **Workout Rep Counter** - big tap zone, vibration feedback per rep
14. **Period/Cycle Tracker** - simple calendar with predictions

## Games (single-file, canvas/DOM)
15. **Flappy Bird Clone** - canvas + touch controls
16. **2048** - swipe gestures, localStorage high score
17. **Memory Match Cards** - flip animation, timer
18. **Whack-a-Mole** - touch targets, difficulty scaling
19. **Trivia Quiz** - JSON question bank embedded inline
20. **Word Scramble/Hangman** - embedded word list

## Fun & Creative
21. **Voice Memo Recorder** - MediaRecorder API, playback, download
22. **Doodle/Sketch Pad** - canvas drawing, touch/pressure support, save as image
23. **Photo Filter Booth** - camera + CSS filters, download result
24. **Meme Generator** - camera/upload + draggable text overlay
25. **Business Card Scanner** - camera + manual field entry, vCard export
26. **QR Business Card** - fill form, generates shareable QR vCard

## Reference/Info
27. **Flashcard Study App** - swipe deck, spaced repetition logic in JS
28. **Recipe Card Viewer** - embedded JSON recipes, checklist mode for ingredients
29. **Offline Cheat Sheet** - searchable reference (e.g. keyboard shortcuts, regex)
30. **Emergency Info Card** - medical info, ICE contacts, works fully offline

## Why single-file mobile-first works well
- **Zero install** - share via link, works instantly
- **PWA-able** - add manifest+SW later without rewriting
- **Offline-first** - localStorage/IndexedDB, no backend needed
- **Easy to test** - open directly in mobile browser, no build tooling
- **Touch-first UI** - large tap targets, swipe gestures, `100dvh` viewport, avoid hover-only interactions

## Quick tech checklist for any pick
- `<meta name="viewport" content="width=device-width, initial-scale=1">`
- CSS: flexbox/grid, `env(safe-area-inset-*)` for notches, `touch-action`
- Storage: `localStorage`/`indexedDB` for persistence
- Optional: `manifest.json` + Service Worker inline via Blob for installable PWA
