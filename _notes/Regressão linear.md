---
---

Links: [[Aprendizado supervisionado]]; [[Algoritmos de regressão]]

A [[Algoritmos de regressão|regressão]] linear é um modelo que considera uma ponderação da soma dos recursos de entrada mais uma constante chama de viés. A formula a seguir indica a equação do modelo. 

$$   \hat{y} = \theta_0 + \theta_1x_1 + \theta_2x_2 + ⋯ + \theta_nx_n $$

- $\hat{y}$ é o valor da predição.
- $n$ é o número de recursos
- $x_i$ é o valor do recurso na posição i
- $\theta_j$ é o valor do peso na posição j (começa em $\theta_0$)

Na forma vetorizada tem-se:

$$\hat{y} = h_\theta(x) = \theta \cdot x$$

- $\theta$ é o vetor de parametrização contendo os pesos $\theta_0$ até $\theta_n$  
- $x$ é o vetor de uma instância dos recursos contendo $x_o$ até $x_n$, sendo $x_0$ sempre igual a 1
- $h_\theta(x)$ é a função hipótese utilizando os parametros $\theta$

No Sci-Kit learn tem-se:

```python
from sklearn.linear_model import LinearRegression #Import the model
lin_reg = LinearRegression() # Define the model
lin_reg.fit(X, y) # Fit the data in the model
lin_reg.intercept_, lin_reg.coef_ # Show coeficcients Beta 0 and Beta 1
```


Para encontrar os melhores parâmetros para a regressão linear pode-se utilizar 2 abordagens:

- [[Equação normal]] com ou sem [[Matrix pseudoinversa]]
- [[Descida de gradiente]]

Compração entre os métodos. 

![[Pasted image 20210831091235.png]]