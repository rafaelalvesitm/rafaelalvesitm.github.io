---
---

Redução Mínima Absoluta e [[Algoritmos de regressão|Regressão]] do Operador de Seleção (ou Least Absolute Shrinkage and Selection Operator Regression) aplica um termo de [[Regularização]] nos pesos da [[Regressão linear]]. A regularização aplicada é a [[Regularização L1]]. Essa regularização tende a zerar os pesos dos recursos mais insignificantes. 

A equação da regressão Lasso é dada por:

$$$J(\Theta) = MSE(\Theta)+\alpha\sum_{i=1}^{n}|\Theta_i|$$
