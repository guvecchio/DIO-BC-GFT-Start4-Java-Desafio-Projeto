# Links Úteis

[Pro Git Book](https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-Sobre-Controle-de-Vers%C3%A3o)

[comandos mais utilizados](https://woliveiras.com.br/posts/comandos-mais-utilizados-no-git/)

[lista de comandos úteis no git](https://gist.github.com/leocomelli/2545add34e4fec21ec16)

# Comandos já Utilizados

 - git init *cria um repositório*
 - git add *inclui o arquivo no repo, preparando para o commit (de modified para staged)*
 - git rm *exclui o arquivo no repo*
 - git commit *envia as modificações para o repo local*
 - git status *indica o estatus atual dos arquivos do repo*
 - git push *envia arquivos/diretórios para o repositório remoto*
 - git pull *atualiza repositório local de acordo com o repositório remoto*
 - git checkout *trocando para um branch existente*
 - git branch *criando um novo branch*
 - git clone *clona um repositório remoto*
 - git --list *as ramificações existentes serão listadas; a ramificação atual será destacada em verde e marcada com um asterisco*
 - git config --list *listando as cofigurações do repositório local*
 - git remote add origin *vinculando a um repositório remoto*
 - git remote -v _**verbose** seja mais detalhado e mostre o url após o nome_
 - -f *forçar algo*

 - o uso do TAB é um autocomplete completando o caminho de diretorios

# Ciclo de vida

![Ciclo de Vida](/images/ciclo-de-vida.jpg)
*representação do ciclo de vida no git*

* untracked - arquivo criado com o git init do qual o git ainda não tem conhecimento, que depois de add vai direto para staged.
* tracked (arquivos que o git conhece)
    * unmodified - arquivo já add no repo sem modificação; quando removido vai para untracked;
    * modified - quando modificado - como? comparando o sha1 do arquivo;
    * staged - após novo add - aguardando o commit, que quando feito, retorna para unmodified, recomeçando o ciclo.

# Ambientes

 - servidor
    - remote repository (transita entre o remoto e local através do push e do pull)
 - ambiente de desenvolvimento (os dois primeiros transitam entre o que está sendo trabalhado - working, e o que está pronto para ser comitado - staging)
    - working directory
    - staging area
    - local repository (transita entre o remoto e local através do push e do pull)

