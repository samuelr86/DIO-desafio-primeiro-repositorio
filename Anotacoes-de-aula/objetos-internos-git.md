# Objetos internos do Git

## Blobs
são objetos que guardam metadados de um arquivo, contém um hash de encriptação tipo SHA-1 e as seguinte informações:
 - blob
 - tamanho 
 - \0
 - conteúdo

## Tree
Responsável por montar a estrutura de onde estão esses arquivos.
Aponta para um blob e contém:
 - blob
 - \0
 - SHA
 - nome do arquivo

## Commit
É o objeto que vai juntar todos os outros objetos.

#### commit -> tree -> parent(ultimo commit) -> autor -> msg

O SHA-1 desse commit é o hash de toda essa informação, também tem um timestamp (data/hora) de criação.

