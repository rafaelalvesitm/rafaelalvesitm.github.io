---
---

Aqui seguem alguns trechos de códigos escritos em [[Python]]. 

## Formas diferentes de imprimir variáveis

```python
def hello(name):
	print(f'Hello, {name}')
	print('Hello,', name)
	print('Hello, %s' % name)
```

## Definição de classes

- Defina os valores de init
- Defini o valor da representação com `def __str__(self)`
- Defina os métodos com funções dentro da classe. Podem ter ou não argumentos. 

```python
class Point():
    def __init__(self, x, y):
        self.x = x
        self.y = y  
    
    def multiply(self):
        return self.x * self.y 

	def __str__(self):
		return f"x: {self.x}, y: {self.y}"

point = Point(1,2)
print(f'O ponto {point} tem x*y= {point.multiply()}')

# Resultado
# O ponto x: 1, y: 2 com x = 1 e y = 2 tem x*y= 2
```

## Manipulação de excessões

```python
def spam(divideBy):
	try:
		return 42 / divideBy 
	except ZeroDivisionError as e:
		print('Error: Invalid argument: {}'.format(e))
	finally: 
		print('Division finished')
```