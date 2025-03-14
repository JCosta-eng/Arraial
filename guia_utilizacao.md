# Guia Rápido de Utilização do GitHub

## 📌 Configuração Inicial
```sh
# Configurar nome de usuário
$ git config --global user.name "Seu Nome"

# Configurar e-mail
$ git config --global user.email "seuemail@example.com"

# Verificar configurações
$ git config --list
```

## 📂 Criando e Clonando Repositórios
```sh
# Criar um novo repositório local
$ git init

# Clonar um repositório existente
$ git clone https://github.com/usuario/repo.git
```

## 📌 Trabalhando com Commits
```sh
# Verificar status dos arquivos
$ git status

# Adicionar arquivos ao stage
$ git add arquivo.txt   # Adiciona um arquivo específico
$ git add .             # Adiciona todos os arquivos modificados

# Criar um commit
$ git commit -m "Mensagem do commit"
```

## 🔄 Sincronizando com o GitHub
```sh
# Associar o repositório local ao remoto
$ git remote add origin https://github.com/usuario/repo.git

# Enviar alterações para o GitHub
$ git push -u origin main  # Primeiro envio
$ git push                 # Enviar alterações futuras

# Atualizar o repositório local com mudanças do remoto
$ git pull origin main
```

## 🔀 Trabalhando com Branches
```sh
# Criar uma nova branch
$ git branch nome-da-branch

# Alternar entre branches
$ git checkout nome-da-branch

# Criar e mudar para uma nova branch
$ git checkout -b nova-branch

# Mesclar uma branch na branch atual
$ git merge nome-da-branch

# Deletar uma branch local
$ git branch -d nome-da-branch
```

## 🤝 Trabalhando com Pull Requests
1. Crie uma branch e faça as alterações.
2. Envie a branch para o GitHub (`git push origin nome-da-branch`).
3. No GitHub, crie um **Pull Request**.
4. Aguarde revisão e aceite o merge.

## 🚀 Dicas Extras
```sh
# Ver histórico de commits
$ git log --oneline --graph --all

# Reverter um commit (desfaz alterações locais)
$ git reset --hard HEAD~1
```

📌 **Dica:** Sempre faça `git pull` antes de começar a trabalhar para evitar conflitos!
