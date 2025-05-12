# 🧙 Magical Labyrinth

**Magical Labyrinth** is a Java-based adventure game set in a procedurally generated magical dungeon. The player navigates through rooms with puzzles, traps, and enemies while collecting artifacts and trying to find the exit. The game emphasizes strategic decision-making and uses several classic software design patterns.

---

## 📁 Project Structure



🧩 Overview
Magical Labyrinth is a Java-based adventure game set in a procedurally generated magical dungeon. The player navigates through rooms with puzzles, traps, and enemies while collecting artifacts and trying to find the exit. The game emphasizes strategic decision-making and incorporates well-known software design patterns.


---

## 🚀 Features

- **Dynamic Dungeon Generation** – Each playthrough is unique
- **Multiple Room Types** – Puzzle, Trap, Monster, Treasure, and Exit Rooms
- **Interactive Combat System** – Based on different combat strategies
- **Puzzle Solving** – Observer pattern-based puzzle mechanisms
- **Dual Interface** – Console and GUI (Swing) views available
- **Player Progression** – Tracks health, artifacts, and position

---

## 🛠️ Design Patterns Used

1. Factory Pattern
- Implemented in the`RoomFactory` class which creates different types of rooms
- Used to create different room types (Regular, Treasure, Monster, Puzzle, etc.)
- Encapsulates room creation logic and provides a centralized way to create room objects
2. Strategy Pattern
- Found in MagicStrategy
- Implements combat behavior through the`CombatStrategy` interface
- Allows for different combat strategies to be swapped at runtime
3. Observer Pattern
- Implemented through PuzzleSubject
- Used for puzzle-related notifications
- Puzzle rooms notify players (observers) of puzzle-related events
- Methods include addObserver, removeObserver, and notifyObservers
4. Template Method Pattern
- Seen in Puzzle abstract class
- Defines the skeleton of puzzle operations
- Subclasses can override specific methods while keeping the basic algorithm structure
5. State Pattern
- Hints of this pattern in trap implementation (reference to HiddenTrapState in Trap.java )
- Manages different states of traps (hidden, revealed, triggered)
6. Inheritance Pattern
- Room hierarchy with`Room` as the base class
- Specialized rooms like TreasureRoom , PuzzleRoom , and RegularRoom
7. Composite Pattern (partially)
- The Labyrinth class manages a collection of Room objects
- Treats individual rooms and the entire labyrinth structure uniformly
These patterns work together to create a flexible and maintainable game architecture:

- Factory Pattern handles room creation
- Strategy Pattern manages combat mechanics
- Observer Pattern handles puzzle events
- Template Method Pattern standardizes puzzle implementation
- State Pattern manages trap states
- Inheritance provides room type specialization
- Composite Pattern organizes the overall game structure
This combination of patterns provides good separation of concerns, maintainability, and extensibility to your game's codebase.

---

## 📦 Requirements

- Java 8 or higher
- No external libraries required

---

## 👩‍💻👨‍💻 Authors:
 Abdimalik Nazerke / Esteu Inkar / Nazarov Aldiyar / Islam Kairgazin /

---

## 🕹️ How to Run
"private static final boolean USE_SWING = false;  " just change the false into true and run; ✌️"

---

## ▶️ How to Run (in terminal)

### Using the Shell Script (Linux/macOS)

```bash
cd MagicalLabyrinth
chmod +x compile_and_run.sh
./compile_and_run.sh

