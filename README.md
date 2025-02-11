# Symon Saya Game

This is a simple Simon Says game built using JavaScript, HTML, and CSS. The game generates a sequence of button flashes that the player must remember and repeat. Each correct sequence completion advances the player to the next level.

## How to Play
1. Click the "Click Me!" button or press any key to start the game.
2. Watch the sequence of colored button flashes carefully.
3. Click the buttons in the exact order they flashed.
4. If you get the sequence correct, the game moves to the next level and adds a new step to the sequence.
5. If you make a mistake, the game ends, and your score is displayed.
6. Press any key to restart the game.

## Features
- Random sequence generation
- Click and keyboard start functionality
- Visual feedback with flashing buttons
- Score tracking
- Game reset on failure

## Files
- `index.html` - Contains the structure of the game.
- `styles.css` - Handles the styling and layout of the game.
- `script.js` - Contains the game logic and event handling.

## Issues and Fixes
### Issue: Incorrect Random Index Calculation
In the `levelUp` function, the random index calculation should be:
```js
let randIdx = Math.floor(Math.random() * 4); // Should be 4 instead of 3
```
Fixing this ensures all four colors are used in the game.

## Future Improvements
- Add sound effects for better user experience.
- Implement difficulty settings.
- Enhance the UI/UX with animations and transitions.
- Store high scores using local storage.

Enjoy the game!

