# Calculator on C++

**Description:**

This C++ program is a console-based calculator that performs basic arithmetic operations: addition, subtraction, multiplication, and division. The user inputs two numbers and selects an operation to receive the result.

## Explanation of the methods used in the code:

### 1. `showMenu`
- Purpose: This function displays the calculator's menu options to the user and captures their choice.
- Input: No parameters are passed to this function.
- Output: It returns an integer representing the user's choice.
  #### **Key Logic:**
- Uses cout to display the menu options.
- Reads the user input using cin.
- Returns the input to the caller.

### 2. `main` Function

The `main` function is the entry point of the program and contains the primary logic flow.

  #### Key Roles of `main`:

 1. Initialize Variables:

    - `num1` and `num2` store the input numbers.
    - choice holds the menu selection returned by `showMenu`.

2. Loop:

    - A `while (true)` loop ensures the calculator keeps running until the user chooses to exit.
    - Inside the loop:
      
        - `showMenu` is called to display options and capture the user's choice.
        - If the choice is `5` (Exit), the program prints a goodbye message and breaks the loop.

3. Input Numbers:

    - After the user selects an operation, the program prompts for two numbers using `cin`.

4. Switch Statement:

    - The `switch` block handles the operation based on the value of `choice`:
    
    - **Case 1:** Addition.
    - **Case 2:** Subtraction.
    - **Case 3:** Multiplication.
    - **Case 4:** Division (with a check for division by zero).
    - **Default Case:** Handles invalid input.

5. Output Results:

    - The results of operations are displayed using `cout`.
    - For division, if the denominator is zero, the program shows an error message.

6. Program Continuation:

    - After displaying the result or error, the program loops back to allow another operation.
