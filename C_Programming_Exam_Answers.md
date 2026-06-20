<![CDATA[<div align="center">

# 📘 C Programming Exam Answer Sheet

### অ্যালগরিদম · ফ্লোচার্ট · সি প্রোগ্রাম

[![C](https://img.shields.io/badge/Language-C99-blue?style=for-the-badge&logo=c&logoColor=white)](#)
[![Questions](https://img.shields.io/badge/Questions-38--78-green?style=for-the-badge)](#)
[![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=for-the-badge)](#)

---

> **ডিপ্লোমা / এইচএসসি / বিশ্ববিদ্যালয় পরীক্ষার জন্য প্রস্তুতকৃত সম্পূর্ণ উত্তরমালা**

</div>

---

## 📑 Table of Contents

| Blueprint | Type | Questions |
|:---|:---|:---|
| [Type 1 – Formula Based](#type-1--formula-based) | সূত্রভিত্তিক | ৭৩, ৭৮ |
| [Type 2 – Decision Making](#type-2--decision-making) | শর্তভিত্তিক | ৩৮, ৩৯, ৪০, ৪১, ৪২, ৪৩, ৭৭ |
| [Type 3 – Loop + Summation](#type-3--loop--summation) | লুপ + যোগফল | ৪৭, ৪৮, ৪৯, ৫০, ৫১, ৫২, ৫৩, ৫৪, ৫৫, ৫৬, ৫৭, ৫৮, ৫৯, ৬১ |
| [Type 4 – Loop + Display](#type-4--loop--display) | লুপ + প্রদর্শন | ৬২, ৬৩, ৬৪, ৭৫ |
| [Type 5 – Loop + Logic](#type-5--loop--logic) | লুপ + লজিক | ৪৪, ৪৫, ৪৬, ৬০, ৭০, ৭১, ৭৪, ৭৬ |
| [Type 6 – Array](#type-6--array) | অ্যারে | ৬৫, ৬৬, ৬৭, ৬৮ |
| [Type 7 – Function](#type-7--function) | ফাংশন | ৬৯ |
| [Type 8 – Character / ASCII](#type-8--character--ascii) | ক্যারেক্টার | ৭২ |

---

## 🧬 Program Blueprints

<details>
<summary><b>Click to expand all blueprints</b></summary>

### 🔹 Type 1 – Formula Based

```
Declare Variables
      ↓
    Input
      ↓
   Formula
      ↓
   Output
```

**Examples:** Area, Interest, Quadratic Formula, Fraction Addition

---

### 🔹 Type 2 – Decision Making

```
    Input
      ↓
  if / else
      ↓
   Output
```

**Examples:** Positive/Negative, Even/Odd, Largest, Smallest, Leap Year, Voter, Grade

---

### 🔹 Type 3 – Loop + Summation

```
    Input
      ↓
  Initialize
      ↓
    Loop
      ↓
 Update Sum
      ↓
   Output
```

**Examples:** Any series sum, Square series, Cube series, Power series

---

### 🔹 Type 4 – Loop + Display

```
    Input
      ↓
    Loop
      ↓
   Display
```

**Examples:** Print numbers, Multiplication table, Even/Odd numbers, A to Z

---

### 🔹 Type 5 – Loop + Logic

```
    Input
      ↓
    Loop
      ↓
   Logic
      ↓
   Output
```

**Examples:** Prime, GCD, LCM, Reverse Number, Factorial

---

### 🔹 Type 6 – Array

```
 Input Size
      ↓
 Input Array
      ↓
    Loop
      ↓
 Operation
      ↓
   Output
```

**Examples:** Array Sum, Search, Swap, Reverse

---

### 🔹 Type 7 – Function

```
   main()
      ↓
Function Call
      ↓
 Processing
      ↓
Return Result
```

**Examples:** String Length, Power Function

---

### 🔹 Type 8 – Character / ASCII

```
Input Character
      ↓
 ASCII Logic
      ↓
   Output
```

**Examples:** Uppercase → Lowercase, ASCII Conversion

</details>

---

---

# Type 1 – Formula Based

---

## প্রশ্ন ৭৩ — দ্বিঘাত সমীকরণের মান নির্ণয়

**Program:** Find Roots of a Quadratic Equation (ax² + bx + c = 0)

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `a`, `b`, `c`, `d`, `r1`, `r2` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: `a`, `b`, `c` এর মান ইনপুট নাও।
ধাপ ৪: `d = b*b - 4*a*c` নির্ণয় কর।
ধাপ ৫: যদি `d > 0` হয়, তবে দুটি বাস্তব মূল `r1 = (-b+√d)/(2a)`, `r2 = (-b-√d)/(2a)` নির্ণয় কর।
ধাপ ৬: যদি `d == 0` হয়, তবে একটি মূল `r1 = -b/(2a)` নির্ণয় কর।
ধাপ ৭: যদি `d < 0` হয়, তবে "বাস্তব মূল নেই" প্রদর্শন কর।
ধাপ ৮: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
    ┌─────────────┐
    │ Input a,b,c │
    └──────┬──────┘
           ▼
    ┌─────────────┐
    │d=b²-4ac     │
    └──────┬──────┘
           ▼
      ┌─────────┐     Yes    ┌────────────────┐
      │ d > 0 ? ├───────────►│ Two real roots │
      └────┬────┘            └────────────────┘
           │ No
           ▼
      ┌─────────┐     Yes    ┌────────────────┐
      │ d == 0 ?├───────────►│ One real root   │
      └────┬────┘            └────────────────┘
           │ No
           ▼
    ┌──────────────┐
    │ No real root │
    └──────┬───────┘
           ▼
       ┌───────┐
       │  End  │
       └───────┘
```

### সি প্রোগ্রাম

```c
#include <stdio.h>
#include <math.h>

int main() {
    float a, b, c, d, r1, r2;
    printf("Enter a, b, c: ");
    scanf("%f %f %f", &a, &b, &c);

    d = b * b - 4 * a * c;

    if (d > 0) {
        r1 = (-b + sqrt(d)) / (2 * a);
        r2 = (-b - sqrt(d)) / (2 * a);
        printf("Root 1 = %.2f\nRoot 2 = %.2f\n", r1, r2);
    } else if (d == 0) {
        r1 = -b / (2 * a);
        printf("Root = %.2f\n", r1);
    } else {
        printf("No real roots.\n");
    }

    return 0;
}
```

---

## প্রশ্ন ৭৮ — ভগ্নাংশ সংখ্যার যোগফল নির্ণয়

**Program:** Find Sum of Two Fractions

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `n1`, `d1`, `n2`, `d2`, `rn`, `rd` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: প্রথম ভগ্নাংশের লব (`n1`) ও হর (`d1`) ইনপুট নাও।
ধাপ ৪: দ্বিতীয় ভগ্নাংশের লব (`n2`) ও হর (`d2`) ইনপুট নাও।
ধাপ ৫: `rn = n1*d2 + n2*d1` এবং `rd = d1*d2` হিসাব কর।
ধাপ ৬: ফলাফল `rn/rd` প্রদর্শন কর।
ধাপ ৭: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
        ┌───────┐
        │ Start │
        └───┬───┘
            ▼
  ┌───────────────────┐
  │ Input n1,d1,n2,d2 │
  └─────────┬─────────┘
            ▼
  ┌───────────────────────┐
  │ rn = n1*d2 + n2*d1    │
  │ rd = d1*d2            │
  └─────────┬─────────────┘
            ▼
  ┌───────────────────┐
  │ Print rn / rd     │
  └─────────┬─────────┘
            ▼
        ┌───────┐
        │  End  │
        └───────┘
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int n1, d1, n2, d2, rn, rd;
    printf("Enter first fraction (numerator denominator): ");
    scanf("%d %d", &n1, &d1);
    printf("Enter second fraction (numerator denominator): ");
    scanf("%d %d", &n2, &d2);

    rn = n1 * d2 + n2 * d1;
    rd = d1 * d2;

    printf("Sum = %d/%d\n", rn, rd);

    return 0;
}
```

---

---

# Type 2 – Decision Making

---

## প্রশ্ন ৩৮ — ভোটার নির্ণয়

**Program:** Determine Voter Eligibility

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `age` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: বয়স ইনপুট নাও।
ধাপ ৪: যদি `age >= 18` হয়, তবে "ভোটার" প্রদর্শন কর।
ধাপ ৫: অন্যথায় "ভোটার নয়" প্রদর্শন কর।
ধাপ ৬: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
     ┌───────────┐
     │ Input age │
     └─────┬─────┘
           ▼
      ┌──────────┐
      │age >= 18?│
      └──┬───┬───┘
     Yes │   │ No
         ▼   ▼
  ┌────────┐ ┌──────────┐
  │ Voter  │ │ Not Voter│
  └───┬────┘ └─────┬────┘
      │            │
      └─────┬──────┘
            ▼
        ┌───────┐
        │  End  │
        └───────┘
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int age;
    printf("Enter age: ");
    scanf("%d", &age);

    if (age >= 18)
        printf("You are a Voter.\n");
    else
        printf("You are not a Voter.\n");

    return 0;
}
```

---

## প্রশ্ন ৩৯ — শূন্য, ধনাত্মক নাকি ঋণাত্মক নির্ণয়

**Program:** Check if a Number is Zero, Positive or Negative

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `num` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: সংখ্যা ইনপুট নাও।
ধাপ ৪: যদি `num > 0` হয়, তবে "Positive" প্রদর্শন কর।
ধাপ ৫: যদি `num < 0` হয়, তবে "Negative" প্রদর্শন কর।
ধাপ ৬: অন্যথায় "Zero" প্রদর্শন কর।
ধাপ ৭: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
     ┌───────────┐
     │ Input num │
     └─────┬─────┘
           ▼
      ┌──────────┐  Yes  ┌──────────┐
      │ num > 0? ├──────►│ Positive │
      └────┬─────┘       └──────────┘
           │ No
           ▼
      ┌──────────┐  Yes  ┌──────────┐
      │ num < 0? ├──────►│ Negative │
      └────┬─────┘       └──────────┘
           │ No
           ▼
      ┌──────────┐
      │   Zero   │
      └────┬─────┘
           ▼
       ┌───────┐
       │  End  │
       └───────┘
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    float num;
    printf("Enter a number: ");
    scanf("%f", &num);

    if (num > 0)
        printf("Positive\n");
    else if (num < 0)
        printf("Negative\n");
    else
        printf("Zero\n");

    return 0;
}
```

---

## প্রশ্ন ৪০ — শূন্য, জোড় নাকি বিজোড় নির্ণয়

**Program:** Check if a Number is Zero, Even or Odd

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `num` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: সংখ্যা ইনপুট নাও।
ধাপ ৪: যদি `num == 0` হয়, তবে "Zero" প্রদর্শন কর।
ধাপ ৫: যদি `num % 2 == 0` হয়, তবে "Even" প্রদর্শন কর।
ধাপ ৬: অন্যথায় "Odd" প্রদর্শন কর।
ধাপ ৭: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
     ┌───────────┐
     │ Input num │
     └─────┬─────┘
           ▼
      ┌──────────┐  Yes  ┌──────┐
      │num == 0? ├──────►│ Zero │
      └────┬─────┘       └──────┘
           │ No
           ▼
      ┌────────────┐  Yes  ┌──────┐
      │num%2 == 0? ├──────►│ Even │
      └─────┬──────┘       └──────┘
            │ No
            ▼
        ┌───────┐
        │  Odd  │
        └───┬───┘
            ▼
        ┌───────┐
        │  End  │
        └───────┘
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int num;
    printf("Enter a number: ");
    scanf("%d", &num);

    if (num == 0)
        printf("Zero\n");
    else if (num % 2 == 0)
        printf("Even\n");
    else
        printf("Odd\n");

    return 0;
}
```

---

## প্রশ্ন ৪১ — তিনটি সংখ্যার মধ্যে বড় সংখ্যা নির্ণয়

**Program:** Find the Largest Among Three Numbers

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `a`, `b`, `c` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: তিনটি সংখ্যা ইনপুট নাও।
ধাপ ৪: যদি `a > b` এবং `a > c` হয়, তবে `a` বড়।
ধাপ ৫: যদি `b > a` এবং `b > c` হয়, তবে `b` বড়।
ধাপ ৬: অন্যথায় `c` বড়।
ধাপ ৭: ফলাফল প্রদর্শন কর।
ধাপ ৮: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
    ┌─────────────┐
    │ Input a,b,c │
    └──────┬──────┘
           ▼
  ┌────────────────┐  Yes  ┌────────────┐
  │a > b && a > c? ├──────►│ a is max   │
  └───────┬────────┘       └────────────┘
          │ No
          ▼
  ┌────────────────┐  Yes  ┌────────────┐
  │b > a && b > c? ├──────►│ b is max   │
  └───────┬────────┘       └────────────┘
          │ No
          ▼
     ┌──────────┐
     │ c is max │
     └────┬─────┘
          ▼
      ┌───────┐
      │  End  │
      └───────┘
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    float a, b, c;
    printf("Enter three numbers: ");
    scanf("%f %f %f", &a, &b, &c);

    if (a >= b && a >= c)
        printf("Largest = %.2f\n", a);
    else if (b >= a && b >= c)
        printf("Largest = %.2f\n", b);
    else
        printf("Largest = %.2f\n", c);

    return 0;
}
```

---

## প্রশ্ন ৪২ — তিনটি সংখ্যার মধ্যে ছোট সংখ্যা নির্ণয়

**Program:** Find the Smallest Among Three Numbers

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `a`, `b`, `c` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: তিনটি সংখ্যা ইনপুট নাও।
ধাপ ৪: যদি `a < b` এবং `a < c` হয়, তবে `a` ছোট।
ধাপ ৫: যদি `b < a` এবং `b < c` হয়, তবে `b` ছোট।
ধাপ ৬: অন্যথায় `c` ছোট।
ধাপ ৭: ফলাফল প্রদর্শন কর।
ধাপ ৮: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
    ┌─────────────┐
    │ Input a,b,c │
    └──────┬──────┘
           ▼
  ┌────────────────┐  Yes  ┌────────────┐
  │a < b && a < c? ├──────►│ a is min   │
  └───────┬────────┘       └────────────┘
          │ No
          ▼
  ┌────────────────┐  Yes  ┌────────────┐
  │b < a && b < c? ├──────►│ b is min   │
  └───────┬────────┘       └────────────┘
          │ No
          ▼
     ┌──────────┐
     │ c is min │
     └────┬─────┘
          ▼
      ┌───────┐
      │  End  │
      └───────┘
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    float a, b, c;
    printf("Enter three numbers: ");
    scanf("%f %f %f", &a, &b, &c);

    if (a <= b && a <= c)
        printf("Smallest = %.2f\n", a);
    else if (b <= a && b <= c)
        printf("Smallest = %.2f\n", b);
    else
        printf("Smallest = %.2f\n", c);

    return 0;
}
```

---

## প্রশ্ন ৪৩ — অধিবর্ষ (Leap Year) নির্ণয়

**Program:** Check Leap Year

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `year` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: বছর ইনপুট নাও।
ধাপ ৪: যদি `year` ৪০০ দ্বারা বিভাজ্য হয়, তবে অধিবর্ষ।
ধাপ ৫: যদি `year` ১০০ দ্বারা বিভাজ্য হয়, তবে অধিবর্ষ নয়।
ধাপ ৬: যদি `year` ৪ দ্বারা বিভাজ্য হয়, তবে অধিবর্ষ।
ধাপ ৭: অন্যথায় অধিবর্ষ নয়।
ধাপ ৮: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
        ┌───────┐
        │ Start │
        └───┬───┘
            ▼
     ┌─────────────┐
     │ Input year  │
     └──────┬──────┘
            ▼
    ┌──────────────┐  Yes  ┌───────────┐
    │year%400 == 0?├──────►│ Leap Year │
    └──────┬───────┘       └───────────┘
           │ No
           ▼
    ┌──────────────┐  Yes  ┌───────────────┐
    │year%100 == 0?├──────►│ Not Leap Year │
    └──────┬───────┘       └───────────────┘
           │ No
           ▼
    ┌──────────────┐  Yes  ┌───────────┐
    │year%4 == 0?  ├──────►│ Leap Year │
    └──────┬───────┘       └───────────┘
           │ No
           ▼
   ┌───────────────┐
   │ Not Leap Year │
   └───────┬───────┘
           ▼
       ┌───────┐
       │  End  │
       └───────┘
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int year;
    printf("Enter year: ");
    scanf("%d", &year);

    if ((year % 400 == 0) || (year % 100 != 0 && year % 4 == 0))
        printf("%d is a Leap Year.\n", year);
    else
        printf("%d is not a Leap Year.\n", year);

    return 0;
}
```

---

## প্রশ্ন ৭৭ — পরীক্ষায় প্রাপ্ত নম্বর অনুযায়ী গ্রেড নির্ণয়

**Program:** Determine Grade from Marks

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `marks` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: নম্বর ইনপুট নাও।
ধাপ ৪: যদি `marks >= 80` হয়, তবে "A+" প্রদর্শন কর।
ধাপ ৫: যদি `marks >= 70` হয়, তবে "A" প্রদর্শন কর।
ধাপ ৬: যদি `marks >= 60` হয়, তবে "A-" প্রদর্শন কর।
ধাপ ৭: যদি `marks >= 50` হয়, তবে "B" প্রদর্শন কর।
ধাপ ৮: যদি `marks >= 40` হয়, তবে "C" প্রদর্শন কর।
ধাপ ৯: যদি `marks >= 33` হয়, তবে "D" প্রদর্শন কর।
ধাপ ১০: অন্যথায় "F (Fail)" প্রদর্শন কর।
ধাপ ১১: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
    ┌─────────────┐
    │ Input marks │
    └──────┬──────┘
           ▼
     ┌───────────┐ Yes ┌────┐
     │marks >= 80├────►│ A+ │
     └─────┬─────┘     └────┘
           │ No
           ▼
     ┌───────────┐ Yes ┌────┐
     │marks >= 70├────►│ A  │
     └─────┬─────┘     └────┘
           │ No
           ▼
     ┌───────────┐ Yes ┌────┐
     │marks >= 60├────►│ A- │
     └─────┬─────┘     └────┘
           │ No
           ▼
     ┌───────────┐ Yes ┌────┐
     │marks >= 50├────►│ B  │
     └─────┬─────┘     └────┘
           │ No
           ▼
     ┌───────────┐ Yes ┌────┐
     │marks >= 40├────►│ C  │
     └─────┬─────┘     └────┘
           │ No
           ▼
     ┌───────────┐ Yes ┌────┐
     │marks >= 33├────►│ D  │
     └─────┬─────┘     └────┘
           │ No
           ▼
        ┌──────┐
        │  F   │
        └──┬───┘
           ▼
       ┌───────┐
       │  End  │
       └───────┘
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    float marks;
    printf("Enter marks: ");
    scanf("%f", &marks);

    if (marks >= 80)
        printf("Grade: A+\n");
    else if (marks >= 70)
        printf("Grade: A\n");
    else if (marks >= 60)
        printf("Grade: A-\n");
    else if (marks >= 50)
        printf("Grade: B\n");
    else if (marks >= 40)
        printf("Grade: C\n");
    else if (marks >= 33)
        printf("Grade: D\n");
    else
        printf("Grade: F (Fail)\n");

    return 0;
}
```

---

---

# Type 3 – Loop + Summation

---

## প্রশ্ন ৪৭ — 1+2+3+...+n ধারার যোগফল

**Program:** Sum of Series 1+2+3+...+n

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `n`, `i`, `sum=0` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: `n` এর মান ইনপুট নাও।
ধাপ ৪: `i=1` থেকে `n` পর্যন্ত লুপ চালাও এবং `sum = sum + i` কর।
ধাপ ৫: `sum` প্রদর্শন কর।
ধাপ ৬: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
     ┌───────────┐
     │ Input n   │
     │ sum=0,i=1 │
     └─────┬─────┘
           ▼
      ┌──────────┐  No   ┌────────────┐
      │ i <= n?  ├───────►│ Print sum │
      └────┬─────┘        └─────┬──────┘
           │ Yes                │
           ▼                    ▼
    ┌─────────────┐         ┌───────┐
    │ sum=sum+i   │         │  End  │
    │ i=i+1       │         └───────┘
    └──────┬──────┘
           │
           └──────────┐
                      ▲
                (back to loop)
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int n, i, sum = 0;
    printf("Enter n: ");
    scanf("%d", &n);

    for (i = 1; i <= n; i++)
        sum += i;

    printf("Sum = %d\n", sum);

    return 0;
}
```

---

## প্রশ্ন ৪৮ — 1+3+5+...+n (বিজোড় সংখ্যার যোগফল)

**Program:** Sum of Odd Numbers 1+3+5+...+n

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `n`, `i`, `sum=0` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: `n` এর মান ইনপুট নাও।
ধাপ ৪: `i=1` থেকে `n` পর্যন্ত ২ করে বৃদ্ধি করে লুপ চালাও এবং `sum = sum + i` কর।
ধাপ ৫: `sum` প্রদর্শন কর।
ধাপ ৬: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
     ┌───────────┐
     │ Input n   │
     │ sum=0,i=1 │
     └─────┬─────┘
           ▼
      ┌──────────┐  No   ┌────────────┐
      │ i <= n?  ├───────►│ Print sum │
      └────┬─────┘        └─────┬──────┘
           │ Yes                │
           ▼                    ▼
    ┌─────────────┐         ┌───────┐
    │ sum=sum+i   │         │  End  │
    │ i=i+2       │         └───────┘
    └──────┬──────┘
           └──► (back to loop)
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int n, i, sum = 0;
    printf("Enter n: ");
    scanf("%d", &n);

    for (i = 1; i <= n; i += 2)
        sum += i;

    printf("Sum = %d\n", sum);

    return 0;
}
```

---

## প্রশ্ন ৪৯ — 2+4+6+...+n (জোড় সংখ্যার যোগফল)

**Program:** Sum of Even Numbers 2+4+6+...+n

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `n`, `i`, `sum=0` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: `n` এর মান ইনপুট নাও।
ধাপ ৪: `i=2` থেকে `n` পর্যন্ত ২ করে বৃদ্ধি করে লুপ চালাও এবং `sum = sum + i` কর।
ধাপ ৫: `sum` প্রদর্শন কর।
ধাপ ৬: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
     ┌───────────┐
     │ Input n   │
     │ sum=0,i=2 │
     └─────┬─────┘
           ▼
      ┌──────────┐  No   ┌────────────┐
      │ i <= n?  ├───────►│ Print sum │
      └────┬─────┘        └─────┬──────┘
           │ Yes                │
           ▼                    ▼
    ┌─────────────┐         ┌───────┐
    │ sum=sum+i   │         │  End  │
    │ i=i+2       │         └───────┘
    └──────┬──────┘
           └──► (back to loop)
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int n, i, sum = 0;
    printf("Enter n: ");
    scanf("%d", &n);

    for (i = 2; i <= n; i += 2)
        sum += i;

    printf("Sum = %d\n", sum);

    return 0;
}
```

---

## প্রশ্ন ৫০ — 1²+2²+3²+...+N² ধারার যোগফল

**Program:** Sum of Squares 1²+2²+3²+...+N²

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `n`, `i`, `sum=0` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: `n` এর মান ইনপুট নাও।
ধাপ ৪: `i=1` থেকে `n` পর্যন্ত লুপ চালাও এবং `sum = sum + i*i` কর।
ধাপ ৫: `sum` প্রদর্শন কর।
ধাপ ৬: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
     ┌───────────┐
     │ Input n   │
     │ sum=0,i=1 │
     └─────┬─────┘
           ▼
      ┌──────────┐  No   ┌────────────┐
      │ i <= n?  ├───────►│ Print sum │
      └────┬─────┘        └─────┬──────┘
           │ Yes                │
           ▼                    ▼
    ┌──────────────┐        ┌───────┐
    │ sum=sum+i*i  │        │  End  │
    │ i=i+1        │        └───────┘
    └──────┬───────┘
           └──► (back to loop)
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int n, i, sum = 0;
    printf("Enter n: ");
    scanf("%d", &n);

    for (i = 1; i <= n; i++)
        sum += i * i;

    printf("Sum = %d\n", sum);

    return 0;
}
```

---

## প্রশ্ন ৫১ — 100²+95²+90²+...+10²

**Program:** Sum of Series 100²+95²+90²+...+10²

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `i`, `sum=0` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: `i=100` থেকে `10` পর্যন্ত ৫ করে কমিয়ে লুপ চালাও এবং `sum = sum + i*i` কর।
ধাপ ৪: `sum` প্রদর্শন কর।
ধাপ ৫: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
        ┌───────┐
        │ Start │
        └───┬───┘
            ▼
     ┌─────────────┐
     │sum=0, i=100 │
     └──────┬──────┘
            ▼
      ┌───────────┐  No   ┌────────────┐
      │ i >= 10?  ├───────►│ Print sum │
      └─────┬─────┘        └─────┬──────┘
            │ Yes                 │
            ▼                     ▼
    ┌───────────────┐         ┌───────┐
    │ sum=sum+i*i   │         │  End  │
    │ i=i-5         │         └───────┘
    └───────┬───────┘
            └──► (back to loop)
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int i, sum = 0;

    for (i = 100; i >= 10; i -= 5)
        sum += i * i;

    printf("Sum = %d\n", sum);

    return 0;
}
```

---

## প্রশ্ন ৫২ — 99²+88²+77²+66²+...+5² (Not standard)

**Program:** Sum of Series 99²+88²+77²+...  (decreasing by 11, down to a small value)

> **Note:** Pattern: starts at 99, decreases by 11 → 99, 88, 77, 66, 55, 44, 33, 22, 11. The question ends with 5², but the nearest in the pattern would be stopping before going below some threshold. We interpret the series as: **i = 99, 88, 77, ..., 11** (step -11).

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `i`, `sum=0` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: `i=99` থেকে `i > 0` পর্যন্ত ১১ করে কমিয়ে লুপ চালাও এবং `sum = sum + i*i` কর।
ধাপ ৪: `sum` প্রদর্শন কর।
ধাপ ৫: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
        ┌───────┐
        │ Start │
        └───┬───┘
            ▼
     ┌────────────┐
     │sum=0, i=99 │
     └──────┬─────┘
            ▼
      ┌──────────┐  No   ┌────────────┐
      │ i > 0?   ├───────►│ Print sum │
      └────┬─────┘        └─────┬──────┘
           │ Yes                │
           ▼                    ▼
    ┌──────────────┐        ┌───────┐
    │ sum=sum+i*i  │        │  End  │
    │ i=i-11       │        └───────┘
    └──────┬───────┘
           └──► (back to loop)
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int i, sum = 0;

    for (i = 99; i > 0; i -= 11)
        sum += i * i;

    printf("Sum = %d\n", sum);

    return 0;
}
```

---

## প্রশ্ন ৫৩ — 1000+950+900+...+22 (Not standard ending)

**Program:** Sum of Series 1000+950+900+...  (decreasing by 50, down to ≥22)

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `i`, `sum=0` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: `i=1000` থেকে `i >= 22` পর্যন্ত ৫০ করে কমিয়ে লুপ চালাও এবং `sum = sum + i` কর।
ধাপ ৪: `sum` প্রদর্শন কর।
ধাপ ৫: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
        ┌───────┐
        │ Start │
        └───┬───┘
            ▼
     ┌──────────────┐
     │sum=0, i=1000 │
     └──────┬───────┘
            ▼
      ┌───────────┐  No   ┌────────────┐
      │ i >= 22?  ├───────►│ Print sum │
      └─────┬─────┘        └─────┬──────┘
            │ Yes                 │
            ▼                     ▼
    ┌──────────────┐          ┌───────┐
    │ sum=sum+i    │          │  End  │
    │ i=i-50       │          └───────┘
    └──────┬───────┘
           └──► (back to loop)
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int i, sum = 0;

    for (i = 1000; i >= 22; i -= 50)
        sum += i;

    printf("Sum = %d\n", sum);

    return 0;
}
```

---

## প্রশ্ন ৫৪ — 1·2 + 2·3 + 3·4 + ... + n(n+1)

**Program:** Sum of Series i×(i+1)

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `n`, `i`, `sum=0` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: `n` এর মান ইনপুট নাও।
ধাপ ৪: `i=1` থেকে `n` পর্যন্ত লুপ চালাও এবং `sum = sum + i*(i+1)` কর।
ধাপ ৫: `sum` প্রদর্শন কর।
ধাপ ৬: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
     ┌───────────┐
     │ Input n   │
     │ sum=0,i=1 │
     └─────┬─────┘
           ▼
      ┌──────────┐  No   ┌────────────┐
      │ i <= n?  ├───────►│ Print sum │
      └────┬─────┘        └────────────┘
           │ Yes
           ▼
   ┌────────────────┐
   │sum=sum+i*(i+1) │
   │ i=i+1          │
   └────────┬───────┘
            └──► (back to loop)
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int n, i, sum = 0;
    printf("Enter n: ");
    scanf("%d", &n);

    for (i = 1; i <= n; i++)
        sum += i * (i + 1);

    printf("Sum = %d\n", sum);

    return 0;
}
```

---

## প্রশ্ন ৫৫ — 1¹+2²+3³+...+Nᴺ

**Program:** Sum of Series i^i

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `n`, `i`, `sum` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: `n` এর মান ইনপুট নাও।
ধাপ ৪: `i=1` থেকে `n` পর্যন্ত লুপ চালাও এবং `sum = sum + pow(i, i)` কর।
ধাপ ৫: `sum` প্রদর্শন কর।
ধাপ ৬: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
     ┌───────────┐
     │ Input n   │
     │ sum=0,i=1 │
     └─────┬─────┘
           ▼
      ┌──────────┐  No   ┌────────────┐
      │ i <= n?  ├───────►│ Print sum │
      └────┬─────┘        └────────────┘
           │ Yes
           ▼
   ┌──────────────────┐
   │sum=sum+pow(i, i) │
   │ i=i+1            │
   └────────┬─────────┘
            └──► (back to loop)
```

### সি প্রোগ্রাম

```c
#include <stdio.h>
#include <math.h>

int main() {
    int n, i;
    double sum = 0;
    printf("Enter n: ");
    scanf("%d", &n);

    for (i = 1; i <= n; i++)
        sum += pow(i, i);

    printf("Sum = %.0lf\n", sum);

    return 0;
}
```

---

## প্রশ্ন ৫৬ — 2²+4²+8²+...+n² (ভিত্তি ×2 করে বৃদ্ধি)

**Program:** Sum of Squares of Powers of 2 (2²+4²+8²+...)

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `n`, `i`, `sum=0` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: `n` এর মান ইনপুট নাও।
ধাপ ৪: `i=2` থেকে `i <= n` পর্যন্ত `i = i*2` করে লুপ চালাও এবং `sum = sum + i*i` কর।
ধাপ ৫: `sum` প্রদর্শন কর।
ধাপ ৬: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
     ┌───────────┐
     │ Input n   │
     │ sum=0,i=2 │
     └─────┬─────┘
           ▼
      ┌──────────┐  No   ┌────────────┐
      │ i <= n?  ├───────►│ Print sum │
      └────┬─────┘        └────────────┘
           │ Yes
           ▼
    ┌──────────────┐
    │ sum=sum+i*i  │
    │ i=i*2        │
    └──────┬───────┘
           └──► (back to loop)
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int n, sum = 0;
    long long i;
    printf("Enter n: ");
    scanf("%d", &n);

    for (i = 2; i <= n; i *= 2)
        sum += i * i;

    printf("Sum = %d\n", sum);

    return 0;
}
```

---

## প্রশ্ন ৫৭ — 3²+9²+81²+...+n² (ভিত্তি ×3 করে বৃদ্ধি)

**Program:** Sum of Squares of Powers of 3 (3²+9²+27²+81²+...)

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `n`, `i`, `sum=0` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: `n` এর মান ইনপুট নাও।
ধাপ ৪: `i=3` থেকে `i <= n` পর্যন্ত `i = i*3` করে লুপ চালাও এবং `sum = sum + i*i` কর।
ধাপ ৫: `sum` প্রদর্শন কর।
ধাপ ৬: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
     ┌───────────┐
     │ Input n   │
     │ sum=0,i=3 │
     └─────┬─────┘
           ▼
      ┌──────────┐  No   ┌────────────┐
      │ i <= n?  ├───────►│ Print sum │
      └────┬─────┘        └────────────┘
           │ Yes
           ▼
    ┌──────────────┐
    │ sum=sum+i*i  │
    │ i=i*3        │
    └──────┬───────┘
           └──► (back to loop)
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int n, sum = 0;
    long long i;
    printf("Enter n: ");
    scanf("%d", &n);

    for (i = 3; i <= n; i *= 3)
        sum += i * i;

    printf("Sum = %d\n", sum);

    return 0;
}
```

---

## প্রশ্ন ৫৮ — 1³+2³+3³+...+N³ ধারার যোগফল

**Program:** Sum of Cubes 1³+2³+3³+...+N³

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `n`, `i`, `sum=0` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: `n` এর মান ইনপুট নাও।
ধাপ ৪: `i=1` থেকে `n` পর্যন্ত লুপ চালাও এবং `sum = sum + i*i*i` কর।
ধাপ ৫: `sum` প্রদর্শন কর।
ধাপ ৬: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
     ┌───────────┐
     │ Input n   │
     │ sum=0,i=1 │
     └─────┬─────┘
           ▼
      ┌──────────┐  No   ┌────────────┐
      │ i <= n?  ├───────►│ Print sum │
      └────┬─────┘        └────────────┘
           │ Yes
           ▼
   ┌───────────────┐
   │sum=sum+i*i*i  │
   │ i=i+1         │
   └───────┬───────┘
           └──► (back to loop)
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int n, i, sum = 0;
    printf("Enter n: ");
    scanf("%d", &n);

    for (i = 1; i <= n; i++)
        sum += i * i * i;

    printf("Sum = %d\n", sum);

    return 0;
}
```

---

## প্রশ্ন ৫৯ — 1 + 1/2² + 1/3³ + ... + 1/nⁿ

**Program:** Sum of Series 1 + 1/2² + 1/3³ + ... + 1/nⁿ

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `n`, `i` এবং `sum=0.0` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: `n` এর মান ইনপুট নাও।
ধাপ ৪: `i=1` থেকে `n` পর্যন্ত লুপ চালাও এবং `sum = sum + 1/pow(i, i)` কর।
ধাপ ৫: `sum` প্রদর্শন কর।
ধাপ ৬: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
     ┌────────────┐
     │ Input n    │
     │sum=0.0,i=1 │
     └──────┬─────┘
            ▼
      ┌──────────┐  No   ┌────────────┐
      │ i <= n?  ├───────►│ Print sum │
      └────┬─────┘        └────────────┘
           │ Yes
           ▼
  ┌─────────────────────┐
  │sum=sum+1/pow(i, i)  │
  │ i=i+1               │
  └─────────┬───────────┘
            └──► (back to loop)
```

### সি প্রোগ্রাম

```c
#include <stdio.h>
#include <math.h>

int main() {
    int n, i;
    double sum = 0.0;
    printf("Enter n: ");
    scanf("%d", &n);

    for (i = 1; i <= n; i++)
        sum += 1.0 / pow(i, i);

    printf("Sum = %.6lf\n", sum);

    return 0;
}
```

---

## প্রশ্ন ৬১ — 1×2 + 2×3 + 3×4 + ... + N×(N+1)

**Program:** Sum of Series i×(i+1)

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `n`, `i`, `sum=0` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: `n` এর মান ইনপুট নাও।
ধাপ ৪: `i=1` থেকে `n` পর্যন্ত লুপ চালাও এবং `sum = sum + i*(i+1)` কর।
ধাপ ৫: `sum` প্রদর্শন কর।
ধাপ ৬: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
     ┌───────────┐
     │ Input n   │
     │ sum=0,i=1 │
     └─────┬─────┘
           ▼
      ┌──────────┐  No   ┌────────────┐
      │ i <= n?  ├───────►│ Print sum │
      └────┬─────┘        └────────────┘
           │ Yes
           ▼
   ┌────────────────┐
   │sum=sum+i*(i+1) │
   │ i=i+1          │
   └────────┬───────┘
            └──► (back to loop)
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int n, i, sum = 0;
    printf("Enter n: ");
    scanf("%d", &n);

    for (i = 1; i <= n; i++)
        sum += i * (i + 1);

    printf("Sum = %d\n", sum);

    return 0;
}
```

---

---

# Type 4 – Loop + Display

---

## প্রশ্ন ৬২ — ১ থেকে ১০০ এর মধ্যে জোড় ও বিজোড় সংখ্যা প্রদর্শন

**Program:** Display Even and Odd Numbers from 1 to 100

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `i` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: `i=1` থেকে `100` পর্যন্ত লুপ চালাও।
ধাপ ৪: যদি `i % 2 == 0` হয়, তবে "Even" হিসাবে প্রদর্শন কর, অন্যথায় "Odd"।
ধাপ ৫: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
       ┌───────┐
       │ i = 1 │
       └───┬───┘
           ▼
     ┌───────────┐  No   ┌───────┐
     │ i <= 100? ├───────►│  End  │
     └─────┬─────┘        └───────┘
           │ Yes
           ▼
     ┌───────────┐ Yes ┌────────────┐
     │ i%2==0?   ├────►│ Print Even │
     └─────┬─────┘     └────────────┘
           │ No
           ▼
     ┌───────────┐
     │ Print Odd │
     └─────┬─────┘
           │
       ┌───┴───┐
       │ i=i+1 │
       └───┬───┘
           └──► (back to loop)
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int i;

    printf("Even numbers: ");
    for (i = 2; i <= 100; i += 2)
        printf("%d ", i);

    printf("\nOdd numbers: ");
    for (i = 1; i <= 100; i += 2)
        printf("%d ", i);

    printf("\n");

    return 0;
}
```

---

## প্রশ্ন ৬৩ — ১, ২, ৩, ..., n ধারা প্রদর্শন

**Program:** Display Series 1, 2, 3, ..., n

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `n`, `i` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: `n` এর মান ইনপুট নাও।
ধাপ ৪: `i=1` থেকে `n` পর্যন্ত লুপ চালাও এবং `i` প্রদর্শন কর।
ধাপ ৫: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
     ┌───────────┐
     │ Input n   │
     │   i = 1   │
     └─────┬─────┘
           ▼
      ┌──────────┐  No   ┌───────┐
      │ i <= n?  ├───────►│  End  │
      └────┬─────┘        └───────┘
           │ Yes
           ▼
      ┌──────────┐
      │ Print i  │
      │ i = i+1  │
      └────┬─────┘
           └──► (back to loop)
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int n, i;
    printf("Enter n: ");
    scanf("%d", &n);

    for (i = 1; i <= n; i++)
        printf("%d ", i);

    printf("\n");

    return 0;
}
```

---

## প্রশ্ন ৬৪ — যেকোনো সংখ্যার নামতা (Multiplication Table)

**Program:** Print Multiplication Table

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `num`, `i` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: সংখ্যা ইনপুট নাও।
ধাপ ৪: `i=1` থেকে `10` পর্যন্ত লুপ চালাও এবং `num × i` প্রদর্শন কর।
ধাপ ৫: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
     ┌───────────┐
     │ Input num │
     │   i = 1   │
     └─────┬─────┘
           ▼
      ┌──────────┐  No   ┌───────┐
      │ i <= 10? ├───────►│  End  │
      └────┬─────┘        └───────┘
           │ Yes
           ▼
   ┌────────────────┐
   │Print num×i=res │
   │   i = i+1      │
   └────────┬───────┘
            └──► (back to loop)
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int num, i;
    printf("Enter a number: ");
    scanf("%d", &num);

    for (i = 1; i <= 10; i++)
        printf("%d x %d = %d\n", num, i, num * i);

    return 0;
}
```

---

## প্রশ্ন ৭৫ — A হতে Z পর্যন্ত লেটার প্রদর্শন

**Program:** Display Letters A to Z

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `ch` ক্যারেক্টার ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: `ch='A'` থেকে `'Z'` পর্যন্ত লুপ চালাও এবং `ch` প্রদর্শন কর।
ধাপ ৪: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
      ┌──────────┐
      │ ch = 'A' │
      └────┬─────┘
           ▼
      ┌───────────┐  No   ┌───────┐
      │ch <= 'Z'? ├───────►│  End  │
      └─────┬─────┘        └───────┘
            │ Yes
            ▼
      ┌──────────┐
      │ Print ch │
      │ ch = ch+1│
      └────┬─────┘
           └──► (back to loop)
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    char ch;

    for (ch = 'A'; ch <= 'Z'; ch++)
        printf("%c ", ch);

    printf("\n");

    return 0;
}
```

---

---

# Type 5 – Loop + Logic

---

## প্রশ্ন ৪৪ — ল.সা.গু (LCM) নির্ণয়

**Program:** Find LCM of Two Numbers

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `a`, `b`, `lcm` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: দুটি সংখ্যা ইনপুট নাও।
ধাপ ৪: `lcm` = `a` ও `b` এর মধ্যে বড়টি ধরো।
ধাপ ৫: যতক্ষণ `lcm` উভয় সংখ্যা দ্বারা বিভাজ্য না হয়, ততক্ষণ `lcm` ১ করে বাড়াও।
ধাপ ৬: `lcm` প্রদর্শন কর।
ধাপ ৭: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
    ┌─────────────┐
    │ Input a, b  │
    └──────┬──────┘
           ▼
    ┌─────────────────┐
    │lcm = max(a, b)  │
    └────────┬────────┘
             ▼
  ┌──────────────────────┐  No
  │lcm%a==0 && lcm%b==0?├──────┐
  └──────────┬───────────┘      │
             │ Yes              ▼
             ▼           ┌────────────┐
     ┌─────────────┐     │ lcm=lcm+1 │
     │ Print lcm   │     └──────┬─────┘
     └──────┬──────┘            │
            ▼              (back to check)
        ┌───────┐
        │  End  │
        └───────┘
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int a, b, lcm;
    printf("Enter two numbers: ");
    scanf("%d %d", &a, &b);

    lcm = (a > b) ? a : b;

    while (lcm % a != 0 || lcm % b != 0)
        lcm++;

    printf("LCM = %d\n", lcm);

    return 0;
}
```

---

## প্রশ্ন ৪৫ — গ.সা.গু (GCD/HCF) নির্ণয়

**Program:** Find GCD of Two Numbers (Euclidean Algorithm)

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `a`, `b`, `temp` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: দুটি সংখ্যা ইনপুট নাও।
ধাপ ৪: যতক্ষণ `b != 0`, ততক্ষণ `temp = b`, `b = a % b`, `a = temp` কর।
ধাপ ৫: `a` (GCD) প্রদর্শন কর।
ধাপ ৬: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
    ┌─────────────┐
    │ Input a, b  │
    └──────┬──────┘
           ▼
      ┌──────────┐  No   ┌────────────┐
      │ b != 0?  ├───────►│ Print a   │
      └────┬─────┘        │  (GCD)    │
           │ Yes          └─────┬──────┘
           ▼                    ▼
    ┌────────────┐          ┌───────┐
    │ temp = b   │          │  End  │
    │ b = a % b  │          └───────┘
    │ a = temp   │
    └──────┬─────┘
           └──► (back to loop)
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int a, b, temp;
    printf("Enter two numbers: ");
    scanf("%d %d", &a, &b);

    while (b != 0) {
        temp = b;
        b = a % b;
        a = temp;
    }

    printf("GCD = %d\n", a);

    return 0;
}
```

---

## প্রশ্ন ৪৬ — মৌলিক সংখ্যা নির্ণয়

**Program:** Check if a Number is Prime

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `n`, `i`, `flag=0` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: সংখ্যা ইনপুট নাও।
ধাপ ৪: `i=2` থেকে `n/2` পর্যন্ত লুপ চালাও; যদি `n % i == 0` হয়, তবে `flag=1` করে লুপ ভাঙ্গো।
ধাপ ৫: যদি `flag == 0` এবং `n > 1` হয়, তবে "Prime" প্রদর্শন কর, অন্যথায় "Not Prime"।
ধাপ ৬: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
    ┌─────────────┐
    │ Input n     │
    │ flag=0, i=2 │
    └──────┬──────┘
           ▼
     ┌───────────┐  No   ┌─────────────┐
     │ i <= n/2? ├───────►│flag==0&&n>1?│
     └─────┬─────┘        └──┬──────┬──┘
           │ Yes          Yes│      │No
           ▼                 ▼      ▼
     ┌───────────┐    ┌───────┐ ┌───────────┐
     │ n%i==0?   │    │ Prime │ │ Not Prime │
     └──┬────┬───┘    └───┬───┘ └─────┬─────┘
    Yes │    │No           └─────┬─────┘
        ▼    ▼                   ▼
  ┌────────┐┌──────┐         ┌───────┐
  │flag=1  ││i=i+1 │         │  End  │
  │break   │└──┬───┘         └───────┘
  └────────┘   └──► (loop)
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int n, i, flag = 0;
    printf("Enter a number: ");
    scanf("%d", &n);

    for (i = 2; i <= n / 2; i++) {
        if (n % i == 0) {
            flag = 1;
            break;
        }
    }

    if (flag == 0 && n > 1)
        printf("%d is Prime.\n", n);
    else
        printf("%d is not Prime.\n", n);

    return 0;
}
```

---

## প্রশ্ন ৬০ — ফ্যাক্টরিয়াল নির্ণয়

**Program:** Find Factorial of a Number

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `n`, `i`, `fact=1` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: সংখ্যা ইনপুট নাও।
ধাপ ৪: `i=1` থেকে `n` পর্যন্ত লুপ চালাও এবং `fact = fact * i` কর।
ধাপ ৫: `fact` প্রদর্শন কর।
ধাপ ৬: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
     ┌────────────┐
     │ Input n    │
     │ fact=1,i=1 │
     └──────┬─────┘
            ▼
      ┌──────────┐  No   ┌─────────────┐
      │ i <= n?  ├───────►│ Print fact │
      └────┬─────┘        └──────┬──────┘
           │ Yes                 │
           ▼                     ▼
    ┌─────────────┐          ┌───────┐
    │ fact=fact*i  │          │  End  │
    │ i=i+1       │          └───────┘
    └──────┬──────┘
           └──► (back to loop)
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int n, i;
    long long fact = 1;
    printf("Enter a number: ");
    scanf("%d", &n);

    for (i = 1; i <= n; i++)
        fact *= i;

    printf("Factorial = %lld\n", fact);

    return 0;
}
```

---

## প্রশ্ন ৭০ — কোনো সংখ্যার ঘাত নির্ণয়

**Program:** Calculate Power (base^exponent) Using Loop

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `base`, `exp`, `i`, `result=1` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: ভিত্তি ও ঘাত ইনপুট নাও।
ধাপ ৪: `i=1` থেকে `exp` পর্যন্ত লুপ চালাও এবং `result = result * base` কর।
ধাপ ৫: `result` প্রদর্শন কর।
ধাপ ৬: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
        ┌───────┐
        │ Start │
        └───┬───┘
            ▼
  ┌─────────────────┐
  │Input base, exp  │
  │ result=1, i=1   │
  └────────┬────────┘
           ▼
     ┌───────────┐  No   ┌───────────────┐
     │ i <= exp? ├───────►│ Print result │
     └─────┬─────┘        └───────┬───────┘
           │ Yes                  │
           ▼                      ▼
  ┌────────────────┐          ┌───────┐
  │result=result   │          │  End  │
  │       *base    │          └───────┘
  │ i=i+1          │
  └────────┬───────┘
           └──► (back to loop)
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int base, exp, i;
    long long result = 1;
    printf("Enter base and exponent: ");
    scanf("%d %d", &base, &exp);

    for (i = 1; i <= exp; i++)
        result *= base;

    printf("%d^%d = %lld\n", base, exp, result);

    return 0;
}
```

---

## প্রশ্ন ৭১ — ইন্টিজার নম্বর উল্টো করে প্রদর্শন

**Program:** Reverse an Integer Number

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `num`, `rev=0`, `rem` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: সংখ্যা ইনপুট নাও।
ধাপ ৪: যতক্ষণ `num != 0`, ততক্ষণ `rem = num % 10`, `rev = rev * 10 + rem`, `num = num / 10` কর।
ধাপ ৫: `rev` প্রদর্শন কর।
ধাপ ৬: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
    ┌─────────────┐
    │ Input num   │
    │ rev = 0     │
    └──────┬──────┘
           ▼
      ┌──────────┐  No   ┌────────────┐
      │num != 0? ├───────►│ Print rev │
      └────┬─────┘        └─────┬──────┘
           │ Yes                │
           ▼                    ▼
   ┌────────────────┐      ┌───────┐
   │rem = num % 10  │      │  End  │
   │rev=rev*10+rem  │      └───────┘
   │num = num / 10  │
   └────────┬───────┘
            └──► (back to loop)
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int num, rev = 0, rem;
    printf("Enter a number: ");
    scanf("%d", &num);

    while (num != 0) {
        rem = num % 10;
        rev = rev * 10 + rem;
        num /= 10;
    }

    printf("Reversed = %d\n", rev);

    return 0;
}
```

---

## প্রশ্ন ৭৪ — ৪ ডিজিটের সংখ্যা উল্টো ক্রমে সাজানো

**Program:** Reverse a 4-Digit Number

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `num`, `rev=0`, `rem` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: ৪ ডিজিটের সংখ্যা ইনপুট নাও।
ধাপ ৪: যতক্ষণ `num != 0`, ততক্ষণ `rem = num % 10`, `rev = rev * 10 + rem`, `num = num / 10` কর।
ধাপ ৫: `rev` প্রদর্শন কর।
ধাপ ৬: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
  ┌─────────────────┐
  │Input 4-digit num│
  │ rev = 0         │
  └────────┬────────┘
           ▼
      ┌──────────┐  No   ┌────────────┐
      │num != 0? ├───────►│ Print rev │
      └────┬─────┘        └─────┬──────┘
           │ Yes                │
           ▼                    ▼
   ┌────────────────┐      ┌───────┐
   │rem = num % 10  │      │  End  │
   │rev=rev*10+rem  │      └───────┘
   │num = num / 10  │
   └────────┬───────┘
            └──► (back to loop)
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int num, rev = 0, rem;
    printf("Enter a 4-digit number: ");
    scanf("%d", &num);

    while (num != 0) {
        rem = num % 10;
        rev = rev * 10 + rem;
        num /= 10;
    }

    printf("Reversed = %d\n", rev);

    return 0;
}
```

---

## প্রশ্ন ৭৬ — কোনো সংখ্যার পাওয়ার নির্ণয় (pow ব্যবহার করে)

**Program:** Calculate Power Using pow() Function

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `base`, `exp`, `result` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: ভিত্তি ও ঘাত ইনপুট নাও।
ধাপ ৪: `result = pow(base, exp)` নির্ণয় কর।
ধাপ ৫: `result` প্রদর্শন কর।
ধাপ ৬: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
        ┌───────┐
        │ Start │
        └───┬───┘
            ▼
  ┌─────────────────┐
  │Input base, exp  │
  └────────┬────────┘
           ▼
  ┌─────────────────────┐
  │result=pow(base, exp)│
  └────────┬────────────┘
           ▼
  ┌─────────────────┐
  │ Print result    │
  └────────┬────────┘
           ▼
       ┌───────┐
       │  End  │
       └───────┘
```

### সি প্রোগ্রাম

```c
#include <stdio.h>
#include <math.h>

int main() {
    double base, exp, result;
    printf("Enter base and exponent: ");
    scanf("%lf %lf", &base, &exp);

    result = pow(base, exp);

    printf("%.2lf ^ %.2lf = %.2lf\n", base, exp, result);

    return 0;
}
```

---

---

# Type 6 – Array

---

## প্রশ্ন ৬৫ — অ্যারের সংখ্যাগুলোর যোগফল

**Program:** Sum of Array Elements

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `n`, `i`, `sum=0`, `arr[]` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: অ্যারের আকার ও উপাদানগুলো ইনপুট নাও।
ধাপ ৪: `i=0` থেকে `n-1` পর্যন্ত লুপ চালাও এবং `sum = sum + arr[i]` কর।
ধাপ ৫: `sum` প্রদর্শন কর।
ধাপ ৬: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
    ┌──────────────┐
    │ Input n      │
    │ Input arr[]  │
    │ sum=0, i=0   │
    └──────┬───────┘
           ▼
      ┌──────────┐  No   ┌────────────┐
      │ i < n?   ├───────►│ Print sum │
      └────┬─────┘        └─────┬──────┘
           │ Yes                │
           ▼                    ▼
   ┌───────────────┐       ┌───────┐
   │sum=sum+arr[i] │       │  End  │
   │ i=i+1         │       └───────┘
   └───────┬───────┘
           └──► (back to loop)
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int n, i, sum = 0;
    printf("Enter size: ");
    scanf("%d", &n);

    int arr[n];
    printf("Enter elements: ");
    for (i = 0; i < n; i++)
        scanf("%d", &arr[i]);

    for (i = 0; i < n; i++)
        sum += arr[i];

    printf("Sum = %d\n", sum);

    return 0;
}
```

---

## প্রশ্ন ৬৬ — অ্যারের মধ্যে দুটি সংখ্যার বিনিময় (Swap)

**Program:** Swap Two Elements in an Array

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `arr[]`, `n`, `p`, `q`, `temp` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: অ্যারের আকার, উপাদানসমূহ এবং swap-এর দুটি ইনডেক্স ইনপুট নাও।
ধাপ ৪: `temp = arr[p]`, `arr[p] = arr[q]`, `arr[q] = temp` কর।
ধাপ ৫: অ্যারে প্রদর্শন কর।
ধাপ ৬: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
  ┌──────────────────┐
  │ Input n, arr[]   │
  │ Input p, q       │
  └────────┬─────────┘
           ▼
  ┌──────────────────┐
  │ temp = arr[p]    │
  │ arr[p] = arr[q]  │
  │ arr[q] = temp    │
  └────────┬─────────┘
           ▼
  ┌──────────────────┐
  │ Print arr[]      │
  └────────┬─────────┘
           ▼
       ┌───────┐
       │  End  │
       └───────┘
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int n, i, p, q, temp;
    printf("Enter size: ");
    scanf("%d", &n);

    int arr[n];
    printf("Enter elements: ");
    for (i = 0; i < n; i++)
        scanf("%d", &arr[i]);

    printf("Enter two positions to swap (0-indexed): ");
    scanf("%d %d", &p, &q);

    temp = arr[p];
    arr[p] = arr[q];
    arr[q] = temp;

    printf("After swap: ");
    for (i = 0; i < n; i++)
        printf("%d ", arr[i]);
    printf("\n");

    return 0;
}
```

---

## প্রশ্ন ৬৭ — অ্যারেতে সংখ্যা সার্চ (Linear Search)

**Program:** Search an Element in Array (Linear Search)

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `arr[]`, `n`, `key`, `i`, `found=0` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: অ্যারের আকার, উপাদানসমূহ ও খোঁজার সংখ্যা ইনপুট নাও।
ধাপ ৪: `i=0` থেকে `n-1` পর্যন্ত লুপ চালাও; যদি `arr[i] == key` হয়, তবে `found=1`, পজিশন প্রদর্শন কর।
ধাপ ৫: যদি `found == 0` হয়, তবে "Not Found" প্রদর্শন কর।
ধাপ ৬: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
  ┌──────────────────┐
  │Input n, arr[],key│
  │ found=0, i=0     │
  └────────┬─────────┘
           ▼
     ┌──────────┐  No   ┌──────────────┐
     │ i < n?   ├───────►│found==0?    │
     └────┬─────┘        └──┬──────┬───┘
          │ Yes          Yes│      │No
          ▼                 ▼      ▼
    ┌────────────┐   ┌──────────┐ ┌──────┐
    │arr[i]==key?│   │Not Found │ │ Done │
    └──┬─────┬──┘   └──────────┘ └──────┘
   Yes │     │No
       ▼     ▼
  ┌────────┐┌──────┐
  │found=1 ││i=i+1 │
  │Print i │└──┬───┘
  └────────┘   └──► (loop)
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int n, i, key, found = 0;
    printf("Enter size: ");
    scanf("%d", &n);

    int arr[n];
    printf("Enter elements: ");
    for (i = 0; i < n; i++)
        scanf("%d", &arr[i]);

    printf("Enter element to search: ");
    scanf("%d", &key);

    for (i = 0; i < n; i++) {
        if (arr[i] == key) {
            printf("Found at position %d\n", i);
            found = 1;
            break;
        }
    }

    if (!found)
        printf("Not Found.\n");

    return 0;
}
```

---

## প্রশ্ন ৬৮ — অ্যারের সংখ্যাগুলো অদলবদল (Reverse Array)

**Program:** Reverse an Array

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `arr[]`, `n`, `i`, `temp` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: অ্যারের আকার ও উপাদানসমূহ ইনপুট নাও।
ধাপ ৪: `i=0` থেকে `n/2` পর্যন্ত লুপ চালাও এবং `arr[i]` ও `arr[n-1-i]` অদলবদল কর।
ধাপ ৫: অ্যারে প্রদর্শন কর।
ধাপ ৬: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
  ┌────────────────┐
  │Input n, arr[]  │
  │    i = 0       │
  └────────┬───────┘
           ▼
     ┌───────────┐  No   ┌──────────────┐
     │ i < n/2?  ├───────►│ Print arr[] │
     └─────┬─────┘        └──────┬───────┘
           │ Yes                 │
           ▼                     ▼
  ┌──────────────────┐       ┌───────┐
  │swap arr[i] &     │       │  End  │
  │    arr[n-1-i]    │       └───────┘
  │ i=i+1            │
  └────────┬─────────┘
           └──► (back to loop)
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    int n, i, temp;
    printf("Enter size: ");
    scanf("%d", &n);

    int arr[n];
    printf("Enter elements: ");
    for (i = 0; i < n; i++)
        scanf("%d", &arr[i]);

    for (i = 0; i < n / 2; i++) {
        temp = arr[i];
        arr[i] = arr[n - 1 - i];
        arr[n - 1 - i] = temp;
    }

    printf("Reversed: ");
    for (i = 0; i < n; i++)
        printf("%d ", arr[i]);
    printf("\n");

    return 0;
}
```

---

---

# Type 7 – Function

---

## প্রশ্ন ৬৯ — ফাংশনে স্ট্রিংয়ের দৈর্ঘ্য নির্ণয়

**Program:** Find String Length Using a Function

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `str[]`, `length` ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: স্ট্রিং ইনপুট নাও।
ধাপ ৪: `stringLength()` ফাংশন কল করে দৈর্ঘ্য নির্ণয় কর।
ধাপ ৫: ফাংশনে `\0` না পাওয়া পর্যন্ত গণনা চালাও।
ধাপ ৬: দৈর্ঘ্য প্রদর্শন কর।
ধাপ ৭: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
    ┌──────────────┐
    │ Input str[]  │
    └──────┬───────┘
           ▼
   ┌─────────────────┐
   │Call stringLength │
   │    (str)         │
   └────────┬─────────┘
            ▼
     ┌─────────────┐
     │ len=0       │
     └──────┬──────┘
            ▼
     ┌─────────────┐  No   ┌────────────┐
     │str[len]!=\0?├───────►│ Return len│
     └──────┬──────┘        └────────────┘
            │ Yes
            ▼
       ┌──────────┐
       │ len=len+1│
       └────┬─────┘
            └──► (loop)

       ┌────────────────┐
       │ Print length   │
       └───────┬────────┘
               ▼
           ┌───────┐
           │  End  │
           └───────┘
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int stringLength(char str[]) {
    int len = 0;
    while (str[len] != '\0')
        len++;
    return len;
}

int main() {
    char str[100];
    printf("Enter a string: ");
    scanf("%s", str);

    printf("Length = %d\n", stringLength(str));

    return 0;
}
```

---

---

# Type 8 – Character / ASCII

---

## প্রশ্ন ৭২ — বড় হাতের অক্ষরকে ছোট হাতে রূপান্তর

**Program:** Convert Uppercase to Lowercase

### অ্যালগরিদম

ধাপ ১: প্রোগ্রাম শুরু কর।
ধাপ ২: `ch` ক্যারেক্টার ভেরিয়েবল ঘোষণা কর।
ধাপ ৩: বড় হাতের অক্ষর ইনপুট নাও।
ধাপ ৪: `ch = ch + 32` করে ছোট হাতে রূপান্তর কর।
ধাপ ৫: রূপান্তরিত অক্ষর প্রদর্শন কর।
ধাপ ৬: প্রোগ্রাম শেষ কর।

### ফ্লোচার্ট

```
       ┌───────┐
       │ Start │
       └───┬───┘
           ▼
     ┌───────────┐
     │ Input ch  │
     └─────┬─────┘
           ▼
     ┌────────────┐
     │ ch = ch+32 │
     └──────┬─────┘
            ▼
     ┌────────────┐
     │ Print ch   │
     └──────┬─────┘
            ▼
        ┌───────┐
        │  End  │
        └───────┘
```

### সি প্রোগ্রাম

```c
#include <stdio.h>

int main() {
    char ch;
    printf("Enter an uppercase letter: ");
    scanf("%c", &ch);

    if (ch >= 'A' && ch <= 'Z')
        ch = ch + 32;

    printf("Lowercase: %c\n", ch);

    return 0;
}
```

---

---

<div align="center">

## 📊 Quick Reference Table

| # | Program | Type | Key Construct |
|:---:|:---|:---:|:---|
| ৩৮ | Voter Eligibility | 2 | `if (age >= 18)` |
| ৩৯ | Positive / Negative / Zero | 2 | `if-else if-else` |
| ৪০ | Zero / Even / Odd | 2 | `num % 2` |
| ৪১ | Largest of Three | 2 | `if-else if-else` |
| ৪২ | Smallest of Three | 2 | `if-else if-else` |
| ৪৩ | Leap Year | 2 | `% 400, % 100, % 4` |
| ৪৪ | LCM | 5 | `while` loop |
| ৪৫ | GCD | 5 | Euclidean `while` |
| ৪৬ | Prime Check | 5 | `for` + flag |
| ৪৭ | Sum 1+2+...+n | 3 | `for` + `sum` |
| ৪৮ | Sum of Odds | 3 | `i += 2` |
| ৪৯ | Sum of Evens | 3 | `i += 2` |
| ৫০ | Sum of Squares | 3 | `i * i` |
| ৫১ | 100²+95²+...+10² | 3 | `i -= 5` |
| ৫২ | 99²+88²+...+11² | 3 | `i -= 11` |
| ৫৩ | 1000+950+...+≥22 | 3 | `i -= 50` |
| ৫৪ | i×(i+1) series | 3 | `i*(i+1)` |
| ৫৫ | i^i series | 3 | `pow(i, i)` |
| ৫৬ | 2²+4²+8²+... | 3 | `i *= 2` |
| ৫৭ | 3²+9²+27²+... | 3 | `i *= 3` |
| ৫৮ | Sum of Cubes | 3 | `i*i*i` |
| ৫৯ | 1+1/2²+1/3³+... | 3 | `1.0/pow(i,i)` |
| ৬০ | Factorial | 5 | `fact *= i` |
| ৬১ | i×(i+1) series | 3 | `i*(i+1)` |
| ৬২ | Even/Odd 1–100 | 4 | two `for` loops |
| ৬৩ | Display 1 to n | 4 | `for` print |
| ৬৪ | Multiplication Table | 4 | `num * i` |
| ৬৫ | Array Sum | 6 | `arr[]` + `for` |
| ৬৬ | Array Swap | 6 | `temp` swap |
| ৬৭ | Array Search | 6 | Linear search |
| ৬৮ | Reverse Array | 6 | two-pointer swap |
| ৬৯ | String Length (func) | 7 | custom function |
| ৭০ | Power (loop) | 5 | `result *= base` |
| ৭১ | Reverse Integer | 5 | `% 10`, `/ 10` |
| ৭২ | Upper → Lower | 8 | `ch + 32` |
| ৭৩ | Quadratic Equation | 1 | `sqrt`, discriminant |
| ৭৪ | Reverse 4-digit | 5 | `% 10`, `/ 10` |
| ৭৫ | A to Z | 4 | `char` loop |
| ৭৬ | Power (pow) | 5 | `pow()` |
| ৭৭ | Grade from Marks | 2 | `if-else if` chain |
| ৭ৈ | Fraction Addition | 1 | cross-multiply |

---

### 🛠️ Compilation Note

All programs use **C99 standard**. Compile with:

```bash
gcc -std=c99 -lm program.c -o program
```

---

*Generated for Diploma / HSC / University C Programming Examination Preparation*

</div>
]]>
