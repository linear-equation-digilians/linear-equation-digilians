#  Linear Equation System Manager (C++)

A console-based C++ application for managing and solving systems of
linear equations using Object-Oriented Programming principles.

------------------------------------------------------------------------

##  Overview

This project implements a **Linear Equation System Manager** that allows
users to:

-   Input multiple linear equations
-   Parse equations dynamically
-   Manage variables automatically
-   Perform matrix operations
-   Compute determinants
-   Apply Cramer's Rule
-   Solve the system
-   Perform substitution
-   Add and subtract equations

The system is built using clean OOP design and modular architecture.

------------------------------------------------------------------------

##  Project Architecture

### 1️ Equation Class

Responsible for: - Storing coefficients - Storing constant term -
Performing equation operations (Addition, Subtraction, Scalar
multiplication) - Converting equation to formatted string - Debug
printing

### 2️ EquationManager Class

Responsible for: - Reading equations from user - Parsing equation
strings - Managing global variable list - Building coefficient matrix -
Computing determinant - Generating Cramer matrices - Performing
substitution - Solving system - Executing user commands

------------------------------------------------------------------------

 Project Structure
Linear-Equation-System
│
├── ConsoleApplication1.cpp
│   └── Main entry point of the application
│
├── Equation.h
│   └── Declaration of the Equation class
│
├── Equation.cpp
│   └── Implementation of the Equation class
│
├── EquationManager.h
│   └── Declaration of the EquationManager class
│
├── EquationManager.cpp
│   └── Implementation of equation management logic
│
├── Linear_Equation_System_Documentation.pdf
│   └── Project documentation
│
└── README.md
    └── Project description and instructions

------------------------------------------------------------------------
⚙️ How It Works

The program allows users to create and store linear equations.
Each equation is represented using an Equation class, while an EquationManager class manages a collection of equations and performs operations between them.

Example operations supported:

Adding two equations

Subtracting two equations

Viewing all stored equations

------------------------------------------------------------------------

How to Run

Clone the repository

git clone https://github.com/rabea-shaban/Linear-Equation-System.git

Open the project in Visual Studio or any C++ IDE.

Build and run the project.

------------------------------------------------------------------------
Test Case
Input Equations
<p>3</p>
<p>2x1 + 3x2 + 4x3 = 16</p>
<p>3x1 + 1x2 + 2x3 = 13</p>
<p>1x1 + 2x2 + 1x3 = 8</p>




The first number represents the number of equations and variables.

Level 1 Operations
Print Number of Variables

Command

num_vars

Output

3
Print Equation

Command

equation 2

Output

1x1 + 2x2 + 1x3 = 8
Print Column of Variable

Command

column x2

Output

3
2
1
Level 2 Operations
Add Equations

Command

add 1 3

Result

(2x1 + 3x2 + 4x3 = 16)
+
(3x1 + 1x2 + 2x3 = 13)

= 5x1 + 4x2 + 6x3 = 29
Subtract Equations

Command

subtract 1 3

Result

(2x1 + 3x2 + 4x3 = 16)
-
(3x1 + 1x2 + 2x3 = 13)

= -1x1 + 2x2 + 2x3 = 3
Substitute Variable

Command

substitute x2 1 3

Meaning

Substitute variable x2 in equation 1 using equation 3 and remove it from equation 1.

Level 3 Operations
Print Coefficient Matrix

Command

D

Output

| 2  3  4 |
| 1  2  1 |
| 3  1  2 |
Cramer's Matrix for x1

Command

D x1

Replace column x1 with constants.

Determinant Value

Command

D_value

Output

Determinant = -9
Solve the System

Command

solve

Output

x1 = 2
x2 = 1
x3 = 2
No Solution Case

If the system has no valid solution the program prints:

No Solution

------------------------------------------------------------------------
# How to Run

Follow these steps to run the project on your machine.

### 1. Clone the Repository

```bash
git clone https://github.com/linear-equation-digilians/linear-equation-digilians.git
```

### 2. Open the Project

Open the project using **Visual Studio** or any C++ IDE.

### 3. Build the Project

Compile the project using your IDE or a C++ compiler.

Example using g++:

```bash
g++ ConsoleApplication1.cpp Equation.cpp EquationManager.cpp -o linear_solver
```

### 4. Run the Program

```bash
./linear_solver
```

The program will start and you can enter the equations and commands.

---

# Repository

Project Repository:

```bash
https://github.com/linear-equation-digilians/linear-equation-digilians
```

---


---

# License

This project is developed for educational purposes.

------------------------------------------------------------------------



##  Features

-   Dynamic variable detection\
-   Equation parsing from text input\
-   Matrix construction\
-   Determinant calculation\
-   Cramer's Rule implementation\
-   Equation addition and subtraction\
-   Variable substitution\
-   Formatted equation printing

------------------------------------------------------------------------

##  Technologies Used

-   C++
-   Standard Template Library (STL)
-   Object-Oriented Programming
-   Matrix mathematics

------------------------------------------------------------------------

##  How to Run

### Using Visual Studio

1.  Open the solution file.
2.  Build the solution.
3.  Run the project.

### Using g++

g++ ConsoleApplication1.cpp Equation.cpp EquationManager.cpp -o solver
./solver

------------------------------------------------------------------------

##  Mathematical Techniques Used

-   Matrix Representation of Linear Systems
-   Determinant Calculation (Recursive Method)
-   Cramer's Rule
-   Row-based Equation Operations

------------------------------------------------------------------------

##  Limitations

-   Floating-point precision limitations
-   Determinant recursion may be inefficient for very large matrices

------------------------------------------------------------------------

##  Future Improvements

-   Gaussian Elimination implementation
-   Performance optimization
-   GUI version
-   Step-by-step solving visualization

------------------------------------------------------------------------

##  Project Team

-   Sama Yasser Gemeay -- 12265
-   Hager Sherif Ibrahim -- 12266
-   Rabea Shaban Ibrahim -- 11219

------------------------------------------------------------------------

## Academic Purpose

This project was developed as part of the **Fundamentals of Programming** course at **Digilians**.  
The main objective of this project is to apply Object-Oriented Programming (OOP) principles and implement matrix-based methods to solve systems of linear equations programmatically.
