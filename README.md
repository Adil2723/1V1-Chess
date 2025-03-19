# ♟️ 1v1 Chess Game  

## 🏆 Overview  

The **1v1 Chess Game** is a visually rich chess application where two players compete against each other. The game strictly follows **standard chess rules** and features a **timed turn system**, ensuring a competitive and fair experience.  

Developed using **C++ and SFML**, this project leverages **Object-Oriented Programming (OOP) principles** to create a maintainable and scalable chess system.  

---

## 🚀 Features  

✅ **Graphical User Interface (GUI)** – Smooth and interactive gameplay powered by **SFML**  
✅ **1v1 Gameplay** – Players take turns in a standard chess manner  
✅ **Timed Turns** – Players must move within a set time limit to keep the game fast-paced  
✅ **Valid Move Highlighting** – Legal moves are visually highlighted for better guidance  
✅ **Drag & Drop Movement** – Click and drag pieces for intuitive movement  
✅ **Check, Checkmate & Stalemate Detection** – Full chess rule enforcement  
✅ **Custom Timer** – Players have a countdown for each move, enhancing strategy and competition  

---

## 🏗️ Object-Oriented Design  

The game is structured using **OOP principles** like **Encapsulation, Inheritance, Polymorphism, and Abstraction** for modular and maintainable code.  

### 🏛️ **Key Classes**  

- **`Piece` Class** – Defines chess pieces, including their color, type, and position. Manages piece movement and validation.  
- **`Board` Class** – Represents the chessboard, tracks piece positions, and enforces game rules.  
- **`Player` Class** – Manages each player's pieces, moves, and timer.  
- **`Game` Class** – Handles game flow, turn management, and win conditions.  
- **`Timer` Class** – Controls the countdown clock for each player's turn.  

### 🏹 **OOP Concepts Applied**  

- **Inheritance** – The `Piece` class is a base class, while `King`, `Queen`, `Pawn`, etc., inherit from it, implementing unique movement logic.  
- **Polymorphism** – Each piece type overrides the `getValidMoves()` function to apply its own movement strategy.  
- **Encapsulation** – Data like a piece's position and color are private and accessed via controlled methods.  
- **Abstraction** – The `Game` class abstracts the complexity of chess logic, allowing high-level interaction without handling low-level mechanics.  

---

## 🛠️ Technologies Used  

| Technology | Purpose |
|------------|---------|
| **C++** | Core game logic and OOP implementation |
| **SFML** | Graphics rendering and user input handling |
| **Makefile** | Simplifies project compilation |

---

## 🔧 Installation  

Follow these steps to install and run the **1v1 Chess Game**:

### 📌 **Prerequisites**  

- Install **SFML** on your system:  
  - **Linux**: `sudo apt-get install libsfml-dev`  
  - **Windows**: [Download SFML](https://www.sfml-dev.org/download.php)  
  - **MacOS**: `brew install sfml`  

---

### 💡 **Run the Game**  

1️⃣ **Clone the repository**  
```sh
git clone https://github.com/Adil2723/1v1-Chess-Game.git
cd 1v1-Chess-Game