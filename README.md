# calculator-In-Cognorise


# CALCULATOR APP
def calculator():
    print("Simple Calculator")

    num1 = int(input("Enter the 1st number: "))
    num2 = int(input("Enter the 2nd number: "))

    print("1. Addition (+)")
    print("2. Subtraction (-)")
    print("3. Multiplication (*)")
    print("4. Division (//)")

    #Choose an operation
    operation = input("\nChoose an operation ( + | - | * | // ): ")

    if operation == '+':
        result = num1 + num2
        print(f"\nResult: {num1} + {num2} = {result}")
    elif operation == '-':
        result = num1 - num2
        print(f"\nResult: {num1} - {num2} = {result}")
    elif operation == '*':
        result = num1 * num2
        print(f"\nResult: {num1} * {num2} = {result}")
    elif operation == '//':
        # Check if the second number is zero for division
        if num2 != 0:
            result = num1 // num2
            print(f"\nResult: {num1} // {num2} = {result}")
        else:
            print("\nError: Division with zero is not allowed.")
    else:
        print("\nInvalid operation. Please choose +, -, *, or //.")


calculator()
