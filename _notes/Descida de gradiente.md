---
---

O principio da descida de gradiente é medir o gradiente local da função de erro em relação ao vetor de parâmetro $\theta$, e vai na direção de descida do gradiente. A descida de gradiente é amplamente utilizada para otimizar funções de custo por exemplo. 

Dois problemas principais que fazem o método não encontrar o mínimo global:
- É possível econtrar mínimos locais 
- É possível encontrar platôs gigantes

Quando usar o gradiente descendente é importante que todos os dados estejam na mesma escala, senão o método pode demorar muito para convergir. 

A avaliação do melhor método de aprendizagem utilizando a descida de gradiente nem sempre é possível já que mínimos locais podem existir. Para isso pode-se utilizar o ponto de [[Parada antecipada]]. 

Três formas de implementar a descida de gradiente:
- [[Descida de gradiente em lote]]
- [[Descida de gradiente estocástico]]
- [[Descida de gradiente em mini lotes]]