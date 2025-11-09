# Grade Evaluation Program

## 📝 Problem Statement
Write a C program that determines a student's letter grade based on their percentage score.

The program should take an integer input representing the student's percentage and output the corresponding grade according to the following scale:

| Percentage Range | Grade |
|------------------|--------|
| 90–100           | A      |
| 80–89            | B      |
| 70–79            | C      |
| 60–69            | D      |
| 40–59            | E      |
| 0–39             | F      |

---

## 💡 Input
- A single integer `pct` (0 ≤ pct ≤ 100) representing the student's percentage.

---

## 🎯 Output
- Print a single uppercase letter (`A`, `B`, `C`, `D`, `E`, or `F`) indicating the student's grade.

---

## 🧩 Example

### Example 1
**Input**
```c
85
```

**Output**

```c
B
```

### Example 2
**Input**

```c
37
```

**Output**

```c
F
```

---

## ⚙️ Constraints
- `0 ≤ pct ≤ 100`
- Input is always an integer.
