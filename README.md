# Comandos Essenciais do Git

## 📌 Configuração Inicial

### Definir utilizador e email
```bash
git config --global user.name "Teu Nome"
git config --global user.email "teu.email@exemplo.com"
```
Configura o nome e email usados nos commits.

### Ver configurações
```bash
git config --list
```
Mostra as configurações do Git.

---

## 📁 Inicializar e Clonar Repositório

### Criar um novo repositório
```bash
git init
```
Inicializa um novo repositório Git.

### Clonar um repositório remoto
```bash
git clone <url-do-repositorio>
```
Cria uma cópia local de um repositório remoto.

---

## 🔍 Estado do Repositório

### Verificar estado
```bash
git status
```
Mostra o estado atual dos ficheiros.

### Ver histórico de commits
```bash
git log
```
Exibe os commits do repositório.

---

## 📤 Trabalhar com Commits

### Adicionar ficheiros para commit
```bash
git add <ficheiro>
```
Adiciona um ficheiro específico.

```bash
git add .
```
Adiciona todos os ficheiros modificados.

### Fazer commit
```bash
git commit -m "Mensagem do commit"
```
Regista as alterações no repositório.

### Modificar última mensagem de commit
```bash
git commit --amend -m "Nova mensagem"
```
Edita a última mensagem de commit.

---

## 🔄 Sincronizar com Repositório Remoto

### Associar repositório remoto
```bash
git remote add origin <url-do-repositorio>
```
Define um repositório remoto chamado `origin`.

### Enviar alterações
```bash
git push origin <ramo>
```
Envia os commits para um ramo remoto.

### Obter alterações do remoto
```bash
git pull origin <ramo>
```
Atualiza o repositório local com mudanças do remoto.

---

## 🌿 Trabalhar com Ramos (Branches)

### Criar um novo ramo
```bash
git branch <nome-do-ramo>
```
Cria um novo ramo.

### Mudar para outro ramo
```bash
git checkout <nome-do-ramo>
```
Alterna para um ramo diferente.

### Criar e mudar de ramo ao mesmo tempo
```bash
git checkout -b <nome-do-ramo>
```
Cria e muda automaticamente para o novo ramo.

### Listar ramos
```bash
git branch
```
Mostra os ramos existentes.

### Eliminar um ramo
```bash
git branch -d <nome-do-ramo>
```
Apaga um ramo local.

---

## 🔗 Trabalhar com Merges

### Fazer merge de um ramo
```bash
git merge <nome-do-ramo>
```
Combina as alterações de um ramo com o atual.

### Resolver conflitos
```bash
git status
```
Verifica quais ficheiros têm conflitos.

Depois de resolver manualmente, adicionar os ficheiros resolvidos:
```bash
git add <ficheiro>
git commit -m "Resolvendo conflito"
```

---

## 🚨 Reverter Alterações

### Desfazer alterações em ficheiros não adicionados
```bash
git checkout -- <ficheiro>
```
Restaura um ficheiro modificado para a última versão commitada.

### Remover ficheiros do stage
```bash
git reset <ficheiro>
```
Remove um ficheiro da área de staging sem apagar alterações.

### Desfazer um commit
```bash
git revert <id-do-commit>
```
Cria um novo commit que reverte o commit especificado.

### Resetar repositório para um estado anterior
```bash
git reset --hard <id-do-commit>
```
Restaura o repositório para um commit anterior e apaga mudanças posteriores.

---

## 🔍 Ver e Comparar Alterações

### Ver diferenças entre ficheiros modificados e commitados
```bash
git diff
```
Mostra diferenças entre ficheiros alterados e a última versão commitada.

### Ver diferenças entre commits
```bash
git diff <commit1> <commit2>
```
Compara dois commits.

---

## 🗑️ Apagar e Restaurar

### Apagar ficheiro do repositório
```bash
git rm <ficheiro>
git commit -m "Removendo ficheiro"
```
Remove um ficheiro do repositório.

### Restaurar ficheiro apagado
```bash
git checkout HEAD -- <ficheiro>
```
Restaura um ficheiro apagado antes de um commit.

---

## 📌 Conclusão
Este guia contém os comandos mais essenciais do Git. Usa-o como referência rápida para gerir o teu código de forma eficiente! 🚀
