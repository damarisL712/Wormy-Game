# Wormy Snake Game

A fully playable Snake-style game built with **Python** and **Pygame**. This project focuses on separating game logic from graphics and screen management to create code that is easier to test, maintain, and extend.

## Project Overview

The Wormy Snake Game allows the player to control a growing worm as it moves around a grid collecting apples. Each apple increases the worm's length and score. The game ends if the worm collides with a wall or with its own body.

The project was completed from starter code by implementing the core game logic, main game loop, collision detection, scoring system, movement controls, and Pygame graphics.

## Skills Demonstrated

- Python function design and decomposition
- Boolean logic and conditional statements
- List and dictionary manipulation
- Coordinate-based movement
- Collision detection
- Object movement on a 2D grid
- Event handling with Pygame
- Rendering graphics with `pygame.draw`
- Separation of game logic and presentation
- Unit testing with `pytest`
- Writing code designed for automated testing

## Project Structure

```text
ASG06-starter-code/
├── wormy.py          # Main entry point and game loop
├── constants.py      # Game constants and colors
├── logic.py          # Movement, collision, scoring, and direction logic
├── graphics.py       # Worm, apple, grid, and score rendering
├── screens.py        # Start and game-over screens
└── test_wormy.py     # Instructor-provided pytest test suite
```

## Core Features

The game includes:

- WASD and arrow-key movement
- Direction-reversal prevention
- Randomized starting positions
- Random apple placement
- Worm growth after eating apples
- Score tracking
- Wall collision detection
- Self-collision detection
- Game-over behavior
- Grid-based movement
- Pygame-based rendering

## Game Logic

The game logic is separated into independently testable functions within `logic.py`.

These functions handle:

- Calculating the worm's next head position
- Detecting wall collisions
- Detecting self-collisions
- Detecting when an apple is eaten
- Calculating the player's score
- Preventing opposite-direction movement

Keeping this logic separate from Pygame rendering allows the core behavior of the game to be tested without requiring the graphical interface.

## Technologies Used

- **Python**
- **Pygame**
- **Pytest**
- **Git / GitHub**

## Installation

Install the required dependencies:

```bash
pip install -r requirements.txt
```

## Running the Game

Start the game with:

```bash
python wormy.py
```

### Controls

- **W / Up Arrow** — Move up
- **S / Down Arrow** — Move down
- **A / Left Arrow** — Move left
- **D / Right Arrow** — Move right
- **ESC** — Exit the game

## Running Tests

Run the instructor-provided automated test suite with:

```bash
pytest test_wormy.py -v
```

The test suite contains **48 automated tests** covering the game's logic and integration behavior.

## Development Approach

This project was developed incrementally, with each core function implemented and tested independently before being integrated into the full game.

Separating the project into logic, graphics, screen management, and the main game loop made it easier to debug individual components and helped reinforce the importance of modular software design.

## Future Improvements

Possible future enhancements include:

- Improved worm animations
- Additional visual effects
- Multiple difficulty levels
- High-score persistence
- Sound effects and background music
- Pause functionality
- Custom game settings

## Author

**Damaris Lubin**

Cybersecurity Analytics and Operations Student  
Penn State University