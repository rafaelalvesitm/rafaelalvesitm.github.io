---
---

Decorador é uma função de ordem superior que pode modificar outra função. Por exemplo, vamos escrever um decorador que anuncie quando uma função está prestes a começar e quando ela termina. Podemos então aplicar este decorador usando um símbolo `@`.

```python
def announce(f):
    def wrapper():
        print("About to run the function")
        f()
        print("Done with the function")
    return wrapper

@announce
def hello():
    print("Hello, world!")

hello()

""" Output:
About to run the function
Hello, world!
Done with the function
"""
```