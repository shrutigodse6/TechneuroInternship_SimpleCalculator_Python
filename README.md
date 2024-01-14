# TechneuroInternship_SimpleCalculator_Python
Task 2: 
Simple Calculator:

Create a Python script for basic arithmetic operations such as addition, subtraction, multiplication, and division. It's a hands-on project for Python beginners.

Code Explanation:

1. The program starts with a print statement, displaying information about the calculator and the author:

   print('Simple Calculator for Arithmetic Operations By Shruti Godse\n')
   
   This line prints a header for the simple calculator program.

2. Next, there are four functions defined for basic arithmetic operations - addition, subtraction, multiplication, and division:

   def add(x, y):
    return x + y

   def subtract(x, y):
    return x - y

   def multiply(x, y):
    return x * y

   def divide(x, y):
    if y == 0:
        return "Cannot divide by zero"
    else:
        return x / y
   
   These functions take two parameters (x and y) and perform the corresponding arithmetic operation.
   
4. The program enters a while loop with the condition while True:

   This creates an infinite loop that will continue until the user decides to exit by choosing option 5.

5. Inside the loop, the program displays a menu of operations and prompts the user to enter a choice:

   print("Select operation:")
   print("1. Addition")
   print("2. Subtraction")
   print("3. Multiplication")
   print("4. Division")
   print("5. Exit")
   choice = input("Enter choice (1/2/3/4/5): ")

6. If the user enters '5', the program prints a farewell message and breaks out of the loop, effectively ending the calculator:

  if choice == '5':
    print("Exiting the calculator. Goodbye!")
    break
    
7. If the user enters a valid operation choice (1, 2, 3, or 4), the program prompts the user to enter two numbers and performs the selected operation:

  num1 = float(input("Enter first number: "))
  num2 = float(input("Enter second number: "))
  
  The program then uses the appropriate function (add, subtract, multiply, or divide) to perform the operation and prints the result.

8. If the user enters an invalid choice, the program displays an error message:

   else:
       print("Invalid Input. Please enter a valid option.")
   
   The loop continues, allowing the user to perform more calculations until choosing option 5 to exit the calculator.
