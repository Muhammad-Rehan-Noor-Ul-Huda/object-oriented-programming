# C++ OOP: Custom String & Date Management

This repository contains my solutions for Object-Oriented Programming (Assignment 2). The project is divided into two tasks focused on manual memory management, operator overloading, and logical algorithms in C++.

## 📂 Project Structure

### Task 1: Custom String Class (`String.h`, `String.cpp`)
A robust implementation of a string class built from scratch without using `std::string`. This task demonstrates low-level memory handling.

* **Dynamic Memory Management:** Uses `new` and `delete` to manage character arrays manually.
* **Deep Copying:** Implements a Copy Constructor and Assignment Operator (`operator=`) to prevent shallow copy issues and handle self-assignment.
* **Functionality:**
    * `at(index)`: specific character access with bounds checking.
    * `Setstring` / `display`: Modifiers and output handlers.
    * Destructors for memory cleanup to prevent memory leaks.

### Task 2: Smart Date Class (`date.h`, `date.cpp`)
A logic-heavy `Date` class capable of handling date arithmetic and validation.

* **Date Arithmetic:** Includes logic to add Days, Months, or Years while automatically handling "rollover" (e.g., adding 40 days moves to the next month/year).
* **Validation:**
    * **Leap Year Logic:** Correctly calculates leap years (divisible by 4 but not 100, unless divisible by 400).
    * **Input Handling:** Ensures days/months are within valid ranges (e.g., February 29 checks).
* **Static Members:** distinct usage of static variables for default dates.

## 🚀 How to Run

1.  **Clone the repo:**
    ```bash
    git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
    ```
2.  **Compile Task 1 (String):**
    ```bash
    g++ "Assignment 2/task 1/main.cpp" "Assignment 2/task 1/String.cpp" -o string_app
    ./string_app
    ```
3.  **Compile Task 2 (Date):**
    ```bash
    g++ "Assignment 2/task 2/main.cpp" "Assignment 2/task 2/date.cpp" -o date_app
    ./date_app
    ```

## 🛠️ Concepts Covered
* Classes & Objects
* Constructors & Destructors
* Operator Overloading
* Deep vs. Shallow Copy
* `const` correctness
* Static data members
