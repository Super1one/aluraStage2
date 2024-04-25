# O GIT é um CVS
É um sistema de controle de versão


# Comandos de terminal do gitbash

pwd (print working directory) = indica o diretorio atual/ativo
ls (list) = indica os arquivos do diretorio atual

cd (change directory)         = muda o diretorio
  cd pasta -> muda para pasta do diretorio
  cd ..    -> retorna para o diretori pai
  cd caminho/absoluto/diretorio


--------------------------------------------------------------------------
## BRANCH - Trabalhando em EQUIPE

git checkout -b novaBranch -> (cria e entra na nova branch)
git branch novaBranch      -> cria uma nova branch (não entra nela ainda)
git checkout novaBranch    -> entra na nova branch

head -> versao atual do codigo (ultimo commit)

## GIT MERGE (SINCRONIZAR)
git merge nomeBranch -> Incorporar  o codigo de uma branch paralela (income) a branch atual (current)
OBS: o merge é sucedido de um commit para registrar a fusão (esse commit pode ser auto ou manual)

DICA: por 'default', o editor do gitbash é o VIM. Assim, quando finalizar um "merge", edite a menssagem do merge/commit e execute ": + x + enter".

OBS2: O merge não exclui nenhuma das branch fundidas e o código se torna identico em ambas timeline

# GIT REBASE
git rebase branchParalela -> faz a união dos historicos de commits das branchs, colocando Master na frente (como HEAD)
DICA: talvez a ideia seja eliminar uma branch

# GIT MERGER vs GIT REBASE
O merge faz a união dos códigos de duas ou mais branch, porém o histórico de ambas permanece
O Rebase literalmente uni duas branch, ou seja, seus códigos e suas timelines de commit.
O REBASE é conveniente quando é necessário se desfazer de uma das branch.

OBS: para trabalho em equipe, é recomendável fazer PULL antes de PUSH, pois um colega pode já ter alterado o código no repositorio remoto.

## DELETAR BRANCH
git branch -d nomeBranch -> vai deleter a branch selecionada
