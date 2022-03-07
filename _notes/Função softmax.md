---
---

A função softmax também é conhecida por função exponencial normalizada. A função é dada por:

$$\sigma(s(x))_k = \frac{\exp(s_k(x))}{\sum_{j=1}^k\exp(s_j(x))}$$

No qual:
- $K$ é o número de classes
- $s(x)$ é um vetor de pontuações da instância X
- $\sigma(s(x))_k$ é a probabilidade estimada da instância $x$ pertencer a classe $k$ dado os pontos dessa instância para cada classe