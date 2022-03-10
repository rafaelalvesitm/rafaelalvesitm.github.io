---
---

As funções do Lambda fornecem uma forma prática de definir funções de apenas entrada e saida, como exemplificado abaixo 

```python
square = lambda x: x * x # lambda entrada: saída
```


Isso pode ser útil quando não queremos escrever uma função inteira separada para um único e pequeno uso. Como exemplo tem-se a ordenação de um dicionário: 

```python
people = [
    {"name": "Harry", "house": "Gryffindor"},
    {"name": "Cho", "house": "Ravenclaw"},
    {"name": "Draco", "house": "Slytherin"}
]

people.sort(key=lambda person: person["name"]) # Person recebe 1 item do dicionário. 

print(people)

""" Output:
[{'name': 'Cho', 'house': 'Ravenclaw'}, {'name': 'Draco', 'house': 'Slytherin'}, {'name': 'Harry', 'house': 'Gryffindor'}]
"""
```