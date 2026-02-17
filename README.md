♟️ Chess Engine with AI (Pygame)

A fully functional desktop chess game built using Python + Pygame, featuring a custom chess engine, legal move validation, and an AI opponent powered by NegaMax with Alpha–Beta pruning.

This project focuses on implementing chess from scratch — including game rules, move generation, state evaluation, and AI decision-making.

🚀 Features

✅ Complete chess rule implementation
✅ Player vs Player mode
✅ Player vs AI mode
✅ Legal move validation system
✅ Checkmate & stalemate detection
✅ Castling, en-passant, pawn promotion
✅ Move animations & square highlighting
✅ Undo moves (Z key)
✅ Game reset (R key)

🧠 AI System

The AI opponent uses:

NegaMax search

Alpha–Beta pruning

Material-based evaluation function

The engine evaluates board states using piece values:

Queen = 10
Rook  = 5
Bishop/Knight = 3
Pawn  = 1


Search depth is configurable and balances performance vs difficulty.

AI logic implemented in:

SmartMoveFinder.py


The algorithm recursively explores future positions and selects moves that maximize positional advantage while minimizing opponent gain 

SmartMoveFinder

.

⚙️ Project Architecture
Chess/
│
├── ChessMain.py        → Game loop + UI rendering
├── ChessEngine.py      → Core chess logic & rules
├── SmartMoveFinder.py  → AI search algorithm
├── images/             → Piece sprites
└── chess_game_screenshot.png

🔹 Game Engine

Handles:

Board representation (8×8 matrix)

Move generation

Legal move filtering

Check detection

Castling & en-passant logic

Move undo system

Implemented inside GameState class 

ChessEngine

.

🔹 Rendering System (Pygame)

Responsible for:

Board drawing

Piece rendering

Move animations

Mouse interaction

Highlighting valid moves

Main game loop located in:

ChessMain.py


ChessMain

🎮 Controls
Action	Key / Input
Move Piece	Mouse Click (select → destination)
Undo Move	Z
Restart Game	R
Quit	Close Window
🛠️ Installation
1️⃣ Clone Repository
git clone https://github.com/Yuvrraaj/<chess-game>.git
cd <repo-name>

2️⃣ Install Dependencies
pip install pygame

3️⃣ Run the Game
python ChessMain.py

🧩 Core Concepts Implemented

Game State Modeling

Move Generation Algorithms

Search Trees

Recursive Game Evaluation

Alpha–Beta Optimization

Event-driven GUI programming

📈 Future Improvements

♟️ Positional evaluation tables

♟️ Opening book support

♟️ Move ordering optimization

♟️ Difficulty levels

♟️ GUI improvements & sounds

♟️ Transposition tables (Zobrist hashing)

👨‍💻 Author

Yuvraj Jha

AI / ML Engineer — Computer Vision & Systems
Building intelligent systems combining algorithms, AI, and real-world applications.
