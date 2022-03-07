---
---

O [[CSS]] apresenta diversos  [seletores CSS](https://www.w3schools.com/cssref/css_selectors.asp).  Os principais são 
-  **elemento**: Aplica o estilo a todos os elementos 
    -   **id**: Utiliza uma identificação única para o elemento através do atributo `id="identificação única"`.
    -   **classe**: Utiliza uma identificação que pode ser utilizada em diversos elementos para aplicar determinado estilo. 

A aplicação dos estilos CSS segue uma ordem de prioridade sendo ela:
1. Estilos em linha
2. Estilos por ID
3. Estilo por classes
4. Estilo por tipo do elemento

Também é possível combinar diversas formas de seleciona os elementos que devem ser estilizados como apresentados na tabela abaixo. 

| tipo  | descrição                  |
| ----- | -------------------------- |
| a, b  | Seleção múltipla           |
| a b   | Seleção do descendente     |
| a > b | Seleção do filho           |
| a + b | Seleção do irmão adjacente |
| [a=b] | Seleção do atributo        |
| a:b   | Seleção da pseudoclasse    |
| a::b  | Seleção do pseudoelemento  |

Os estilos podem ser aplicados a pseudoclasses como para quando queremos aplicar os estilos em determinada situação, por exemplo, ao flutuar um elemento com o mouse. |                            |