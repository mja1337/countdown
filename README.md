# Meeting Countdown

A sleek, feature-rich countdown timer for tracking meetings with built-in break reminders. Set a meeting start and end time, and the app counts down to the end while intelligently managing breaks at the halfway point.

## Features

- **Meeting-Centric Design** — Set both start and end times for complete meeting tracking
- **Intelligent Break Scheduling** — Automatically places a 5-minute break at the 50% mark of your meeting
- **Smart Countdown Logic** — Before the meeting starts, counts down to the start time; once started, counts down to the end time
- **Visual Break Alerts** — Display flashes during the last 30 seconds before the break and while the break is active
- **Pause & Resume** — Intelligently pause and resume, whether before or during the meeting
- **Session Persistence** — Automatically saves and restores your meeting times via localStorage
- **Live Time Display** — Real-time current time, meeting times, and break schedule displayed in elegant pills
- **Datetime Input** — Easy date-and-time picker interface for precise scheduling
- **Quick Setup** — "Now + 30m" button for instant meeting scheduling
- **Responsive Design** — Optimized for both mobile and desktop
- **Dark Theme** — Beautiful glassmorphism UI with purple and green gradient accents
- **No Dependencies** — Pure HTML, CSS, and vanilla JavaScript

## How to Use

1. **Set meeting times** — Use the datetime inputs to specify when your meeting starts and ends
2. **Quick setup** — Click "Now + 30m" to automatically set a meeting starting now, ending in 30 minutes
3. **Start the countdown** — Click "Start" to begin tracking
4. **Manage the timer**:
   - **Pause** — Temporarily freeze the countdown without losing progress
   - **Resume** — Click "Start" again to continue from where you paused
   - **Reset** — Clear everything and return to the setup state
5. **Monitor the break** — The interface shows when your 5-minute break is scheduled and alerts you when it approaches

## Display Elements

- **Main Timer** — Shows remaining time in HH:MM:SS format with a status indicator (Waiting to start / Until end / On break / Done)
- **Now Pill** — Live display of current local time (updates every 250ms)
- **Meeting Pill** — Shows the scheduled meeting start and end times
- **Break Pill** — Displays break timing and countdown (5 minutes at the 50% point)
- **Mode Pill** — Indicates the current state (Not running / Waiting to start / Running / Break / Paused / Finished)

## Break Logic

The break window is calculated at 50% of the total meeting duration and automatically:
- **Before the meeting** — Shows the exact break time and counts down to it
- **During the meeting** — Tracks your break, warning you 30 seconds before it starts
- **After the break** — Shows that the break is complete

Flash animations trigger when:
- 30 seconds remain before the break starts
- The break is currently active

## Keyboard Shortcuts

- **Enter** — While editing start or end time, press Enter to start the countdown immediately

## Technical Details

- Built with vanilla HTML, CSS, and JavaScript (ES6)
- Uses the browser's `Date` API for accurate local timekeeping
- Smart state management supporting pause/resume before and during meetings
- localStorage integration for automatic session recovery
- Efficient rendering with 200ms update intervals
- Fully responsive with mobile-first CSS Grid layout
- CSS custom properties for easy theming

## Browser Compatibility

Works on all modern browsers that support ES6 JavaScript (Chrome, Firefox, Safari, Edge, and modern mobile browsers).
