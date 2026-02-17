# Chess Engine with AI (Pygame)

A fully functional desktop chess game built using Python and Pygame, featuring a custom chess engine, legal move validation, and an AI opponent powered by NegaMax with Alpha–Beta pruning.

This project focuses on implementing chess from scratch, including game rules, move generation, state evaluation, and AI decision-making.

---

## Features

- Complete chess rule implementation
- Player vs Player mode
- Player vs AI mode
- Legal move validation
- Checkmate and stalemate detection
- Castling, en-passant, and pawn promotion
- Move animations and square highlighting
- Undo moves (Z key)
- Game reset (R key)

---

## AI System

The AI opponent uses:

- NegaMax search
- Alpha–Beta pruning
- Material-based evaluation function

### Piece Evaluation

| Piece | Value |
|------|------|
| Queen | 10 |
| Rook | 5 |
| Bishop | 3 |
| Knight | 3 |
| Pawn | 1 |

Search depth is configurable to balance performance and difficulty.

AI logic is implemented in:

SmartMoveFinder.py

The algorithm recursively evaluates future positions and selects moves that maximize positional advantage while minimizing opponent gain.

---

## Project Architecture

Chess/
│
├── ChessMain.py # Game loop and UI rendering
├── ChessEngine.py # Core chess logic and rules
├── SmartMoveFinder.py # AI search algorithm
├── images/ # Piece sprites
└── chess_game_screenshot.png



---

## Game Engine

Handles:

- Board representation (8×8 matrix)
- Move generation
- Legal move filtering
- Check detection
- Castling and en-passant logic
- Move undo system

Implemented inside the GameState class in ChessEngine.py.

---

## Rendering System (Pygame)

Responsible for:

- Board drawing
- Piece rendering
- Move animations
- Mouse interaction
- Highlighting valid moves

Main game loop is located in ChessMain.py.

---

## Controls

| Action        | Input |
|--------------|-------|
| Move Piece   | Mouse Click (select → destination) |
| Undo Move    | Z |
| Restart Game | R |
| Quit         | Close Window |

---

## Installation

1. Clone Repository

git clone https://github.com/Yuvrraaj/chess-game.git
cd chess-game

2. Install Dependencies

pip install pygame

3. Run the Game

python ChessMain.py

---

## Core Concepts Implemented

- Game state modeling
- Move generation algorithms
- Search trees
- Recursive game evaluation
- Alpha–Beta optimization
- Event-driven GUI programming

---

## Future Improvements

- Positional evaluation tables
- Opening book support
- Move ordering optimization
- Difficulty levels
- GUI improvements and sound effects
- Transposition tables (Zobrist hashing)

---

## Author

Yuvraj Jha  
AI / ML Engineer — Computer Vision and Systems

Building intelligent systems combining algorithms, AI, and real-world applications.
