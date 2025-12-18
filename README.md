# 🏓 Pong Game (Python Turtle)

A classic **Pong game** built using **Python** and the **Turtle graphics module**, applying Object-Oriented Programming (OOP) principles. The game features smooth paddle controls, ball collision physics, and dynamic speed increase with a capped maximum speed for balanced gameplay.

---

## 📌 Features

* Two-player Pong game
* Left & right paddles controlled via keyboard
* Ball movement with realistic bounce physics
* Ball speed increases on paddle collision
* Speed capped at a minimum threshold (prevents unplayable speeds)
* Clean OOP structure (`Paddle`, `Ball`, `Screen`)

---

## 🛠️ Technologies Used

* **Python 3**
* **Turtle Graphics Module**
* Object-Oriented Programming (OOP)

---

## 🎮 Controls

| Action            | Key              |
| ----------------- | ---------------- |
| Left Paddle Up    | `W`              |
| Left Paddle Down  | `S`              |
| Right Paddle Up   | `↑` (Up Arrow)   |
| Right Paddle Down | `↓` (Down Arrow) |

---

## 🚀 How to Run

1. Make sure **Python 3** is installed on your system
2. Clone this repository:

   ```bash
   git clone https://github.com/your-username/pong-game-turtle.git
   ```
3. Navigate into the project folder:

   ```bash
   cd pong-game-turtle
   ```
4. Run the main file:

   ```bash
   python main.py
   ```

---

## 🧠 Game Logic Overview

### Paddle

* Inherits from `turtle.Turtle`
* Uses `goto(position)` to allow flexible placement
* Moves vertically based on key input

### Ball

* Moves continuously across the screen
* Bounces off top & bottom walls
* Reverses direction on paddle collision
* Increases speed on each paddle hit
* Speed is capped using a minimum sleep threshold

```python
self.move_speed = max(self.min_speed, self.move_speed * 0.9)
```

---

## 📂 Project Structure

```
pong-game/
│
├── main.py          # Game loop & screen setup
├── paddle.py        # Paddle class
├── ball.py          # Ball class
└── README.md        # Project documentation
```

---

## 🎯 Learning Objectives

This project demonstrates:

* Python OOP fundamentals
* Class inheritance
* Game loops and event listeners
* Collision detection
* Speed control and constraints

---

## 🔮 Possible Improvements

* Add score tracking and display
* Add sound effects
* Single-player mode with AI paddle
* Difficulty levels

---

## 📜 License

This project is open-source and available under the **MIT License**.

---

## 🙌 Acknowledgements

Inspired by the classic **Pong arcade game** and built as a learning project using Python Turtle.

Happy coding! 🚀
