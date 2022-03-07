---
---

Este problema é encontrado em [[Redes neurais]] e [[Redes profundas]] quando existem muitas camadas na rede. O que ocorre é que conforme os erros são propagados da camada final para a camada inicial é possível que gradiente do erro fique cada vez maior e assim os pesos da camada incial são atualizados com valores altos e portanto o algoritmo diverge. O contrário pode ser observado nos [[Gradientes que somem]]. 