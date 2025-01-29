
### 1. **Hello World**
```python
# Program to print "Hello, World!"
print("Hello, World!")
```

### 2. **Sum of Two Numbers**
```python
# Program to add two numbers
num1 = float(input("Enter the first number: "))
num2 = float(input("Enter the second number: "))
sum = num1 + num2
print(f"The sum is: {sum}")
```

### 3. **Check Even or Odd**
```python
# Program to check if a number is even or odd
num = int(input("Enter a number: "))
if num % 2 == 0:
    print(f"{num} is Even")
else:
    print(f"{num} is Odd")
```

### 4. **Find the Largest of Three Numbers**
```python
# Program to find the largest of three numbers
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))
num3 = float(input("Enter third number: "))
largest = max(num1, num2, num3)
print(f"The largest number is: {largest}")
```

### 5. **Simple Calculator**
```python
# Program for a simple calculator
def add(x, y):
    return x + y
def subtract(x, y):
    return x - y
def multiply(x, y):
    return x * y
def divide(x, y):
    return x / y

print("Select operation:")
print("1. Add")
print("2. Subtract")
print("3. Multiply")
print("4. Divide")

choice = input("Enter choice (1/2/3/4): ")

num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))

if choice == '1':
    print(f"{num1} + {num2} = {add(num1, num2)}")
elif choice == '2':
    print(f"{num1} - {num2} = {subtract(num1, num2)}")
elif choice == '3':
    print(f"{num1} * {num2} = {multiply(num1, num2)}")
elif choice == '4':
    print(f"{num1} / {num2} = {divide(num1, num2)}")
else:
    print("Invalid input")
```

### 6. **Factorial of a Number (Using Recursion)**
```python
# Program to find factorial using recursion
def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n - 1)

num = int(input("Enter a number: "))
print(f"The factorial of {num} is: {factorial(num)}")
```

### 7. **Fibonacci Sequence**
```python
# Program to print Fibonacci sequence up to n terms
def fibonacci(n):
    a, b = 0, 1
    for _ in range(n):
        print(a, end=" ")
        a, b = b, a + b

num = int(input("Enter the number of terms: "))
print("Fibonacci sequence:")
fibonacci(num)
```

### 8. **Palindrome Checker**
```python
# Program to check if a string is a palindrome
def is_palindrome(string):
    return string == string[::-1]

string = input("Enter a string: ")
if is_palindrome(string):
    print(f"{string} is a palindrome")
else:
    print(f"{string} is not a palindrome")
```

### 9. **Count Vowels and Consonants**
```python
# Program to count vowels and consonants
def count_vowels_and_consonants(string):
    vowels = "aeiouAEIOU"
    vowels_count = sum(1 for char in string if char in vowels)
    consonants_count = sum(1 for char in string if char.isalpha() and char not in vowels)
    return vowels_count, consonants_count

string = input("Enter a string: ")
vowels, consonants = count_vowels_and_consonants(string)
print(f"Vowels: {vowels}, Consonants: {consonants}")
```

### 10. **Sum of List Elements**
```python
# Program to find the sum of elements in a list
numbers = [1, 2, 3, 4, 5]
sum_of_elements = sum(numbers)
print(f"The sum of the list elements is: {sum_of_elements}")
```

### 11. **Find the Prime Numbers**
```python
# Program to print prime numbers up to a given number n
def is_prime(num):
    if num <= 1:
        return False
    for i in range(2, int(num**0.5) + 1):
        if num % i == 0:
            return False
    return True

n = int(input("Enter the number: "))
print("Prime numbers up to", n, "are:")
for i in range(2, n + 1):
    if is_prime(i):
        print(i, end=" ")
```

### 12. **Print Multiplication Table**
```python
# Program to print multiplication table of a number
num = int(input("Enter a number: "))
for i in range(1, 11):
    print(f"{num} x {i} = {num * i}")
```

### 13. **Reverse a String**
```python
# Program to reverse a string
string = input("Enter a string: ")
reversed_string = string[::-1]
print(f"The reversed string is: {reversed_string}")
```

### 14. **Count Words in a String**
```python
# Program to count words in a string
string = input("Enter a sentence: ")
words = string.split()
word_count = len(words)
print(f"The number of words is: {word_count}")
```

### 15. **Find the Common Elements Between Two Lists**
```python
# Program to find common elements between two lists
list1 = [1, 2, 3, 4, 5]
list2 = [4, 5, 6, 7, 8]
common_elements = set(list1) & set(list2)
print(f"The common elements are: {common_elements}")
```

### 16. **Create a Dictionary**
```python
# Program to create a dictionary
person = {"name": "John", "age": 30, "city": "New York"}
print(person["name"])  # Output: John
```

### 17. **Sum of Digits**
```python
# Program to calculate the sum of digits
num = int(input("Enter a number: "))
sum_of_digits = sum(int(digit) for digit in str(num))
print(f"The sum of digits is: {sum_of_digits}")
```

### 18. **Check for Armstrong Number**
```python
# Program to check Armstrong number
def is_armstrong(num):
    num_str = str(num)
    power = len(num_str)
    return num == sum(int(digit) ** power for digit in num_str)

num = int(input("Enter a number: "))
if is_armstrong(num):
    print(f"{num} is an Armstrong number")
else:
    print(f"{num} is not an Armstrong number")
```

### 19. **Remove Duplicates from List**
```python
# Program to remove duplicates from a list
numbers = [1, 2, 3, 4, 4, 5, 5]
unique_numbers = list(set(numbers))
print(f"List after removing duplicates: {unique_numbers}")
```

### 20. **Create a Simple ATM Machine**
```python
# Program to simulate a simple ATM machine
balance = 1000

def check_balance():
    print(f"Your balance is: ${balance}")

def deposit():
    amount = float(input("Enter amount to deposit: "))
    global balance
    balance += amount
    print(f"Deposited ${amount}. New balance: ${balance}")

def withdraw():
    amount = float(input("Enter amount to withdraw: "))
    global balance
    if amount <= balance:
        balance -= amount
        print(f"Withdrew ${amount}. New balance: ${balance}")
    else:
        print("Insufficient funds!")

while True:
    print("\nATM Menu:")
    print("1. Check balance")
    print("2. Deposit")
    print("3. Withdraw")
    print("4. Exit")
    choice = input("Enter your choice: ")

    if choice == '1':
        check_balance()
    elif choice == '2':
        deposit()
    elif choice == '3':
        withdraw()
    elif choice == '4':
        print("Thank you for using the ATM!")
        break
    else:
        print("Invalid choice!")
```