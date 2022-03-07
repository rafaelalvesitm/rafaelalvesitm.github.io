---
---

Links: [[Aprendizado supervisionado]]; [[Algoritmos de regressão]]

Esse algoritmo pode ser utilizado para [[Algoritmos de regressão|regressão]] mas também é comumente utilizado para [[Algoritmos de classificação|classificação]]. É usado para estimar a a probalidade de algo pertencer a determinada categoria (por isso dá para utilizar esse método para classificação). 

Também calcula a soma ponderada dos recursos de entrada mais um viés e tem como saida a  logística desse resultado. A equação do modelo é dada por:

$$\hat{p} = h_\theta(x) = \sigma(X^T\Theta)$$

no qual a função $\sigma$ é a [[Função sigmoide]]. 

Uma vez que o modelo calculou $\hat{p}$ é possível utilizar tal probalidadade para classificar os dados sendo:

$$\hat{y} = \begin{cases} 0 \text{ if } \hat{p} <0.5 \\ 1 \text{ if } \hat{p} \geq0.5\end{cases}$$

O treinamento do modelo é feito com base na estimativa do vetor $\Theta$ sendo que o modelo estima uma alta probabilidade para instâncias positivas $(y=1)$ e baixas probabilidades para instâncias negativas $(y=0)$. A função de custo para o treinamento do modelo logistico é dado por:

$$J(\Theta) = -\frac{1}{m}\sum_{i=1}^m[y^{(i)}\log(\hat{p}^{(i)})+(1-y^{(i)})\log(1-\hat{p}^{(i)})$$

Essa função é convexa logo qualquer algoritmo de [[Descida de gradiente]] encontrará o mímimo da função dado uma taxa de aprendizagem e tempo adequados. 