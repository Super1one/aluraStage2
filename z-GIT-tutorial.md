# O GIT é um CVS
É um sistema de controle de versão


# Comandos de terminal do gitbash
pwd (print working directory) = indica o diretorio atual/ativo
ls (list) = indica os arquivos do diretorio atual

cd (change directory)         = muda o diretorio
  cd pasta -> muda para pasta do diretorio
  cd ..    -> retorna para o diretori pai
  cd caminho/absoluto/diretorio


## Git bare?
É um respositorio/servidor que não armazena arquivo? Apenas alterações?
git init --bare
# OBS -> Por hora entenda que o proprio github é um servidor bare (só armazena alterações)

## -----------------------------------------------------------------------------------------------

## BRANCH - Trabalhando em EQUIPE

git branch novaBranch   -> cria uma nova branch (não entra nela ainda)
git checkout novaBranch -> entra na nova branch

Cada branch para uma parte do codigo?