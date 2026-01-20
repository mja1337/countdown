# Countdown

A simple, elegant countdown timer web application that uses your device's local clock. Set a target time in 12-hour format and watch it count down until the moment arrives.

## Features

- **Easy Setup** — Set a target time using hour and minute inputs with AM/PM selector
- **Smart Scheduling** — If your target time has already passed today, it automatically counts down to tomorrow
- **Start/Pause/Reset Controls** — Full control over the countdown with intuitive buttons
- **Live Clock Display** — See the current time and target time updated in real-time
- **Quick Actions** — "Set to next hour" button for fast scheduling
- **Responsive Design** — Works beautifully on mobile and desktop
- **Dark Theme** — Modern glassmorphism UI with gradient accents
- **No Dependencies** — Pure HTML, CSS, and vanilla JavaScript

## How to Use

1. **Set your target time** — Enter the hour (1-12) and minute (0-59), then select AM or PM
2. **Start the countdown** — Click the "Start" button to begin
3. **Manage the timer**:
   - **Pause** — Temporarily stop the countdown without resetting
   - **Resume** — Click "Start" again to continue from where it paused
   - **Reset** — Clear the countdown and return to the start state
4. **Quick set** — Use "Set to next hour" for fast scheduling

## Display Elements

- **Main Clock** — Shows the remaining time in `HH:MM:SS` format with status indicator
- **Now Pill** — Displays the current local time
- **Target Pill** — Shows your scheduled target time
- **Mode Pill** — Indicates the countdown state (Not running, Counting down, Paused)

## Technical Details

- Built with vanilla HTML, CSS, and JavaScript
- Uses the browser's `Date` API for accurate local timekeeping
- Leverages `requestAnimationFrame` for smooth, performant updates
- Fully responsive with mobile-first design
- No external dependencies required

## Browser Compatibility

Works on all modern browsers that support ES6 JavaScript (Chrome, Firefox, Safari, Edge, and modern mobile browsers).
