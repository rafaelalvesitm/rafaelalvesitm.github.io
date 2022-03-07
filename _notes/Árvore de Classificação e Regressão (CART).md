---
---

Esse algoritmo é do tipo [[Algoritmo guloso]]

## [[Algoritmos de classificação|Classificação]]
Esse método visa dividir os dados de forma a encontrar um subset puro, ou seja, apenas com uma categoria definida. O algoritmo continua a subdividir o conjunto de dados a cada nível até atingir um limite determinado ou então separar completamente as categorias (isso pode resultar em uma árvore com vários níveis).

Para realizar tal divisão o algoritmo usa a seguinte equação:

$$ J(k,t_k) = \frac{m_{left}}{m}G_{left} + \frac{m_{left}}{m}G_{left} $$

Sendo:
- $G_{left/right}$ a medadia de impureza do subset da esquerda ou direita.
- $m_{left/right}$ é o número de instâncias do subset da esquerda ou direita.

## [[Algoritmos de regressão|Regressão]]
Esse método visa dividir os dados de forma a reduzir o [[Erro médio quadrático]]. O algoritmo continua a subdividir o conjunto de dados  a cada nível até atingir um limite determinado ou então separar completamente as categorias (isso pode resultar em uma árvore com vários níveis).

Para realizar tal divisão o algoritmo usa a seguinte equação:

$$ J(k,t_k) = \frac{m_{left}}{m}EMQ_{left} + \frac{m_{left}}{m}EMQ_{left} $$

Sendo:
- $EMQ_{left/right}$ a medida do erro quadrático médio do subset da esquerda ou direita.
- $m_{left/right}$ é o número de instâncias do subset da esquerda ou direita.
- $EMQ_{node} = \sum_{i\in node}(\hat{y}_{node}-y^{(i)})^2$
- $\hat{y}_{node} = \frac{1}{m_{node}} \sum_{i\in node}y^{(i)}$