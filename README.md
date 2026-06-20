# Seeding Pattern (Inverted Star Triangle) in C++

A beginner-friendly C++ program that demonstrates pattern printing using nested loops.

This project generates an **Inverted Right-Angled Triangle Star Pattern**, where the number of stars decreases by one in each row. It is a common pattern-printing exercise used to strengthen understanding of nested loops and iteration logic.

---

## 📌 Features

* Prints an inverted star triangle pattern
* Uses nested `for` loops
* Demonstrates decreasing loop boundaries
* Beginner-friendly implementation
* Helps build pattern recognition and logic-building skills

---

## 🛠️ Technologies Used

* C++
* Standard Input/Output (`iostream`)

---

## 📂 Problem Statement

Given an integer `N`, print an inverted right-angled triangle pattern where each row contains one fewer star than the previous row.

### Example

For:

```txt
N = 5
```

Output:

```txt
* * * * *
* * * *
* * *
* *
*
```

---

## 📸 Screenshot

<img width="1206" height="786" alt="Screenshot 2026-06-20 074247" src="https://github.com/user-attachments/assets/19dd52da-1e07-4170-89cd-b093625188ab" />

Example folder structure:

```txt
project-folder/
│
├── main.cpp
├── README.md
└── screenshots/
    └── output.png
```

---

## 💻 Source Code

```cpp
void seeding(int n) {
    for(int i = 1; i <= n; i++) {
        for(int j = 0; j < n - i + 1; j++) {
            cout << "* ";
        }
        cout << endl;
    }
}
```

---

## ▶️ How to Run

1. Compile the program:

```bash
g++ main.cpp -o main
```

2. Run the executable:

```bash
./main
```

3. Enter the value of `N`.

---

## 📸 Example Output

### Input

```txt
4
```

### Output

```txt
* * * *
* * *
* *
*
```

---

## 📖 Learning Concepts

This project helps beginners understand:

* Nested loops
* Pattern printing
* Loop control and boundaries
* Decreasing iteration patterns
* Algorithmic thinking
* Basic time complexity analysis

---

## 🔍 Pattern Explanation

The outer loop controls the number of rows:

```cpp
for(int i = 1; i <= n; i++)
```

The inner loop controls the number of stars printed in each row:

```cpp
for(int j = 0; j < n - i + 1; j++)
```

As the value of `i` increases, the number of stars decreases by one, forming an inverted right-angled triangle.

---

## ⏱️ Complexity Analysis

### Time Complexity

```txt
O(N²)
```

### Space Complexity

```txt
O(1)
```

No additional memory is used apart from loop variables.

---

## 👨‍💻 Author

Developed as a beginner-friendly C++ practice project for learning nested loops, pattern printing, and problem-solving techniques.
