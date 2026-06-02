# 📚 Library Management System - Professional Database Application

## 📋 Overview

A comprehensive, production-grade Library Management System (LMS) demonstrating advanced C++ programming concepts including object-oriented design patterns, persistent file-based data storage, CRUD operations, user authentication, and complex business logic. This project represents enterprise-level application architecture suitable for real-world library operations.

**Complexity Level:** ⭐⭐⭐⭐⭐ Advanced  
**Primary Concepts:** Advanced OOP, File I/O, Data Persistence, CRUD Operations, Authentication, Date/Time Management

---

## 🎯 Project Objectives Achieved

✅ **Advanced OOP Architecture** - Multi-class design with clear separation of concerns  
✅ **Persistent Data Storage** - File-based database with read/write operations  
✅ **User Authentication** - Secure login system with credential validation  
✅ **CRUD Operations** - Complete Create, Read, Update, Delete functionality  
✅ **Business Logic** - Complex rules for book issuance and returns  
✅ **Data Integrity** - Prevent operations that would violate business rules  
✅ **Professional UI** - Formatted table output with clear information display  
✅ **Error Handling** - Comprehensive validation and error management

---

## 🏗️ System Architecture

### Multi-Class Design Pattern

**Book Class** - Data model
```cpp
class Book {
    public:
        int id, publicationYear, totalCopies, availableCopies;
        string title, author, isbn, issuedTo, issuedDate;
        bool issued;
}
```

**Library Class** - Business logic
```cpp
class Library {
    private: vector<Book> books;
    public:
        void loadBooks()          // Load from persistent storage
        void addBook()            // CREATE
        void displayBooks()       // READ
        void searchBook()         // SEARCH
        void issueBook()          // UPDATE
        void returnBook()         // UPDATE
        void deleteBook()         // DELETE
}
```

---

## ✨ Core Features

### 🔐 Authentication System

**Login Credentials:**
- **Username:** `shan`
- **Password:** `1903`

### 📖 CRUD Operations

**CREATE** - Add Book
```cpp
void addBook() {
    // Duplicate ID prevention
    // Multi-word string input support
    // Automatic data persistence
}
```

**READ** - Display/Search Books
```cpp
void displayBooks() {
    // Formatted table output using iomanip
    // Aligned columns for readability
    // Status indicator for issued books
}
```

**UPDATE** - Issue/Return Book
```cpp
void issueBook() {
    // Business rule: Cannot issue already-issued book
    // Tracks borrower name and date
    // Decrements available copy count
}
```

**DELETE** - Remove Book
```cpp
void deleteBook() {
    // Business rule: Cannot delete issued book
    // Maintains referential integrity
}
```

### 💾 File I/O & Data Persistence

**Data Storage Format:**
```
books.txt:
[ID] [Title] [Author] [ISBN] [Year] [Copies]
[Issued To]
[Issue Date]
[Status]
```

### 📅 Date/Time Management

**Automatic Date Generation** - `YYYY-MM-DD` format

---

## 🎮 Menu System

```
1. Add Book          - Insert new book
2. Display Books     - View all books
3. Search Book       - Find specific book
4. Issue Book        - Borrow book
5. Return Book       - Accept returned book
6. Delete Book       - Remove book
7. Exit              - Save and close
```

---

## 🚀 Getting Started

### Prerequisites
- GCC/Clang C++ compiler
- C++11 or higher standard
- File I/O capable filesystem

### Compilation
```bash
cd 3_Library_Management_System/
g++ -O2 -g -Wall -Wextra -std=c++11 -o library library.cpp
```

### Execution
```bash
./library
```

---

## 📖 Usage Guide

### Authentication
```
Enter username: shan
Enter password: 1903
```

### Adding Books
```
Enter Book ID: 1
Enter book title: C++ Programming Language
Enter book author: Bjarne Stroustrup
Enter book ISBN: 978-0-321-56384-2
Enter publication year: 2013
Enter total copies: 5
Book added successfully!
```

---

## 🎬 Proof of Execution

**Documentation Proof:** `LMS PROOF`

Includes:
- ✅ System initialization and login
- ✅ Complete CRUD operation examples
- ✅ Data persistence across sessions
- ✅ Error handling demonstrations
- ✅ Business rule enforcement

---

## 📁 Files

| File | Size | Purpose |
|------|------|----------|
| `library.cpp` | 11.1 KB | Implementation (295 lines) |
| `README.md` | - | Documentation |
| `LMS PROOF` | 1.8 KB | Execution proof |
| `books.txt` | Dynamic | Auto-created storage |

---

**Status:** ✅ Production Ready | **Quality:** ⭐⭐⭐⭐⭐ | **Enterprise Grade**
