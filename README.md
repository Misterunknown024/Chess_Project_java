# Chess Game — OOP Java Project (B13 Basic)

## How to Run
### Windows
Double-click `compile_and_run.bat` or run in terminal.

### Mac / Linux
```bash
chmod +x compile_and_run.sh
./compile_and_run.sh
```
Requires: Java JDK 8 or above.

## Project Structure
```
src/chess/
├── Movable.java          ← Interface
├── Piece.java            ← Abstract base class
├── PieceTypes.java       ← King, Queen, Rook, Bishop, Knight, Pawn (extends Piece)
├── Board.java            ← 8x8 board, piece management, check detection
├── Player.java           ← Player info, captured piece count
├── Game.java             ← Game logic, move validation, checkmate/stalemate
├── InvalidMoveException.java  ← Custom exception
├── CheckException.java        ← Custom exception
└── ChessGUI.java         ← Swing GUI (JFrame, JPanel, paintComponent, ActionListener)
```

## OOP Concepts Covered
| Concept | Where |
|---|---|
| Encapsulation | All fields private with getters/setters |
| Inheritance | King/Queen/Rook/Bishop/Knight/Pawn extend Piece |
| Polymorphism | isValidMove() overridden per piece; Movable interface |
| Abstraction | Abstract Piece class + Movable interface |
| Exception Handling | InvalidMoveException, CheckException with try-catch |
| Packages | chess package with import |
| Constructor Overloading | Piece(color), Piece(color, captured); Player(name,color), Player(color) |
| GUI (Module 05) | ChessGUI: paintComponent board, selection highlight, status JLabel |
