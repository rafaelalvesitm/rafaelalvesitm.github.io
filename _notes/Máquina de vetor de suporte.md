---
---

Links: [[Aprendizado supervisionado]]; [[Aprendizado não supervisionado]]; [[Algoritmos de regressão]]

O método de máquina de vetor de suporte é utilizado para tarefas de [[Algoritmos de regressão|regressão]] e [[Algoritmos de classificação|classificação]] para dados lineares ou não lineares bem como detecção de outliers. Esse algoritmo tenta encontrar a linha que melhor separe os dados e se mantenha o mais distante possível das instâncias de treinamento (vetores de suporte).

Esse método é sensível as escalas dos recursos, logo é interessante usar um método de [[Transformação dos dados]]. 

O método pode ser duro, todos os dados ficarão de um lado da linha, ou mole, alguns dados podem ficar do lado oporto da sua classificação. Esse parâmetro é controlado pelo hyperparâmetro C no Sci-kit learn. 

![[SVM example.png]]

Para realizar a classificação de dados não lineares basta realizar uma combinação polinomial dos dados e usar o método nessa nova combinação de dados. Também é possível utilizar kernels diferentes para esse propósito como o linear, polynomial, gausiano e sigmoid.