---
---

One-hot enconder transfor uma atributo com X categorias em X atributos com dados 0 e 1. 

Assim um atributo preço por exemplo, com categorias barato, médio e caro é transformado em 3 atributos (1 para cada categoria) com valores 1 (se o atributo for verdadeiro) e 0 (se o atributo for falso). 

Essa função está disponível no Scikit-learn através da biblioteca 

```python
from sklearn.preprocessing import OneHotEncoder  
encoder = OneHotEncoder()  
data_1hot = encoder.fit_transform(data)  
data_1hot
```