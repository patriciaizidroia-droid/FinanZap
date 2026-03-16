# 💸 FinanZap

> Controle financeiro pessoal pelo WhatsApp com IA

![Status](https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow)
![Fase](https://img.shields.io/badge/Fase-1%20Ideação-blue)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 📌 Sobre o Projeto

O **FinanZap** é um sistema de controle financeiro pessoal que permite registrar despesas
diretamente pelo **WhatsApp**, utilizando **Inteligência Artificial para interpretar
mensagens em linguagem natural**.

A aplicação transforma mensagens simples em **registros estruturados de despesas**,
exibidos em um **dashboard financeiro inteligente**.

**Exemplo de uso:**
👤 Usuário: "gastei 45 reais no almoço hoje"

🤖 FinanZap: "✅ Registrado! R$ 45,00 em Alimentação."




---

## 🎯 Problema

Grande parte das pessoas não controla seus gastos porque:

- Aplicativos financeiros exigem disciplina para abrir
- Registrar despesas manualmente é cansativo
- Planilhas são abandonadas rapidamente

---

## 💡 Solução

O **FinanZap** utiliza o **WhatsApp** — canal que as pessoas já usam diariamente:

- O usuário envia uma mensagem como se estivesse conversando
- A IA interpreta, extrai os dados e registra automaticamente a despesa
- Os dados são exibidos em gráficos e relatórios no dashboard

---

## 🏗️ Arquitetura
Usuário → WhatsApp → Evolution API → Backend Node.js │ OpenAI API │ Supabase (PostgreSQL) │ Dashboard React




---

## 📊 Funcionalidades

### 🤖 Bot WhatsApp
- [x] Registrar despesas via mensagem natural
- [x] Responder consultas ("Quanto gastei esse mês?")
- [x] Alertar gastos excessivos por categoria
- [x] Confirmar registros ao usuário

### 📈 Dashboard Web
- [x] Gráfico de gastos por categoria
- [x] Gastos por mês (barras)
- [x] Histórico completo de despesas
- [x] Filtros por período e categoria

### 🎮 Gamificação
- [x] Sistema de XP por registros consistentes
- [x] Níveis financeiros (Iniciante → Expert)
- [x] Conquistas e recompensas

---

## 🛠️ Tecnologias

| Camada         | Tecnologia            |
|----------------|-----------------------|
| Backend        | Node.js               |
| Banco de Dados | Supabase (PostgreSQL) |
| WhatsApp API   | Evolution API         |
| Frontend       | React + Tailwind CSS  |
| IA             | OpenAI API            |

---

## 📅 Cronograma

| Fase   | Descrição                  | Data       |
|--------|----------------------------|------------|
| Fase 1 | Ideação e Estruturação     | 25/03/2026 |
| Fase 2 | Arquitetura do Sistema     | 15/04/2026 |
| Fase 3 | Construção do MVP          | 20/05/2026 |
| Fase 4 | Entrega Final              | 27/05/2026 |

---

## 👩‍💻 Autora

Desenvolvido por **Patrícia** — Projeto Acadêmico 2026

---

## 📄 Licença

Este projeto está sob a licença [MIT](LICENSE).
