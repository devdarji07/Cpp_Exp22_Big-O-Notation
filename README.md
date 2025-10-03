# Cpp_Exp22_Big-O-Notation

# 📘 Report: Big-O Notation

---

## 🧾 Introduction
Algorithms are step-by-step procedures to solve problems.  
Algorithm analysis evaluates their efficiency in terms of:

- **Time Complexity:** How fast an algorithm runs.  
- **Space Complexity:** How much memory it uses.  

**Big O notation** is the standard way to express these complexities.

---

## 📌 Importance of Algorithm Analysis
- Predict performance for large input sizes.  
- Compare algorithms to choose the best.  
- Identify bottlenecks in programs.  
- Ensure scalability for real-world data.  

**Analogy:** Like planning a road trip, algorithm analysis tells you if your route will take 10 minutes or 10 hours as traffic increases.

---

## 🔑 Key Types of Analysis

| Type            | Description                        | Example                                |
|-----------------|------------------------------------|----------------------------------------|
| Time Complexity | Measures running time               | Sorting a list of 1000 numbers         |
| Space Complexity| Measures extra memory used          | Storing intermediate results in recursion |
| Worst-case      | Maximum time for any input          | Searching last element in an array     |
| Best-case       | Minimum time for any input          | Searching first element in an array    |
| Average-case    | Expected time for random input      | Searching random element in array      |

---

## 📏 Big O Notation
- Describes growth rate of an algorithm.  
- Ignores constants and lower-order terms.  

**Formal Definition:**  
f(n) = O(g(n)) means that for large n, f(n) grows at most like g(n) up to a constant factor.

---

## ⏱ Common Big O Complexities

| Complexity | Name        | Example           | Description |
|-----------|------------|-----------------|-------------|
| O(1)      | Constant    | Access array[0]  | Time does not change with input size |
| O(log n)  | Logarithmic | Binary Search    | Reduces problem by half each step |
| O(n)      | Linear      | Linear Search    | Time grows directly with input size |
| O(n log n)| Linearithmic| Merge Sort       | Efficient for large data |
| O(n²)     | Quadratic   | Bubble Sort      | Nested loops over input |
| O(n³)     | Cubic       | Matrix multiplication | Triple nested loops |
| O(2^n)    | Exponential | Recursive Fibonacci | Doubles with each input increment |
| O(n!)     | Factorial   | Brute-force TSP  | Extremely slow for large n |

---

## 📌 Real-Life Analogies

| Complexity | Analogy |
|-----------|---------|
| O(1)     | Picking one book from a shelf |
| O(log n) | Guessing a number in a 1–100 game using yes/no questions |
| O(n)     | Checking each book on a shelf one by one |
| O(n log n)| Sorting books efficiently using a smart method |
| O(n²)    | Comparing every book with every other book |
| O(2^n)   | Flipping all possible combinations of a light switch sequence |
| O(n!)    | Trying every seating arrangement at a dinner party |

---

## 📝 Examples of Algorithms

**O(1) – Constant**
```cpp
int getFirstElement(int arr[], int n) { 
    return arr[0]; 
}
