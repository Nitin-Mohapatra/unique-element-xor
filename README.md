# 🧮 Single Number (Python)

This repository contains an efficient Python implementation to solve the classic **Single Number** problem using **bitwise XOR**.

---

## 📘 Problem Statement

Given a **non-empty array** of integers, where every element appears **twice** except for one, find the element that appears **only once**.

### Constraints:
- You must implement a solution with **linear runtime complexity**.
- You must use **constant extra memory**.

---

## 🧠 Approach

This solution uses the **bitwise XOR (`^`)** operator:

- `a ^ a = 0` → any number XORed with itself is 0  
- `a ^ 0 = a` → any number XORed with 0 remains the same  

By XORing all elements in the array, all duplicates cancel each other out, and only the unique number remains.

---

## ⚠️ Limitation

This approach **only works** when **each element appears exactly twice except for one**.  

It **will not work** if elements appear **three times** or more.  
For example:
```python
[2, 2, 2, 3]  # XOR result is not 3
```
Because
2 ^ 2 ^ 2 = 2 (not 0)

