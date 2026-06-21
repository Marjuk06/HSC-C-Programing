# 📘 C Programming Exam Answer Sheet

**অ্যালগরিদম · ফ্লোচার্ট · সি প্রোগ্রাম**

[![Language](https://img.shields.io/badge/Language-C99-00599C?style=for-the-badge&logo=c&logoColor=white)](#-compilation)
[![Questions](https://img.shields.io/badge/Questions-38--78-2ea44f?style=for-the-badge)](#-quick-reference)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](#)

> এইচএসসি পরীক্ষার জন্য প্রস্তুতকৃত সম্পূর্ণ উত্তরমালা

---

## 📑 Table of Contents

- [Program Blueprints](#-program-blueprints)
- [Quick Reference](#-quick-reference)
- [Full Answers](#-full-answers)
- [Compilation](#-compilation)

---

##  Program Blueprints

> প্রতিটি প্রশ্ন নিচের ৮টি ব্লুপ্রিন্ট প্যাটার্নের যেকোনো একটি অনুসরণ করে।

<details>
<summary><b>🔹 Type 1 — Formula Based (সূত্রভিত্তিক)</b></summary>

```
Declare Variables → Input → Formula → Output
```

**Examples:** Area, Interest, Quadratic Formula, Fraction Addition

</details>

<details>
<summary><b>🔹 Type 2 — Decision Making (শর্তভিত্তিক)</b></summary>

```
Input → if / else → Output
```

**Examples:** Positive/Negative, Even/Odd, Largest, Smallest, Leap Year, Voter, Grade

</details>

<details>
<summary><b>🔹 Type 3 — Loop + Summation (লুপ + যোগফল)</b></summary>

```
Input → Initialize → Loop → Update Sum → Output
```

**Examples:** Any series sum, Square series, Cube series, Power series

</details>

<details>
<summary><b>🔹 Type 4 — Loop + Display (লুপ + প্রদর্শন)</b></summary>

```
Input → Loop → Display
```

**Examples:** Print numbers, Multiplication table, Even/Odd numbers, A to Z

</details>

<details>
<summary><b>🔹 Type 5 — Loop + Logic (লুপ + লজিক)</b></summary>

```
Input → Loop → Logic → Output
```

**Examples:** Prime, GCD, LCM, Reverse Number, Factorial

</details>

<details>
<summary><b>🔹 Type 6 — Array (অ্যারে)</b></summary>

```
Input Size → Input Array → Loop → Operation → Output
```

**Examples:** Array Sum, Search, Swap, Reverse

</details>

<details>
<summary><b>🔹 Type 7 — Function (ফাংশন)</b></summary>

```
main() → Function Call → Processing → Return Result
```

**Examples:** String Length, Power Function

</details>

<details>
<summary><b>🔹 Type 8 — Character / ASCII (ক্যারেক্টার)</b></summary>

```
Input Character → ASCII Logic → Output
```

**Examples:** Uppercase → Lowercase, ASCII Conversion

</details>

---

##  Quick Reference

| # | Program | Type | Key Construct |
|:-:|:--------|:----:|:-------------|
| ৩৮ | Voter Eligibility | 2 | `if (age >= 18)` |
| ৩৯ | Positive / Negative / Zero | 2 | `if-else if-else` |
| ৪০ | Zero / Even / Odd | 2 | `num % 2` |
| ৪১ | Largest of Three | 2 | `if-else if-else` |
| ৪২ | Smallest of Three | 2 | `if-else if-else` |
| ৪৩ | Leap Year | 2 | `% 400, % 100, % 4` |
| ৪৪ | LCM | 5 | `while` loop |
| ৪৫ | GCD | 5 | Euclidean `while` |
| ৪৬ | Prime Check | 5 | `for` + flag |
| ৪৭ | Sum 1+2+…+n | 3 | `for` + `sum` |
| ৪৮ | Sum of Odds | 3 | `i += 2` |
| ৪৯ | Sum of Evens | 3 | `i += 2` |
| ৫০ | Sum of Squares | 3 | `i * i` |
| ৫১ | 100²+95²+…+10² | 3 | `i -= 5` |
| ৫২ | 99²+88²+…+11² | 3 | `i -= 11` |
| ৫৩ | 1000+950+…+≥22 | 3 | `i -= 50` |
| ৫৪ | i(i+1) series | 3 | `i*(i+1)` |
| ৫৫ | i^i series | 3 | `pow(i, i)` |
| ৫৬ | 2²+4²+8²+… | 3 | `i *= 2` |
| ৫৭ | 3²+9²+27²+… | 3 | `i *= 3` |
| ৫৮ | Sum of Cubes | 3 | `i*i*i` |
| ৫৯ | 1+1/2²+1/3³+… | 3 | `1.0/pow(i,i)` |
| ৬০ | Factorial | 5 | `fact *= i` |
| ৬১ | i(i+1) series | 3 | `i*(i+1)` |
| ৬২ | Even/Odd 1–100 | 4 | two `for` loops |
| ৬৩ | Display 1 to n | 4 | `for` print |
| ৬৪ | Multiplication Table | 4 | `num * i` |
| ৬৫ | Array Sum | 6 | `arr[]` + `for` |
| ৬৬ | Array Swap | 6 | `temp` swap |
| ৬৭ | Array Search | 6 | Linear search |
| ৬৮ | Reverse Array | 6 | Two-pointer swap |
| ৬৯ | String Length (func) | 7 | Custom function |
| ৭০ | Power (loop) | 5 | `result *= base` |
| ৭১ | Reverse Integer | 5 | `% 10`, `/ 10` |
| ৭২ | Upper to Lower | 8 | `ch + 32` |
| ৭৩ | Quadratic Equation | 1 | `sqrt`, discriminant |
| ৭৪ | Reverse 4-digit | 5 | `% 10`, `/ 10` |
| ৭৫ | A to Z | 4 | `char` loop |
| ৭৬ | Power (pow) | 5 | `pow()` |
| ৭৭ | Grade from Marks | 2 | `if-else if` chain |
| ৭৮ | Fraction Addition | 1 | Cross-multiply |

---

##  Full Answers

**সম্পূর্ণ উত্তরমালা (অ্যালগরিদম + ফ্লোচার্ট + সি প্রোগ্রাম) দেখতে নিচের লিঙ্কে যান:**

 **[C_Programming_Exam_Answers.md](C_Programming_Exam_Answers.md)**

প্রতিটি প্রশ্নের জন্য আছে:
- বাংলায় অ্যালগরিদম (৫–৮ ধাপ)
- Mermaid ফ্লোচার্ট
- সম্পূর্ণ C99 প্রোগ্রাম

---

## Compilation

All programs use **C99 standard**. Compile with:

```bash
gcc -std=c99 -lm program.c -o program
```

> The `-lm` flag links the math library, required for programs using `math.h`.

---

**Made by Marjuk for C Programming Exam Preparation**
