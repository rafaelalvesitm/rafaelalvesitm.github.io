---
---

Links: [[Aprendizado supervisionado]]

Esse método é capaz de realizar tarefas de [[Algoritmos de regressão|regressão]] e [[Algoritmos de classificação|classificação]]. Esse método cria uma árvore onde a cada nível uma determinada decisão é tomada com base nos dados. É necessário verificar a informação de decisão do nó sempre que um filho existir, caso ele não exista basta olhar a classificação dada no nó. 

Beneficios:
- Precisa de pouca preparação dos dados, não sendo necessário escalar ou centralizar os dados. 
- Simples de entender
- Rápido de realizar a predição ou classificação uma vez que a árvore está construida. 

Problemas:
-  Grande tendência de sobreajustar os dados com uma árvore muito profunda, logo é necessário restringir a árvore limitando sua profundidade. 
-  Sensível a variação alterando os dados utilizados para treinamento

Exemplo para os dados de iris:

![[Exemplo de árvore de decisão para iris.png]]

- A medida de amostras indicam para quantas instancas tal decisão se aplica. 
- O valor do nó indica quantas instâncias existem em cada categoria. 
- O valor da [[Impureza de Gini]] indica quanta "incerteza" existe na tomada de decisão. pode ser substituido pela medida de [[Entropia]] resultando em uma árvore similar. 

Tipos de algoritmo:
- [[Árvore de Classificação e Regressão (CART)]]