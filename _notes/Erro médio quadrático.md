---
---

O erro médio quadrático mede a raiz da médida das distâncias quadráticas entre o valor experado e o valor real de determinada medida. 

$EMQ(X,h) = \sqrt{\frac{1}{m}\sum^m_{i=1}(h(x^{(i)})-y^{(i)}))^2}$

Para o caso de [[Aprendizagem de máquina]] tem-se a seguinte definição:

- $m$ é o número de instancias
- $x^{(i)}$ é o vetor contendo todos os recursos excluindo o rótulo para a instância i
- $y^{(i)}$ é o rótulo para a instância i
- $X$ é a matriz que contém todos os recursos exeto os rótulos. 
- $h$ é a função de previsão do sistema, também chamada de hipótese. Dado um valor de $x^{(i)}$ essa função retorna um valor $\hat{y}^{i}$ previsto. 