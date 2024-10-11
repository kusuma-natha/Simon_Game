# Simon Game

This is a web-based version of the classic "Simon Says" game. Test your memory and pattern-recognition skills by following an increasingly complex sequence of colors as you advance through the levels!

## Project Structure

This game is built using **JavaScript**, **HTML**, and **CSS**.

- **JavaScript** manages the game logic, sequence generation, user interaction, and scoring.
- **HTML** provides the structure and layout for the game's user interface.
- **CSS** defines the styles for the color buttons, effects, and overall presentation.

## How to Play

1. **Start the Game:** Press any key to begin. A random color in the sequence will flash.
2. **Follow the Pattern:** Watch the sequence closely. Then, repeat the pattern by clicking the colored buttons in the same order.
3. **Level Up:** If you complete the sequence correctly, you'll advance to the next level, where the sequence grows longer by one color.
4. **Game Over:** If you make a mistake, the game ends, displaying your score. Press any key to restart.

## Code Overview

### JavaScript Code (`app.js`)

- **Global Variables:**
  - `gameSeq`: Array that stores the game’s color sequence.
  - `userSeq`: Array that records the user's inputs.
  - `level`: Tracks the current level of the game.
  - `started`: Boolean that checks if the game is in progress.

- **Functions:**
  - `levelUp()`: Increments the level, generates a new random color for the sequence, and updates the display.
  - `btnFlash(btn)`: Creates a flash effect on a button.
  - `checkAns(idx)`: Verifies if the user’s input matches the game sequence.
  - `btnPress()`: Handles the user's button clicks and calls `checkAns`.
  - `reset()`: Resets all game variables to start over.

### HTML Code (`index.html`)

Defines the basic structure with a title, instructions, and buttons for each color. Colors are represented by `.btn` divs with unique IDs.

### CSS Code (`style.css`)

- **Styles** the colored buttons (pink, orange, green, purple).
- **Flash Effect**: When a button is clicked or part of the sequence, it flashes white.
  
## Installation

1. Clone this repository:
   ```bash
   git clone <your-repo-url>

2. Open the index.html file in a web browser to play the game.

# Installation
- Clone the repository, and open the index.html file in your browser to play.

# License
- This project is open-source under the MIT License.
