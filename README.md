# Chess Timer

A simple, lightweight, and responsive chess timer web application designed for smartphones.

## Features

*   **Responsive Design:** Optimized for mobile screens with large touch areas.
*   **Dual Timers:** Supports two players with independent countdowns.
*   **Customizable Time Controls:** Set initial minutes and increment (in seconds) per move.
*   **Face-to-Face Mode:** Player 2's interface is inverted for easy viewing from the opposite side of the device.
*   **Visual Indicators:**
    *   Green background for the active player.
    *   Red background and "TIME UP" message when time runs out.
*   **Controls:** Pause, Reset, and detailed configuration settings.
*   **Single File:** All HTML, CSS, and JavaScript are contained in one `index.html` file, requiring no internet connection or external dependencies.

## How to Use

1.  Open `index.html` in your web browser (mobile preferred).
2.  **Setup:**
    *   Enter the desired time in minutes.
    *   Enter the increment in seconds (optional).
    *   Click "START".
3.  **To Start the Game:**
    *   **The player who moves first should tap their own timer area to start their time.**
4.  **During Play:**
    *   After making a move, tap your timer area to end your turn and start the opponent's timer.
    *   The timer adds the increment (if set) automatically when you end your turn.
5.  **Controls:**
    *   **Pause:** Temporarily stops the timer. Use "Resume" to continue.
    *   **Reset:** Resets the current game to initial values.
    *   **New:** Returns to the setup screen to change time controls.

## Installation

No installation required. Simply download the `index.html` file and open it in any modern web browser.

## Technologies

*   HTML5
*   CSS3
*   JavaScript (ES6+)
