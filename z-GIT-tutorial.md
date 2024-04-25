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

## FAZENDO O MERGE (SINCRONIZAR)
git merge nomeBranch -> Unir branch ativa/atual com outra branch (nomeBranch)
OBS: o merge é sucedido de um commit para registrar a fusão (esse commit pode ser auto ou manual)

DICA: por 'default', o editor do gitbash é o VIM. Assim, quando finalizar um "merge", edite a menssagem do merge/commit e execute ": + x + enter".

OBS2: O merge não exclui nenhuma das branch fundidas e o código se torna identico em ambas timeline

# trazer commit da paralelar para a master
git rebase branchParalela -> faz a união dos historicos de commits das branchs
DICA: talvez a ideia seja eliminar uma branch