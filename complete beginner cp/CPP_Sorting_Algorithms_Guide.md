# 🔄 Mastering Sorting Algorithms in C++

Sorting is one of the most fundamental concepts in programming. It is used to **arrange elements in a specific order (ascending/descending).**

This guide covers essential **sorting algorithms** you need to solve **beginner** problems and smoothly transition into **intermediate** problems.

---

## 🔹 **1. What is Sorting?**
Sorting is the process of **arranging elements in increasing or decreasing order**.  
It is a key concept in **searching, optimization, and competitive programming**.

There are two major types of sorting algorithms:

1️⃣ **Comparison-Based Sorting:** (Bubble Sort, Selection Sort, Merge Sort, etc.)  
2️⃣ **Non-Comparison-Based Sorting:** (Counting Sort, Radix Sort, etc.)  

---

## 🔹 **2. Bubble Sort (O(n²))**
Bubble Sort repeatedly swaps adjacent elements if they are in the wrong order.

✅ **When to use?**  
- When the **array size is small**  
- When the **data is nearly sorted**  

### ✅ **C++ Implementation:**
```cpp
#include <iostream>
using namespace std;

void bubbleSort(int arr[], int n) {
    for (int i = 0; i < n - 1; i++) {
        for (int j = 0; j < n - i - 1; j++) {
            if (arr[j] > arr[j + 1]) swap(arr[j], arr[j + 1]);
        }
    }
}

int main() {
    int arr[] = {5, 1, 4, 2, 8};
    int n = sizeof(arr) / sizeof(arr[0]);

    bubbleSort(arr, n);

    for (int i = 0; i < n; i++) cout << arr[i] << " ";
    return 0;
}
```

---

## 🔹 **3. Selection Sort (O(n²))**
Selection Sort selects the smallest element and swaps it with the first element.

✅ **When to use?**  
- When the **array size is small**  
- When you want **in-place sorting** with fewer swaps  

### ✅ **C++ Implementation:**
```cpp
#include <iostream>
using namespace std;

void selectionSort(int arr[], int n) {
    for (int i = 0; i < n - 1; i++) {
        int minIdx = i;
        for (int j = i + 1; j < n; j++) {
            if (arr[j] < arr[minIdx]) minIdx = j;
        }
        swap(arr[i], arr[minIdx]);
    }
}

int main() {
    int arr[] = {64, 25, 12, 22, 11};
    int n = sizeof(arr) / sizeof(arr[0]);

    selectionSort(arr, n);

    for (int i = 0; i < n; i++) cout << arr[i] << " ";
    return 0;
}
```

---

## 🔹 **4. Insertion Sort (O(n²))**
Insertion Sort builds a sorted list by inserting elements at their correct positions.

✅ **When to use?**  
- When the **array is nearly sorted**  
- When sorting **small datasets**  

### ✅ **C++ Implementation:**
```cpp
#include <iostream>
using namespace std;

void insertionSort(int arr[], int n) {
    for (int i = 1; i < n; i++) {
        int key = arr[i];
        int j = i - 1;
        while (j >= 0 && arr[j] > key) {
            arr[j + 1] = arr[j];
            j--;
        }
        arr[j + 1] = key;
    }
}

int main() {
    int arr[] = {12, 11, 13, 5, 6};
    int n = sizeof(arr) / sizeof(arr[0]);

    insertionSort(arr, n);

    for (int i = 0; i < n; i++) cout << arr[i] << " ";
    return 0;
}
```

---

## 🔹 **5. Merge Sort (O(n log n))**
Merge Sort is a **divide-and-conquer** algorithm that splits the array and merges sorted parts.

✅ **When to use?**  
- When sorting **large datasets**  
- When **stable sorting** is required  

### ✅ **C++ Implementation:**
```cpp
#include <iostream>
using namespace std;

void merge(int arr[], int left, int mid, int right) {
    int n1 = mid - left + 1, n2 = right - mid;
    int L[n1], R[n2];

    for (int i = 0; i < n1; i++) L[i] = arr[left + i];
    for (int i = 0; i < n2; i++) R[i] = arr[mid + 1 + i];

    int i = 0, j = 0, k = left;
    while (i < n1 && j < n2) arr[k++] = (L[i] <= R[j]) ? L[i++] : R[j++];
    while (i < n1) arr[k++] = L[i++];
    while (j < n2) arr[k++] = R[j++];
}

void mergeSort(int arr[], int left, int right) {
    if (left < right) {
        int mid = left + (right - left) / 2;
        mergeSort(arr, left, mid);
        mergeSort(arr, mid + 1, right);
        merge(arr, left, mid, right);
    }
}

int main() {
    int arr[] = {38, 27, 43, 3, 9, 82, 10};
    int n = sizeof(arr) / sizeof(arr[0]);

    mergeSort(arr, 0, n - 1);

    for (int i = 0; i < n; i++) cout << arr[i] << " ";
    return 0;
}
```

---

## 🔹 **6. Additional Learning Resources**

📘 **Documentation:**  
- [C++ Sorting Documentation (cplusplus.com)](https://www.cplusplus.com/reference/algorithm/sort/)  
- [GeeksforGeeks - Sorting Algorithms](https://www.geeksforgeeks.org/sorting-algorithms/)  

📺 **Tutorial Video:**  
- [YouTube: Sorting Algorithms Explained](https://www.youtube.com/watch?v=ZZuD6iUe3Pc)  

---

🚀 **Master these sorting techniques and level up your competitive programming skills!** 🚀  
