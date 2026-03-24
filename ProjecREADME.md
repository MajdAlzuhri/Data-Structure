📌 Stack Using Dynamic Array (OOP)
📖 Overview

This project — Stack Using Dynamic Array (OOP) — implements a Stack data structure in C++ using a custom-built Dynamic Array class.

Instead of relying on STL containers, the Stack is built manually to demonstrate how data structures operate internally and how memory is managed dynamically.

The project shows how a higher-level data structure (Stack) can be constructed on top of a lower-level structure (Dynamic Array) while following Object-Oriented Programming principles.

🎯 Learning Purpose

This project is designed to strengthen understanding of Data Structures and OOP concepts.

Through this implementation, we learn how to:

Build Stack from scratch using a Dynamic Array
Understand LIFO (Last In, First Out) behavior
Manage data using manual memory structures
Apply Object-Oriented Programming principles
Reuse existing data structures to build new ones
⚙️ Core Functionality
🔹 Stack Operations
Push → insert element at the top
Pop → remove element from the top
Top → access the top element
Bottom → access the bottom element
Size → get number of elements
IsEmpty → check if stack is empty
🔹 Extended Features
Peek at bottom element without removing it
Reuse a Queue/Dynamic Array as the underlying storage
Optional: Reverse stack, clear stack
🧠 Educational Insight

This project demonstrates a key concept:

“Complex data structures can be built on top of simpler ones.”

By implementing a Stack using a Dynamic Array, we understand how abstraction and code reuse allow us to construct more complex systems efficiently.

⚠️ Performance Note
Push operation → efficient (O(1) if inserting at beginning)
Pop operation → efficient (O(1) if removing from beginning)
Bottom access → O(1)
Limitation → array resizing can be costly when memory needs to expand

This highlights the trade-offs of array-based stacks and motivates advanced implementations like linked-list-based stacks for dynamic growth without resizing overhead.

🧩 Project Philosophy

The design follows key OOP principles:

Encapsulation → Stack logic is separated from array implementation
Abstraction → User interacts with simple stack operations
Code Reusability → Dynamic Array is reused as a base structure
🔧 Technologies
💻 C++
🧠 Object-Oriented Programming (OOP)
🧩 Templates
⚙️ Manual Memory Management
