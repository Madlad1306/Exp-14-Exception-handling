# Exception Handling in C++

### Introduction

Exception handling in C++ provides a **structured mechanism** to manage runtime errors or abnormal conditions during program execution. Instead of terminating abruptly, the program can **detect errors**, **throw exceptions**, and **handle them gracefully**.

Key benefits include:

* Separating normal program flow from error-handling code
* Improving program **robustness, readability, and maintainability**
* Minimizing resource leaks through techniques like **RAII**

C++ provides three main keywords for exception handling:

* `try` – defines a block of code that may generate an exception
* `throw` – signals an exception when an error occurs
* `catch` – handles the thrown exception and executes recovery code

---

### Key Concepts

* **try** – Wrap code that might throw an exception.
* **throw** – Raise an exception when an error occurs.
* **catch** – Process the exception and provide a response.

**Additional Features:**

* Multiple `catch` blocks for handling different exception types.
* Exception propagation up the call stack for centralized handling.
* Custom exception classes for user-defined error scenarios.

---

### Importance of Exception Handling

* Prevents unexpected program termination
* Provides meaningful error messages to the user
* Improves program reliability and robustness
* Separates error-handling logic from normal program logic

---

## Algorithms

### 1️⃣ Handle Exception for Age < 18 (Voting Eligibility)

**Algorithm:**

1. Start
2. Input `age` from user
3. Begin `try` block

   * If `age < 18`, `throw age`
   * Else, display "You are eligible to vote."
4. `catch` block

   * If exception occurs, display:
     `"Exception caught: You must be at least 18 years old to vote."`
5. End

---

### 2️⃣ Handle Exception for Divide by Zero

**Algorithm:**

1. Start
2. Input `numerator` and `denominator` from user
3. Begin `try` block

   * If `denominator == 0`, `throw denominator`
   * Else, perform division: `div = numerator / denominator`
   * Display result
4. `catch` block

   * If exception occurs, display:
     `"Exception caught: Division by zero is not possible."`
5. End

---

### Conclusion

Exception handling in C++ ensures that programs can manage errors **systematically** rather than crashing unexpectedly. By using `try`, `throw`, and `catch`:

* Programs become more **stable** and **user-friendly**
* Abnormal conditions can be handled without terminating the program
* Resource leaks and unexpected behavior can be minimized
