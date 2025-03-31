# Tetris Game (C++ with Raylib)

This is a simple yet engaging Tetris game built using C++ and the Raylib graphics library. It closely follows the classic Tetris mechanics while incorporating smooth animations and a colorful interface.

## Features
- Classic Tetris Gameplay: Stack falling blocks to complete lines and score points.
- Colorful and Vibrant Design: Each block has a distinct color for better visibility.
- Smooth Animations: Blocks move and rotate seamlessly.
- Score Tracking: Earn points for completing lines and track your progress.
- Responsive Controls: Intuitive controls for a seamless gaming experience.

## Requirements
To build and run this game, ensure you have the following:
- A C++ compiler (GCC, Clang, or MSVC)
- The Raylib library, which can be downloaded and installed from [Raylib's official site](https://www.raylib.com/). 
  - On Windows: Use the precompiled binaries.
  - On macOS/Linux: Use a package manager such as Homebrew (`brew install raylib`) or manually compile from source.

## How to Build and Run
### Running the Game
Open `main.cpp` in your preferred IDE and press F5 to build and run the game.

## Gameplay Controls
- Left/Right Arrow Keys: Move the block left or right
- Down Arrow: Soft drop (speeds up descent)
- Up Arrow: Rotate the block
- Spacebar: Hard drop (instantly places the block)
- R: Restart the game
- Esc: Exit the game

## Code Structure and Functions
The game is structured with multiple C++ files, each handling different aspects of the Tetris logic.

### Block Functions
- `Draw(offsetX, offsetY)`: Draws the block at the given position.
- `Move(rows, columns)`: Moves the block by the specified rows and columns.
- `Rotate()`: Rotates the block clockwise.
- `UndoRotation()`: Reverts the last rotation.

### Game Functions
- `Draw()`: Draws the game elements.
- `HandleInput()`: Processes player input.
- `MoveBlockDown()`: Moves the current block down.
- `MoveBlockLeft()`: Moves the block left.
- `MoveBlockRight()`: Moves the block right.
- `MoveBlockStraightDown()`: Instantly moves the block to the lowest position.
- `GetRandomBlock()`: Generates a new random block.
- `IsBlockOutside()`: Checks if the block is outside the grid.
- `RotateBlock()`: Rotates the current block.
- `LockBlock()`: Locks the block in place when it lands.
- `BlockFits()`: Checks if the block fits in its current position.
- `Reset()`: Resets the game.
- `UpdateScore(linesCleared, moveDownPoints)`: Updates the player's score.

### Grid Functions
- `Initialize()`: Initializes the grid.
- `Print()`: Prints the grid state (for debugging).
- `Draw()`: Draws the grid on the screen.
- `IsCellOutside(row, column)`: Checks if a cell is outside the grid boundaries.
- `IsCellEmpty(row, column)`: Checks if a cell is empty.
- `ClearFullRows()`: Clears any full rows and returns the number cleared.
- `IsRowFull(row)`: Checks if a row is completely filled.
- `ClearRow(row)`: Clears a specific row.
- `MoveRowDown(row, numRows)`: Moves rows down after clearing.

## Future Improvements
Some potential enhancements for future updates:
- Pausing the game: To pause the game in between and to replay it from where we stopped.
- High Score Tracking: Saving high scores to track progress over multiple sessions.
- Multiplayer Mode: Introducing a competitive multiplayer feature.

Enjoy playing Tetris

