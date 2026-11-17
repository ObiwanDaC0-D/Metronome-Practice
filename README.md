# Metronome-Practice

A browser-based metronome, tuner, and passage-focused music practice tracker, designed for GitHub Pages.

**[Open the Practice Lab](https://obiwandac0-d.github.io/Metronome-Practice/practice.html)** · **[Open the metronome and tuner](https://obiwandac0-d.github.io/Metronome-Practice/)**

## What it does

- **Music library:** Organize instruments, compositions, and passages or measure ranges.
- **Practice sessions:** Count-up or countdown timer, goals, repetitions, starting tempo, highest clean tempo, notes, and self-assessed difficulty and mastery.
- **Metronome:** Embedded metronome and tuner, with experimental practice-timer integration and manual, repetition-based, or time-based tempo progression.
- **Progress:** Passage-specific session history, duration chart, clean-tempo records, and separate retention assessments.
- **Retention checks:** Record how accurately a passage can be performed before rehearsal and view a heuristic next-review suggestion.
- **Audio:** Record, replay, export, delete, and compare two performances in the same browser, subject to microphone permissions and browser support.
- **Export:** Session CSV, practice-data JSON, and a complete JSON export that includes audio recordings.

## Getting started

1. Open [Practice Lab](https://obiwandac0-d.github.io/Metronome-Practice/practice.html).
2. Add an instrument and composition in **Music library**.
3. Add a passage to the selected composition.
4. Set a practice target and starting tempo, then start a session.
5. Save the session assessment to record your progress.
6. Optionally record performances and conduct retention checks on later days.

## Storage and backups

Practice records are stored locally in the browser; recordings use IndexedDB. They are **not synchronized between devices**.

**Important:** The ordinary JSON export does **not** include audio. Use **Complete Backup (JSON + audio)** to export recordings along with practice data. At present, the import feature restores practice-data JSON only; it does **not** restore recordings from a complete backup. Keep your existing browser data until full restore support is implemented and tested.

Clearing browser/site data or using a different browser may make locally stored data unavailable.

## Browser considerations

- Microphone recording requires permission and a compatible browser on HTTPS.
- Mobile browsers, particularly iOS Safari, can suspend audio or timers when the app is backgrounded.
- Metronome synchronization, recovery, and backup workflows still require live-browser regression testing.

## Project files

- `index.html` — metronome and tuner
- `practice.html` — Practice Lab interface and browser-side data handling
- `README.md` — project documentation

## Status

This project is under active development. Features described here reflect the repository implementation, **not a guarantee that every workflow has been verified on every device**. Report reproducible issues in GitHub Issues.

This is a separate repository from the original Metronome project.
