# 🔢 Arrays 

<p align="center">
  <img src="https://img.shields.io/badge/Data%20Structure-Arrays-blue" alt="Arrays Badge"/>
  <img src="https://img.shields.io/badge/Language-Python-green?logo=python" alt="Python Badge"/>
</p>



## 📌 Introduction
Arrays (or **lists** in Python) hold values of the same type in **contiguous memory locations**.  
For interviews, they are **fundamental** — even problems from other topics often involve arrays.

- In Python, arrays are **dynamic lists** — no need to predefine size.  
- Two things matter most: **index** (position) and **element** (value).  
- Mastery of arrays is essential for coding interviews.

---

## ✅ Advantages
- Store multiple elements of the same type with **one variable**.  
- **Fast access** if you know the index (`O(1)` lookup).  

## ❌ Disadvantages
- **Insertion/Deletion in the middle** is slow (`O(n)`), since elements must be shifted.  
- Fixed-size arrays (in some languages) need costly **resizing & copying** (`O(n)`).  

---

## 📚 Common Terms
- **Subarray**: contiguous part of the array  
  - Example: `[3, 6, 1]` is a subarray of `[2, 3, 6, 1, 5, 4]`.  
- **Subsequence**: can delete elements without changing order  
  - Example: `[3, 1, 5]` is a subsequence of `[2, 3, 6, 1, 5, 4]`.  

---

## ⏱️ Time Complexity

| Operation                  | Big-O    | Notes |
|-----------------------------|----------|-------|
| Access                      | O(1)     | Direct index lookup |
| Search (unsorted)           | O(n)     | Linear scan |
| Search (sorted)             | O(log n) | Binary search |
| Insert (middle)             | O(n)     | Shifting required |
| Insert (end)                | O(1)     | Amortized |
| Remove (middle)             | O(n)     | Shifting required |
| Remove (end)                | O(1)     | Amortized |

---

## ⚠️ Interview Tips
- Clarify if **duplicates** are allowed.  
- Watch out for **index out-of-bounds**.  
- Be mindful of **array slicing/concatenation** — they take `O(n)`.  
- Prefer **start/end indices** over copying subarrays when possible.  

---

## 🧩 Corner Cases
- Empty array `[]`  
- Single-element `[x]`  
- Two elements `[x, y]`  
- Repeated values `[1, 1, 1, 1]`  
- Mixed duplicates `[1, 2, 2, 3]`  

---

## 🛠️ Techniques

Here I’ll apply classic array problem-solving strategies in Python.  
Each technique links to a **notebook with examples & practice problems**.

- [Sliding Window](./techniques/sliding_window.ipynb)  
  Efficient for subarray/substring problems.  
  ✅ Examples: *Longest Substring Without Repeating Characters, Minimum Size Subarray Sum*  

- [Two Pointers](./techniques/two_pointers.ipynb)  
  Generalized approach, can work across arrays.  
  ✅ Examples: *Merge Sorted Array, Sort Colors, Palindromic Substrings*  

- [Traversing from the Right](./techniques/traverse_right.ipynb)  
  Useful when right-to-left information is required.  
  ✅ Examples: *Daily Temperatures, Number of Visible People in a Queue*  

- [Sorting the Array](./techniques/sorting.ipynb)  
  Sorting can simplify problems & enable binary search.  
  ✅ Examples: *Merge Intervals, Non-overlapping Intervals*  

- [Precomputation (Prefix/Suffix)](./techniques/precomputation.ipynb)  
  Store cumulative sums/products for faster queries.  
  ✅ Examples: *Product of Array Except Self, Prefix Sum problems*  

- [Index as Hash Key](./techniques/index_as_hash.ipynb)  
  Use array indices as hash to track presence.  
  ✅ Examples: *First Missing Positive*  

- [Multiple Traversals](./techniques/multiple_traversals.ipynb)  
  Traversing 2–3 times is still `O(n)` and often cleaner.  
  ✅ Examples: *Problems requiring separate passes*  

---

## 📚 References  
- **[Tech Interview Handbook: Arrays](https://www.techinterviewhandbook.org/algorithms/array)**  

