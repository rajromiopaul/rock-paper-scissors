# 🪨📄✂️ Rock Paper Scissors (Python)

A simple command-line **Rock, Paper, Scissors** game built using Python. Play against the computer and test your luck!

---

## 🚀 Features

* User vs Computer gameplay
* Randomized computer choices
* ASCII art visuals for each move
* Input validation for incorrect entries

---

## 🧠 How It Works

* You choose:

  * `0` → Rock 🪨
  * `1` → Paper 📄
  * `2` → Scissors ✂️

* The computer randomly selects one of the three options.

* The winner is decided based on classic rules:

  * Rock beats Scissors
  * Scissors beats Paper
  * Paper beats Rock

---

## ▶️ How to Run

1. Make sure Python is installed on your system.
2. Save the script as `game.py`.
3. Open terminal or command prompt.
4. Run the program:

```bash
python game.py
```

---

## 💻 Example Output

```
What do you choose? Type 0 for Rock, 1 for Paper or 2 for Scissors.
0

    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)

Computer chose:

    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)

You lose!
```

---

## ⚠️ Known Issues

* The condition:

  ```python
  elif user_choice > user_choice:
  ```

  is incorrect and will never be true.

* The condition:

  ```python
  elif computer_choice == computer_choice:
  ```

  will always result in `Draw!`.

### ✅ Suggested Fix

Replace the final logic with:

```python
elif user_choice > computer_choice:
    print("You win!")
elif user_choice == computer_choice:
    print("Draw!")
```

---

## 🛠️ Future Improvements

* Add score tracking
* Allow multiple rounds
* Create a GUI version
* Improve input handling (avoid crashes on invalid input)

---

## 📚 Requirements

* Python 3.x

---

## 👨‍💻 Author

Created as a beginner-friendly Python project to practice:

* Conditionals
* Lists
* Random module

---

Enjoy the game and keep coding! 🎉
