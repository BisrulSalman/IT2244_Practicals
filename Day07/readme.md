
# 🔮 Life Path Number - Astrology Script (Shell)

Welcome to the **Astrology Life Path Number Calculator** — a fun and simple shell script that uses your **birth date** to calculate your **life path number** and give a short astrological prediction! 🌟🧙

---

## ✨ Features

- 📅 Takes your **birth date** as input
- 🔢 Calculates your **life path number** using numerology (sum of digits)
- 🔮 Displays a unique message based on the number using a `case` statement
- ✅ Lightweight, terminal-based, and easy to use

---

## 🧮 How It Works

Given your **birth date (1–31)**:
- It splits the date into two digits.
- Adds them together to form your **life path number**.
- Uses a `case` block to show a predefined message.

📌 **Example:**
```
Enter your Birth date: 23

Calculation:
a = 23 % 10 = 3
b = 23 / 10 = 2
c = a + b = 5

Result: "can get help"
```

---

## 📜 Life Path Messages

| Number | Message                  |
|--------|---------------------------|
| 1      | Lucky                    |
| 2      | Careful, do your works   |
| 3      | Stronger                 |
| 4      | Happy                    |
| 5      | Can get help             |
| 6      | Doubt                    |
| 7      | Sad                      |
| 8      | Like                     |
| 9      | Courage                  |

---

## 🚀 How to Run

1. Open terminal and create the script:
   ```bash
   vi life_path.sh
   ```
2. Paste the code, save, and exit.
3. Make it executable:
   ```bash
   chmod +x life_path.sh
   ```
4. Run it:
   ```bash
   ./life_path.sh
   ```

---

## 🛠 Requirements

- 🐧 Linux terminal (or PuTTY with a remote server)
- 📜 Basic shell knowledge

---

