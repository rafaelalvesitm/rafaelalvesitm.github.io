---
---

Um modelo Heptagon contém 4 elementos principais:
- Node: Define blocos de equações ou automatons com variáveis de entrada e saída. 
- Equation: Equação defini o valor de saída de um nó. 
- Automaton: Descrição formal contendo variáveis de entrada, saída e o espaço de estados. 
- Contract: Defini as regras que o [[Síntese do controlador discreto | controlador ]] deve seguir. 

Como exemplo tem-se um sincronizador de lâmpadas, dado abaixo:

![[Controle sincronia de lampadas.png]]

O automaton é o bloco Lamp. Cada lâmpada tem dois estados possíveis: ON ou OFF com OFF sendo o estado inicial. Cada estado está associado a uma equação que determina a saída do autômato neste estado. Neste caso, o variável de saída lamp_s representa se a lâmpada modelada está ligada ou desligada. C é uma variável que pode assumir valores verdadeiros ou falsos e indicar se este dispositivo pode operar ou não. Duas variáveis de entrada definem transições entre estados. Neste caso, quando c e push são verdadeiros, o estado da lâmpada muda para ON. Se c for falso ou ocorrer o push do evento, ele retornará para OFF. Neste modelo, c é um evento de controle e representa o controlador atuando no modelo para coordenar a transição entre os estados, permitindo que ele mude de OFF para ON ou obrigue-o a fazer o inverso transição. A variável push é um evento incontrolável e representa uma ação externa, como um botão de pressão, que pode ser executada por qualquer ser humano ou máquina, por exemplo. Para definir um modelo de controle para as lâmpadas é necessário definir outro nó com os dois autômatos. 