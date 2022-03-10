---
---

É possível escrever funções em um arquivo e executá-las em outro. Pode-se por exemplo definir uma função `square` (eleva ao quadrado) em um arquivo chamado `functions.py` e executar em outro arquivo usando

```python
from functions import square

for i in range(10):
    print(f"The square of {i} is {square(i)}")
```

Ou alternativamente:

```python
import functions

for i in range(10):
    print(f"The square of {i} is {functions.square(i)}")
```