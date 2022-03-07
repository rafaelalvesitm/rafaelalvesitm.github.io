---
---

A [[Algoritmos de regressão|regressão]] de rede elástica é um meio termo entre a [[Regressão de cume]] e a [[Regressão Lasso]] onde a regularazação é dada pela mistura da [[Regularização L1]] e da [[Regularização L2]] através do termo $r$. A equação é dada a seguir:

$$$J(\Theta) = MSE(\Theta)+r\alpha\sum_{i=1}^{n}|\Theta_i| + \frac{1-r}{2}\alpha\sum_{i=1}^{n}\Theta_i^2$$