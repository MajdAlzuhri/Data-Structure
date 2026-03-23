# 📌 Data Structures Project - Doubly Linked List & Queue

## 📖 Overview

This project implements a **generic Doubly Linked List** and a **Queue data structure** using C++ templates.
It demonstrates core Data Structures concepts along with Object-Oriented Programming (OOP) principles such as encapsulation, abstraction, and modular design.

---

## 🚀 Features

### 🔹 Doubly Linked List

* Insert at beginning
* Insert at end
* Insert at specific index
* Delete node (first, last, specific)
* Search (Find)
* Reverse the list
* Update node value
* Get node by index

### 🔹 Queue (Implemented using Doubly Linked List)

* Push (enqueue)
* Pop (dequeue)
* Front element access
* Back element access
* Check if empty
* Get size
* Reverse queue
* Update elements

---

## 🛠️ Technologies Used

* C++
* Templates (Generic Programming)
* Object-Oriented Programming (OOP)

---

## 🧠 Concepts Applied

* Doubly Linked List
* Queue Data Structure
* Dynamic Memory Allocation
* Pointers (Next & Previous)
* Encapsulation
* Abstraction
* Modular Design

---

## 📂 Project Structure

```
- clsDblLinkedList.h
- clsMyQueue.h
- main.cpp
- README.md
```

---

## ▶️ How to Run

1. Open the project in Visual Studio
2. Build the solution
3. Run the program

---

## 💡 Example Usage

```cpp
clsMyQueue<int> q;

q.push(10);
q.push(20);
q.push(30);

q.Print(); // Output: 10 20 30

q.pop();
q.Print(); // Output: 20 30
```

---

## 📌 Notes

* The implementation uses templates to support different data types.
* Queue is implemented using a Doubly Linked List for flexibility.
* Memory management is handled manually using pointers.

---

## 👨‍💻 Author

Majd Alzuhri

---
