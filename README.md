# Turtle Crossing Game

Turtle Crossing is a simple game developed using Python's Turtle module. The player controls a turtle character that needs to cross a busy road without getting hit by cars. The goal is to reach the other side of the road safely.

## How to Play

1. Run the Python script `turtle_crossing.py`.
2. Use the `Up` arrow key to move the turtle character upwards.
3. Avoid colliding with cars moving across the road.
4. Reach the other side of the road to advance to the next level.
5. The game gets progressively harder with each level.

## Gameplay Features

- **Player Controls:** Use the `Up` arrow key to move the turtle character.
- **Obstacles:** Cars move horizontally across the screen, and the player must avoid colliding with them.
- **Levels:** The game becomes more challenging as the player advances through levels, with more cars moving at higher speeds.
- **Scoreboard:** Keep track of your score and current level as you play.

## Files

- `turtle_crossing.py`: Main Python script containing the game logic.
- `player.py`: Module defining the player's character and its movements.
- `car_manager.py`: Module managing the cars' movements and generation.
- `scoreboard.py`: Module handling the game scoreboard and level progression.

## Dependencies

- Python 3.x
- Turtle module

## Installation

1. Clone the repository:

```git clone https://github.com/your_username/turtle-crossing.git```

2. Navigate to the project directory:

```cd turtle-crossing```

3. Run the game script:

```python turtle_crossing.py```

# Turtle Crossing Game - Documentation

This document provides an overview of the methods available in the Python files `car_manager.py`, `player.py`, `scoreboard.py`, and `main.py`, which are used in the Turtle Crossing game.

## car_manager.py

### Methods

#### `__init__(self)`

- Initializes a new instance of the `CarManager` class.
- Sets up attributes such as `all_cars` list and `car_speed`.

#### `create_car(self)`

- Creates a new car object at a random position on the right side of the screen with a random color.

#### `move_cars(self)`

- Moves all the cars towards the left side of the screen based on their current speed.

#### `level_up(self)`

- Increases the speed of the cars when the player advances to the next level.

## player.py

### Methods

#### `__init__(self)`

- Initializes a new instance of the `Player` class.
- Sets up attributes such as `shape`, `position`, and `heading` of the player's character.

#### `go_up(self)`

- Moves the player's character upwards by a fixed distance.

#### `is_at_finish_line(self)`

- Checks if the player's character has reached the finish line.

#### `go_to_start(self)`

- Moves the player's character back to the starting position.

## scoreboard.py

### Methods

#### `__init__(self)`

- Initializes a new instance of the `Scoreboard` class.
- Sets up attributes such as `level`, `pen`, and initial position of the scoreboard.

#### `update_scoreboard(self)`

- Updates the scoreboard with the current level.

#### `increase_level(self)`

- Increases the level of the game and updates the scoreboard display.

#### `game_over(self)`

- Displays "GAME OVER" message at the center of the screen.

## main.py

This file contains the main game loop and setup code.

### Methods

- `game_loop()`
  - The main game loop that controls the flow of the game.
  - Listens for player input and updates the game state accordingly.
