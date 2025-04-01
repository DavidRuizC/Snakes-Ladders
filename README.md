
# 🎲 Snake & Ladders - Java Console Game

This is a Java implementation of a simplified **Snake & Ladders** game with some special mechanics such as **death squares** and **occupied square penalties**. It is designed for multiple players and runs directly in the terminal.

## 🚀 Features

- Fully playable in the terminal.
- Support for multiple players.
- Snakes and ladders that move players forward or backward.
- Death squares that eliminate players from the game.
- Logic to avoid moving beyond the last square.
- Turn-based gameplay with automatic dice rolling.

## 🧩 Core Components

- `Board`: Initializes the game board, places snakes, ladders, and death squares.
- `Square`: Base class for all squares on the board.
- `SnakeOrLadder`: Subclass of `Square` that moves a player to a new position.
- `Death`: Subclass of `Square` that eliminates players.
- `FirstSquare`: Starting square that tracks players.
- `Player`: Represents each player with movement, death status, and winning logic.
- `Die`: Simulates a dice roll (1-6).
- `Game`: Manages the flow of the game including turn rotation and winner detection.
- `Main`: Entry point to launch the game with configurable board size and rules.

## ▶️ How to Run

1. Compile all `.java` files:
   ```bash
   javac *.java
   ```

2. Run the game:
   ```bash
   java Main
   ```

3. Follow the output in the terminal to watch the game progress.

## 🎮 Game Rules

- Players take turns rolling a dice.
- If a player lands on a snake or ladder, they are moved accordingly.
- Landing on a death square eliminates the player.
- If a player attempts to land on an occupied square, they are sent back to the first square.
- The first player to reach the last square wins.

## 🛠 Configuration

You can customize the game board in `Main.java`:

- `NUM_SQUARES`: Total number of squares on the board.
- `SNAKES_AND_LADDERS`: Array of `[from, to]` positions for snakes and ladders.
- `DEATH_SQUARES`: Array of square positions that cause player elimination.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
