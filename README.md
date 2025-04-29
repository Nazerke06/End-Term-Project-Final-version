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

| Pattern     | Usage Description                                              |
|-------------|----------------------------------------------------------------|
| Factory     | `RoomFactory` creates different room types                     |
| Strategy    | `CombatStrategy` allows enemies to use different tactics       |
| State       | `EnemyState`, `TrapState` encapsulate behavior changes         |
| Observer    | `PuzzleSubject`, `PuzzleObserver` for puzzle notification flow |

---

## 📦 Requirements

- Java 8 or higher
- No external libraries required

---

## ▶️ How to Run

### Using the Shell Script (Linux/macOS)

```bash
cd MagicalLabyrinth
chmod +x compile_and_run.sh
./compile_and_run.sh
