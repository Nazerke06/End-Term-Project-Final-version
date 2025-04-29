📄 Project Documentation: Magical Labyrinth

🧩 Overview
Magical Labyrinth is a Java-based adventure game set in a procedurally generated magical dungeon. The player navigates through rooms with puzzles, traps, and enemies while collecting artifacts and trying to find the exit. The game emphasizes strategic decision-making and incorporates well-known software design patterns.

🗂️ Project Structure
bash
Copy
Edit

MagicalLabyrinth/
├── controller/       # Controls game logic (e.g., GameController)
├── model/            # Core game entities and logic
│   ├── combat/       # Combat strategies using Strategy Pattern
│   ├── entities/     # Enemy behavior using State Pattern
│   ├── puzzle/       # Puzzle interactions using Observer Pattern
│   ├── rooms/        # Room types and factory (Factory Pattern)
│   └── traps/        # Trap states (State Pattern)
├── view/             # Console and Swing-based UI
└── MagicalLabyrinth.java  # Main class to start the game
🔑 Key Features
Multiple Room Types: PuzzleRoom, MonsterRoom, TrapRoom, TreasureRoom, ExitRoom.

Design Patterns Used:

Factory Method (for room creation)

Strategy (for enemy combat strategies)

State (for enemy and trap behaviors)

Observer (for puzzle-solving logic)

Two View Modes: ConsoleView and SwingView for different UI experiences.

Player Stats: Health, artifacts collected, and position.

Randomized Labyrinth Generation: Ensures a unique experience every game.

🧪 How to Run
If you’re using a Linux/Mac environment:

bash
Copy
Edit
cd MagicalLabyrinth
chmod +x compile_and_run.sh
./compile_and_run.sh
Alternatively, compile and run manually:

bash
Copy
Edit
javac -d out src/main/java/game/**/*.java
java -cp out game.MagicalLabyrinth
🛠️ Dependencies
Java 8 or higher

No external libraries required

🚀 Design Patterns Summary

Pattern	Purpose
Factory	Used in RoomFactory to generate various types of rooms
Strategy	CombatStrategy allows enemies to fight with different tactics
State	EnemyState, TrapState encapsulate behavior changes
Observer	PuzzleObserver updates components when puzzle state changes
