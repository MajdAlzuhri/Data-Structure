# 📌 Dynamic Array Class

**C++ | Object-Oriented Programming | Manual Memory Management**

---

## 📖 Introduction

This project demonstrates how to build a fully functional **Dynamic Array class** from scratch in C++ without relying on STL containers.

The goal is not just to store data —
but to deeply understand how dynamic memory works internally and how real containers are engineered.

This class acts as a foundational building block for more advanced data structures.

---

## 🎯 Project Goals

* Implement a reusable Dynamic Array class using templates
* Manage heap memory manually (allocation & deallocation)
* Control resizing behavior efficiently
* Support insertion, deletion, searching, and updating operations
* Apply Object-Oriented Programming (OOP) design principles
* Build a scalable and extensible architecture

---

## 🧠 Core Concepts Applied

* Templates (Generic Programming)
* Dynamic Memory Allocation (`new` / `delete`)
* Constructors & Destructors
* Encapsulation
* Defensive Programming
* Code Reusability
* Modular Design
* Method Composition (Lego-style architecture)

---

## 🏗 Class Design Philosophy

This class fully owns and manages its memory.

✔ When an object is created → memory is allocated dynamically
✔ When the object is destroyed → memory is properly released
✔ All operations maintain internal size consistency
✔ No STL containers are used

The design emphasizes:

* Clear responsibility
* No duplicated logic
* Reusable internal methods
* Extensibility through composition

High-level operations are built on top of core methods instead of rewriting logic.

---

## 🧩 Implemented Features

### 🔹 Basic Operations

* Initialize with specific size
* SetItem
* GetItem
* Size
* IsEmpty
* PrintList
* Clear
* Resize

---

### 🔹 Searching

* Find (by value)

---

### 🔹 Deletion

* DeleteItemAt (by index)
* DeleteFirstItem
* DeleteLastItem
* DeleteItem (by value)

---

### 🔹 Insertion

* InsertAt (core insertion logic)
* InsertAtBeginning
* InsertAtEnd
* InsertBefore
* InsertAfter

All advanced methods are built on top of core logic to ensure clean and maintainable architecture.

---

## 🧪 What This Project Teaches

By implementing this structure manually, we gain a deep understanding of:

* How arrays resize internally
* Memory reallocation strategies
* Shifting mechanics during insertion and deletion
* Trade-offs between arrays and linked lists
* How real-world containers are designed

This shifts the mindset from:

**Using data structures**
➡️ to
**Engineering data structures**

---

## 🔄 Architectural Pattern Used

The project follows a **Core + Extensions model**:

* Build powerful base methods
* Reuse them to construct higher-level behavior
* Avoid duplicate logic
* Compose functionality

### 💡 Examples

* `DeleteFirstItem()` → calls `DeleteItemAt(0)`
* `DeleteItem(Value)` → uses `Find()` + `DeleteItemAt()`
* `InsertAtBeginning()` → calls `InsertAt(0, Value)`

Programming here is treated like assembling **Lego blocks** 🧱

---

## 🛠 Technologies

* 💻 C++
* 🧩 Templates
* 🧠 Object-Oriented Programming (OOP)
* ⚙️ Manual Heap Memory Management

---

## 🗺 Learning Journey Context

This project is part of a structured roadmap covering:

* Data Structures & Algorithms
* OOP Mastery
* Memory Management
* Clean Code Practices

---
