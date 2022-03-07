---
---

A descida de gradiente em lote opera através de derivadas parciais. Cada derivada parcial será calculada com base em um parâmetro a ser analisado. 

Exemplo para o [[Erro médio quadrático]]:

$$\frac{\partial}{\partial\theta_j}EQM(\theta) = \frac{2}{m} \sum_{i=1}^{m}(\theta^Tx^{(i)}-y^{(i)})x_j^{(i)}$$

Para algoritmos [[Aprendizagem de máquina]] tem-se o seguinte:

$$\nabla_{\theta}EQM(\theta) = \frac{2}{m}X^T(X\theta-y)$$

Desta forma o gradiente descendente em lote trabalho com todo o data set de uma vez. Uma vez calculado o gradiente descendente tem-se:

$$\theta^{(\text{novo)}} = \theta - \eta \nabla_{\theta}EQM(\theta)$$

- $\eta$ é a taxa de aprendizagem.

A taxa de aprendizagem influência no tempo que o método demora para convergir. Uma taxa pequena demais pode demorar muito para convergir e uma taxa muito grande pode nunca convergir. Escolha uma taxa baixa e defini uma tolerância para a mudança de um passo para outro. 