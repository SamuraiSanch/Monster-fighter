# ⚔️ Monster Fighter

A console-based RPG survival game built in C++. Fight monsters, collect gold,
and level up your way to victory — or die trying!

## 📋 Description

**Monster Fighter** is a turn-based console RPG. You create a character and face
randomly generated monsters. Each victory earns you gold and a level-up.
Reach **level 20** to win — but watch your HP!

You can also attempt to **flee** from a fight, though success is never guaranteed.

## 🐉 Monsters

| Monster | Symbol | HP | Damage | Gold |
|---------|--------|----|--------|------|
| Dragon  | `D`    | 20 | 4      | 100  |
| Orc     | `o`    | 4  | 2      | 25   |
| Slime   | `s`    | 1  | 1      | 10   |

## 🎯 Game Rules

- You start with **10 HP**, **1 damage**, and **0 gold**
- Each turn: choose to **(F)ight** or **(R)un**
- Winning a fight gives you the monster's gold and **+1 level / +1 damage**
- Running has a **50% chance** of failure — the monster attacks if you fail
- Reach **level 20** to win the game

## 🛠️ Technologies

- **C++**
- **OOP:** `Creature` base class with `Player` and `Monster` inheritance
- **`rand()` / `srand()`:** randomized monster generation and flee outcomes
- **`friend` functions:** `attackMonster` / `attackPlayer` for combat logic
- **Static data:** monster stats stored in a static `MonsterData` array

## 📂 Project Structure
```
monster-fighter/
└── monster-fighter.cpp    # Full game logic
```

## 📋 Example Usage
```
Enter your name: Alex
Welcome, Alex.
You have 10 health, 1 damage and are carrying 0 gold.
You met a slime (s).
Do you want (R)un or (F)ight?: F
You hit the slime for 1. Now monster has 0 hp.
A slime is dead now. You earn 10 gold.
Level up! Your level now: 2
You met a dragon (D).
Do you want (R)un or (F)ight?: R
Running failed. You must to fight!
Monster hit you for 4. Now you have 6 hp.
```

## 🔧 Future Improvements

- [ ] Replace `rand()` with `std::mt19937` for better randomness
- [ ] Add healing items or potions
- [ ] More monster types and special abilities
- [ ] Save/load game progress
- [ ] Difficulty settings

## 👤 Author

**Oleksandr Kopii**
GitHub: [@SamuraiSanch](https://github.com/SamuraiSanch)

---
⭐ If you enjoyed this project, feel free to leave a star!
