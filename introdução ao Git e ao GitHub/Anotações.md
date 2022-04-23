### Introdução ao Git e GitHub
## Comandos Uteis para o terminal
# Windows
 - cd = mudar de diretorios
 - dir = mostrar pastas
 - mkdir = Criar pastas
 - del/ rmdir  = (del é para deletar apenas arquivos), rmdir /S /Q  (deleta a pasta  com tudo dentro)

- cls = limpar terminal

# Unix
 - cd = mudar de diretorios
 - ls = mostrar pastas
 - mkdir = Criar pastas
 - rm -rf = deletar pasta com tudo dentro
 - clear = limpar terminal (ctrl + l)

# Link para download do Git:
[Git Download](https://git-scm.com/downloads)


## Entendendo como git funciona
 - SHA1
 - Objetos Fundamentais
 - Sistema Distribuído
 - Segurança


## SHA1

"A sigla SHA significa Secure Hash Algorithm(Algoritmo de Hash Seguro), é um conjunto de funções hash criptográficas projetadas pela NSA (Agência de Segurança Nacional dos EUA)."

 - A encriptação gera conjunto de characteres identificador de 40 dígitos.


## Objetos Fundamentais
 - blobs
tem o sha1 do arquivo
"Armazena metadados exemplo: 
Blob tamanho 42 \0 Ola mundo
exemplo 2:
nome/tamanho'9'/'\0'/conteudo
exemplo 3:
'blob 9\0conteudo'

 - trees
tem o sha1 dos blobs
aponta pros blobs

 - commits
commit aponta pra tree
parente
autor
mensagem
time stamp
o commit aponta para a tree que aponta para o blob que aponta pro conteudo.

## Sistemas distribuidos

# Comandos
 - cat nomedoarquivo = Usado para exibir o conteúdo de um arquivo.

 - ssh-keygen -t ed25519 -c mail@mail.com =  Gera uma nova chave SSH

 - eval $(ssh-agent -s) = Usado para adicionar um agent que vai gerenciar as chaves SSH

 - ssh-add arquivodaschaves = Adiciona o arquivo de SSH privado ao agent



 - git init = iniciar repositorio
 - git add = muda o status do arquivo para Staged
 - git commit = remove as modificaçoes da staging area e move pro repositorio local  

 - ls -a = com o '-a' ve os arquivos ocultos

 - git config --global user.email "email@mail.com" = adiciona o email do autor 
 - git config --global user.name username = adiciona o username do autor

 - git add * / git add . = muda o status de todos os arquivos para Staged

 - git commit -m "commit inicial" = remove as modificaçoes da staging area e move pro repositorio local adicionado um comentario relativo ao que foi feito.

 - mv strogonoff.md ./receitas/ = dentro do git bash mv move as coisas. no exemplo move o strogoff.md para pasta receitas



 - git remote add origin https://github.com/NerdDoGueto/livro-receitas.git = adiciona um repositorio remoto ao projeto.


 - git push origin main/master = adiciona os commits do repositorio local para o repositorio remoto.

 - git pull = atualiza o repositorio local com a versao mais rescente do repositorio remoto.