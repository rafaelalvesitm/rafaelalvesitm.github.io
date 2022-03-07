---
---

A matrix pseudoinversa, ou Matrix inversa de Moore-Penrose, é computada através do método [[Decomposição de valor singular (SVD)]] através da equação:

$$   X^+ = V\Sigma^+U^T $$

Para calcular a matriz $\Sigma^+$, o algoritmo pega $\Sigma$ e define para zero todos os valores menores que um pequeno valor limite, então ele substitui todos os valores diferentes de zero por seus inversos e, finalmente,ele transpõe a matriz resultante.