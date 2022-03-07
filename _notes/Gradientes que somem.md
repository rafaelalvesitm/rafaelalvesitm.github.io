---
---

Este problema é encontrado em [[Redes neurais]] e [[Redes profundas]] quando existem muitas camadas na rede. O que ocorre é que conforme os erros são propagados da camada final para a camada inicial o gradiente do erro vai ficando cada vez menor e assim é possível que os pesos da camda inicial permaneçam virtualmente os mesmos. O contrário pode acontecer nos[[Gradientes que explodem]]. 

O problema ocorrem principalmente quando se utiliza a [[Função sigmoide]] com uma inicialização aleatória dos pesos. Isso se deve ao fato de que quando os valores de entrada da função logistica são muito positivos ou negativos a saída tende a ser 0 ou 1, sendo a derivada deste ponto próximo a 0. Desta forma não sobra gradiente para ser utilizado na atualização dos pesos. 

Para alivar este problema utiliza-se algumas inicializações diferentes como propostas por He, LeCun e Glorot. 

Qual ativação utilizar? Em geral SELU > ELU > leaky ReLU > ReLU > tanh > logistic.