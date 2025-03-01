# 🚀 Roadmaps Collection

## 📌 Jump To:
- [DSA Roadmap with c++](#dsa-roadmap-with-c++)
- [DSA ROADMAP WITH PYTHON](#dsa-roadmap-with-python)
- [Cyber Security Roadmap](#cyber-roadmap)
- [Competitive Programming Roadmap](#competitive-programming-roadmap)
- [c++ roadmap](#c++-roadmap)
- [custom roadmap](#custom-roadmap)

--------------------------------------------------------------------
## DSA ROADMAP WITH C++
# 📌 Beginner's Guide to Arrays, Strings, Searching & Sorting

This guide will help you learn **Arrays, Strings, Searching, and Sorting Algorithms** for Competitive Programming (CP). 🚀

---

## 🔹 **1. Arrays**  
An **array** is a collection of elements stored in contiguous memory locations.  

### ✅ **What You Should Learn:**  
✔ Declaring and Initializing Arrays  
✔ Accessing Elements  
✔ Traversing an Array  
✔ Finding Maximum & Minimum  
✔ Reversing an Array  

### 🎯 **Example Problem:**  
**Find Maximum in an Array**  
```cpp
#include <iostream>
using namespace std;
int main() {
    int arr[] = {3, 1, 5, 9, 2};
    int maxVal = arr[0];
    for (int i = 1; i < 5; i++) {
        if (arr[i] > maxVal) maxVal = arr[i];
    }
    cout << "Max: " << maxVal;
}
```

### 📌 **Resources to Learn Arrays:**  
- 📺 [Arrays in C++ (Apna College)](https://youtu.be/B9bjGmS8bak)  
- 📘 [GeeksforGeeks Array Basics](https://www.geeksforgeeks.org/arrays-in-c-cpp/)  

---

## 🔹 **2. Strings**  
A **string** is a sequence of characters stored in memory.  

### ✅ **What You Should Learn:**  
✔ Declaring and Using Strings  
✔ String Functions (Length, Concatenation)  
✔ Reversing a String  
✔ Palindrome Check  

### 🎯 **Example Problem:**  
**Reverse a String**  
```cpp
#include <iostream>
#include <algorithm>
using namespace std;
int main() {
    string s = "hello";
    reverse(s.begin(), s.end());
    cout << s; // Output: "olleh"
}
```

### 📌 **Resources to Learn Strings:**  
- 📺 [String Basics (Apna College)](https://youtu.be/ZzaPdXTrSb8)  
- 📘 [GeeksforGeeks String Handling](https://www.geeksforgeeks.org/cpp-string/)  

---

## 🔹 **3. Searching Algorithms**  
### ✅ **Linear Search**  
- **Use when:** The array is **unsorted** or small.  
- **Time Complexity:** O(N)  
```cpp
int linearSearch(int arr[], int n, int key) {
    for (int i = 0; i < n; i++) {
        if (arr[i] == key) return i; 
    }
    return -1;
}
```  

### ✅ **Binary Search**  
- **Use when:** The array is **sorted**.  
- **Time Complexity:** O(log N)  
```cpp
int binarySearch(int arr[], int left, int right, int key) {
    while (left <= right) {
        int mid = left + (right - left) / 2;
        if (arr[mid] == key) return mid;
        else if (arr[mid] < key) left = mid + 1;
        else right = mid - 1;
    }
    return -1;
}
```  

### 📌 **Resources to Learn Searching:**  
- 📺 [Binary Search (CodeWithHarry)](https://youtu.be/f6UU7V3szVw)  
- 📘 [Binary Search - GeeksforGeeks](https://www.geeksforgeeks.org/binary-search/)  

---

## 🔹 **4. Sorting Algorithms**  
### ✅ **Bubble Sort (Basic Sorting Algorithm)**  
- **Time Complexity:** O(N²)  
- **Use when:** Learning sorting, but not efficient for large data.  
```cpp
void bubbleSort(int arr[], int n) {
    for (int i = 0; i < n - 1; i++) {
        for (int j = 0; j < n - i - 1; j++) {
            if (arr[j] > arr[j + 1]) swap(arr[j], arr[j + 1]);
        }
    }
}
```  

### ✅ **Built-in Sorting (Best for CP)**  
C++ provides an in-built sorting function that works in **O(N log N)** time.  
```cpp
sort(arr, arr + n); // Sorts an array
sort(vec.begin(), vec.end()); // Sorts a vector
```  

### 📌 **Resources to Learn Sorting:**  
- 📺 [Sorting Algorithms (Apna College)](https://youtu.be/pkkFqlG0Hds)  
- 📘 [Sorting - GeeksforGeeks](https://www.geeksforgeeks.org/sorting-algorithms/)  

---

## 🎯 **Next Steps**  
Now that you have learned the basics, start practicing problems on **Codeforces (Div 2A)** or **LeetCode (Easy).** 🚀  

# 📌 Beginner's Guide to Arrays, Strings, Searching & Sorting (Python)

This guide will help you learn **Arrays, Strings, Searching, and Sorting Algorithms** for Competitive Programming (CP) using Python. 🚀

----------------------------------------------------------------------------------------------------------------------------------------------
## DSA ROADMAP WITH PYTHON
## 🔹 **1. Arrays (Lists in Python)**

An **array (list in Python)** is a collection of elements stored in contiguous memory locations.

### ✅ **What You Should Learn:**

✔ Declaring and Initializing Lists  
✔ Accessing Elements  
✔ Traversing a List  
✔ Finding Maximum & Minimum  
✔ Reversing a List

### 🎯 **Example Problem:**

**Find Maximum in a List**

```python
arr = [3, 1, 5, 9, 2]
max_val = max(arr)  # Finding the maximum value
print("Max:", max_val)
```

**accessing Elements**

```python
a = [10, 20, 15]

print(a[0])
```

**Traversing a list**

```python
a = [1, 3, 5, 7, 9]

# On each iteration val
# represents the current item/element
for val in a:
    print(val)
```

**Finding Maximum & Minimum**

```python
a = [1,2,3,4,5]
#find maximum value
max_val = max(a)
#find the minimum value
min_val = min(a)
```

**Reversing a Lis**

```python
a = [1, 2, 3, 4, 5]

# Reverse the list in-place
a.reverse()
print(a)
```

### 📌 **Resources to Learn Lists:**

- 📺 [Python Lists Tutorial (Programiz)](https://www.programiz.com/python-programming/list)
- 📘 [GeeksforGeeks List Basics](https://www.geeksforgeeks.org/python-list/)

---

## 🔹 **2. Strings**

A **string** is a sequence of characters stored in memory.

### ✅ **What You Should Learn:**

✔ Declaring and Using Strings  
✔ String Functions (Length, Concatenation)  
✔ Reversing a String  
✔ Palindrome Check

### 🎯 **Example Problem:**

**Reverse a String**

```python
s = "hello"
reversed_s = s[::-1]  # Slicing method to reverse a string
print(reversed_s)  # Output: "olleh"
```

### 📌 **Resources to Learn Strings:**

- 📺 [Python Strings (W3Schools)](https://www.w3schools.com/python/python_strings.asp)
- 📘 [GeeksforGeeks String Handling](https://www.geeksforgeeks.org/python-strings/)

---

## 🔹 **3. Searching Algorithms**

### ✅ **Linear Search**

- **Use when:** The list is **unsorted** or small.
- **Time Complexity:** O(N)

```python
def linear_search(arr, key):
    for i in range(len(arr)):
        if arr[i] == key:
            return i  # Return index of found element
    return -1  # Not found

arr = [10, 20, 30, 40, 50]
key = 30
print(linear_search(arr, key))  # Output: 2
```

### ✅ **Binary Search**

- **Use when:** The list is **sorted**.
- **Time Complexity:** O(log N)

```python
def binary_search(arr, key):
    left, right = 0, len(arr) - 1
    while left <= right:
        mid = (left + right) // 2
        if arr[mid] == key:
            return mid
        elif arr[mid] < key:
            left = mid + 1
        else:
            right = mid - 1
    return -1

arr = [10, 20, 30, 40, 50]
key = 30
print(binary_search(arr, key))  # Output: 2
```

### 📌 **Resources to Learn Searching:**

- 📺 [Binary Search (Python)](https://www.youtube.com/watch?v=D5SrAga1pno)
- 📘 [Binary Search - GeeksforGeeks](https://www.geeksforgeeks.org/python-program-for-binary-search/)

---

## 🔹 **4. Sorting Algorithms**

### ✅ **Bubble Sort (Basic Sorting Algorithm)**

- **Time Complexity:** O(N²)
- **Use when:** Learning sorting, but not efficient for large data.

```python
def bubble_sort(arr):
    n = len(arr)
    for i in range(n - 1):
        for j in range(n - i - 1):
            if arr[j] > arr[j + 1]:
                arr[j], arr[j + 1] = arr[j + 1], arr[j]  # Swap elements

arr = [5, 3, 8, 1, 2]
bubble_sort(arr)
print(arr)  # Output: [1, 2, 3, 5, 8]
```

### ✅ **Built-in Sorting (Best for CP)**

Python provides an in-built sorting function that works in **O(N log N)** time.

```python
arr = [5, 3, 8, 1, 2]
arr.sort()  # In-place sorting
print(arr)  # Output: [1, 2, 3, 5, 8]
```

### 📌 **Resources to Learn Sorting:**

- 📺 [Sorting Algorithms (Python)](https://www.youtube.com/watch?v=ZDezxfN_WJA)
- 📘 [Sorting - GeeksforGeeks](https://www.geeksforgeeks.org/python-sort-list/)

---------------------------------------------------------------------------------------
## CYBER SECURITY ROADMAP

## 🎯 **Next Steps**

Now that you have learned the basics, start practicing problems on **Codeforces (Div 2A)** or **LeetCode (Easy).** 🚀
-----------------------------------------------------------------------------------------------------------------------------
# 🔐 Cybersecurity Roadmap

## 📌 Phase 1: Fundamentals of Cybersecurity
### ✅ Learn the Basics
- **Networking Concepts** (OSI Model, TCP/IP, Subnetting, DNS, DHCP, VPNs)
- **Operating Systems** (Windows, Linux - especially Kali Linux & Parrot OS)
- **Command Line Proficiency** (Bash, PowerShell, CMD)
- **Programming & Scripting** (Python, Bash scripting for automation)

### ✅ Learn Cybersecurity Concepts
- **Types of Attacks** (MITM, DoS/DDoS, Phishing, Ransomware, Social Engineering)
- **Encryption & Hashing** (AES, RSA, SHA, MD5)
- **Authentication & Authorization** (JWT, OAuth, SAML)
- **Cybersecurity Laws & Ethics**

---

## 📌 Phase 2: Networking & System Security
### ✅ Network Security
- **Firewalls, IDS & IPS**
- **Network Sniffing & Packet Analysis** (Wireshark, tcpdump)
- **VPNs, Proxy Servers & Anonymity Tools**

### ✅ Web Security
- **OWASP Top 10 Vulnerabilities** (SQL Injection, XSS, CSRF, SSRF, etc.)
- **Understanding HTTP, HTTPS, Cookies, and Sessions**
- **Web Security Testing Tools** (Burp Suite, OWASP ZAP)

### ✅ System Security & Hardening
- **Windows Security & Active Directory Basics**
- **Linux Security Best Practices (SELinux, AppArmor)**
- **Forensics & Log Analysis** (ELK Stack, Splunk, Sysmon)

---

## 📌 Phase 3: Ethical Hacking & Penetration Testing
### ✅ Learn Ethical Hacking Methodologies
- **Reconnaissance & Footprinting** (Shodan, Google Dorking)
- **Scanning & Enumeration** (Nmap, Netcat, Metasploit)
- **Gaining Access** (Exploits, Privilege Escalation)
- **Maintaining Access & Covering Tracks**

### ✅ Master Penetration Testing Tools
- **Kali Linux & Parrot OS Tools**
- **Metasploit Framework** (Exploitation Framework)
- **Nmap, Nikto, Gobuster, and Recon-ng** (Scanning & Enumeration)
- **John the Ripper, Hashcat** (Password Cracking)
- **Burp Suite & OWASP ZAP** (Web App Security Testing)

---

## 📌 Phase 4: Advanced Cybersecurity & Red Teaming
### ✅ Wireless & IoT Security
- **Wi-Fi Hacking** (Aircrack-ng, Wifite, Evil Twin Attacks)
- **Bluetooth & RFID Security** (HCI Sniffing, NFC attacks)

### ✅ Cloud Security & DevSecOps
- **AWS, Azure & Google Cloud Security**
- **CI/CD Pipeline Security** (Jenkins, GitHub Actions)
- **Container Security** (Docker, Kubernetes, Kube-hunter)

### ✅ Malware Analysis & Reverse Engineering
- **Static & Dynamic Analysis of Malware**
- **Using Tools like IDA Pro, Ghidra, OllyDbg**

---

## 📌 Phase 5: Bug Bounty Hunting & Career Growth
### ✅ Get Hands-on Experience
- **Capture the Flag (CTF) Challenges** (Hack The Box, TryHackMe, OverTheWire)
- **Bug Bounty Platforms** (HackerOne, Bugcrowd, OpenBugBounty)
- **Write Reports & Disclosures**

### ✅ Cybersecurity Certifications
- **Beginner:** CompTIA Security+, CEH (Certified Ethical Hacker)
- **Intermediate:** OSCP (Offensive Security Certified Professional)
- **Advanced:** OSWE, OSCE, CISSP, GPEN

### ✅ Career & Specialization Paths
- **Red Teaming (Offensive Security)**
- **Blue Teaming (Defensive Security)**
- **Forensics & Incident Response**
- **Cloud Security & DevSecOps**

🚀 **Stay updated, practice regularly, and keep hacking ethically!** 
------------------------------------------------------------------------------------
# 🏆 Competitive Programming Roadmap

## 📌 Phase 1: Fundamentals of Programming
### ✅ Learn a Programming Language
- **C++** (Most popular for CP due to STL and speed)
- **Python** (Great for problem-solving but slower execution)
- **Java** (Good alternative with strong libraries)

### ✅ Master Core Concepts
- Variables, loops, and conditionals
- Functions and recursion
- Arrays, strings, and pointers
- Object-Oriented Programming (OOP) basics

### ✅ Learn Time Complexity & Big-O Notation
- Understand **O(1), O(log N), O(N), O(N log N), O(N²)** complexities
- Analyze problems based on execution time limits

---

## 📌 Phase 2: Data Structures & Algorithms (DSA)
### ✅ Essential Data Structures
- **Arrays & Strings** (Sorting, searching, prefix sums)
- **Linked Lists** (Singly, Doubly, Circular)
- **Stacks & Queues** (Using arrays and linked lists)
- **HashMaps & HashSets** (Efficient lookups and frequency counting)
- **Trees & Graphs** (DFS, BFS, shortest paths)
- **Heaps & Priority Queues** (Efficient min/max element operations)

### ✅ Important Algorithms
- Sorting (QuickSort, MergeSort, HeapSort)
- Searching (Binary Search, Ternary Search)
- Two Pointers, Sliding Window
- Recursion & Backtracking
- Dynamic Programming (Memoization, Tabulation)
- Greedy Algorithms
- Graph Algorithms (Dijkstra, Floyd-Warshall, Bellman-Ford)
- String Algorithms (KMP, Rabin-Karp, Z-algorithm)
- Bit Manipulation tricks

---

## 📌 Phase 3: Problem-Solving & Practice
### ✅ Beginner Level (~100 Problems)
- **Codeforces Div2 A/B, Leetcode Easy, AtCoder Beginner**
- Basic loops, conditions, arrays, and STL usage

### ✅ Intermediate Level (~200 Problems)
- **Codeforces Div2 C, Leetcode Medium, AtCoder Intermediate**
- Implementing BFS/DFS, Dijkstra, Greedy, Dynamic Programming

### ✅ Advanced Level (~300+ Problems)
- **Codeforces Div1, Leetcode Hard, AtCoder Advanced**
- Heavy use of Graphs, Advanced DP, Segment Trees, Fenwick Trees

### ✅ Speed Up Coding
- Master STL (C++), itertools (Python), Collections (Java)
- Use **fast I/O** techniques (cin/cout optimizations)

---

## 📌 Phase 4: Competitive Programming Strategy
### ✅ Join CP Platforms & Contests
- **Codeforces** (Most popular, frequent contests)
- **AtCoder** (Great for gradual difficulty increase)
- **LeetCode** (Best for interview-based problem-solving)
- **CodeChef** (Monthly contests, long challenges)
- **TopCoder** (Algorithm-heavy challenges)
- **HackerRank & HackerEarth** (Good for beginners)

### ✅ Participate in Live Contests
- Solve **Div2 contests** on Codeforces regularly
- Analyze editorial solutions after contests
- Upsolve unsolved problems to improve

### ✅ Learn Debugging & Optimization Techniques
- Use `assert()` for testing edge cases
- Optimize DP states & use **Bitmasking**
- Reduce unnecessary loops & function calls

---

## 📌 Phase 5: Mastery & Specialization
### ✅ Target High-Level Contests
- **ICPC (International Collegiate Programming Contest)**
- **Google Code Jam**
- **Facebook Hacker Cup**
- **Google Kick Start**
- **Leetcode Weekly/Monthly Contests**

### ✅ Develop a Competitive Mindset
- **Consistency > Speed** (Solve problems daily)
- **Quality > Quantity** (Focus on hard problems, not just solving many)
- **Learn from Top Coders** (Follow grandmasters on CF)

### ✅ Build a Strong CP Profile
- Achieve **Expert/Master** rating on Codeforces
- Publish CP blogs & tutorials
- Mentor beginners & join CP communities

🚀 **Stay consistent, keep competing, and aim for the top!** 
---------------------------------------------------------------------------
# c++ roadmap

# 🚀 C++ Learning Roadmap for Competitive Programming

This roadmap will guide you from **absolute beginner** to **competitive programming level** in C++.

---

## 📌 **1. Basics of C++**

🔹 **Goal:** Learn the fundamentals of C++ programming.

✅ **What to Learn:**

- Input/Output (`cin`, `cout`, `printf`, `scanf`)
- Data Types (`int`, `long long`, `char`, `double`, `string`, `bool`)
- Conditionals (`if-else`, `switch-case`)
- Loops (`for`, `while`, `do-while`)
- Functions and Recursion

✅ **Practice Problems:**

- Print "Hello, World!"
- Sum of Two Numbers
- Maximum of Two Numbers
- Odd or Even
- Factorial of a Number using Recursion

🔗 **Resources:**

- [C++ Basics - GeeksforGeeks](https://www.geeksforgeeks.org/c-plus-plus/)
- [C++ Playlist - CodeWithHarry (YouTube)](https://www.youtube.com/playlist?list=PLu0W_9lII9agS67Uits0UnJyrYiXhDS6q)

---

## 📌 **2. Data Structures in C++ (Using STL)**

🔹 **Goal:** Learn built-in C++ STL (Standard Template Library) to write efficient code.

✅ **What to Learn:**

- **Vectors** (`vector<int> v;` - Dynamic arrays)
- **Pairs** (`pair<int, int> p;` - Store two values together)
- **Maps** (`map<int, int> m;` - Key-value pairs)
- **Sets** (`set<int> s;` - Store unique elements)
- **Stacks & Queues** (`stack<int> s;`, `queue<int> q;`)
- **Priority Queue (Heap)** (`priority_queue<int> pq;`)

✅ **Practice Problems:**

- Reverse an Array using a Vector
- Find the Frequency of Elements using a Map
- Implement Stack & Queue using STL
- Sort a List of Pairs

🔗 **Resources:**

- [STL Cheat Sheet - GeeksforGeeks](https://www.geeksforgeeks.org/the-c-standard-template-library-stl/)
- [STL Guide - CodeNCode (YouTube)](https://www.youtube.com/playlist?list=PL2q4fbVm1Ik4liHX78IRslXzUr8z5QxsG)

---

## 📌 **3. Searching & Sorting Algorithms**

🔹 **Goal:** Learn fundamental algorithms used in CP.

✅ **What to Learn:**

- **Sorting Algorithms:** Bubble Sort, Selection Sort, Insertion Sort, Merge Sort, Quick Sort
- **Binary Search** (`binary_search(arr.begin(), arr.end(), x)`)
- **Two Pointers & Sliding Window Technique**

✅ **Practice Problems:**

- Implement Merge Sort & Quick Sort
- Search for an Element using Binary Search
- Find the Two Numbers that Sum to a Given Value (Two Pointers)

🔗 **Resources:**

- [Sorting Algorithms - GeeksforGeeks](https://www.geeksforgeeks.org/sorting-algorithms/)
- [Binary Search - CodeNCode (YouTube)](https://www.youtube.com/playlist?list=PL2q4fbVm1Ik4KTKZbQcrx-gKSMQwWfGQj)

---

## 📌 **4. Advanced Data Structures**

🔹 **Goal:** Learn commonly used data structures for advanced CP problems.

✅ **What to Learn:**

- **Binary Trees & BST** (`struct Node { int val; Node* left; Node* right; }`)
- **Graphs (BFS, DFS)** (`vector<int> adj[N];`)
- **Trie Data Structure**
- **Segment Tree & Fenwick Tree**

✅ **Practice Problems:**

- Implement BFS & DFS Traversal of a Graph
- Check if a Tree is a BST
- Find Shortest Path using Dijkstra's Algorithm

🔗 **Resources:**

- [Graph Algorithms - CP Algorithms](https://cp-algorithms.com/graph/)
- [Binary Trees & Graphs - Striver (YouTube)](https://www.youtube.com/playlist?list=PLgUwDviBIf0rGEWe64KWas0Nryn7SCRWw)

---

## 📌 **5. Dynamic Programming (DP)**

🔹 **Goal:** Learn optimization techniques for solving CP problems efficiently.

✅ **What to Learn:**

- Introduction to DP (Memoization & Tabulation)
- Classical DP Problems (Fibonacci, Knapsack, LIS, Coin Change)
- Bitmasking & State Space Reduction

✅ **Practice Problems:**

- Fibonacci Number using DP
- 0/1 Knapsack Problem
- Longest Increasing Subsequence (LIS)

🔗 **Resources:**

- [Dynamic Programming - CP Algorithms](https://cp-algorithms.com/dynamic_programming/)
- [DP Playlist - Aditya Verma (YouTube)](https://www.youtube.com/playlist?list=PL_z_8CaSLPWeT1ffjiImo0sYTcnLzo-wY)

---

## 📌 **6. Competitive Programming Preparation**

🔹 **Goal:** Get hands-on experience by solving CP problems.

✅ **Practice Sites:**

- [Codeforces](https://codeforces.com/)
- [AtCoder](https://atcoder.jp/)
- [CodeChef](https://www.codechef.com/)
- [LeetCode](https://leetcode.com/)
- [HackerRank](https://www.hackerrank.com/domains/tutorials/10-days-of-code)

✅ **Challenge Yourself:**

- Participate in **Codeforces Div3/Div2 Contests**
- Solve **A/B Problems on Codeforces**
- Solve **AtCoder Beginner Contests**

🔗 **CP Roadmaps & Guides:**

- [Competitive Programming Handbook - CP Algorithms](https://cp-algorithms.com/)
- [How to Start CP - Errichto (YouTube)](https://www.youtube.com/watch?v=xAeiXyCiyFI)

---

## 🎯 **Final Advice:**

- **Consistency is Key** – Solve problems daily.
- **Participate in Contests** – The best way to improve.
- **Read Editorials & Learn from Mistakes** – Debugging is a skill.
- **Join CP Communities** – Engage with others (Codeforces, Discord servers, etc.).

🚀 **Happy Coding!** 🚀
-------------------------------------------------------------------------------------------
# custom roadmap

# 🛠️ Custom Roadmap: Software Development & Penetration Testing

## 🎯 Goal:

- Master **Competitive Programming (CP)** to strengthen problem-solving skills.
- Build strong **Mathematical Foundations** for CP and software development.
- Choose between **Software Development** (primary job) or **Penetration Testing**, keeping the other as a secondary skill.

---

## 📌 Phase 1: Competitive Programming & Mathematics (6-12 months)

### 🎯 Goals:

- Improve **problem-solving skills** for both software development & pentesting.
- Learn **math fundamentals** to support CP & security algorithms.

### 📚 Topics to Cover:

#### ✅ Mathematics:

- **Number Theory**: Prime Numbers, Modular Arithmetic, GCD, Euler’s Totient Function.
- **Graph Theory**: BFS, DFS, Dijkstra, Floyd-Warshall, MST (Kruskal, Prim).
- **Combinatorics & Probability**: Permutations, Combinations, Binomial Coefficients.
- **Linear Algebra**: Matrices, Vectors (for AI & Cryptography).
- **Discrete Mathematics**: Boolean Algebra, Set Theory.

#### ✅ Competitive Programming Topics:

- **Algorithms**: Sorting, Searching, DP, Graphs, Trees, Bit Manipulation.
- **Data Structures**: Stacks, Queues, HashMaps, Tries, Segment Trees.
- **Advanced CP**: Dynamic Programming (Knapsack, LIS, LCS), Game Theory.

#### 🔗 Resources:

- [CP Algorithms](https://cp-algorithms.com/)
- [CS50: Intro to Computer Science](https://cs50.harvard.edu/)
- [Khan Academy: Mathematics](https://www.khanacademy.org/math/)

---

## 📌 Phase 2: Software Development Fundamentals (6-12 months)

### 🎯 Goals:

- Gain **core programming** knowledge for real-world applications.
- Learn **software architecture** and **best practices**.
- Build **projects** to showcase skills.

### 📚 Topics to Cover:

#### ✅ Programming & System Design:

- **Python & OOP**: Classes, Inheritance, Design Patterns.
- **Database Management**: SQL, NoSQL (PostgreSQL, MongoDB).
- **APIs & Web Development**: REST, Flask/FastAPI, Authentication.
- **Software Development Principles**: Clean Code, SOLID Principles, Testing.

#### ✅ Desktop Development (PyQt/PySide):

- **GUI Development**: Event Handling, Widgets, Multi-threading.
- **Cross-Platform Development**: Packaging, Deployment.

#### 🔗 Resources:

- [Flask Mega-Tutorial](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world)
- [PyQt Documentation](https://doc.qt.io/qtforpython/)

### 📌 **Project Ideas:**

- **To-Do App** (CRUD, Authentication, Database)
- **Password Manager** (Encryption, Secure Storage)
- **Network Monitoring Tool** (Scans, Reports, UI with PyQt)

---

## 📌 Phase 3: Penetration Testing & Cyber Security (6-12 months)

### 🎯 Goals:

- Learn **offensive security** and **ethical hacking** methodologies.
- Build a **cybersecurity toolkit** for pentesting.
- Apply CP knowledge for **CTF challenges**.

### 📚 Topics to Cover:

#### ✅ Cyber Security Foundations:

- **Networking Basics**: TCP/IP, OSI Model, VPN, Proxy, Firewalls.
- **Linux Security**: Bash Scripting, Privilege Escalation.
- **Web Security**: OWASP Top 10, SQL Injection, XSS, CSRF.
- **Cryptography**: Hashing, AES, RSA, Elliptic Curve Cryptography.

#### ✅ Tools & Certifications:

- **Pentesting Tools**: Nmap, Burp Suite, Metasploit, Wireshark.
- **Certifications** (Optional but Valuable):
  - TryHackMe & HackTheBox
  - CompTIA Security+
  - OSCP (Advanced)

#### 🔗 Resources:

- [Hack The Box](https://www.hackthebox.com/)
- [TryHackMe](https://www.tryhackme.com/)
- [OWASP Web Security](https://owasp.org/)

---

## 📌 Phase 4: Specialization & Career Choice (6+ months)

### 🎯 Decision: **Primary vs. Secondary Career Path**

At this point, based on your experience and interest, you should choose:

- **Primary Job:** Software Development (keeping pentesting as a hobby).
- **Primary Job:** Penetration Testing (keeping software dev for automation).

### 📌 **Building a Portfolio:**

Regardless of your primary choice, you should have a strong portfolio with:

1. **Software Projects**: Open-source contributions, real-world applications.
2. **Pentesting Reports**: CTF writeups, Vulnerability Analysis.
3. **Competitive Programming Profile**: Codeforces, Leetcode, AtCoder ranking.

### 🚀 **Extra Suggestions:**

- If choosing **Software Dev** → Learn **Cloud Computing (AWS, Docker, CI/CD).**
- If choosing **Pentesting** → Learn **Reverse Engineering & Exploit Development.**

---

## 🎯 Final Thoughts:

By following this roadmap, you will:
✅ Gain **strong problem-solving** skills through CP.  
✅ Build **real-world software** and **desktop applications**.  
✅ Master **ethical hacking** and penetration testing.  
✅ Be prepared to choose between **Software Development or Pentesting** as a career.

🚀 **Good luck on your journey! Stay consistent, and keep learning!** 🔥

