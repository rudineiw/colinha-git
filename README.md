# Guia de referência rápida de comandos básicos do prompt do Windows e comandos do GIT

## Comandos Básicos de Prompt de Comando do Windows
cd \         -> vai para diretório raiz
cd ..        -> sobe um diretório
cd exemplo   -> vai para diretório "exemplo"
dir          -> lista os arquivos do diretório
mkdir        -> cria um diretório

## Comandos do GIT por linha de comando
### configurar git
git config --global user.name "seu nome aqui"
git config --global user.email "seu e-mail aqui"

### exibir configuração atual do git
git config --list

### inicialiar repositório git
git init

### adiciona um arquivo no repositório
git add aula1.txt

### adicionar todos os arquivos e pastas
git add --all | git add .

### salva as mudanças no repositório
git commit -m "mensagem"

### cria um "branch" (ramo) teste
git branch teste

### listar branches locais
git branch --list

### listar branches locais e online
git branch -a

### trocando de branch (ramo), por padrão o github utiliza "main"
git branch -M main

### excluir um branch no local
git branch -d nomeDoBranchLocal

### excluir um branch remoto
git push origin --delete nomeDoBranchRemoto

### listar commits realizados
git log

### comaçar a trabalhar no ramo teste
git checkout teste

### listar chaves SSH
ls -al ~/.ssh

### gerar chave SSH
ssh-keygen -t ed25519 -C "your_email@example.com"

### adicinar chave SSH ao agente de SSH
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519

### testar conexão SSH
ssh -T git@github.com

### associando um repositório local com o github
git remote add origin git@github.com:USUARIO/RESPOSITORIO.git

### enviando arquivos para o github
git push -u origin main
