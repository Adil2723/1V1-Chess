# ♟️♟️ 1v1 Chess Game

## Overview

The **1v1 Chess Game** is a graphical chess application where two players can compete in a game of chess. The game follows the standard chess rules and incorporates a timed turn feature, ensuring each player has a limited amount of time to make their move. The game is developed using **SFML** (Simple and Fast Multimedia Library), providing an interactive and visually rich experience. The game design is based on **Object-Oriented Programming (OOP)** principles, making it easy to maintain and extend.

## Features

- **Graphical User Interface (GUI)** powered by SFML.
- **1v1 Turns**: Players take turns in a standard chess manner.
- **Timed Turns**: Each player has a set amount of time for their turn to maintain competitive pacing.
- **Piece Movement**: Click and drag pieces to move them.
- **Valid Move Highlighting**: Squares where a piece can legally move are highlighted.
- **Game Timer**: A countdown timer for each player, ensuring fair and timely gameplay.
- **Chess Rules**: Full support for chess rules, including check, checkmate, and stalemate conditions.

## Object-Oriented Programming (OOP) Design

The game is built around the core principles of Object-Oriented Programming (OOP), including **Encapsulation**, **Inheritance**, **Polymorphism**, and **Abstraction**. Below are some key concepts and how they are applied in this project:

### Classes and Objects

- **Piece Class**: Represents a chess piece. Each piece has properties such as its color, type (pawn, rook, bishop, etc.), and position on the board. Methods in this class handle moving pieces, checking for valid moves, and updating the board state.

- **Board Class**: Manages the entire chess board, storing pieces, checking for game conditions (check, checkmate, stalemate), and handling the game logic. It provides a clear abstraction for interacting with the chessboard and the pieces.

- **Player Class**: Represents a player in the game. This class holds information about the player's time, whether they are in check or checkmate, and their active pieces. The player class also manages the timer for each player.

- **Game Class**: This is the core class that controls the flow of the game. It keeps track of the current player, manages the game timer, and checks for game-over conditions like checkmate or stalemate.

- **Timer Class**: A utility class to handle the countdown timer for each player. It keeps track of time, updates the display, and ensures the player’s turn is limited to the specified time.

### Inheritance and Polymorphism

- **Piece Inheritance**: The `Piece` class is a base class, and each specific piece (like `King`, `Queen`, `Pawn`, `Rook`, etc.) inherits from it. Each derived class implements its own logic for valid movements, capturing, and special behaviors (such as castling for the `King` or promotion for the `Pawn`).

- **Move Strategies**: Polymorphism is used for different movement strategies of the chess pieces. Each piece has a method called `getValidMoves()` that is overridden by the specific piece types to calculate its unique set of legal moves.

### Encapsulation

- Each class encapsulates its data, ensuring that players and pieces interact only through the class’s public interface. This approach keeps the game’s internal workings hidden from external components, improving modularity and maintainability.

- Example: The `Piece` class has private members for `position` and `color`, which can only be accessed or modified through getter and setter methods.

### Abstraction

- The game abstracts the complexities of chess logic into manageable objects. For instance, the `Game` class encapsulates the overall game logic, so the main program only needs to interact with this high-level abstraction, rather than dealing with the individual mechanics of pieces and board state.

## Technologies Used

- **SFML**: A multimedia library to create graphical windows and manage user input.
- **C++**: The primary programming language used to implement the game logic and object-oriented structure.
- **Makefile**: For building and compiling the project.

## Installation

To run the 1v1 Chess Game, follow the steps below:

### Prerequisites

- Install **SFML** on your system.
  - On Linux: `sudo apt-get install libsfml-dev`
  - On Windows: Follow the SFML installation guide at [SFML Downloads](https://www.sfml-dev.org/download.php).
  - On macOS: `brew install sfml`

