# Hollo world de novo
# Minoro fez alterações
# Fluxo Básico de Uso do Git com GitHub

Este documento descreve o passo a passo para configurar um repositório Git local a partir do GitHub, fazer commits, push, pull e rollback.

---

## 1. Criar o repositório no GitHub

- Vá até [https://github.com](https://github.com)
- Clique em **New Repository**
- Dê um nome ao repositório
- **Desmarque** a opção de criar um README
- Clique em **Create Repository**

---

## 2. Iniciar o repositório localmente

Ainda no GitHub, copie os comandos que ele gera, depois no terminal do projeto:

```bash
git init //Incio do projeto
git add . //Adicionar TOTOS os arquivos para o commit
git commit -m "Primeiro commit" //Entre aspas é marcada o nome da alteração NUNCA POR PUTARIA
```
Agora cole os comandos que vc copiou 


---

3. Depois, para novos commits

Navegue até a pasta do projeto e rode:
```bash
git add .
git commit -m "Mensagem do commit"
git push //Mandando as alterações commitadas para a branch
```

---

4. Para puxar alterações do repositório remoto (quando outra pessoa fez push ou vc mudou de branch)

```bash
git pull 
```

---
5. Para fazer um fork de outra branch

```bash
git checkout -b nova-branch branch-que-vc-quer-clonar
```
5.1 Fazendo pull request

```bash
após alteração na branch fazer pull request para juntar branchs
```

---
6. Como desfazer um commit local (rollback antes do push)

Se você fez um commit, mas ainda não deu push, pode desfazê-lo com:
```bash
git reset --soft HEAD~1
```
> Isso volta o commit, mas mantém as alterações nos arquivos. Se quiser descartar completamente:


```bash
git reset --hard HEAD~1
```

---

7. Dicas úteis

Ver o histórico de commits:

```bash
git log
```
Ver status de alterações:

```bash
git status
```
Ver diferença de arquivos alterados:

```bash
git diff
```

Mudar de branch
```bash
git checkout nome-da-branch
```

---

Dicas extras, instale as extensões do git para o Vs code.
