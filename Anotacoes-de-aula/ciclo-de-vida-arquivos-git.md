# Ciclo de vida de arquivos no Git

São divididos em Untracked e Tracked.

Untracked
 - são os arquivos não monitorados pelo Git

Tracked 
 - são os arquivos que estão sendo monitorados pelo Git

Dentro do Tracked há três estados:
 - unmodified
 - modified
 - staged

Unmodified: são os arquivos que ainda não sofreram alterações.

Modified: são os arquivos modificados e assim que salvos passa a fazer parte do...

Staged: ao ser acionado o comando 'git add' tanto os arquivos modificados ou não monitorados são enviados ao staged.

Quando o arquivo ja está no repositório ele saí de Unmodified para Modified, o Git percebe as alterações comparando os SHA-1 de cada modificação.

No Staged ele empacota os dados da alteração e prepara o(s) arquivo(s) para o commit, que guarda essa alteração no ciclo de vida do arquivo e devolve uma cópia para o Unmodified.

Ao executarmos o comando 'git push' enviamos a alteração para o Repositório Remoto no GitHub.

## Divisão do Git

O Git é dividido em duas partes:


+-------------------+
|	  SERVIDOR      |
| Remote Repository |
+-------------------+


+---------------------------------+
|   Ambiente de Desenvolvimento   |
|		- Working Directory       |
|		- Staging Area            |
|		- Local Repository		  |
+---------------------------------+


Enquantos estamos modificando os arquivos eles ficam tramitando entre Working Directory e Staging Area.

Após o commit o arquivo modificado vai para o Local Repository e uma cópia volta para o Staging Area.

Com o comando 'git push' esse arquivo modificado é enviado para o Remote Repository, servidor do GitHub.