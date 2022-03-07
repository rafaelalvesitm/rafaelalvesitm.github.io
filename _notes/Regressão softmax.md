---
---

Links: [[Algoritmos de regressão]]; 

A [[Algoritmos de regressão|regressão]] softmax ou regresão logistica multinomial é uma gressão utiizada para generalizar o modelo de [[Regressão logística]] para multiplas classes. A ideia principal é que incialmente o modelo calcula a pontuação $s_k(x)$ para cada classe $k$ e depois estima a probabilidade de cada classe com base na [[Função softmax]]. 

A função $s_k(x)$ é dada por:

$$s_k(x) = x^T\Theta^{(k)}$$

A regressão softmax tem como saida uma classe dentre várias possíveis e não várias classes dentre várias possíveis, logo esse algoritmo deve ser usado apenas com classes mutamente exclusivas. 

Para o aprendizado esse algoritmo usa a [[Entropia cruzada]] através da equação:

$$J(\Theta) = -\frac{1}{m} \sum_{i=1}^m \sum_{k=1}^Ky_k^{(i)} \log{(\hat{p}_k^{(i)})}$$

O vetor gradinete para cada classe $k$ é dada por:

$$\nabla_{\theta^{k}}J(\theta) = \frac{1}{m}\sum_{i=1}^m(\hat{p}_k^{(i)} - y_k^{(i)})x^{(i)}$$