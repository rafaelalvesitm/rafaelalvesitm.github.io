---
---

Uma [Classe Python](https://www.w3schools.com/python/python_classes.asp) é essencialmente um modelo para um novo tipo de objeto que pode armazenar informações e realizar ações. Aqui está uma classe que define um ponto bidimensional:

```python
class Point():
    # A method defining how to create a point:
    def __init__(self, x, y):
        self.x = x
        self.y = y
```

Observe que no código acima, usamos a palavra-chave `self` para representar o objeto com o qual estamos trabalhando atualmente. `self` deve ser o primeiro argumento para qualquer método dentro de uma classe Python.

Para usar a classe tem-se: 

```python
p = Point(2, 8)
print(p.x)
print(p.y)
```

Para um exemplo mais complexo tem-se:

```python
class Flight():
    # Method to create new flight with given capacity
    def __init__(self, capacity):
        self.capacity = capacity
        self.passengers = []

    # Method to add a passenger to the flight:
    def add_passenger(self, name):
        if not self.open_seats():
            return False
        self.passengers.append(name)
        return True

    # Method to return number of open seats
    def open_seats(self):
        return self.capacity - len(self.passengers)
```

Dessa forma é possível definir:
- Um voo com base em sua capacidade e passageiros (inicialmente vazio)
- Avaliar quantos assentos estão disponíveis
- Adicionar um passageiro caso exista um assento disponível. 