# 🔑 Mastering Hashing (Maps & Sets) in C++

**Hashing** is a technique used to **store, retrieve, and manage data efficiently** by using **hash functions**.

This guide covers the **fundamentals of hashing**, focusing on **maps and sets**, essential for **beginner** and **intermediate** competitive programming problems.

---

## 🔹 **1. What is Hashing?**

Hashing is a **data indexing technique** where a **key is mapped to a value** using a **hash function**.

It is commonly used for:  
✅ **Fast Lookups** (O(1) on average)  
✅ **Avoiding Duplicates**  
✅ **Efficient Data Storage**  

### **Types of Hashing Data Structures in C++**  
📌 `unordered_map` - Key-Value Pair with O(1) Average Lookup Time  
📌 `map` - Key-Value Pair with Ordered Keys (O(log N) Lookup Time)  
📌 `unordered_set` - Stores Unique Elements, No Order  
📌 `set` - Stores Unique Elements, Sorted Order  

---

## 🔹 **2. Unordered Map (O(1) Average Time Complexity)**
An **unordered_map** is a **hash table-based associative container** that stores **key-value pairs**.

✅ **When to use?**  
- When **fast retrieval** is needed  
- When **order of keys doesn’t matter**  

### ✅ **C++ Implementation:**
```cpp
#include <iostream>
#include <unordered_map>
using namespace std;

int main() {
    unordered_map<string, int> age;
    age["Alice"] = 25;
    age["Bob"] = 30;

    cout << "Alice's Age: " << age["Alice"] << endl;

    return 0;
}
```

---

## 🔹 **3. Ordered Map (O(log N))**
A **map** stores **key-value pairs** but keeps keys **sorted** using a **balanced BST**.

✅ **When to use?**  
- When you **need sorted keys**  
- When **logarithmic time complexity** is acceptable  

### ✅ **C++ Implementation:**
```cpp
#include <iostream>
#include <map>
using namespace std;

int main() {
    map<int, string> students;
    students[2] = "Alice";
    students[1] = "Bob";
    students[3] = "Charlie";

    for (auto it : students) cout << it.first << ": " << it.second << endl;

    return 0;
}
```

---

## 🔹 **4. Unordered Set (O(1) Average Time Complexity)**
An **unordered_set** stores **unique elements** in **random order**.

✅ **When to use?**  
- When **duplicates need to be avoided**  
- When **ordering doesn’t matter**  

### ✅ **C++ Implementation:**
```cpp
#include <iostream>
#include <unordered_set>
using namespace std;

int main() {
    unordered_set<int> numbers = {1, 2, 3, 4, 5};
    numbers.insert(3);  // Duplicate ignored

    for (int num : numbers) cout << num << " ";

    return 0;
}
```

---

## 🔹 **5. Ordered Set (O(log N))**
A **set** stores **unique elements** in **sorted order**.

✅ **When to use?**  
- When **sorted elements are needed**  
- When **logarithmic operations are acceptable**  

### ✅ **C++ Implementation:**
```cpp
#include <iostream>
#include <set>
using namespace std;

int main() {
    set<int> sortedNumbers = {5, 1, 4, 2, 3};
    sortedNumbers.insert(3); // Duplicate ignored

    for (int num : sortedNumbers) cout << num << " ";

    return 0;
}
```

---

## 🔹 **6. Additional Learning Resources**

📘 **Documentation:**  
- [C++ Unordered Map & Set (cplusplus.com)](https://www.cplusplus.com/reference/unordered_map/)  
- [GeeksforGeeks - Hashing in C++](https://www.geeksforgeeks.org/hashing-data-structure/)  

📺 **Tutorial Video:**  
- [YouTube: Hashing Explained](https://www.youtube.com/watch?v=rvdJDijO2Ro)  

---

🚀 **Mastering hashing will make your coding journey much easier in competitive programming!** 🚀  
