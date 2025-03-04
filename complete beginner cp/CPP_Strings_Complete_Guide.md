# 📌 Mastering Strings in C++ for Competitive Programming

Strings are one of the **most essential** topics in **Competitive Programming (CP)**. They allow efficient **text processing**, searching, and manipulation. Mastering strings will help you solve **beginner** problems and transition smoothly into **intermediate** problems.

---

## 🔹 **1. What is a String in C++?**
A **string** in C++ is a sequence of characters. C++ provides two types of strings:
1. **C-style Strings (`char[]`)** - Old, character array-based strings.
2. **`std::string` (C++ STL)** - Modern and more powerful.

✅ **Example:**  
```cpp
#include <iostream>
using namespace std;

int main() {
    string s = "Hello, World!";
    cout << s;  // Output: Hello, World!
    return 0;
}
```

---

## 🔹 **2. Declaring and Using Strings**

### ✅ **2.1. Declaring Strings**

```cpp
#include <iostream>
using namespace std;

int main() {
    string s1 = "Hello";  // String declaration
    char s2[] = "World";  // C-style string
    cout << s1 << " " << s2;  // Output: Hello World
    return 0;
}
```

### ✅ **2.2. Taking Input for Strings**
Use `getline(cin, s)` to take input for strings with spaces.

```cpp
#include <iostream>
using namespace std;

int main() {
    string s;
    cout << "Enter a string: ";
    getline(cin, s);  // Input: Hello World
    cout << "You entered: " << s;  // Output: You entered: Hello World
    return 0;
}
```

---

## 🔹 **3. String Functions in C++**
C++ provides several built-in string functions:

| Function | Description | Example |
|----------|-------------|----------|
| `s.length()` | Get the length of a string | `"hello".length() → 5` |
| `s.size()` | Alternative to `.length()` | `"hello".size() → 5` |
| `s.append(t)` | Concatenates string `t` to `s` | `"hello".append(" world") → "hello world"` |
| `s.substr(start, length)` | Extracts a substring | `"hello".substr(1,3) → "ell"` |
| `s.find(t)` | Finds the position of `t` | `"hello".find("l") → 2` |
| `s.erase(start, length)` | Erases part of the string | `"hello".erase(1,2) → "ho"` |
| `s.insert(pos, t)` | Inserts `t` at `pos` | `"hello".insert(1,"i") → "hiello"` |
| `s.replace(start, len, t)` | Replaces part of string with `t` | `"hello".replace(1,3,"i") → "hio"` |
| `s.compare(t)` | Compares two strings (`0` if equal) | `"abc".compare("abc") → 0"` |

---

## 🔹 **4. String Traversal**

### ✅ **4.1. Using `for` Loop**
```cpp
#include <iostream>
using namespace std;

int main() {
    string s = "hello";
    for (int i = 0; i < s.length(); i++) {
        cout << s[i] << " ";  // Output: h e l l o
    }
    return 0;
}
```

### ✅ **4.2. Using `for-each` Loop (C++11 and later)**
```cpp
#include <iostream>
using namespace std;

int main() {
    string s = "hello";
    for (char c : s) {
        cout << c << " ";  // Output: h e l l o
    }
    return 0;
}
```

---

## 🔹 **5. Common String Operations**

### ✅ **5.1. Reversing a String**
```cpp
#include <iostream>
#include <algorithm> // For reverse()
using namespace std;

int main() {
    string s = "hello";
    reverse(s.begin(), s.end());
    cout << s;  // Output: olleh
    return 0;
}
```

### ✅ **5.2. Checking for Palindrome**
```cpp
#include <iostream>
#include <algorithm>
using namespace std;

bool isPalindrome(string s) {
    string rev = s;
    reverse(rev.begin(), rev.end());
    return s == rev;
}

int main() {
    string s = "madam";
    cout << (isPalindrome(s) ? "Yes" : "No");  // Output: Yes
    return 0;
}
```

### ✅ **5.3. Sorting a String Alphabetically**
```cpp
#include <iostream>
#include <algorithm>
using namespace std;

int main() {
    string s = "dcba";
    sort(s.begin(), s.end());
    cout << s;  // Output: abcd
    return 0;
}
```

---

## 🔹 **6. Practice Problems**  
Here are some beginner problems to practice:

1️⃣ Reverse a String  
2️⃣ Check if a String is a Palindrome  
3️⃣ Count the Number of Vowels in a String  
4️⃣ Find the Most Frequent Character in a String  
5️⃣ Sort a String Alphabetically  

Practice on **LeetCode**, **Codeforces**, and **AtCoder**.

---

## 🔹 **7. Additional Learning Resources**

📘 **Documentation:**  
- [C++ Strings Documentation (cplusplus.com)](https://www.cplusplus.com/reference/string/)  
- [GeeksforGeeks - C++ Strings](https://www.geeksforgeeks.org/stdstring-class-in-c/)  

📺 **Tutorial Video:**  
- [YouTube: C++ Strings Full Tutorial](https://www.youtube.com/watch?v=aT4vG2N-VpE)  

---

🚀 **Keep Practicing & Level Up!** 🚀  
