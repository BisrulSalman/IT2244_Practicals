### ✅ `README.txt` — Process Control Exercises Using `fork()`, `wait()`, `exit()`

---

#### 📄 Exercise 01: `exit.c`

**Description:**
A simple program demonstrating how to pause execution using `sleep()` and then terminate using `exit()`.

**Code file:** `vi exit.c`
**Commands to compile and run:**

```bash
gcc exit.c -o exit
./exit
```

**Expected Output:**

```
Program started.
Sleeping for 3 seconds...
Exiting the program
```

---

#### 📄 Exercise 02: `wait.c`

**Description:**
Demonstrates parent-child process interaction using `fork()` and `wait()`. The parent waits for the child to finish.

**Code file:** `vi wait.c`
**Commands to compile and run:**

```bash
gcc wait.c -o wait
./wait
```

**Expected Output:**

```
Parent process started. PID: 10093
Parent waiting for child to finish..
Child process. PID: 10094, sleeping for 2 seconds..
Child process exiting.
Child exited with status: 0
Parent process ending.
```

---

#### 📄 Exercise 03: `day15_3.c`

**Description:**
Creates two child processes. First child sleeps 1 second, second child sleeps 3 seconds. Parent waits for both.

**Code file:** `vi day15_3.c`
**Commands to compile and run:**

```bash
gcc day15_3.c -o ex3
./ex3
```

**Expected Output:**

```
First child slept for 1 second
Second child slept for 3 seconds
Parent: both children have finished
```

---

#### 📄 Exercise 04: `day15_4.c`

**Description:**
Creates two children. The first child sleeps 2 seconds and exits with status 2. The second child sleeps 1 second and exits with status 1. Parent identifies the exit order and statuses.

**Code file:** `vi day15_4.c`
**Commands to compile and run:**

```bash
gcc day15_4.c -o ex4
./ex4
```

**Expected Output:**

```
Parent process started. PID: 14156
Parent: waiting for children to finish...
First child: PID 14157, sleeping for 2 seconds.
Second child: PID 14158, sleeping for 1 second.
Second child: exiting with status 1.
First child: exiting with status 2.
Parent: Child with PID 14158 finished first with exit status 1.
Parent: Child with PID 14157 finished second with exit status 2.
Parent: Both children have finished.
```

---

#### 📄 Exercise 05: `day15_5.c`

**Description:**
The parent creates a child. The child creates a grandchild. Grandchild sleeps 2 seconds and exits. Child prints its exit status and exits with 55. Parent prints child's exit status.

**Code file:** `vi day15_5.c`
**Commands to compile and run:**

```bash
gcc day15_5.c -o ex5
./ex5
```

**Expected Output:**

```
Parent started. PID: 14353
Child started. PID: 14354
Grandchild started. PID: 14355, sleeping 2 seconds...
Grandchild exiting with status 2.
Child: Grandchild exited with status 2.
Child exiting with status 55.
Parent: Child exited with status 55.
Parent exiting.
```

---

### 📌 Notes:

* Use `gcc` to compile each `.c` file.
* Use `./filename` to run the compiled program.
* This project demonstrates the basics of **process creation, management, and termination** in Linux using C.

