def main():
    # Get input from the user
    try:
        num1 = float(input("Enter the first number: "))
        num2 = float(input("Enter the second number: "))
    except ValueError:
        print("Please enter a valid number.")
        return

    op = input("Enter an operation (+, -, *, /): ")

    # Perform the operation based on user input
    if op == '+':
        result = num1 + num2
    elif op == '-':
        result = num1 - num2
    elif op == '*':
        result = num1 * num2
    elif op == '/':
        if num2 == 0:
            print("Error: Division by zero is not allowed.")
            return
        result = num1 / num2
    else:
        print("Invalid operation.")
        return

    # Print the result
    print(f"{num1} {op} {num2} = {result}")

if __name__ == "__main__":
    main()
