# 📘 Curso de Git e GitHub - Alura

Este repositório contém anotações e exemplos de uso do Git e GitHub, conforme estudado no curso da [Alura](https://www.alura.com.br/). Aqui você encontrará demonstrações de comandos **básicos**, **intermediários** e **avançados** para versionamento e colaboração.

---

## Configuração Inicial

### Configurar nome e e-mail
```
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@example.com"
```

### Verificar configurações
```
git config --list
```

---

## Criando e Inicializando Repositório

### Iniciar repositório
```
git init
```

### Clonar repositório remoto
```
git clone https://github.com/usuario/repositorio.git
```

---

## Controle de Versionamento

### Verificar status dos arquivos
```
git status
```

### Adicionar arquivos ao staging
```
git add nome_arquivo
```
Ou todos:
```
git add .
```

### Confirmar alterações (commit)
```
git commit -m "Mensagem do commit"
```

### Adicionar e commitar de uma vez
```
git commit -am "Mensagem do commit"
```

---

## Atualização e Sincronização

### Atualizar repositório local
```
git pull
```

### Enviar commits para o remoto
```
git push
```

---

## Trabalhando com Branches

### Criar nova branch
```
git branch nome_da_branch
```

### Listar branches
```
git branch
```

### Mudar de branch
```
git checkout nome_da_branch
```

### Criar e mudar de branch de uma vez
```
git checkout -b nome_da_branch
```

### Mesclar branch atual com outra
```
git merge nome_da_branch
```

---

## Removendo e Desfazendo Alterações

### Remover arquivo do stage
```
git reset nome_arquivo
```

### Desfazer alterações locais (não commitadas)
```
git checkout -- nome_arquivo
```

### Resetar branch para commit anterior (perde alterações)
```
git reset --hard id_do_commit
```

---

## Histórico e Log

### Ver histórico de commits
```
git log
```

### Histórico resumido
```
git log --oneline
```

### Mostrar alterações entre commits
```
git diff
```

---

## Comandos Avançados e Úteis

### Ignorar arquivos
Crie um arquivo chamado `.gitignore` e adicione:
```
*.log
node_modules/
.env
```

---

### Stash (guardar alterações temporariamente)
```
git stash
```

### Listar stashes
```
git stash list
```

### Recuperar stash
```
git stash apply
```

---

### Rebase (reescrever histórico)
```
git rebase nome_da_branch
```

---

### Tag (marcar versões)
```
git tag -a v1.0 -m "Versão 1.0"
git push origin v1.0
```

---

## Dicas

- Sempre verifique o status antes de commitar (`git status`).
- Use branches para novas funcionalidades.
- Para resolver conflitos, edite os arquivos, depois faça `add` e `commit`.
- Nunca faça `rebase` em branches compartilhadas sem combinar com a equipe.

---

## Referências

- [Documentação Oficial do Git](https://git-scm.com/doc)
- [Curso Git e GitHub - Alura](https://www.alura.com.br/)
