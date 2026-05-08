# Library Management System – C++ Console Application

A console-based Library Management System built in C++ for managing book records, librarian operations, and student borrowing/returning functionality.

This project was developed as a semester project for the **CS-101 Computing and AI** course at GIK Institute.

## Repository Contents

This repository contains:

- `main.cpp` - main C++ source code for the Library Management System
- `books.txt` - text file used to store book records after saving
- `Project Documentation` - detailed project report containing scope, features, screenshots, use case diagram, and code explanation
- `README.md` - project overview and run instructions

## Project Description

The Library Management System is a menu-driven C++ program designed to manage basic library operations. It provides separate functionalities for librarians and students.

Librarians can add, view, search, delete, and save book records. Students can view available books, search for books, borrow books, and return books. The system uses file handling to store book data so that records remain available even after the program is closed.

## Features

### Librarian Features

- Add new books to the library
- View all available books
- Search books by unique Book ID
- Delete books by Book ID
- Save book records to a file

### Student Features

- View all available books
- Search books by Book ID
- Borrow books if copies are available
- Return borrowed books

### Data Handling

- Stores book records in `books.txt`
- Loads existing book records when the program starts
- Saves updated records for future use

## Book Details Stored

Each book record contains:

- Book ID
- Book Title
- Author Name
- Publication Year
- Number of Copies

## Program Flow

The program starts with a main menu where the user can choose one of the following roles:

| Option | Role / Action |
|--------|---------------|
| `1` | Librarian |
| `2` | Student |
| `3` | Close Application |

Each role has its own menu with relevant options.

## Important Functions

Some key functions used in the project include:

- `displayMainMenu()` - displays the main menu
- `librarianMenu()` - displays librarian options
- `studentMenu()` - displays student options
- `addBook()` - adds a new book record
- `viewBooks()` - displays all books
- `searchBooks()` - searches for a book by ID
- `deleteBook()` - deletes a book by ID
- `borrowBook()` - allows a student to borrow a book
- `returnBook()` - allows a student to return a book
- `loadBooksFromFile()` - loads saved book records
- `saveBooksToFile()` - saves book records to file

## Concepts Used

This project demonstrates the following C++ concepts:

- Functions
- Arrays
- Character arrays and strings
- File handling
- Input validation
- Menu-driven programming
- Conditional statements
- Loops
- Basic record management
- Console formatting using `iomanip`

## Constraints

- The system supports a maximum of 100 books.
- Each book must have a unique positive Book ID.
- Publication year must be a positive number.
- Number of copies must be greater than zero.
- Book records are stored in `books.txt`.

## How to Run

Make sure you have `g++` installed.

### Compile

```bash
g++ main.cpp -o library_management
