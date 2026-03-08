# Linear Equation System Manager (C++)

A console-based **C++ application** for managing and solving systems of
linear equations using **Object-Oriented Programming (OOP)** principles.

------------------------------------------------------------------------

# Overview

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

The system is built using **clean OOP design and modular architecture**.

------------------------------------------------------------------------

# Project Architecture

## Equation Class

Responsible for:

-   Storing coefficients
-   Storing the constant term
-   Performing equation operations
-   Addition, subtraction, and scalar multiplication
-   Converting equation to formatted string
-   Debug printing

------------------------------------------------------------------------

## EquationManager Class

Responsible for:

-   Reading equations from user input
-   Parsing equation strings
-   Managing the global variable list
-   Building the coefficient matrix
-   Computing determinant
-   Generating Cramer matrices
-   Performing substitution
-   Solving the system
-   Executing user commands

------------------------------------------------------------------------

# Project Structure

Linear-Equation-System │ ├── ConsoleApplication1.cpp ├── Equation.h ├──
Equation.cpp ├── EquationManager.h ├── EquationManager.cpp ├──
Linear_Equation_System_Documentation.pdf └── README.md

------------------------------------------------------------------------

# How It Works

The program allows users to create and store linear equations.

Each equation is represented using an **Equation class**, while an
**EquationManager class** manages a collection of equations and performs
operations between them.

Supported operations:

-   Adding equations
-   Subtracting equations
-   Viewing stored equations
-   Solving linear systems

------------------------------------------------------------------------

# Test Case

Input:

3 2x1 + 3x2 + 4x3 = 16 1x1 + 2x2 + 1x3 = 8 3x1 + 1x2 + 2x3 = 13

------------------------------------------------------------------------

# Level 1 Operations

num_vars

Output

3

equation 2

Output

1x1 + 2x2 + 1x3 = 8

column x2

Output

3 2 1

------------------------------------------------------------------------

# Level 2 Operations

add 1 3

Result

(2x1 + 3x2 + 4x3 = 16) + (3x1 + 1x2 + 2x3 = 13)

= 5x1 + 4x2 + 6x3 = 29

subtract 1 3

Result

## (2x1 + 3x2 + 4x3 = 16)

(3x1 + 1x2 + 2x3 = 13)

= -1x1 + 2x2 + 2x3 = 3

------------------------------------------------------------------------

# Level 3 Operations

D

Output

| 2 3 4 \|
| 1 2 1 \|
| 3 1 2 \|

D_value

Output

Determinant = -9

solve

Output

x1 = 2 x2 = 1 x3 = 2

------------------------------------------------------------------------

# Features

-   Dynamic variable detection
-   Equation parsing from text input
-   Matrix construction
-   Determinant calculation
-   Cramer's Rule implementation
-   Equation addition and subtraction
-   Variable substitution
-   Formatted equation printing

------------------------------------------------------------------------

# Technologies Used

-   C++
-   Standard Template Library (STL)
-   Object-Oriented Programming (OOP)
-   Matrix mathematics

------------------------------------------------------------------------

# How to Run

Compile:

g++ ConsoleApplication1.cpp Equation.cpp EquationManager.cpp -o solver

Run:

./solver

------------------------------------------------------------------------

# Repository

https://github.com/linear-equation-digilians/linear-equation-digilians

------------------------------------------------------------------------

# Contributors

-   Rabea Shaban
-   Team Members

------------------------------------------------------------------------

# Academic Purpose

This project was developed as part of the **Fundamentals of
Programming** course.
