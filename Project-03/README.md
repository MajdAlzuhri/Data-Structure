# 📌 Data Structures Project - Linked List, Queue & Stack

## 📖 Overview

This project implements core Data Structures using C++ templates.
It includes a **Doubly Linked List**, and builds both **Queue** and **Stack** data structures on top of it using Object-Oriented Programming (OOP) principles.

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

---

### 🔹 Queue (FIFO)

* Push (enqueue)
* Pop (dequeue)
* Front element access
* Back element access
* Check if empty
* Get size
* Reverse queue
* Update elements

---

### 🔹 Stack (LIFO)

* Push (insert at top)
* Pop
* Top element access
* Bottom element access

---

## 🛠️ Technologies Used

* C++
* Templates (Generic Programming)
* Object-Oriented Programming (OOP)

---

## 🧠 Concepts Applied

* Doubly Linked List
* Queue (FIFO)
* Stack (LIFO)
* Dynamic Memory Allocation
* Pointers (Next & Previous)
* Encapsulation
* Inheritance
* Code Reusability

---

## 📂 Project Structure

```
- clsDblLinkedList.h
- clsMyQueue.h
- clsMyStack.h
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

### Queue Example

```cpp
clsMyQueue<int> q;

q.push(10);
q.push(20);
q.push(30);

q.Print(); // Output: 10 20 30

q.pop();
q.Print(); // Output: 20 30
```

### Stack Example

```cpp
clsMyStack<int> s;

s.push(10);
s.push(20);
s.push(30);

cout << s.Top(); // Output: 30
```

---

## 📌 Notes

* The project uses templates to support multiple data types.
* Queue is implemented using a Doubly Linked List.
* Stack is implemented using inheritance from Queue.
* Manual memory management is handled using pointers.

---

## 👨‍💻 Author

Majd Alzuhri

---
