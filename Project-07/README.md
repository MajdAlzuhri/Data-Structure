# 📌 Undo & Redo System Using Stack (OOP)

## 📖 Overview

This project — Undo & Redo System Using Stack (OOP) — implements a simple text state management system in C++ using the built-in stack data structure.

The system allows storing multiple states of a string and navigating between them using Undo and Redo operations.

It demonstrates how stacks can be used in real-world applications such as text editors.

## 🎯 Learning Purpose

This project is designed to strengthen understanding of Data Structures and OOP concepts.

Through this implementation, we learn how to:

* Use stacks to manage state history
* Implement Undo and Redo functionality
* Understand LIFO (Last In, First Out)
* Apply Object-Oriented Programming principles
* Manage application state efficiently

## ⚙️ Core Functionality

**Main Operations:**

* Set → assign a new value
* Get → retrieve current value
* Undo → revert to previous value
* Redo → restore undone value

## 🧠 How It Works

* The **Undo stack** stores previous states
* The **Redo stack** stores undone states

### Flow:

1. When setting a new value:

   * Current value is pushed into Undo stack
2. Undo:

   * Current value → Redo stack
   * Last Undo value becomes current
3. Redo:

   * Current value → Undo stack
   * Last Redo value becomes current

## ⚠️ Important Notes

* Undo works only if there are previous states
* Redo works only after Undo operations
* Setting a new value does NOT clear Redo stack (can be improved)

## 🧩 Project Philosophy

* Encapsulation → logic is inside one class
* Abstraction → simple interface (Set, Undo, Redo)
* Reusability → can be used in editors or apps

## 🔧 Technologies

* C++
* STL Stack
* Object-Oriented Programming (OOP)

## 📝 Example Usage

```cpp
#include <iostream>
#include "clsMyString.h"

using namespace std;

int main()
{
    clsMyString Text;

    Text.Value = "A";
    Text.Value = "B";
    Text.Value = "C";

    cout << "Current: " << Text.Value << endl; // C

    Text.Undo();
    cout << "After Undo: " << Text.Value << endl; // B

    Text.Undo();
    cout << "After Undo: " << Text.Value << endl; // A

    Text.Redo();
    cout << "After Redo: " << Text.Value << endl; // B

    return 0;
}
```
