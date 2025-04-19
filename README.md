# Chess Game in C++ with SFML 🎮

![GitHub](https://img.shields.io/github/license/Adil2723/ChessGame?color=blue)
![Build Status](https://img.shields.io/badge/build-passing-brightgreen)
![Contributors](https://img.shields.io/github/contributors/yourusername/ChessGame?color=yellow)
![Repo Size](https://img.shields.io/github/repo-size/yourusername/ChessGame?color=orange)

A **C++** chess game built with **SFML (Simple and Fast Multimedia Library)**. This project demonstrates fundamental concepts of **Object-Oriented Programming (OOP)**, **inheritance**, and **polymorphism**, while also leveraging SFML's powerful graphics capabilities for rendering chess pieces and the chessboard.

---

## Features 🌟

- **Chessboard Rendering**: An 8x8 grid with alternating light and dark squares.
- **Piece Textures**: Chess pieces (Pawn, Rook, Knight, Bishop, Queen, King) are represented with PNG images loaded as textures.
- **Object-Oriented Design**:
  - A base `Piece` class with subclasses for each specific chess piece.
  - Inheritance and polymorphism for customized piece behavior.
- **SFML Integration**: Uses SFML to handle window management, graphics rendering, and events.

---

## Technologies & Concepts 🔧

This project utilizes the following tools and concepts:

- **C++**: Core programming language for game logic and rendering.
- **SFML (Simple and Fast Multimedia Library)**: For rendering the chessboard and managing graphical assets.
- **Object-Oriented Programming**:
  - **Inheritance**: Common functionality in the `Piece` base class, with specialized behavior in subclasses.
  - **Polymorphism**: Different piece behaviors are handled dynamically via method overriding.
- **Textures & Sprites**: Chess pieces are loaded as PNG textures and rendered using SFML sprites.

---

## Project Structure 📂

Here's an overview of the project structure:

```plaintext
ChessGame/
│
├── assets/                  # Folder containing chess piece textures (e.g., white_pawn.png, black_king.png)
│
├── src/                     # Source code files
│   ├── main.cpp             # Main entry point of the application
│   ├── Piece.hpp            # Base class for all pieces
│   ├── Piece.cpp            # Implementation of Piece class
│   ├── Pawn.hpp             # Pawn class header
│   ├── Pawn.cpp             # Pawn class implementation
│   ├── Rook.hpp             # Rook class header
│   ├── Rook.cpp             # Rook class implementation
│   ├── Knight.hpp           # Knight class header
│   ├── Knight.cpp           # Knight class implementation
│   ├── Bishop.hpp           # Bishop class header
│   ├── Bishop.cpp           # Bishop class implementation
│   ├── Queen.hpp            # Queen class header
│   ├── Queen.cpp            # Queen class implementation
│   ├── King.hpp             # King class header
│   ├── King.cpp             # King class implementation
│   ├── chessBoard.hpp       # Chessboard class header
│   ├── chessBoard.cpp       # Chessboard class implementation
│
├── CMakeLists.txt           # CMake build configuration
└── README.md                # Project description (this file)
