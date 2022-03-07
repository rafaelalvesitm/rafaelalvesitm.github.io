---
---

Também conhecido como regularização de Tikhonov é uma versão regularizada da [[Regressão linear]], ou seja é um [[Algoritmos de regressão]], onde um termo de [[Regularização]] é aplicado. A regularização utilizada é a [[Regularização L2]] . 

A fórmula da regressão de cume é dada por:

$$$J(\Theta) = MSE(\Theta)+\alpha\frac{1}{2}\sum_{i=1}^{n}\Theta_i^2$$

Nota-se que o viés $\Theta_0$ não é regularizado. 

Ou na forma fechada:

$$\hat{\Theta} = (X^TX+\alpha A)^{-1}X^Ty$$

Utilizando o Scikit-learn tem-se:

```python 
from sklearn.linear_model import Ridge  
ridge_reg = Ridge(alpha=1, solver="cholesky")  
ridge_reg.fit(X, y)
ridge_reg.predict([[1.5]])
```