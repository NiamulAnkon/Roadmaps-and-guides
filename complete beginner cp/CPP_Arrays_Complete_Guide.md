# 📌 Mastering Arrays in C++ for Competitive Programming

Arrays are one of the **most important** topics in **Competitive Programming (CP)**. They allow storing multiple values in a **contiguous memory location** and are fundamental for **efficient algorithms**.

This guide will cover **everything** you need to learn about arrays to solve **beginner** problems and smoothly transition into **intermediate** problems.

---

## 🔹 **1. What is an Array in C++?**
An **array** is a collection of elements stored **sequentially** in memory. Elements are of the **same data type** and are accessed using **indexing**.

✅ **Example:**  
```cpp
#include <iostream>
using namespace std;

int main() {
    int arr[5] = {10, 20, 30, 40, 50};
    cout << arr[0];  // Output: 10
    return 0;
}
```

---

## 🔹 **2. Declaring and Using Arrays**

### ✅ **2.1. Declaring Arrays**
```cpp
int arr[5];  // Uninitialized array of size 5
int arr2[5] = {1, 2, 3, 4, 5};  // Initialized array
int arr3[] = {10, 20, 30};  // Compiler determines the size
```

### ✅ **2.2. Accessing Elements**
Array elements are accessed using **indexing (0-based)**.

```cpp
#include <iostream>
using namespace std;

int main() {
    int arr[] = {10, 20, 30, 40};
    cout << arr[1];  // Output: 20
    return 0;
}
```

### ✅ **2.3. Modifying Elements**
```cpp
arr[2] = 99;  // Change value at index 2
```

---

## 🔹 **3. Traversing an Array**

### ✅ **3.1. Using a For Loop**
```cpp
#include <iostream>
using namespace std;

int main() {
    int arr[] = {1, 2, 3, 4, 5};
    int n = sizeof(arr) / sizeof(arr[0]);  // Get size of array

    for (int i = 0; i < n; i++) {
        cout << arr[i] << " ";  
    }
    return 0;
}
```

### ✅ **3.2. Using a Range-Based For Loop (C++11 and later)**
```cpp
#include <iostream>
using namespace std;

int main() {
    int arr[] = {1, 2, 3, 4, 5};
    for (int num : arr) {
        cout << num << " ";  // Output: 1 2 3 4 5
    }
    return 0;
}
```

---

## 🔹 **4. Common Array Operations**

| Operation | Description | Example |
|-----------|-------------|----------|
| `sizeof(arr)/sizeof(arr[0])` | Get the number of elements | `sizeof(arr) / sizeof(arr[0]) → 5` |
| `arr[i]` | Access element at index `i` | `arr[2] → 30` |
| `sort(arr, arr+n)` | Sort array in ascending order | `[3,1,2] → [1,2,3]` |
| `reverse(arr, arr+n)` | Reverse array elements | `[1,2,3] → [3,2,1]` |

---

## 🔹 **5. Searching Algorithms in Arrays**

### ✅ **5.1. Linear Search (O(n))**
```cpp
#include <iostream>
using namespace std;

int linearSearch(int arr[], int n, int key) {
    for (int i = 0; i < n; i++) {
        if (arr[i] == key) return i;
    }
    return -1;
}

int main() {
    int arr[] = {10, 20, 30, 40, 50};
    int n = sizeof(arr) / sizeof(arr[0]);
    int key = 30;
    int index = linearSearch(arr, n, key);
    cout << "Element found at index: " << index;  // Output: 2
    return 0;
}
```

### ✅ **5.2. Binary Search (O(log n)) [Array must be sorted]**
```cpp
#include <iostream>
#include <algorithm>
using namespace std;

int main() {
    int arr[] = {10, 20, 30, 40, 50};
    int n = sizeof(arr) / sizeof(arr[0]);
    int key = 30;

    if (binary_search(arr, arr + n, key)) {
        cout << "Element found";
    } else {
        cout << "Element not found";
    }

    return 0;
}
```

---

## 🔹 **6. Sorting Algorithms for Arrays**

### ✅ **6.1. Sorting an Array in Ascending Order**
```cpp
#include <iostream>
#include <algorithm>
using namespace std;

int main() {
    int arr[] = {5, 2, 8, 1, 3};
    int n = sizeof(arr) / sizeof(arr[0]);
    
    sort(arr, arr + n);
    
    for (int i : arr) cout << i << " ";  // Output: 1 2 3 5 8
    return 0;
}
```

### ✅ **6.2. Reversing an Array**
```cpp
#include <iostream>
#include <algorithm>
using namespace std;

int main() {
    int arr[] = {1, 2, 3, 4, 5};
    int n = sizeof(arr) / sizeof(arr[0]);

    reverse(arr, arr + n);

    for (int i : arr) cout << i << " ";  // Output: 5 4 3 2 1
    return 0;
}
```

---

## 🔹 **7. Practice Problems**  
Here are some beginner problems to practice:

1️⃣ Find the **maximum and minimum** in an array  
2️⃣ Reverse an array  
3️⃣ Find the **sum of elements** in an array  
4️⃣ Find the **second largest element**  
5️⃣ Count occurrences of an element in an array  

Practice on **LeetCode**, **Codeforces**, and **AtCoder**.

---

## 🔹 **8. Additional Learning Resources**

📘 **Documentation:**  
- [C++ Arrays Documentation (cplusplus.com)](https://www.cplusplus.com/doc/tutorial/arrays/)  
- [GeeksforGeeks - C++ Arrays](https://www.geeksforgeeks.org/arrays-in-c-cpp/)  

📺 **Tutorial Video:**  
- [YouTube: C++ Arrays Full Tutorial](https://www.youtube.com/watch?v=w3b9c3j_pdg)  

---

🚀 **Keep Practicing & Level Up!** 🚀  
