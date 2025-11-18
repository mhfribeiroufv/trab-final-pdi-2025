# Mini Guia de Uso do Git e GitHub

Este guia apresenta os comandos essenciais para usar **Git** e trabalhar com repositórios no **GitHub**.  
Ideal para quem precisa clonar o repositório do trabalho, fazer commits e sincronizar alterações.

---

## 🚀 1. Configuração Inicial

Configure seu nome e e-mail (necessário para registrar autorias):

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@example.com"
```

Verifique:

```bash
git config --list
```

---

## 📥 2. Clonar um Repositório

Para baixar o repositório para sua máquina:

```bash
git clone https://github.com/usuario/repositorio.git
```

Entre na pasta:

```bash
cd repositorio
```

---

## 📌 3. Verificar Status

Mostra arquivos modificados, adicionados ou não rastreados:

```bash
git status
```

---

## ➕ 4. Adicionar Arquivos ao Commit

Adicionar um arquivo específico:

```bash
git add arquivo.extensao
```

Adicionar tudo:

```bash
git add .
```

---

## 📝 5. Fazer um Commit

```bash
git commit -m "Mensagem do commit explicando o que foi feito"
```

---

## 🔄 6. Baixar Atualizações do Repositório Remoto

Antes de enviar suas alterações, sempre sincronize:

```bash
git pull
```

Se houver conflitos, resolva e confirme com:

```bash
git add .
git commit -m "Resolvendo conflitos"
```

---

## 📤 7. Enviar Alterações para o GitHub

```bash
git push
```

Se for a primeira vez, pode ser necessário:

```bash
git push -u origin main
```

*(ou `master`, dependendo do nome do branch)*

---

## 🌿 8. Criar e Usar Branches (opcional)

Criar um novo branch:

```bash
git branch nome-do-branch
```

Trocar para o branch:

```bash
git checkout nome-do-branch
```

Criar e trocar ao mesmo tempo:

```bash
git checkout -b nome-do-branch
```

Enviar branch para o GitHub:

```bash
git push -u origin nome-do-branch
```

---

## 🔀 9. Mesclar Branches

Voltar para o branch principal:

```bash
git checkout main
```

Mesclar:

```bash
git merge nome-do-branch
```

---

## 🗑️ 10. Descartar Modificações

Voltar um arquivo ao estado salvo:

```bash
git checkout -- arquivo.extensao
```

Remover tudo que não foi commitado:

```bash
git restore .
```

---

## 🗂️ 11. Ignorar Arquivos (com `.gitignore`)

Criar o `.gitignore`:

```bash
touch .gitignore
```

Exemplo de conteúdo:

```
*.pyc
__pycache__/
*.ipynb_checkpoints/
```

---

## 🔐 12. Autenticação no GitHub

Com token pessoal (PAT):

```bash
git clone https://github.com/usuario/repositorio.git
Username: seu-usuario
Password: cole-seu-token-aqui
```

---

## 🎯 Resumo dos Comandos Mais Usados

```bash
git clone URL
git status
git add .
git commit -m "mensagem"
git pull
git push
```

Simples e suficiente para 95% dos casos.

---

## 🆘 Ajuda

Ver documentação:

```bash
git help
git help <comando>
```

---

Bom trabalho! E lembre-se: **commits pequenos e frequentes ajudam muito.**