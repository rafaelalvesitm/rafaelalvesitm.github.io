---
---

## Formatando Strings

Strings podem ser formatadas de diversas formas como por exemplo: 

``` python
name = "Eric"
print("Olá, %s." % name) # Chamando com um marcador de posição
print("Olá, {}.".format(name)) # Chamando com a função format
print(f"Olá, {name}.") # Chamando com a indicação de formatação
print(f"Olá, {name.lower()}") # Chamando com uma função. 
```

A versão com indicação de formatação, também conhecido como f-string, são recomendadas e também é mais rápido executar esse tipo de formatação. 

## Strings

Pode-se pensar em uma string como uma sequência de caracteres. Isso significa que é possível acessar elementos individuais dentro da string! Por exemplo:

``` python
nome = "Harry"
print(nome[0]) # Imprime o primeiro caracter 'H'
print(nome[1]) # Imprime o segundo caracter 'a'
```