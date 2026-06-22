# 🪨📄✂️ Rock, Paper, Scissors

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://github.com/bhavani-builds)
[![CLI](https://img.shields.io/badge/CLI-Game-A78BFA?style=for-the-badge&logo=gnometerminal&logoColor=white)](https://github.com/bhavani-builds)
[![Status](https://img.shields.io/badge/Status-Beginner%20Project-E2E8F0?style=for-the-badge)](https://github.com/bhavani-builds)
[![Author](https://img.shields.io/badge/Author-bhavani--builds-161B22?style=for-the-badge&logo=github&logoColor=white)](https://github.com/bhavani-builds)

A terminal-based Rock-Paper-Scissors game with ASCII art moves and computer-vs-human logic. Built while leveling up Python fundamentals. 🐍

---

## 🕹️ What It Does

```
class RockPaperScissors:
    """
    ╔══════════════════════════════════════════════════════════╗
    ║         Classic Game — Terminal × ASCII Art Hybrid       ║
    ╚══════════════════════════════════════════════════════════╝
    """
    name        = "Rock, Paper, Scissors"
    language    = "Python 3"
    category    = "CLI Game / Beginner Project"

    mechanics   = ["Random computer choice", "ASCII art rendering", "Win/lose/draw logic"]
    modules     = ["random"]

    inputs      = {
        "0" : "Rock",
        "1" : "Paper",
        "2" : "Scissors",
    }

    fun_fact    = "Three symbols, infinite rivalry 🤜🤛"
```

---

## ⚡ How to Play

[#-how-to-play](#-how-to-play)

```bash
python rock_paper_scissors.py
```

1. Type `0`, `1`, or `2` when prompted.
2. Watch your choice render as ASCII art.
3. The computer picks randomly.
4. Result prints instantly — win, lose, or draw.

---

## 📋 Choice Reference

[#-choice-reference](#-choice-reference)

| Input | Choice   | Beats      |
| ----- | -------- | ---------- |
| `0`   | 🪨 Rock   | Scissors   |
| `1`   | 📄 Paper  | Rock       |
| `2`   | ✂️ Scissors | Paper    |

---

## 🧪 Sample Run

[#-sample-run](#-sample-run)

```
what do you choose? Type 0 for Rock, 1 for paper or 2 for scissors: 0

    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)

computer chose 2
you win
```

---

## 🐞 Known Issues

[#-known-issues](#-known-issues)

```
                  ╔══════════════════════════════════════════════╗
                  ║                 Bug Tracker                  ║
                  ╠══════════════════════════════════════════════╣
Prompt typo       ║  "Tyoe" → "Type"                  📌 OPEN    ║
F-string bug      ║  [computer_choice] not interpolated 🔴 BLOCKER║
Dead code branch  ║  Invalid input check unreachable    🔴 BLOCKER║
Message typos     ║  "loose" → "lose", inconsistent !  📌 OPEN    ║
Logic readability ║  Win/loss via > / < comparisons    🌱 REFACTOR║
                  ╚══════════════════════════════════════════════╝
```

- **F-string bug:** `print(F"computer chose [computer_choice]")` uses square brackets instead of curly braces — it prints the literal text `[computer_choice]` instead of the value. Fix:
  ```python
  print(f"computer chose {computer_choice}")
  ```
- **Dead code branch:** the `elif user_choice>=3 or user_choice<0:` check sits at the end of a chain that already resolves every valid comparison, so it can never execute. Move this check immediately after the input is read.
- **Typos:** "Tyoe" → "Type", "loose" → "lose"; messages also mix "You win" / "You win!" capitalization and punctuation.

---

## 🗺️ Roadmap

[#️-roadmap](#️-roadmap)

```
✅  Core game logic ........................ SHIPPED
✅  ASCII art for each move ................ SHIPPED
🔄  Fix f-string + dead code bugs .......... IN PROGRESS
📌  Replay loop (play multiple rounds) ..... PLANNED
📌  Running score tracker .................. PLANNED
🎯  Input validation with re-prompt ........ TARGET 🚀
```

---

## 🛠 Tech Stack

[#-tech-stack](#-tech-stack)

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://github.com/bhavani-builds)
[![Random](https://img.shields.io/badge/random-module-FF6B6B?style=for-the-badge&logo=python&logoColor=white)](https://github.com/bhavani-builds)
[![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)](https://github.com/bhavani-builds)
[![GitHub](https://img.shields.io/badge/GitHub-161B22?style=for-the-badge&logo=github&logoColor=white)](https://github.com/bhavani-builds)

---

## 🤝 Connect

[#-connect](#-connect)

> 💼 Built by **[bhavani-builds](https://github.com/bhavani-builds)** — learning deeply, building consistently.

[![GitHub](https://img.shields.io/badge/GitHub-Explore%20My%20Work-161B22?style=for-the-badge&logo=github&logoColor=white)](https://github.com/bhavani-builds)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/naga-durga-bhavani-neelapala-20767a413/)

---

⚡ *"Rock, paper, scissors — small game, real practice."* ⚡
