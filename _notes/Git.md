---
---

Um repositório [Git](https://git-scm.com/) é um local de arquivo onde armazenaremos todos os arquivos relacionados a um determinado projeto. Eles podem ser remotos (armazenados online no [[GitHub]] por exemplo) ou locais (armazenados em seu computador). A ferramenta permite  controlar a versão do repositório através de diversas funções, como: 
- Acompanhar as alterações que fazemos em nosso código, salvando versões do mesmo em pontos especificados pelo usuário. 
- Permite sincronizar facilmente o código entre diferentes pessoas que trabalham no mesmo projeto, permitindo que várias pessoas extraiam e enviem informações para um repositório armazenado na web.
- Permite fazer alterações e testar o código em um _branch_ diferente sem alterar nossa base de código principal e, em seguida, mesclar os dois.
- Permite reverter para versões anteriores do nosso código se percebermos que cometemos um erro.

# Commit

Depois de fazer algumas alterações em um arquivo, podemos realizar um _commit_ dessas alterações, tirando uma snapshot do estado atual do nosso código. Para fazer isso, executamos: `git commit -m "mensagem"` onde a mensagem descreve as alterações que você acabou de fazer.

Após essa alteração, podemos executar o `git status` para ver como nosso código se compara ao código no repositório remoto

Quando estivermos prontos para publicar nossos commits locais no Github, podemos executar o `git push`. Agora, quando formos ao GitHub em nosso navegador da Web, nossas alterações serão refletidas.

Se você alterou apenas os arquivos existentes e não criou novos, em vez de usar `git add .` e depois `git commit...`, podemos condensar isso em um comando: `git commit -am "some message" `. Este comando confirmará todas as alterações que você fez.

Às vezes, o repositório remoto no [[GitHub]] estará mais atualizado do que a versão local. Nesse caso, você deseja primeiro confirmar as alterações e, em seguida, executar o `git pull` para puxar as alterações remotas para o seu repositório.

# Mesclar conflitos

Um problema que pode surgir ao trabalhar com o Git, especialmente quando você está colaborando com outras pessoas, é algo chamado **conflito de mesclagem**. Um conflito de mesclagem ocorre quando duas pessoas tentam alterar um arquivo de maneira conflitante entre si.

Isso normalmente ocorrerá quando você utilizar `git push` ou `git pull`. Quando isso acontecer, o Git mudará automaticamente o arquivo para um formato que descreva claramente qual é o conflito. Aqui está um exemplo em que a mesma linha foi adicionada de duas maneiras diferentes:

```python
    a = 1
    <<<<< HEAD
    b = 2
    =====
    b = 3
    >>>>> 56782736387980937883
    c = 3
    d = 4
    e = 5
```

No exemplo acima, você adicionou a linha `b = 2` e outra pessoa escreveu `b = 3`, e agora devemos escolher uma delas para manter. O número longo é um _hash_ que representa o commit que está em conflito com suas edições. Muitos editores de texto, como o Visual Studio Code, também fornecem destaque e opções simples, como “aceitar atual” ou “aceitar entrada”, que economizam o tempo de exclusão das linhas adicionadas acima.

Outro comando git potencialmente útil é o `git log`, que fornece um histórico de todos os seus commits nesse repositório.

Potencialmente ainda mais útil, se você perceber que cometeu um erro, poderá reverter para um commit anterior usando o comando `git reset` de duas maneiras:
- `git reset --hard <commit>` reverte seu código exatamente como estava após o commit especificado. Para especificar o commit, use o hash commit associado a um commit que pode ser encontrado usando `git log` como mostrado acima.
- `git reset --hard origin/master` reverte seu código para a versão atualmente armazenada online no Github.

# Ramificação

Depois de trabalhar em um projeto por algum tempo, você pode decidir que deseja adicionar um recurso adicional. No momento, podemos apenas confirmar alterações neste novo recurso, conforme mostrado no gráfico abaixo

Mas isso pode se tornar problemático se descobrirmos um bug em nosso código original e quisermos reverter sem alterar o novo recurso. É aqui que a ramificação pode se tornar realmente útil.

Ramificação é um método de mover-se para uma nova direção ao criar um novo recurso e só combinar esse novo recurso com a parte principal do seu código, ou a ramificação principal, quando terminar. Este fluxo de trabalho será mais parecido com o gráfico abaixo:

![Branch](images/branch.png)

A ramificação que você está olhando no momento é determinada pelo 'HEAD', que aponta para uma das duas ramificações. Por padrão, o HEAD é apontado para o branch master, mas também podemos verificar outros branches.

Agora, vamos ver como realmente implementamos a ramificação em nossos repositórios git:
    1. Execute `git branch` para ver em qual branch você está trabalhando no momento, que terá um asterisco à esquerda do nome.

    ![Terminal de filial](images/git_branch.png)

    1. Para criar um novo branch, vamos executar `git checkout -b <new branch name>`
    2. ![Nova Filial](images/new_branch.png)

    1. Alterne entre as ramificações usando o comando `git checkout <nome da ramificação>` e confirme as alterações em cada ramificação.
    2. Quando estivermos prontos para mesclar nossas duas ramificações, verificaremos a ramificação que desejamos manter (quase sempre a ramificação master) e, em seguida, executaremos o comando `git merge <other branch name>`. Isso será tratado de forma semelhante a um push ou pull, e conflitos de mesclagem podem aparecer