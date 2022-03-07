---
---

É possível [tratar exceções no Python](https://www.w3schools.com/python/python_try_except.asp). No bloco de código a seguir, vamos tentar (`try`) dividir os dois números, exceto (`except`) quando obtivermos um erro de divisão por zero (`ZeroDivisionError`):

```python
import sys

try:
    x = int(input("x: "))
    y = int(input("y: "))
except ValueError:
    print("Error: Invalid input")
    sys.exit(1)

try:
    result = x / y
except ZeroDivisionError:
    print("Error: Cannot divide by 0.")
    # Exit the program
    sys.exit(1)

print(f"{x} / {y} = {result}")
```