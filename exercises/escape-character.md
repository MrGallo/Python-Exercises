# Escape character

With the starter code (given in `main.py`) your program will encounter a `SyntaxError`.

1. Run the program as is. Notice the `SyntaxError`. On what line of the code does the error tell you it found the problem?
    ```
      File "main.py", line 2
        print("Her friend said "Nice to see you!".")
                                ^
    SyntaxError: invalid syntax
    ```
    - Python gets confused with the extra quotes (`"`) in the second print statement.
    - Python uses quotes to determine where a string starts and where a string ends. If we want to actually include a quote in a string, we need to **escape** that quote with the escape character `\`. This will tell Python to skip over that particular quote and to not use it to end the string.
2. Comment-out the second print statement by putting a number-sign (hashtag) infront of the line. For example:
    ```python
    # print(...)
    ```
3. Run the program and observe what the first print statement outputs. Notice:
    - there is no error,
    - the output actually contains the quote characters
    - what is output to the terminal doesn't actually contain the escape characters `\`.
4. Use the escape character (`\`) to allow the second print statement to include the quotes. Be sure to use the first print statement as an example for how to do this correctly. Also, remember to un-comment the second print statement, when you are ready to run it. The final output should look like:
    ```
    She said "Hello" to her friend.
    Her friend said "Nice to see you!".
    ```