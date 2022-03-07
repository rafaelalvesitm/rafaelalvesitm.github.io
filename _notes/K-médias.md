---
---

Links: [[Aprendizado não supervisionado]]; [[Algoritmos de classificação]].

O algoritmo de K-médias funciona escolhendo incialmente k instâncias como centroids. Depois rotulando os pontos mais próximos, atualizando a centroid, rotulando novamente os dados e repetindo isso até que os centroids deixem de se movimentar. O algoritmo se preocupa apenas com a distância da instância até a centroid do grupo. 

O algoritmo converge mas pode encontrar um mínimo local ao invés de encontrar o mínimo global. Para isso é sugerido que o algoritmo seja aplicado várias vezes com inicializações aleatórias ( no Scikit-learn por padrão são 10). 

![[Exemplo de agrupamento por K-médias.png]]

A escolha do número de cluster pode ser feita pela [[Regra do cotovelo]] ou pelo [[Coeficiente de silhueta]]. Também recomenda-se escalar os dados já que o K-médias não funciona bem para dados que não sejam esféricos. 

