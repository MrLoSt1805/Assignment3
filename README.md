# README

## Project: Calculator Application

### Author
**Name:** Daniel John Jacob  
**PRN:** 23070126027  
**Batch:** 2023-27, AIML A2  

### Overview
This is a simple Java-based calculator application that provides basic arithmetic operations, Fibonacci series calculation, and statistical operations such as mean, variance, and standard deviation. The application allows user input and provides results through a console-based interface.

---

## Files and Classes
### 1. **Calculator.java**
Handles all mathematical calculations.

#### Methods:
- **`double add(double a, double b)`**: Returns the sum of `a` and `b`.
- **`double subtract(double a, double b)`**: Returns the difference between `a` and `b`.
- **`double multiply(double a, double b)`**: Returns the product of `a` and `b`.
- **`double divide(double a, double b)`**: Returns the quotient of `a` divided by `b`. Throws an `ArithmeticException` if `b` is zero.
- **`void printFibonacciSeries(int n)`**: Prints the first `n` Fibonacci numbers.
- **`double sumArray(double[] array)`**: Returns the sum of all elements in `array`.
- **`double meanArray(double[] array)`**: Returns the mean (average) of elements in `array`.
- **`double varianceArray(double[] array)`**: Returns the variance of elements in `array`.
- **`double stdDevArray(double[] array)`**: Returns the standard deviation of elements in `array`.

---

### 2. **Main.java**
Acts as the entry point of the program and manages user interactions.

#### Workflow:
1. Displays a menu for the user to select an operation.
2. Takes user input using the `UserInput` class.
3. Calls the corresponding method from the `Calculator` class.
4. Displays the result.

#### Operations:
- **Addition** (calls `add` method)
- **Subtraction** (calls `subtract` method)
- **Multiplication** (calls `multiply` method)
- **Division** (calls `divide` method)
- **Fibonacci Series** (calls `printFibonacciSeries` method)
- **Sum of Array** (calls `sumArray` method)
- **Mean of Array** (calls `meanArray` method)
- **Variance of Array** (calls `varianceArray` method)
- **Standard Deviation of Array** (calls `stdDevArray` method)
- **Exit** (terminates the program)

---

### 3. **UserInput.java**
Handles user input through the console.

#### Methods:
- **`int getOperationChoice()`**: Reads and returns the user’s menu selection.
- **`double[] getTwoNumbers()`**: Prompts the user for two numbers and returns them as an array.
- **`int getSingleNumber()`**: Prompts the user for a single number and returns it.
- **`double[] getArrayInput()`**: Prompts the user to input an array of numbers and returns it.

---

## How to Run the Application
1. Compile all Java files using:
   ```sh
   javac *.java
   ```
2. Run the program:
   ```sh
   java Main
   ```
3. Follow the on-screen menu to perform operations.

---

## Notes
- The program handles invalid choices with an error message.
- Division by zero is prevented.
- The Fibonacci method currently prints the series instead of returning a value.
- The statistical functions work only with numerical arrays provided by the user.
