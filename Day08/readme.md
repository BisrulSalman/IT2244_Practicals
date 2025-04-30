
# 🔢 Bash Script Collection – Fibonacci, Factorial, Multiples

A collection of simple and beginner-friendly Linux shell scripts to demonstrate basic number operations like generating Fibonacci numbers, computing factorials, and listing multiples of 3.

---

## 📂 Contents

- [Q1️⃣ Fibonacci Series](#q1️⃣-fibonacci-series)
- [Q2️⃣ Factorial Calculation](#q2️⃣-factorial-calculation)
- [Q3️⃣ Multiples of 3](#q3️⃣-multiples-of-3)

---

## Q1️⃣ Fibonacci Series

📌 **Description:**  
Generates the first `n` Fibonacci numbers using a loop.

📥 **User Input:**  
Enter how many Fibonacci numbers to generate.

📤 **Sample Output:**
```
Enter the number:
10
0
1
1
2
3
5
8
13
21
34
```

🔧 **Script (fibonacci.sh):**
```bash
#!/bin/bash

echo "Enter the number:"
read num

a=0
b=1

for (( i=0; i<num; i++ ))
do
  echo "$a"
  c=$((a + b))
  a=$b
  b=$c
done
```

---

## Q2️⃣ Factorial Calculation

📌 **Description:**  
Calculates the factorial of a given number (example: 5).

📤 **Sample Output:**
```
factorial of 5 is: 120
```

🔧 **Script (factorial.sh):**
```bash
#!/bin/bash

num=5
fact=1

for (( i=1; i<=num; i++ ))
do
  fact=$((fact * i))
done

echo "factorial of $num is: $fact"
```

---

## Q3️⃣ Multiples of 3

📌 **Description:**  
Prints all multiples of 3 between 1 and 50.

📤 **Sample Output:**
```
3
6
9
12
15
18
21
24
27
30
33
36
39
42
45
48
```

🔧 **Script (multiples.sh):**
```bash
#!/bin/bash

i=3
while [ $i -le 50 ]
do
  echo $i
  i=$((i + 3))
done
```

---

## ▶️ How to Run

1. Create each `.sh` file using `vi` or any editor:
   ```bash
   vi fibonacci.sh
   vi factorial.sh
   vi multiples.sh
   ```
2. Give execution permission:
   ```bash
   chmod +x *.sh
   ```
3. Run a script:
   ```bash
   ./fibonacci.sh
   ```

---

## 🛠 Requirements

- Linux OS or compatible shell environment
- Basic shell scripting knowledge

---

