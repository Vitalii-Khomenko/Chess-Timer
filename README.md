# Chess Timer

A lightweight, full-screen, mobile-friendly chess clock built as a single HTML file.

## Highlights

- Responsive layout designed for smartphone touch input.
- Two independent player timers with turn switching.
- Configurable base time (minutes) and per-move increment (seconds).
- Face-to-face mode with the top side rotated for Player 2.
- Clear state indicators for active play, low time, and time loss.
- Active player highlighted in green.
- Low-time warning in orange during the last 10 seconds.
- Time loss shown in red with a "TIME UP" message.
- Central controls for `Pause/Resume`, `Reset`, and `New` game setup.

## How It Works

1. Open `index.html` in any modern browser.
2. Set:
   - `Minutes per player`
   - `Extra Seconds (Increment)`
3. Press `START`.
4. Start the clock by tapping the side of the player who is to move first.
5. After each move, tap your own side to end your turn and start the opponent's clock.
6. Use:
   - `Pause/Resume` to temporarily stop or continue.
   - `Reset` to restart with current setup values.
   - `New` to return to setup and choose different time controls.

## Technical Notes

- Runs fully offline.
- No external libraries or frameworks.
- Includes protection against duplicate animation loops for stable timing behavior.

## Manual Smoke Check (Phone)

Use this quick checklist on a real smartphone (for example Samsung A55):

1. Open `index.html`, set `5` minutes and `2` increment, tap `START`.
Expected: setup screen hides, both timers show `05:00`, center button shows `Start`.
2. Tap Player 1 area once.
Expected: Player 1 timer starts decreasing, Player 1 side is active (green), button shows `Pause`.
3. Tap Player 1 area again after 2-3 seconds.
Expected: turn switches to Player 2, Player 1 gets `+2` seconds, Player 2 timer starts decreasing.
4. Tap `Pause`, wait 3 seconds, then tap `Resume`.
Expected: time does not change while paused, then continues from same value after resume.
5. Set a very short game (`1` minute, `0` increment), let one side run to zero.
Expected: losing side becomes red, shows `TIME UP`, timer stops, button shows `Game Over`.
6. Tap `Reset`.
Expected: confirmation dialog appears; after confirm, game resets with same setup values.
7. Tap `New`.
Expected: returns to setup screen and allows changing time controls.

## Stack

- HTML5
- CSS3
- Vanilla JavaScript (ES6+)
