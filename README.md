# Student Data Management System Using Singly Linked List

## Project Overview

The Student Data Management System is a menu-driven C application developed using the Singly Linked List data structure.

The project is designed to manage student records dynamically and demonstrates important C programming concepts such as structures, pointers, dynamic memory allocation, linked lists, searching, sorting, and file handling.

## Objectives

* To implement a student record management system using C.
* To understand and implement a Singly Linked List.
* To use dynamic memory allocation.
* To perform insertion, deletion, searching, and updating operations.
* To sort student records based on roll number.
* To store student information in a file.

## Technologies Used

* Programming Language: C
* Data Structure: Singly Linked List
* Compiler: GCC
* Operating Environment: Linux/Unix
* File Handling: C File I/O

## Student Record Structure

Each student node contains:

* Roll Number
* Student Name
* Marks
* Pointer to the next node

```c
typedef struct student
{
    int rollno;
    char name[40];
    float marks;
    struct student *next;
} SLL;
```

## Features

### 1. Add Student

Adds a new student record to the linked list using dynamic memory allocation.

### 2. Display Students

Displays all student records stored in the linked list.

### 3. Search Student

Searches for a student using the roll number.

### 4. Update Student

Updates the roll number, name, and marks of an existing student.

### 5. Delete Student

Deletes a student record based on the roll number.

### 6. Sort Student Records

Sorts student records in ascending order based on roll number.

### 7. Save File

Stores student information in the `STUDENT.INFO` file.

### 8. Exit

Terminates the application.

## Data Structure

The project uses a Singly Linked List.

```text
HEAD
 |
 v
+---------+---------+-------+------+
| Roll No | Name    | Marks | Next |
+---------+---------+-------+------+
                              |
                              v
                       +---------+---------+-------+------+
                       | Roll No | Name    | Marks | Next |
                       +---------+---------+-------+------+
                                                        |
                                                        v
                                                       NULL
```

## Program Flow

```text
Start
  |
  v
Initialize Linked List
  |
  v
Display Menu
  |
  v
Select Operation
  |
  +--> Add Student
  |
  +--> Display Students
  |
  +--> Search Student
  |
  +--> Update Student
  |
  +--> Delete Student
  |
  +--> Sort by Roll Number
  |
  +--> Save Data to File
  |
  +--> Exit
```

## Sample Student Data

| Roll Number | Name   | Marks |
| ----------: | ------ | ----: |
|         101 | Ravi   | 85.50 |
|         102 | Suresh | 68.50 |
|         103 | Kiran  | 91.00 |
|         104 | Ramesh | 79.50 |
|         105 | Arun   | 72.50 |

## Concepts Demonstrated

* Structures
* Pointers
* Pointer to pointer
* Dynamic memory allocation
* `malloc()`
* `free()`
* Singly Linked List
* Linked List Traversal
* Searching
* Sorting
* String handling
* File handling
* `fopen()`
* `fprintf()`
* `fclose()`
* Menu-driven programming

## File Handling

The student information is saved into:

```text
STUDENT.INFO
```

The program opens the file using:

```c
FILE *fp = fopen("STUDENT.INFO", "w");
```

Student records are written using:

```c
fprintf(fp, "%d %s %.2f\n",
        ptr->rollno,
        ptr->name,
        ptr->marks);
```

## Expected Result

The application successfully performs student record management operations including insertion, display, searching, updating, deletion, sorting, and file storage.

## Future Enhancements

The project can be extended by adding:

* Load records from file at program startup
* Duplicate roll number validation
* Name-based searching
* Marks-based sorting
* Input validation
* Delete all records
* Count total students
* Highest and lowest marks
* Average marks calculation
* Binary file storage
* Graphical user interface

## Conclusion

The Student Data Management System successfully demonstrates the practical implementation of a Singly Linked List in C. The project provides a simple and efficient way to perform basic student record management operations while strengthening concepts related to pointers, dynamic memory allocation, data structures, and file handling.

## Author

**Uday**

## Project Type

Mini Project — C Programming / Data Structures
