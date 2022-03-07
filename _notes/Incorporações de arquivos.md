---
---

# Incorporações de arquivos

Você pode incorporar arquivos anexos como imagens ou áudio em suas notas. Use a sintaxe `![[filename.png]]` assim:

![[Engelbart.jpg]]

![[Excerpt from Mother of All Demos (1968).ogg]]

Você pode incorporar um arquivo PDF em suas notas com a mesma sintaxe. Além disso, você pode escrever `![[Meu pdf.pdf#page=numero]]` para abrir diretamente nessa página específica do PDF.

# Incorporar notas

Você também pode incorporar notas do próprio Obsidian

![[Formatos aceitos]]

# iframe

"iframe" é uma maneira de incorporar uma página da Web em outra. É útil porque o Markdown pode aceitar HTML.

Por exemplo

```html
<iframe src="https://www.youtube.com/embed/NnTvZWp5Q7o"></iframe>
```

Produz o seguinte:

<iframe src="https://www.youtube.com/embed/NnTvZWp5Q7o"></iframe>

A sintaxe básica é assim:

```html
<iframe src="INSERT YOUR URL HERE"></iframe>
```

Alguns sites tem formas especificas de incoporar seus conteúdos, por exemplo. você não pode incorporar um vídeo do Youtube utilizando apenas a URL dele acima, exemplo:

<iframe src="https://youtu.be/gN6yMot7_Zk"></iframe>

Viu como fica ruim? O que fazer então ? 

Acesse o video do Youtube, click em compartilhar e escolha a opção incorporar. Copie e cole o código diretamente na nota do obsidian, assim!

<iframe width="560" height="315" src="https://www.youtube.com/embed/gN6yMot7_Zk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Caso você entenda de HTML e CSS você pode personalizar a visualização dentro do Obsidian. 