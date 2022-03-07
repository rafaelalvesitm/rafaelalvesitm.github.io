---
---

CSS, ou Cascading Style Sheets, é utilizado para customizar a aparência de um website. O CSS pode ser adicionado das seguintes formas:
- Diretamente a um elemento utilizando o atributo `style="propriedade CSS: valor;"`, 
- Descrito entre elementos `<style>` no cabeçalho do arquivo HTML
- Em um arquivo separado utilizando o elemento HMTL `<link` no cabeçalho do arquivo HTML. 

É importante destacar que uma vez que o CSS é aplicado a um elemento pai, todos os elementos filhos recebem o estilo aplicado a não ser que seja expressamente dito no elemento filho. 

Um exemplo de CSS é apresentado abaixo sendo a cor do texto em azul e o alinhamento do texto centralizado. 

``` html
<!DOCTYPE html>
<html lang="en">
    <head>
        <title>Hello!</title>
    </head>
    <body>
        <h1 style="color: blue; text-align: center;">A Colorful Heading!</h1>
        Hello, world!
    </body>
<html>
```

Existem muitas propriedades CSS, basta pesquisar na internet. Alguns dos mais comuns, porém, são:
-   `color`: Muda a cor do texto. 
-   `text-align`: Indica onde os elementos devem ser apresentados.
-   `background-color`: Muda a cor do fundo do elemento.
-   `width`: Largura em pixels ou porcentagem da página.
-   `height`: Altura em pixels ou porcentagem da página.
-   `padding`: Quanto espaço deve existir dentro do elemento.
-   `margin`: Quanto espaço deve existir fora do elemento. 
-   `font-family`: Tipo da fonte a ser utilizada.
-   `font-size`: Altura da fonte em pixels.
-   `border`: Tipo, cor e dimensão das bordas do elemento.

O CSS possuí diversos [[Seletores CSS]]

Também é possível utilizar o [[SASS]] para escrever arquivos CSS de maneira mais rápida, efetiva e clara. 