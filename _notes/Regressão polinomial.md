---
---

Links: [[Aprendizado supervisionado]]; [[Algoritmos de regressão]]

A regressão polinomial é uma [[Regressão linear]] em que os dados de entrada são transformados através do seu quadrado, cubo, multiplicação entre elementos etc. Após tal transformação uma regressão linear é utilizada para encontrar a equação de ajuste dos dados. 

- No Scikit learn tem-se a função `PolynomialFeatures(degree=d)` que transforma um vetor contendo n recursos em um vetor contendo $\frac{(n+d)!}{d!n!}$ recursos. 