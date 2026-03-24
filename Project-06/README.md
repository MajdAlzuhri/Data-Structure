# 📌 Stack Using Dynamic Array (OOP)

## 📖 Overview

This project — Stack Using Dynamic Array (OOP) — implements a Stack data structure in C++ using a custom-built Dynamic Array class.

Instead of relying on STL containers, the Stack is built manually to demonstrate how data structures operate internally and how memory is managed dynamically.

The project highlights how a higher-level data structure (Stack) can be constructed on top of a lower-level structure (Dynamic Array).

## 🎯 Learning Purpose

This project is designed to strengthen understanding of Data Structures and OOP concepts.

Through this implementation, we learn how to:

* Build Stack from scratch using a Dynamic Array
* Understand LIFO (Last In, First Out) behavior
* Manage data using manual memory structures
* Apply Object-Oriented Programming principles
* Reuse existing data structures to build new ones

## ⚙️ Core Functionality

**Stack Operations:**

* Push → insert element at the top
* Pop → remove element from the top
* Top → access the top element
* Bottom → access the bottom element
* Size → get number of elements
* IsEmpty → check if stack is empty

**Extended Features:**

* Peek at bottom element without removing it
* Reverse stack
* Update item by index
* Insert at front, back, or after a specific item
* Clear entire stack

## 🧠 Educational Insight

This project demonstrates an important concept:
*"Complex data structures can be built on top of simpler ones."*

By implementing a Stack using a Dynamic Array, we understand how abstraction allows us to reuse logic and build more complex systems efficiently.

## ⚠️ Performance Note

* Push operation → efficient (O(1) when inserting at beginning)
* Pop operation → efficient (O(1) when removing from beginning)
* Access bottom element → O(1)

This highlights the trade-offs of array-based stacks and motivates advanced implementations for dynamic growth without resizing overhead.

## 🧩 Project Philosophy

* Encapsulation → Stack logic is separated from array implementation
* Abstraction → User interacts with simple stack operations
* Code Reusability → Dynamic Array is reused as a base structure

## 🔧 Technologies

* C++
* Object-Oriented Programming (OOP)
* Templates
* Manual Memory Management

## 🏗️ Suggested Project Structure

Stack-Using-Dynamic-Array/
├─ Core/
│  └─ clsDynamicArray.h
├─ DataStructures/
│  └─ clsMyStackArr.h
├─ Application/
│  └─ main.cpp
└─ README.md

## 📝 Example Usage

```cpp
#include <iostream>
#include "clsMyStackArr.h"

using namespace std;

int main()
{
    clsMyStackArr<int> MyStack;

    MyStack.push(10);
    MyStack.push(20);
    MyStack.push(30);
    MyStack.push(40);
    MyStack.push(50);

    cout << "\nStack: \n";
    MyStack.Print();

    cout << "\nStack Size: " << MyStack.Size();
    cout << "\nStack Top: " << MyStack.Top();
    cout << "\nStack Bottom: " << MyStack.Bottom();

    MyStack.pop();

    cout << "\n\nStack after pop() : \n";
    MyStack.Print();

    // Extension #1
    cout << "\n\n Item(2) : " << MyStack.GetItem(2);

    // Extension #2
    MyStack.Reverse();
    cout << "\n\nStack after reverse() : \n";
    MyStack.Print();

    // Extension #3
    MyStack.UpdateItem(2, 600);
    cout << "\n\nStack after updating Item(2) to 600 : \n";
    MyStack.Print();

    // Extension #4
    MyStack.InsertAfter(2, 800);
    cout << "\n\nStack after Inserting 800 after Item(2) : \n";
    MyStack.Print();

    // Extension #5
    MyStack.InsertAtFront(1000);
    cout << "\n\nStack after Inserting 1000 at top: \n";
    MyStack.Print();

    // Extension #6
    MyStack.InsertAtBack(2000);
    cout << "\n\nStack after Inserting 2000 at bottom: \n";
    MyStack.Print();

    // Extension #7
    MyStack.Clear();
    cout << "\n\nStack after Clear(): \n";
    MyStack.Print();

    system("pause>0");
}
```
