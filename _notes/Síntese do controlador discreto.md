---
---

A síntese do controlador discreto é um método formal usado para gerar um controlador a partir de um conjunto de regras (contrato) definido por um modelo. É construído com base na [[Teoria do Controle Supervisório]]. 

O método divide o modelo em variáveis de entrada controláveis e não controláveis. Assim dado um conjunto de regras o modelo calcula as restrições nas variáveis de controle com base na exploração simbólica do espaço de estados e providencia um controlador para atingir o conjunto de regras determinadas. 

A linguagem [[Heptagon BZR]] pode ser utilizada para a implementação deste método. 