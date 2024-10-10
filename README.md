# codsoftassignment
https://www.linkedin.com/feed/update/urn:li:activity:7243151603355017216?updateEntityUrn=urn%3Ali%3Afs_updateV2%3A%28urn%3Ali%3Aactivity%3A7243151603355017216%2CFEED_DETAIL%2CEMPTY%2CDEFAULT%2Cfalse%29
CALCULATOR
 Design a simple calculator with basic arithmetic operations.
 Prompt the user to input two numbers and an operation choice.
 Perform the calculation and display the result.

 code:
 # calculator.py
def calculator():
    print("----------------")
    print("Simple Calculator")
    print("----------------")

    num1 = float(input("Enter the first number: "))
    num2 = float(input("Enter the second number: "))
    operation = input("Enter the operation (+, -, *, /): ")

    if operation == "+":
        result = num1 + num2
    elif operation == "-":
        result = num1 - num2
    elif operation == "*":
        result = num1 * num2
    elif operation == "/":
        if num2 != 0:
            result = num1 / num2
        else:
            print("Error: Division by zero!")
            return
    else:
        print("Error: Invalid operation!")
        return
    print(f"Result: {num1} {operation} {num2} = {result:.2f}")

if __name__ == "__main__":
    calculator()
