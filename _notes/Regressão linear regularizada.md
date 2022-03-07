---
---

Links: [[Aprendizado supervisionado]]

Uma forma de reduzir o sobreajuste em modelos de [[Regressão linear]] é realizar a transformação dos dados utilizando alguma técnica de [[Regularização]]. Por issso existem os modelos lineares regularizados que aplicam um método de [[Regularização]]. 

- [[Regressão de cume]]
- [[Regressão Lasso]]
- [[Regressão de rede elástica]]

Como escolher o melhor modelo? 
- Um pouco de regularização costuma ser bom. 
- [[Regressão de cume]] é boa em geral mas caso alguns recursos não sejam relaventes prefira a [[Regressão Lasso]] ou [[Regressão de rede elástica]].
- No geral a [[Regressão de rede elástica]] é a melhor do que a lasso já que esta pode se comprtar erraticamente quando o número de recursos for muito maior que o número de instâncias. 