# 📚 My Data Structures Library (DS Lib)

A comprehensive C++ library implementing essential **Data Structures** with a clean, template-based, object-oriented approach. Built as a personal toolkit for efficient and reusable data structures in various applications.

---

## 📦 Library Overview

This is my personal **Data Structures Library** that I built to master C++ templates, OOP, and memory management. It provides ready-to-use implementations of fundamental data structures with intuitive APIs.

---

## 🏗️ Data Structures Included

### 🔹 Core Data Structures
| Structure | Class | Description |
|-----------|-------|-------------|
| **Dynamic Array** | `clsDynamicArray<T>` | Resizable array with full CRUD operations |
| **Doubly Linked List** | `clsDblLinkedList<T>` | Efficient insertion/deletion from both ends |
| **Queue** | `clsMyQueue<T>` | FIFO data structure (Linked List based) |
| **Queue** | `clsMyQueueArr<T>` | FIFO data structure (Array based) |
| **Stack** | `clsMyStack<T>` | LIFO data structure (Linked List based) |
| **Stack** | `clsMyStackArr<T>` | LIFO data structure (Array based) |

### 🔹 Utility Libraries
| Utility | Class | Description |
|---------|-------|-------------|
| **String** | `clsString` | Advanced string operations (split, join, trim, reverse, case conversion) |
| **Date** | `clsDate` | Comprehensive date operations (add/subtract, compare, format) |
| **Queue Line System** | `clsQueueLine` | Real-world ticket/queue management system |

### 🔹 Advanced Features
- ✅ **Undo/Redo** functionality (`clsMyString`)
- ✅ **Ticket Queue System** with waiting time estimation
- ✅ **Stack/Queue Reversal** operations
- ✅ **Dynamic Capacity Management** with auto-resizing

---

## 🛠️ How to Use

### 1️⃣ Include the Library
```cpp
#include "clsDynamicArray.h"
#include "clsDblLinkedList.h"
#include "clsMyQueue.h"
#include "clsMyStack.h"
#include "clsString.h"
#include "clsDate.h"
```

### 2️⃣ Example: Dynamic Array
```cpp
clsDynamicArray<int> arr(5);

arr.SetItem(0, 10);
arr.SetItem(1, 20);
arr.SetItem(2, 30);
arr.InsertAtEnd(40);
arr.InsertAtBeginning(5);

arr.PrintList(); // Output: 5 10 20 30 40

arr.Reverse();
arr.PrintList(); // Output: 40 30 20 10 5
```

### 3️⃣ Example: Queue System
```cpp
clsMyQueue<string> queue;

queue.push("First");
queue.push("Second");
queue.push("Third");

queue.Print(); // Output: First Second Third
cout << "Front: " << queue.front(); // First
cout << "Back: " << queue.back();   // Third
```

### 4️⃣ Example: Ticket Queue Line
```cpp
clsQueueLine bankQueue("A", 5); // Prefix "A", avg serve time 5 min

bankQueue.IssueTicket(); // Ticket A1
bankQueue.IssueTicket(); // Ticket A2
bankQueue.IssueTicket(); // Ticket A3

bankQueue.PrintInfo();
bankQueue.PrintTicketsLineLTR();
```

---

## 📂 Library Structure

```
My-DS-Lib/
│
├── Algorithm Level 5/                     # Library source folder
│   ├── clsDynamicArray.h                  # Dynamic array
│   ├── clsDblLinkedList.h                 # Doubly linked list
│   ├── clsMyQueue.h                       # Queue (linked list based)
│   ├── clsMyQueueArr.h                    # Queue (array based)
│   ├── clsMyStack.h                       # Stack (linked list based)
│   ├── clsMyStackArr.h                    # Stack (array based)
│   ├── clsString.h                        # String utilities
│   ├── clsDate.h                          # Date utilities
│   ├── clsMyString.h                      # String with undo/redo
│   ├── clsQueueLine.h                     # Queue line system
│   ├── Algorithm Level 5.cpp              # Demo / Test file
│   └── Algorithm Level 5.vcxproj          # Visual Studio project
│
├── Algorithm Level 5.sln                  # Solution file
└── README.md                              # Documentation
```

---

## 🎯 Why This Library?

- ✅ **Template-based**: Works with any data type
- ✅ **OOP Design**: Clean, modular, and extensible
- ✅ **Memory Safe**: Proper allocation/deallocation
- ✅ **Intuitive API**: Easy to use and understand
- ✅ **Production Ready**: Well-tested and reliable
- ✅ **Educational**: Clean code for learning purposes

---

## 🚀 Quick Start

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Abdulrhman774/Algorithm-Level-5-Course-13-.git
   ```

2. **Open the solution:**
   ```bash
   Algorithm Level 5.sln
   ```

3. **Build & Run** using Visual Studio (2019 or later)

4. **Start using the library in your projects!**

---

## 📊 Library Methods Overview

### Dynamic Array (`clsDynamicArray<T>`)
| Method | Description |
|--------|-------------|
| `SetItem(index, value)` | Set value at index |
| `GetItem(index)` | Get value at index |
| `InsertAtBeginning(value)` | Insert at start |
| `InsertAtEnd(value)` | Insert at end |
| `DeleteItemAt(index)` | Delete at index |
| `Reverse()` | Reverse array |
| `Find(value)` | Find element index |
| `Clear()` | Clear all elements |

### Doubly Linked List (`clsDblLinkedList<T>`)
| Method | Description |
|--------|-------------|
| `InsertAtBeginning(value)` | Insert at start |
| `InsertAtEnd(value)` | Insert at end |
| `InsertAfter(node, value)` | Insert after node |
| `DeleteNode(node)` | Delete specific node |
| `DeleteFirstNode()` | Delete first node |
| `DeleteLastNode()` | Delete last node |
| `Reverse()` | Reverse list |
| `Find(value)` | Find node by value |

### Queue (`clsMyQueue<T>`)
| Method | Description |
|--------|-------------|
| `push(value)` | Add to back |
| `pop()` | Remove from front |
| `front()` | Get front element |
| `back()` | Get back element |
| `Size()` | Get queue size |
| `Clear()` | Clear queue |

### Stack (`clsMyStack<T>`)
| Method | Description |
|--------|-------------|
| `push(value)` | Add to top |
| `pop()` | Remove from top |
| `Top()` | Get top element |
| `Bottom()` | Get bottom element |
| `Size()` | Get stack size |
| `Clear()` | Clear stack |

---

## 🧪 Test & Demo

The library includes a comprehensive demo in `Algorithm Level 5.cpp` that showcases all data structures in action. Run it to see:

- Dynamic array operations
- Linked list manipulation
- Queue and stack operations
- String utilities
- Date calculations
- Queue line system simulation

---

## 🤝 Contributing

This is my personal library, but I welcome suggestions and improvements!

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/Improvement`)
3. Commit your changes (`git commit -m 'Add improvement'`)
4. Push to the branch (`git push origin feature/Improvement`)
5. Open a Pull Request

---

## 📫 Contact

**Developer**: Abdulrhman  
**Library**: My DS Lib  
**Built With**: ❤️ + C++

---

## 📝 Notes

- All classes are **template-based** for maximum reusability
- **Memory management** is handled with proper allocation/deallocation
- Code is **well-commented** for easy understanding
- Perfect for **educational** and **production** use

---

*Your personal Data Structures Library - Built from scratch with passion* 🚀
