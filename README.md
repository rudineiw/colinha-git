# Guia de referência rápida de comandos básicos do prompt do Windows e comandos do GIT

## Comandos do GIT por linha de comando
### configurar git
```
git config --global user.name "seu nome aqui"
```
```
git config --global user.email "seu e-mail aqui"
```

### exibir configuração atual do git
```
git config --list
```

### inicializar repositório git
```
git init
```

### adiciona um arquivo no repositório
```
git add aula1.txt
```

### adicionar todos os arquivos e pastas
```
git add --all | git add .
```

### lista o estado atual de arquivos e pastas do repositório
```
git status
```

### salva as mudanças no repositório
```
git commit -m "mensagem"
```

### cria um branch: teste
```
git branch teste
```

### mudar para outro branch: teste
```
git checkout teste
```

### listar branches locais
```
git branch
```

### listar branches locais e online
```
git branch -a
```

### renomear branch. OBS: branch padrão do github é o "main"
```
git branch -m nome-antigo novo-nome
```

### excluir um branch local. OBS: não deve estar localizado no branch que deseja remover
```
git branch -d nome-do-branch-local
```

### excluir um branch remoto
```
git push origin --delete nome-do-branch-remoto
```

### listar commits realizados
```
git log
```

### começar a trabalhar no ramo teste
```
git checkout teste
```

### listar chaves SSH
```
ls -al ~/.ssh
```

### gerar chave SSH
```
ssh-keygen -t ed25519 -C "your_email@example.com"
```

### adicionar chave SSH ao agente de SSH
```
eval "$(ssh-agent -s)"
```
```
ssh-add ~/.ssh/id_ed25519
```

### testar conexão SSH
```
ssh -T git@github.com
```

### associando um repositório local com o github
```
git remote add origin git@github.com:USUARIO/RESPOSITORIO.git
```
### enviando arquivos para o github
```
git push -u origin main
```
