# 📘 Fluxo Oficial de Trabalho — GrowDev

Este documento define **como a GrowDev trabalha no dia a dia usando GitHub**.

Ele existe para:

* Evitar confusão
* Ajudar quem nunca trabalhou em equipe
* Criar um padrão claro e justo
* Simular um ambiente profissional real

👉 **Não é para decorar. É para consultar.**

---

## 🌱 Princípios da GrowDev

Antes da técnica, alguns acordos importantes:

* Todos estão aprendendo
* Errar faz parte do processo
* Código não é pessoal
* Comunicação é obrigatória
* Organização vem antes de velocidade

---

## 🧩 Papéis no time

### 👤 Integrante (desenvolvedor)

* Pode pegar issues
* Cria branches
* Desenvolve código
* Abre Pull Requests
* Participa de reviews

### 🧭 Líder técnico (fundador)

* Define padrões
* Ajuda nas decisões técnicas
* Revisa Pull Requests
* Realiza merges (por enquanto)
* Garante a saúde do projeto

⚠️ Isso **não significa hierarquia rígida**, apenas responsabilidade.

---

## 📝 Issues — ponto de partida de tudo

Na GrowDev, **tudo começa por uma Issue**.

Uma issue pode representar:

* Um bug
* Uma funcionalidade
* Uma tarefa técnica
* Um estudo ou melhoria

### 📌 Regras importantes

* Não trabalhe sem issue
* 1 issue = 1 responsável
* 1 issue = 1 branch

As issues existem para:

* Dar clareza
* Evitar trabalho duplicado
* Registrar decisões

---

## 🌿 Branches — onde o trabalho acontece

Nunca trabalhamos direto na `main`.

### 🔹 Passo 1 — Atualizar a base

Antes de criar qualquer branch:

```bash
git checkout main
git pull origin main
```

Isso garante que sua branch nasce atualizada.

---

### 🔹 Passo 2 — Criar a branch

Padrão GrowDev:

```
tipo/numero-da-issue-descricao
```

Exemplos:

* `feature/12-login`
* `bug/7-corrigir-erro-auth`
* `task/20-ajustar-readme`

Comando:

```bash
git checkout -b feature/12-login
```

👉 Todo o trabalho da issue acontece **somente nessa branch**.

---

## 💾 Commits — pequenos e claros

Commits devem ser:

* Pequenos
* Objetivos
* Relacionados à issue

Exemplo:

```
feat: cria endpoint de login
```

Evite:

* Commits gigantes
* Mensagens genéricas ("ajustes", "teste")

---

## 📤 Pull Requests — pedido de revisão

Quando a issue estiver concluída:

1. Envie sua branch:

```bash
git push origin feature/12-login
```

2. Abra um Pull Request no GitHub

### 📄 Estrutura do PR

**Título:**

```
[FEATURE] Login de usuários
```

**Descrição:**

```md
## O que foi feito
- Tela de login criada
- Validação básica

## Issue relacionada
Closes #12
```

⚠️ Quem cria o PR **não faz o próprio merge**.

---

## 👀 Review — aprender juntos

O review serve para:

* Melhorar código
* Aprender
* Garantir qualidade

Durante o review, observe:

* Código funciona?
* Está legível?
* Segue a issue?

Ações possíveis:

* ✅ Approve
* 🔄 Request changes

---

## 🔗 Merge — juntando na main

Por enquanto, na GrowDev:

👉 **O líder técnico realiza o merge**

O merge só acontece quando:

* O PR foi revisado
* Está aprovado

Após o merge:

* A issue é fechada automaticamente
* A branch pode ser deletada

---

## 🔁 Fluxo resumido

```
Issue criada
   ↓
Dev pega a issue
   ↓
Cria branch
   ↓
Desenvolve
   ↓
Commit
   ↓
Pull Request
   ↓
Review
   ↓
Merge
   ↓
Issue fechada
```

---

## 🚫 O que evitar

* Trabalhar sem issue
* Commits diretos na main
* PR sem descrição
* Merge sem review

---

## 🤝 Cultura GrowDev

Mais importante que código:

* Comunicação
* Respeito
* Compromisso
* Vontade de aprender

Aqui ninguém é perfeito.
Aqui todo mundo cresce.

---

> GrowDev — crescer juntos é o projeto.
