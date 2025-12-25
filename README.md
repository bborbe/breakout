# Breakout

A classic Breakout game built with vanilla JavaScript, HTML5 Canvas, and CSS. Break all the bricks with the ball while keeping it from falling below the paddle!

## Features

- **Classic Gameplay**: Paddle-controlled ball bouncing and brick breaking
- **Progressive Difficulty**: Ball speed increases as bricks are destroyed
- **Lives System**: 3 lives to clear all bricks
- **Score Tracking**: Points awarded based on brick row (higher rows = more points)
- **High Score Persistence**: Best score saved in browser localStorage
- **Dual Control**: Control paddle with arrow keys or mouse
- **Pause/Restart**: Pause gameplay and restart anytime
- **Victory Detection**: Win screen when all bricks cleared
- **Modern UI**: Clean gradient design matching Tetris/Snake style

## How to Play

1. Open `index.html` in a web browser
2. Use **arrow keys** or **mouse** to move the paddle
3. Keep the ball bouncing to destroy all bricks
4. Don't let the ball fall below the paddle!
5. Clear all bricks to win

## Controls

- **← →** or **Mouse**: Move paddle left/right
- **P** or **Esc**: Pause/unpause game
- **R**: Restart game

## Gameplay Rules

- You start with **3 lives**
- Ball destroys bricks on contact
- Ball bounces off paddle, walls, and bricks
- Lose a life if ball falls below paddle
- Game over when all lives lost
- Victory when all bricks destroyed

## Scoring System

Bricks award different points based on row position:
- Row 1 (Top): **80 points** (Red)
- Row 2: **70 points** (Orange)
- Row 3: **60 points** (Yellow)
- Row 4: **50 points** (Green)
- Row 5: **40 points** (Blue)
- Row 6: **30 points** (Purple)
- Row 7: **20 points** (Pink)
- Row 8 (Bottom): **10 points** (Cyan)

**Total possible score**: 4,400 points (80 bricks)

## Technical Details

- **Canvas Size**: 800x600 pixels
- **Paddle**: 100x20 pixels
- **Ball**: 8 pixel radius
- **Bricks**: 75x20 pixels, 8 rows × 10 columns
- **Initial Ball Speed**: 5 pixels per frame
- **Speed Increase**: 2% per brick destroyed
- **No Dependencies**: Pure vanilla JavaScript

## Game Architecture

The game follows a modular architecture pattern:

- **Game State Module**: Manages game state, collision detection, scoring
- **Renderer Module**: Handles all canvas drawing operations
- **Input Handler Module**: Processes keyboard and mouse input
- **Game Loop**: Uses requestAnimationFrame for smooth gameplay

## Browser Compatibility

Works in all modern browsers supporting:
- HTML5 Canvas
- ES6 JavaScript
- localStorage API

## Play Online

**Play now:** https://bborbe.github.io/breakout/

## Development

Built following the same architectural patterns as the companion Tetris and Snake games.

## License

Free to use and modify.
