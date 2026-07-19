# 🧮 Algorithm Level 5 - Data Structures Library

A comprehensive C++ library implementing essential **Data Structures** and **Algorithms** with a clean, template-based, object-oriented approach. Built for educational purposes and practical use in various applications.

---

## ✨ Features

### 📊 Core Data Structures
- ✅ **Dynamic Array** (`clsDynamicArray`) - Resizable array with full CRUD operations
- ✅ **Doubly Linked List** (`clsDblLinkedList`) - Efficient insertion/deletion from both ends
- ✅ **Queue** (`clsMyQueue`) - FIFO data structure using linked list
- ✅ **Queue Array** (`clsMyQueueArr`) - FIFO data structure using dynamic array
- ✅ **Stack** (`clsMyStack`) - LIFO data structure using linked list
- ✅ **Stack Array** (`clsMyStackArr`) - LIFO data structure using dynamic array

### 🔧 Utility Libraries
- ✅ **String Manipulation** (`clsString`) - Advanced string operations (split, join, trim, reverse, case conversion)
- ✅ **Date Handling** (`clsDate`) - Comprehensive date operations (add/subtract days, compare dates, format)
- ✅ **Queue Line System** (`clsQueueLine`) - Real-world ticket/queue management system

### 🎯 Advanced Features
- 🔄 **Undo/Redo** functionality (`clsMyString`)
- 📝 **Ticket Queue System** with waiting time estimation
- 🔁 **Stack/Queue Reversal** operations
- 📊 **Capacity Management** with dynamic resizing

---

## 🛠️ Tech Stack

- **Language**: C++17
- **Paradigm**: Object-Oriented Programming (OOP)
- **Key Concepts**: Templates, Data Structures, Algorithms, File I/O
- **Libraries**: Standard C++ Library (STL concepts)

---

## 📂 Project Structure

```
Algorithm-Level-5-Course-13-/
│
├── Algorithm Level 5/                     # Main source folder
│   ├── clsString.h                        # String manipulation library
│   ├── clsDate.h                          # Date operations library
│   ├── clsDynamicArray.h                  # Dynamic array implementation
│   ├── clsDblLinkedList.h                 # Doubly linked list implementation
│   ├── clsMyQueue.h                       # Queue (Linked List based)
│   ├── clsMyQueueArr.h                    # Queue (Array based)
│   ├── clsMyStack.h                       # Stack (Linked List based)
│   ├── clsMyStackArr.h                    # Stack (Array based)
│   ├── clsMyString.h                      # String with Undo/Redo
│   ├── clsQueueLine.h                     # Queue Line System
│   ├── Algorithm Level 5.cpp              # Entry point / Demo
│   └── Algorithm Level 5.vcxproj          # Visual Studio project file
│
├── Algorithm Level 5.sln                  # Visual Studio solution
└── README.md                              # Project documentation
```

---

## 📊 Data Structures Overview

### 1. **Dynamic Array** (`clsDynamicArray<T>`)
- Resize dynamically
- Insert/Delete at any index
- Find and Update elements
- Reverse array

### 2. **Doubly Linked List** (`clsDblLinkedList<T>`)
- Insert at beginning/end/after node
- Delete node/first/last
- Reverse list
- Find and Update elements

### 3. **Queue** (`clsMyQueue<T>` & `clsMyQueueArr<T>`)
- FIFO (First In, First Out)
- Push, Pop, Front, Back
- Print all elements
- Clear queue

### 4. **Stack** (`clsMyStack<T>` & `clsMyStackArr<T>`)
- LIFO (Last In, First Out)
- Push, Pop, Top, Bottom
- Insert at top/bottom
- Clear stack

### 5. **Queue Line System** (`clsQueueLine`)
- Real-world ticket management
- Issue tickets with unique IDs
- Track waiting clients
- Estimate waiting time
- Print tickets in LTR/RTL order

### 6. **String Library** (`clsString`)
- Split, Join, Trim
- Case conversion (Upper/Lower/Invert)
- Count letters, words, vowels
- Remove punctuations
- Replace words

---

## 🚀 How to Run

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Abdulrhman774/Algorithm-Level-5-Course-13-.git
   ```

2. **Open the solution:**
   ```bash
   Algorithm Level 5.sln
   ```

3. **Build & Run** using Visual Studio (2019 or later)

---

## 💻 Code Example

### Using the Queue System:

```cpp
#include "clsQueueLine.h"

int main() {
    // Create a queue line with prefix "A" and average serve time 5 minutes
    clsQueueLine Queue("A", 5);
    
    // Issue tickets
    Queue.IssueTicket();
    Queue.IssueTicket();
    Queue.IssueTicket();
    
    // Print queue info
    Queue.PrintInfo();
    
    // Print tickets
    Queue.PrintTicketsLineLTR();
    
    return 0;
}
```

### Using Dynamic Array:

```cpp
#include "clsDynamicArray.h"

int main() {
    clsDynamicArray<int> arr(5);
    
    arr.SetItem(0, 10);
    arr.SetItem(1, 20);
    arr.SetItem(2, 30);
    
    arr.InsertAtEnd(40);
    arr.InsertAtBeginning(5);
    
    arr.PrintList(); // 5 10 20 30 40
    
    arr.Reverse();
    arr.PrintList(); // 40 30 20 10 5
    
    return 0;
}
```

---

## 📌 Key Features in Detail

### 🧵 String Library (`clsString`)
| Method | Description |
|--------|-------------|
| `Sblit()` | Split string by delimiter |
| `JoinString()` | Join vector of strings |
| `Trim()` | Remove spaces from both ends |
| `AllUpperLetters()` | Convert to uppercase |
| `ReverseWordsInString()` | Reverse word order |
| `RemovePunctuationsFromString()` | Remove punctuation marks |

### 📅 Date Library (`clsDate`)
| Method | Description |
|--------|-------------|
| `IsLeapYear()` | Check leap year |
| `NumOfDaysInMonth()` | Days in month |
| `DateAddDays()` | Add days to date |
| `CalculateDiffrenceDays()` | Difference between dates |
| `DayShortName()` | Get day name (Sun, Mon, etc.) |
| `PrintMonthCalender()` | Print calendar for month |

---

## 🎯 Use Cases

- ✅ **Queue Line System**: Ticket management for banks, hospitals, or service centers
- ✅ **String Processing**: Text analysis, formatting, and manipulation
- ✅ **Date Calculations**: Scheduling, age calculation, vacation planning
- ✅ **Data Structure Learning**: Educational reference for students
- ✅ **Undo/Redo**: Text editors or form applications

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first.

### To contribute:
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📧 Contact

**Developer**: Abdulrhman  
**Project**: Algorithm Level 5 - Course 13  
**Course**: Data Structures & Algorithms

---

## 📝 Notes

- All classes are **template-based** for maximum reusability
- **Memory management** is handled with proper allocation/deallocation
- **Educational focus** with clean, well-commented code

---

*Built with ❤️ for learning and teaching Data Structures & Algorithms*
