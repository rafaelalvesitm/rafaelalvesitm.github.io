---
---

É uma alteração da [[Otimização de momento]] onde o cálculo do gradiente é feito não na posição local mais sim em uma posição ligeramente a frente na direção do momento. Assim tem-se:

1. $$m \leftarrow \beta m - \eta \nabla _\Theta J(\Theta + \beta m )$$
2. $$\Theta = \Theta + m$$