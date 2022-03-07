---
---

O Python pode trabalhar com variáveis individuais ou sequências. Existem vários tipos de sequências que são semelhantes em alguns aspectos, mas diferentes em outros. Ao explicar essas diferenças, usaremos os termos **mutável/imutável** e **ordenado/não ordenado**. 
- **Mutável** significa que, uma vez definida uma sequência, podemos alterar elementos individuais dessa sequência, 
- **Ordenado** significa que a ordem dos objetos é importante.

A seguir tem um resumo dos tipos de squências:

|            Nome            |    Mutável    | Ordenado |
|:--------------------------:|:-------------:|:--------:|
|          Strings           |      Não      |   Sim    |
|       Listas (Lists)       |      Sim      |   Sim    |
|       Tupla (Tuples)       |      Não      |   Sim    |
|      Conjuntos (sets)      | Não se aplica |   Não    |
| Dicionários (Dictionaries) |      Sim      |   Não    |

# Listas

Uma [lista Python](https://www.w3schools.com/python/python_lists.asp) permite armazenar qualquer tipo de variável. Criamos uma lista usando colchetes e vírgulas, conforme mostrado abaixo. Da mesma forma que as strings, podemos imprimir uma lista inteira ou alguns elementos individuais. Também podemos adicionar elementos a uma lista usando `append` e classificar uma lista usando `sort`

``` python
# Este é um comentário em Python
nomes = ["Harry", "Ron", "Hermione"]
# Imprime a lista inteira:
print(nomes)
# Imprime o segundo elemento da lista:
print(nomes[1])
# Adicione um novo nome à lista:
nomes.append("Draco")
# Ordena a lista:
nomes.sort()
# Imprime a nova lista:
imprimir(nomes)
```

# Tupla

[Tuplas](https://www.w3schools.com/python/python_tuples.asp) geralmente são usadas quando você precisa armazenar apenas dois ou três valores juntos, como os valores x e y para um ponto. No código Python, usamos parênteses:

```python
point = (12.5, 10.6)
```

# Conjuntos (Sets)

[Conjuntos](https://www.w3schools.com/python/python_sets.asp) são **não ordenados**. Um conjunto armazenará cada valor apenas uma vez. 

``` python
# Crie um conjunto vazio:
s = set()

# Adicione alguns elementos:
s.add(1)
s.add(2)
s.add(3)
s.add(4)
s.add(3)
s.add(1)

#Remove 2 do conjunto
s.remove(2)

# Imprime o conjunto:
print(s)

# Encontre o tamanho do conjunto:
print(f"O conjunto tem {len(s)} elementos.");

""" Este é um comentário de várias linhas em python:
Saída:
{1, 3, 4}
O conjunto tem 3 elementos.
"""
```

# Dicionários

[Dicionários Python](https://www.w3schools.com/python/python_dictionaries.asp) ou `dict`, é um conjunto de **pares chave-valor**, onde cada chave tem um valor correspondente, assim como em um dicionário, cada palavra (a chave) tem uma definição correspondente (o valor). Em Python, usamos chaves para conter um dicionário e dois pontos para indicar chaves e valores. Por exemplo:

```python
# Define a dictionary
houses = {"Harry": "Gryffindor", "Draco": "Slytherin"}
# Print out Harry's house
print(houses["Harry"])
# Adding values to a dictionary:
houses["Hermione"] = "Gryffindor"
# Print out Hermione's House:
print(houses["Hermione"])

""" Output:
Gryffindor
Gryffindor
"""
```