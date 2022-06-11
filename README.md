#Guia de referência rápida de comandos básicos do prompt do Windows e comandos do GIT:

##Comandos Básicos de Prompt de Comando do Windows:
CD \         -> vai para diretório raiz
CD ..        -> sobe um diretório
CD exemplo   -> vai para diretório "exemplo"
DIR          -> lista os arquivos do diretório
MKDIR        -> cria um diretório

##Comandos do GIT por linha de comando:
=> para configurar 
git config --global user.name "seu nome aqui"
git config --global user.email "seu e-mail aqui"

=> ver configuração
git config --list

=> inicializa um diretório com o git
git init

=> adiciona um arquivo no índice
git add aula1.txt

=> adiciona tudo no índice
git add --all

=> salva as mudanças no repositório
git commit -m "mensagem"

=> retorna os arquivos de trabalho
git restore .

=> Cria um "branch" (ramo) teste
git branch teste

=> Passa a trabalhar no ramo teste
git checkout teste

=> Mostra o log
git log

=> Enviar
git push https://TOKEN@github.com/rudineiw/aulagit.git (para github rudineiw, repositório aulagit.git)

=> Buscar
git pull https://TOKEN@github.com/rudineiw/aulagit.git

=> Clonar
git clone https://TOKEN@github.com/rudineiw/aulagit.git
