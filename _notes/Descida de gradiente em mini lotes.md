---
---

A descidade de gradiente em mini lotes é um caso intermediário entre a [[Descida de gradiente em lote]] e a [[Descida de gradiente estocástico]]. Ao invés de usar todo o lote ou então apenas uma instância, a descida de gradiente em mini lotes realizar a descidade de gradiente em uma pequena amostra dos dados. 

- Um ponto positivo desta abordagem é que é possível utilizar a aceleração de hardware para realizar a multiplicação de matrizes nas GPUs e assim ganhar no tempo de execução do algoritmo. 