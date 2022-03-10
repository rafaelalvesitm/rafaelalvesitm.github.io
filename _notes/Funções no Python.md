---
---

Para definir funções utilize o termo `def` seguido pelo nome da função e entre () seus argumentos, como a seguir: 

```python
def square(x):
    return x * x # Indica o retorno da função. 
```

Podemos então “chamar” esta função da mesma forma que chamamos outras: usando parênteses:

```python
for i in range(10):
    print(f"The square of {i} is {square(i)}")
```