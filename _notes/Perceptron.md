---
---

O perceptron é baseado na [[Unidade Lógica de Limite]] sendo nada mais do que uma camada de unidades agrupadas mais um  valor de viés. 

$$   h_{W, b}(X) = \phi(XW + b)$$

- Sendo $X$ a matriz dos dados de entrada. 
- $W$ é a matrix com os pesos exceto o viés. 
- $b$ é o vetor de viéses.
- A função $\phi$ é a função de ativação, no caso de perceptrons são funções degraus. 

![[Perceptron.png]]

O aprendizado do perceptron é realizado com base na [[Regra de Hebb]], no qual as instâncias de treinamento são apresentadas uma a uma e para cada uma delas uma predição é realizada. Assim para cada predição o aprendizado reforça os pesos que contribuiram para chegar próximo do valor esperado e penaliza os pesos que contribuem para se distanciar do valor esperado. É dado pela equação a seguir:

$$   w_{i,j}^{\text{next step}} = w_{i,j} + \eta(y_j - \hat{y}_jx_i)$$

- $w_{i,j}$ é o peso da conexão entre o neurônio de entrada i e o neurônio de saídda j. 
- $x_i$ é o valor da entrada i.
- $\hat{y}_j$ é o valor predito para a saida do neurônio j da instância de treinamento.
- $y_j$ é o valor esperado para a saída do neurônio j.
- $\eta$ é a taxa de aprendizado.  