---
---

A descidade de gradiente estocástico utiliza uma única instância aleatória para realizar a descidade de gradiente ao invés de todo o banco de dados como a [[Descida de gradiente em lote]] tradicional. 

- Um benefício desta abordagem é que apenas uma instância precisa ser armazenada na memória o que diminui a carga computacional para realizar a descida de gradiente. 
- Outro benefício é que por ser aleatório esse método tem maior capacidade de fugir de mínimos locais e encontrar o mínimo global. 
- Um problema desta abordagem é que ela fica "pulando" ao invés de ir decaindo até o mínimo. 

Uma estratégia interessante é utilizar uma taxa de aprendizagem variável ao longo do tempo, começando com uma taxa alta e aos poucos ir diminuindo tal taxa. 