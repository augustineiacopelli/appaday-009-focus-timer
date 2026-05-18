# 009 · Focus Timer

A Pomodoro-style focus timer with configurable work and break intervals, a circular progress ring, and a clean fullscreen mode.

## What It Does

Focus Timer runs a standard Pomodoro cycle: work sessions separated by short breaks, with a long break after a configurable number of completed sessions. A circular progress ring drains in real time, session dots show your position in the current cycle, and the accent color shifts from yellow to teal when a break begins. Desktop notifications fire when each phase ends.

## How to Use

1. Hit **Start** (or press **Space**) to begin a work session.
2. When the timer ends, the app automatically advances to the next phase — short break, long break, or back to work.
3. Use **Reset** (or **R**) to restart the current phase, and **Skip** (or **S**) to advance immediately.
4. Tap the **⚙** icon to open Settings and adjust work duration, short break, long break, and the number of sessions before a long break takes effect. Changes apply when you close settings.
5. Tap **⛶** to enter fullscreen mode for a distraction-free view.

## Technical Notes

- Vanilla HTML, CSS, and JavaScript — no frameworks or dependencies beyond Google Fonts.
- Progress ring uses SVG `stroke-dashoffset` on a single `<circle>` element driven by a `setInterval` tick.
- Desktop notifications use the browser Notifications API; permission is requested on first Start.
- Keyboard shortcuts: `Space` to start/pause, `R` to reset, `S` to skip.
- All state is in-memory; settings reset on page reload by design.

## Definition of Complete

- [x] Work session counts down with a visible progress ring
- [x] Short break and long break phases trigger automatically on session completion
- [x] Session dot indicators track position in the Pomodoro cycle
- [x] Work/break durations and sessions-per-cycle are configurable
- [x] Fullscreen mode available
- [x] Desktop notification fires on phase completion
- [x] Keyboard shortcuts functional
- [x] Mobile friendly at 375px viewport
- [x] Published to GitHub Pages
