# 🔍 Mastering Searching Algorithms in C++

Searching is a fundamental concept in programming where we **locate an element** in a data structure. It is a crucial skill for **competitive programming** and real-world applications.

This guide covers essential **searching algorithms** you need to solve **beginner** problems and smoothly transition into **intermediate** problems.

---

## 🔹 **1. What is Searching?**

Searching refers to the process of finding an element in an **array, list, or dataset**.  
There are two main types of searching techniques:

1️⃣ **Linear Search** (Brute Force, O(n))  
2️⃣ **Binary Search** (Optimized, O(log n), works only on sorted arrays)

---

## 🔹 **2. Linear Search (O(n))**

Linear search checks **each element** one by one until the target element is found or the array ends.

✅ **When to use?**

- When the data is **unsorted** or **small**
- When there are **duplicates** in the dataset

### ✅ **C++ Implementation:**

```cpp
#include <iostream>
using namespace std;

int linearSearch(int arr[], int n, int key) {
    for (int i = 0; i < n; i++) {
        if (arr[i] == key) return i;  // Return index if found
    }
    return -1;  // Element not found
}

int main() {
    int arr[] = {10, 20, 30, 40, 50};
    int n = sizeof(arr) / sizeof(arr[0]);
    int key = 30;

    int index = linearSearch(arr, n, key);
    if (index != -1) cout << "Element found at index: " << index;
    else cout << "Element not found";

    return 0;
}
```

---

## 🔹 **3. Binary Search (O(log n))**

Binary search **divides** the sorted array into halves and checks the middle element to locate the target.

✅ **When to use?**

- When the data is **sorted**
- When **fast searching** is needed (logarithmic time complexity)

### ✅ **C++ Implementation (Iterative):**

```cpp
#include <iostream>
using namespace std;

int binarySearch(int arr[], int left, int right, int key) {
    while (left <= right) {
        int mid = left + (right - left) / 2;

        if (arr[mid] == key) return mid;
        else if (arr[mid] < key) left = mid + 1;
        else right = mid - 1;
    }
    return -1;
}

int main() {
    int arr[] = {10, 20, 30, 40, 50};
    int n = sizeof(arr) / sizeof(arr[0]);
    int key = 30;

    int index = binarySearch(arr, 0, n - 1, key);
    if (index != -1) cout << "Element found at index: " << index;
    else cout << "Element not found";

    return 0;
}
```

### ✅ **C++ Implementation (Recursive):**

```cpp
#include <iostream>
using namespace std;

int binarySearchRecursive(int arr[], int left, int right, int key) {
    if (left > right) return -1;

    int mid = left + (right - left) / 2;

    if (arr[mid] == key) return mid;
    else if (arr[mid] < key) return binarySearchRecursive(arr, mid + 1, right, key);
    else return binarySearchRecursive(arr, left, mid - 1, key);
}

int main() {
    int arr[] = {10, 20, 30, 40, 50};
    int n = sizeof(arr) / sizeof(arr[0]);
    int key = 30;

    int index = binarySearchRecursive(arr, 0, n - 1, key);
    if (index != -1) cout << "Element found at index: " << index;
    else cout << "Element not found";

    return 0;
}
```

---

## 🔹 **4. Ternary Search (O(log n))**

Ternary search is an extension of binary search that divides the array into **three parts** instead of two.  
✅ **When to use?**

- When the dataset is **sorted**
- When **binary search is applicable**, but optimization is needed

### ✅ **C++ Implementation:**

```cpp
#include <iostream>
using namespace std;

int ternarySearch(int arr[], int left, int right, int key) {
    while (left <= right) {
        int mid1 = left + (right - left) / 3;
        int mid2 = right - (right - left) / 3;

        if (arr[mid1] == key) return mid1;
        if (arr[mid2] == key) return mid2;

        if (key < arr[mid1]) right = mid1 - 1;
        else if (key > arr[mid2]) left = mid2 + 1;
        else {
            left = mid1 + 1;
            right = mid2 - 1;
        }
    }
    return -1;
}

int main() {
    int arr[] = {10, 20, 30, 40, 50};
    int n = sizeof(arr) / sizeof(arr[0]);
    int key = 30;

    int index = ternarySearch(arr, 0, n - 1, key);
    if (index != -1) cout << "Element found at index: " << index;
    else cout << "Element not found";

    return 0;
}
```

---

## 🔹 **5. Comparison of Searching Algorithms**

| Algorithm          | Time Complexity (Best) | Time Complexity (Worst) | When to Use                     |
| ------------------ | ---------------------- | ----------------------- | ------------------------------- |
| **Linear Search**  | O(1)                   | O(n)                    | Unsorted or small data          |
| **Binary Search**  | O(1)                   | O(log n)                | Sorted data                     |
| **Ternary Search** | O(1)                   | O(log n)                | Optimization over Binary Search |

---

## 🔹 **6. Practice Problems**

Solve these problems to strengthen your search algorithm skills:

1️⃣ Find an element in an **unsorted array** (Linear Search)  
2️⃣ Find an element in a **sorted array** (Binary Search)  
3️⃣ Find the **first and last occurrence** of a number  
4️⃣ Count the **number of occurrences** of an element  
5️⃣ Find the **square root** of a number using Binary Search

---

## 🔹 **7. Additional Learning Resources**

📘 **Documentation:**

- [C++ Searching Documentation (cplusplus.com)](https://www.cplusplus.com/reference/algorithm/binary_search/)
- [GeeksforGeeks - Searching Algorithms](https://www.geeksforgeeks.org/searching-algorithms/)

📺 **Tutorial Video:**

- [YouTube: Searching Algorithms Explained](https://www.youtube.com/watch?v=_HRA37X8N_Q)

---

🚀 **Master these searching techniques and level up your competitive programming skills!**
