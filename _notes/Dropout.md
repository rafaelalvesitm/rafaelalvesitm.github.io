---
---

O dropout é uma regularização onde com probabilidade p um determinando neurônio é desativado durante o passo de treinamento. Esse neurônio pode estar ativado em outros passos de treinamento. Depois do treinamento todos os neurônios são utilizados. 

![[Exemplo de dropout.png]]

Beneficios e aplicações:
- Dropout pode melhorar a rede neural de em 2%. 
- Se o modelo estiver sobreajustado pode-se aumentar o dropout, se estiver sobajustado pode-se diminuir o dropout. 
- É interessante aumentar o dropout para grandes camadas e diminuir para camadas menores. 
- É interessante avaliar o dropout apenas depois da última camada escondida. 