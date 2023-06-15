# go_greetings

This is the first code for your module. It returns a greeting to any caller that asks for one.
  
In this code, you:

- Declare a greetings package to collect related functions.
- Implement a Hello function to return the greeting.
    This function takes a name parameter whose type is string. The function also returns a string. In Go, a function whose name starts with a capital letter can be called by a function not in the same package. This is known in Go as an exported name. For more about exported names, see Exported names in the Go tour.

    ![Function syntax](function-syntax.png)
- Declare a message variable to hold your greeting.
    In Go, the := operator is a shortcut for declaring and initializing a variable in one line (Go uses the value on the right to determine the variable's type). Taking the long way, you might have written this as:
    ```
    var message string
    message = fmt.Sprintf("Hi, %v. Welcome!", name)
    ```
- Use the fmt package's `Sprintf` function to create a greeting message. The first argument is a format string, and `Sprintf` substitutes the name parameter's value for the `%v` format verb. Inserting the value of the name parameter completes the greeting text.
- Return the formatted greeting text to the caller.