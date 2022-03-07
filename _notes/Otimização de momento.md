---
---

A otimização de momento modifica a atualização dos pesos pela[[Descida de gradiente]] adicionando um vetor de momento e também um coeficiente de fricção. 

1. $$m \leftarrow \beta m - \eta \nabla _\Theta J(\Theta)$$
2. $$\Theta = \Theta + m$$

Com essa atualização a atualização dos pesos fica bem mais rápidd do que apenas utilizar a descida de gradiente, possibilitanto também sair de platôs. 