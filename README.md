# Python-Chess-Game

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/1d17645a-e06c-4828-9492-32859d8fad1b" />

♟️ Chess Game – Python Project 📖 Overview The Chess Game is a Python-based interactive application where two players can play chess on a graphical board. It uses object-oriented programming to define chess pieces, rules, and valid moves, while providing a GUI interface built with Tkinter or Pygame. This project is an excellent practice for learning game logic, OOP concepts, GUI programming, and algorithm design in Python.

# 🚀 Features

🎮 Two-player chess gameplay with a GUI board

✅ Enforces legal chess moves (pawn, rook, knight, bishop, queen, king)

👑 Detects check and checkmate conditions

🖥️ Graphical interface built with Tkinter/Pygame

🎓 Beginner-friendly example of combining OOP + game development

# 🛠 Tech Stack

Language → Python

Libraries → Tkinter / Pygame

Concepts → Object-Oriented Programming, Event Handling, Game Loops

📂 Project Structure project/ │── chess.py # Main game logic
│── pieces.py # Classes for chess pieces (Pawn, Rook, etc.)
│── gui.py # GUI implementation (Tkinter/Pygame)
│── assets/ # Chess piece images (PNG)
│── README.md # Documentation

# ▶️ How to Play

Run the game:

python chess.py

Select and move pieces using mouse clicks

Game enforces legal moves & alternating turns

📸 Example Screenshot

(Add chessboard screenshot here)

🔮 Future Enhancements

🤖 Add an AI opponent using the Minimax algorithm

⏱️ Implement a timer and move history log

🌍 Add online multiplayer support

🎨 Improve UI with enhanced piece graphics

📜 License

This project is licensed under the MIT License – free to use and modify.

🔹 Sample Python Code (Simplified – Tkinter) import tkinter as tk

# Board size
BOARD_SIZE = 8 TILE_SIZE = 60

root = tk.Tk() root.title("Chess Game")

canvas = tk.Canvas(root, width=BOARD_SIZETILE_SIZE, height=BOARD_SIZETILE_SIZE) canvas.pack()

Draw chessboard tiles
for row in range(BOARD_SIZE): for col in range(BOARD_SIZE): color = "white" if (row+col) % 2 == 0 else "gray" canvas.create_rectangle(colTILE_SIZE, rowTILE_SIZE, (col+1)*TILE_SIZE, (row+1)*TILE_SIZE, fill=color)

Place sample pieces (simplified as text instead of images)
pieces = {"R": (0,0), "N": (0,1), "B": (0,2), "Q": (0,3), "K": (0,4)} for p, (row, col) in pieces.items(): canvas.create_text(colTILE_SIZE+30, rowTILE_SIZE+30, text=p, font=("Arial", 24))

root.mainloop()
