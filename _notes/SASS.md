---
---

Sass](https://sass-lang.com/) é uma linguagem que permite escrever [[CSS]] de maneira mais eficiente e prática utilizando variáveis e outros elementos para definir os arquivos [[CSS]]. Como exemplo abaixo utiliza-se uma variável para definir a cor vermelha. 

``` scss
$color: red;

ul {
    font-size: 14px;
    color: $color;
}

ol {
    font-size: 18px;
    color: $color;
}
```

Resultando em 

```css
div {
    font-size: 18px;

    p {
        color: blue;
    }

    ul {
        color: green;
    }
}
```


É importante destacar que os navegadores não entendem o arquivo `.scss` e que portanto é necessário conversar o código SASS em código [[CSS]]. É possível realizar tal conversão com o comando `sass arquivo.scss:arquivo.css`. Também é possível converter automaticamente de Sass para [[CSS]] através do comando `sass --watch arquivo.scss:arquivo.css`. 

Também é possível adicionar herança através do SASS como indicado abaixo onde os elementos `success`, `warning` e `error` herdam as caracteristicas descritas em `%message`. 

``` scss
%message {
    font-family: sans-serif;
    font-size: 18px;
    font-weight: bold;
    border: 1px solid black;
    padding: 20px;
    margin: 20px;
}

.success {
    @extend %message;
    background-color: green;
}

.warning {
    @extend %message;
    background-color: orange;
}

.error {
    @extend %message;
    background-color: red;
}
```

![[Exemplo Sass.png]]