# Links Úteis

[Pro Git Book](https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-Sobre-Controle-de-Vers%C3%A3o)

# Comandos já Utilizados

git init **cria um repositório**
git add **inclui o arquivo no repo, e também o prepara para o commit (de modified para staged)**
git rm 
git commit **envia as modificações para o repo local**
git status **indica o estatus atual dos arquivos do repo**
git push
git pull
git checkout
git branch
git clone
git --list
-r
-a
git config --list


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

