# Date Difference in Days Calculator in C++ 📅⚡

A clean, modular C++ implementation designed to accurately calculate the difference in days between two calendar dates (`Date1` and `Date2`). The project demonstrates structural programming principles, custom type encapsulation (`stDate`), and precise boundary arithmetic.

---

## 🌟 Key Features
- **Inclusive & Exclusive Ranges:** Configurable parameter `IncludeEndDay` allowing calculation with or without the endpoint date.
- **Modular Architecture:** Relies on dedicated helper functions (`isLeapYear`, `NumberOfDaysInAMonth`, `isLastDayInMonth`, `IncreaseDateByOneDay`, and `IsDate1BeforeDate2`).
- **Edge Case Resilient:** Seamlessly transitions across irregular month bounds, leap-year Februaries, and multi-year spans.

---

## 💡 How It Works
The algorithm uses an iterative progression model:
1. Evaluates chronological ordering using `IsDate1BeforeDate2`.
2. Advances `Date1` incrementally using `IncreaseDateByOneDay` until matching `Date2`.
3. Keeps an internal counter `Days++` for each step.
4. Optionally appends the final day if `IncludeEndDay` is flagged as `true`.

---

## 💻 Sample Output
```text
Please enter a Day? 1
Please enter a Month? 1
Please enter a Year? 2022

Please enter a Day? 25
Please enter a Month? 3
Please enter a Year? 2022

Diffrence is: 83 Day(s).
Diffrence (Including End Day) is: 84 Day(s).
