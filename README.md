# Java_suduko
# 🧩 Sudoku Solver in Java

This project is a Java implementation of a Sudoku puzzle solver using **backtracking**. The program takes a partially-filled 9x9 Sudoku board and fills in the empty cells (denoted by `'.'`) with valid digits (1-9), ensuring the final board follows all Sudoku rules.

---

## 📌 Features

- Solves any valid 9x9 Sudoku puzzle.
- Uses **recursive backtracking algorithm**.
- Checks for validity in:
  - Rows
  - Columns
  - 3x3 subgrids
- Easy to understand and modify.

---

## 🛠 How It Works

1. **Backtracking**:  
   It tries placing digits 1 to 9 in each empty cell.
   - If placing a digit is **valid**, it moves to the next empty cell.
   - If not, it **backtracks** and tries the next digit.

2. **Validation**:  
   Before placing a digit, the program checks:
   - The digit is not already in the current **row**.
   - The digit is not already in the current **column**.
   - The digit is not in the current **3x3 box**.

---

## 📂 Code Structure

### `Sudoku.java`

- `main()`  
  Initializes the Sudoku board and starts solving.

- `solve(char[][] board)`  
  Recursive function that applies the backtracking algorithm.

- `isValid(char[][] board, int row, int col, char num)`  
  Helper function to validate whether a number can be placed in a given cell.

---

## ▶️ Sample Input

