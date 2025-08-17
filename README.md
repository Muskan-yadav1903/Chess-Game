
# ♟️ Real-Time Multiplayer Chess Game

A real-time chess application built with Node.js, Express, Socket.io, and Chess.js.
It allows two players to compete online while additional users can join as spectators. The game supports drag-and-drop moves, turn validation, and live board updates.







# 🚀 Features

🔄 Real-time gameplay with Socket.io

✅ Accurate move validation using Chess.js

🎯 Drag-and-drop chessboard interface

♟️ Automatic board flip for black players

👀 Support for multiple spectators

⚡ Smooth synchronization across all clients




#  🖥️ Tech Stack

- Frontend:

HTML, CSS, JavaScript

Socket.io (client)

Chess.js

- Backend:

Node.js + Express

Socket.io (server)

Chess.js





#  ⚙️ How It Works

🔹 Frontend (Client-Side)

- Establishes WebSocket connection with const socket = io();
- Uses Chess.js for game logic (valid moves, checkmate, etc.)
- Drag-and-drop support for moving chess pieces
- Board dynamically rendered with Unicode chess characters
- Sends moves to server → validated → broadcasted to all clients

🔹 Backend (Server-Side)

- Manages players (White/Black) and spectators
- Validates moves with Chess.js
- Enforces correct turn order
- Broadcasts updated board state (FEN) to clients
- Handles disconnections and role re-assignment

