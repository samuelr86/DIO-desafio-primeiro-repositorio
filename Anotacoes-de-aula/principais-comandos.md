# Principais comandos do git

## git init
Inicia um repositório a ser monitorado pelo Git

## git add
Adiciona as alterações dos arquivos a serem comitados

## git commit
Empacota as alterações dos arquivos e os reserva no 'Local Repository'

## git push
Envia as alterações dos arquivos ao repositório remoto no Github, costuma-se usar acrescido de um apelido para o repositório(origin) seguido da branch (main, por exemplo)

## git pull
Puxa as alterações feitas no arquivo em outro repositório local

## git remote add origin <url repositorio>
Vincula o 'Local Repository' ao 'Remote Repository'

## git status
Verifica a situação dos arquivos monitorados

## git log
Lista o log de alterações comitadas na branch, a flag '--oneline' lista em uma linha por log abreviando dados de leitura

## git config
Acessa menu de configurações do Git. A flag --list lista todas as configurações.
Para efetuar a configuração usar 'git config --global(ou --local) <nome-da-configuração>'
Para desfazer alguma configuração usar 'git config --global(ou --local) --unset <nome-da-configuração>'

## git clone
Baixa para seu ambiente de desenvolvimento o repositório de outrem.