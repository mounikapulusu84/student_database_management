# Student Record Management System

## Project Overview

The **Student Record Management System** is a menu-driven application developed using the C programming language. It is designed to manage student information efficiently using a Singly Linked List.

The application allows users to add, delete, display, modify, search, sort, save, and retrieve student records. It also supports reversing the linked list and deleting all records.

This project demonstrates the practical implementation of data structures, dynamic memory allocation, modular programming, and file handling in C.

## Key Features

- **Add Records:** Add new student details with automatically assigned unique roll numbers.
- **Delete Records:** Delete student records using roll number or name.
- **Display Records:** View all student details in a clear tabular format.
- **Modify Records:** Update student information by searching with roll number, name, or percentage.
- **Save Records:** Store student information permanently in `student.dat`.
- **Load Records:** Automatically retrieve previously saved records when the application starts.
- **Sort Records:** Arrange records alphabetically by name or in descending order of percentage.
- **Delete All Records:** Remove all records from the linked list and release allocated memory.
- **Reverse List:** Reverse the order of student records by changing linked-list pointers.
- **Exit Options:** Save and exit or exit without saving.

## Technologies and Concepts Used

- Programming Language: C
- Data Structure: Singly Linked List
- Dynamic Memory Allocation: `malloc()` and `free()`
- File Handling: `fopen()`, `fread()`, `fwrite()`, `fclose()`
- Pointers and Structures
- Modular Programming
- Searching and Sorting
- Header Files and Makefile

## Project Structure

| File Name | Description |
|---|---|
| `stud_main.c` | Main function and menu management |
| `stud_add.c` | Adding new student records |
| `stud_del.c` | Deleting student records |
| `stud_show.c` | Displaying student records |
| `stud_mod.c` | Modifying existing records |
| `stud_save.c` | Saving and loading student records |
| `stud_sort.c` | Sorting student records |
| `stud_reverse.c` | Reversing the linked list |
| `stud_delete_all.c` | Deleting all records |
| `student.h` | Structure definition and function declarations |
| `Makefile` | Automates the compilation process |
| `student.dat` | Stores student records |

## Student Record Structure

Each student record contains the following information:

- **Roll Number:** Unique identification number.
- **Name:** Student's name.
- **Percentage:** Student's academic percentage.
- **Next Pointer:** Points to the next node in the linked list.

## Compilation

Make sure you have a C compiler and Make utility installed.

To compile the project using the Makefile:

```bash
make exe
```

## Execution

Run the generated executable:

```bash
./student
```

The application displays a menu and waits for the user to select an operation.

## Data Storage

Student records are stored in a binary file named `student.dat`.

When the application starts, it checks for the saved file and loads the available records. Users can save their current records whenever required.

## Memory Management

Dynamic memory allocation is used to create student nodes at runtime. Whenever a record is deleted, its allocated memory is released using `free()`.

All remaining dynamically allocated nodes are released before the application terminates to avoid memory leaks.

## Learning Outcomes

Through this project, I gained practical experience in:

- Implementing singly linked lists in C.
- Working with structures and pointers.
- Managing memory dynamically.
- Performing searching, sorting, insertion, and deletion operations.
- Handling files for permanent data storage.
- Organizing a C application into multiple source files.
- Using Makefile to simplify compilation.
