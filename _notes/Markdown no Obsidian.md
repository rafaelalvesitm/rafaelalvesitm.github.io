---
---


O Obsidian é uma ferramente para tomar notar que utiliza uma linguagem similar ao Markdown. Tem-se abaixo diversos exemplos de sua utilização. 

---

### Links internos

A principal função do Obsidian é a de linkar notas. Segue o exemplo abaixo. 

```md
Link para uma página: [[Nome da página]].
```

Link para uma página: [[Nome da página]].

---

### Incorporações 

Você pode incorporar arquivos dentro de uma página do Obsidian (Veja mais em [[Incorporações de arquivos]]). Segue o exemplo:

```md
![[Obsidian#O que é o Obsidian]] -> Incorpora uma seção inteira
![[Obsidian#^4f15cc]] -> Incorpora um bloco (Normalmente 1parágrafo)
```

![[Obsidian#O que é o Obsidian]]

![[Obsidian#^4f15cc]]

---

### Cabeçalhos

São utilizados para determinar a hierarquia das seções do seu texto. 

```md
### Headers
# This is a heading 1
## This is a heading 2
### This is a heading 3 
#### This is a heading 4
##### This is a heading 5
###### This is a heading 6
```

# Cabeçalho nível 1
## Cabeçalho nível 2
### This is a heading 3 
#### This is a heading 4
##### This is a heading 5
###### This is a heading 6

---

### Enfase

Você pode escrever o seu texto em _Itálico_, **Negrito** ou **_Ambos_**

```md
*Este é um texto em itálico*
_Este também é um texto em itálico_
```

*Este é um texto em itálico*
_Este também é um texto em itálico_

```md
**Este é um texto em negrito**
__Este também é um texto em negrito__
```

**Este é um texto em negrito**
__Este também é um texto em negrito__

```md
**Você também pode _combinar ambos_**
```

**Você também pode _combinar ambos_**

---

### Listas

Você pode criar listar numeradas ou não numeradas. Para indentar um item utilize a tecla **TAB**. Para remover a identação pressione a tecla **SHIFT+TAB**. 

```md
- Item 1
- Item 2
  - Item 2a
  - Item 2b

1. Item 1
1. Item 2 -> A numeração será incluida automáticamente, 
1. Item 3
   1. Item 3a -> Aqui a nomeração começa novamente devido a indentação
   1. Item 3b
```

- Item 1
- Item 2
  - Item 2a
  - Item 2b

1. Item 1
1. Item 2
1. Item 3
   1. Item 3a
   1. Item 3b

--- 

### Imagens

Você pode incluir imagens, áudio, gif etc, que estejam na pasta do Obdisian ou na internet!

```md
![Engelbart](https://history-computer.com/ModernComputer/Basis/images/Engelbart.jpg) -> Imagem da internet

![Gif da internet](https://giphy.com/embed/1BmWIWMqfNS7OxnI7D)

```

![Engelbart](https://history-computer.com/ModernComputer/Basis/images/Engelbart.jpg)

![Gif da internet|200](https://media.giphy.com/media/VbnUQpnihPSIgIXuZv/giphy.gif)


#### Redimensionando imagens

Você pode redimensionar as imagens incluindo um filtro de largura como indicado abaixo!

```md
![Engelbart|100](https://history-computer.com/ModernComputer/Basis/images/Engelbart.jpg)
```

![Engelbart|100](https://history-computer.com/ModernComputer/Basis/images/Engelbart.jpg)

---

### Links

Os links no obsidian pode indicar páginas internas ou externas. Colchetes simples indicam links externos e colchetes duplos indicam links internos. 

```md
http://obsidian.md - automático!
[Nome da página](URL do link) -> 
```

http://obsidian.md - automático!
[Obsidian](http://obsidian.md)

---

### Blocos de citações 

```md
> É perigoso ir sozinho, leve isso!

\- Velho da lenda de Zelda
```

> É perigoso ir sozinho, leve isso!

\- Velho da lenda de Zelda

---

### Códigos em linha

```md
O texto dentro de `acentos graves` (Fica normalmente na mesma tecla do til e acima do TAB) será formatado como código.
```

O texto dentro de `backticks` será formatado como código.

---

### Blocos de código

O destaque de sintaxe é suportado especificando a linguagem após o primeiro conjunto de acentos graves. Uma lista de idiomas suportados pode ser encontrada [no site do prismjs](https://prismjs.com/#supported-languages). abaixo tem um exemplo de código em JavaScript

<pre><code>```javascript
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }
}
```</code></pre>

```javascript
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }
}
```
    
	
```md
    O texto identado é formatado assim e também se parecerá com um bloco de código na visualização. 
```

	O texto identado é formatado assim e também se parecerá com um bloco de código na visualização.  
    
---

### Lista de tarefas

```md
- [x] Utilize um grupo de [] para idicar um item de tarefa
- [x] Este é um item finalizado
- [?] Este também é um item finalizado (funciona com qualquer caracter)
- [ ] Este é um item incompleto
- [ ] Você pode completar uma tarefa clicando no botão na página de visualização
```

- [x] Utilize um grupo de [] para idicar um item de tarefa
- [x] Este é um item finalizado
- [?] Este também é um item finalizado (funciona com qualquer caracter)
- [ ] Este é um item incompleto
- [ ] Você pode completar uma tarefa clicando no botão na página de visualização

---

### Tabelas

Você pode criar tabelas montando uma lista de palavras e dividindo-as com hífens `-` (para a primeira linha) e, em seguida, separando cada coluna com uma barra vertical `|`:

```md
Primeiro cabeçalho | Cegundo cabeçalho
------------ | ------------
Conteúdo da célula 1 | Conteúdo da célula 2
Conteúdo da primeira coluna | Conteúdo da segunda coluna
```

Primeiro cabeçalho | Cegundo cabeçalho
------------ | ------------
Conteúdo da célula 1 | Conteúdo da célula 2
Conteúdo da primeira coluna | Conteúdo da segunda coluna

---

```md
As tabelas podem ser justificadas com dois pontos | Outro exemplo com um título longo
:----------------|-------------:
Devido ao uso dos `:` | esse texto vai ser justificado

Você pode inlcuir links nas tabelas, mas se for usar uma incorporação lembre-se de adicionar um `\` antes do `!`, assim \![Nome](link)
```

As tabelas podem ser justificadas com dois pontos | Outro exemplo com um título longo
:----------------|-------------:
Devido ao uso dos `:` | esse texto vai ser justificado

Você pode inlcuir links nas tabelas, mas se for usar uma incorporação lembre-se de adicionar um `\` antes do `!`, assim:

```md
Primeiro cabeçalho | Second Header
------------ | ------------
[[Formate suas notas\|Formatação]]	|  [[Atalhos do teclado\|teclas]]
```

Primeiro cabeçalho | Second Header
------------ | ------------
[[Formate suas notas\|Formatação]]	|  [[Atalhos do teclado\|teclas]]

---

### Riscado

```md
Qualquer palavra precedida por dois tils (~~assim~~) vai aparecer riscado
```

Qualquer palavra precedida por dois tils (~~assim~~) vai aparecer riscado

---

### Destaque

```md
Use dois sinais de iguais para ==destacar o texto==.
```

Use dois sinais de iguais para ==destacar o texto==.

---

### Notas de rodapé

```md
Essa é uma simples nota de rodapé,[^1] e aqui tem uma nota maior.[^bignote]

[^1]: Significado da nota de rodapé!

[^bignote]: Esse é uma descrição mais completa

    Indente os parágrafos dentro do bloco

    `{ meu código por exemplo }`

    Adicione quantos paragrafos for necessário
```

Here's a simple footnote,[^1] and here's a longer one.[^bignote]

Essa é uma simples nota de rodapé,[^1] e aqui tem uma nota maior.[^bignote]

[^1]: Significado da nota de rodapé!

[^bignote]: Esse é uma descrição mais completa

    Indente os parágrafos dentro do bloco

    `{ meu código por exemplo }`

    Adicione quantos paragrafos for necessário
	
```md
Você também pode incluir notas de rodapé na mesma linha ^[Assim você não perde o texto que está escrevendo]
```

Você também pode incluir notas de rodapé na mesma linha ^[Assim você não perde o texto que está escrevendo]

### Equações matemáticas

Você pode escrever equações matemáticas dentro do Obsidian, muito parecido com o que é feito no [Latex](https://www.latex-project.org/).

```md
$$\begin{vmatrix}a & b\\
c & d
\end{vmatrix}=ad-bc$$
```

$$\begin{vmatrix}a & b\\
c & d
\end{vmatrix}=ad-bc$$

Você também pode escrever equações utilizando `$` entre a equação, assim: $e^{2i\pi} = 1$ .

O obsidian utiliza o [Mathjax](http://docs.mathjax.org/en/latest/basic/mathjax.html). Você pode verificar os pacotes suportados [aqui](http://docs.mathjax.org/en/latest/input/tex/extensions/index.html).

### Comentários

Use `%%` para incluir comentários que não serão apresentados no mode de visualização. 

```md
Aqui tem um comentário na mesma linha: %%Você não vai ver esse testo%% (Você não consegue ver, acredite!)

Aqui tem um bloco de comentário:
%%
Ele pode se expandir
por multiplas linhas
%%
```

Aqui tem um comentário na mesma linha: %%Você não vai ver esse testo%% (Você não consegue ver, acredite!)

Aqui tem um bloco de comentário:
%%
Ele pode se expandir
por multiplas linhas
%%
Você também não está vendo! 
