# Student Management System in C++

## Overview

The Student Management System is a C++ application developed as part of Western Governors University's C867: Scripting and Programming Applications course. The project simulates the migration of an existing university student information system to a new platform by parsing, storing, validating, and managing student records.

The application demonstrates core Object-Oriented Programming (OOP) concepts, including encapsulation, constructors, accessors and mutators, dynamic memory management, class relationships, and data validation.

---

## Problem Statement

A university needed to migrate student data from an existing system into a new platform developed in C++. The system needed to parse student records, store them in memory, validate data quality, and provide administrative functions for managing student information.

The solution required implementing a Student class and a Roster class to manage student records and perform common operations such as searching, filtering, validation, and reporting.

---

## Features

* Parse student data from raw comma-separated strings
* Store student records using object-oriented design
* Add and remove students from the roster
* Validate student email addresses
* Calculate average days required to complete courses
* Filter students by degree program
* Display complete student roster information
* Dynamically allocate and release memory using pointers and destructors

---

## Technologies Used

* C++
* Object-Oriented Programming (OOP)
* Dynamic Memory Allocation
* Arrays and Pointers
* Enumerations
* String Parsing
* Data Validation

---

## Project Structure

```text
Student-Management-System/
│
├── degree.h
├── student.h
├── student.cpp
├── roster.h
├── roster.cpp
└── main.cpp
```

### degree.h

Defines the DegreeProgram enumeration:

* SECURITY
* NETWORK
* SOFTWARE

### Student Class

Responsible for storing individual student information:

* Student ID
* First Name
* Last Name
* Email Address
* Age
* Days to Complete Courses
* Degree Program

Includes:

* Constructors
* Getters and Setters
* print() method

### Roster Class

Responsible for managing the collection of students.

Includes functionality to:

* Add students
* Remove students
* Print all student records
* Validate email addresses
* Calculate average course completion time
* Filter students by degree program

---

## Key Concepts Demonstrated

### Object-Oriented Programming

* Classes and Objects
* Encapsulation
* Constructors
* Accessor and Mutator Functions
* Separation of Interface and Implementation

### Memory Management

Student objects are dynamically allocated and stored in an array of pointers.

The Roster destructor releases allocated memory to prevent memory leaks.

### Data Parsing

Student records are parsed from raw string input and converted into structured Student objects.

### Data Validation

Email addresses are validated based on the following rules:

* Must contain "@"
* Must contain "."
* Must not contain spaces

Invalid email addresses are identified and displayed.

---

## Example Functionality

### Print All Students

```text
A1    First Name: John    Last Name: Smith
Age: 20
Days In Course: {30,35,40}
Degree Program: SECURITY
```

### Print Invalid Emails

```text
Erickson_1990@gmailcom
The_lawyer99yahoo.com
```

### Print Average Days in Course

```text
A1: 35
A2: 40
A3: 31
```

### Filter by Degree Program

```text
SOFTWARE Students:
A3
A5
```

---

## What I Learned

Through this project I strengthened my understanding of:

* Object-oriented software design
* Working with header and implementation files
* Dynamic memory allocation and destructors
* String manipulation and parsing
* Data validation techniques
* Debugging C++ applications

This project helped build a strong foundation in C++ development and reinforced best practices for designing maintainable software systems.

---

## Future Enhancements

* Replace arrays with STL containers such as vector
* Implement file-based data storage
* Add search functionality
* Build a command-line menu interface
* Add unit tests using a C++ testing framework
* Store student data in a database

---

## Console Output

<img width="1172" height="561" alt="Screenshot 2026-06-12 at 22 47 29" src="https://github.com/user-attachments/assets/77e80e79-8bb4-4d86-8801-6fc1c2118c38" />

