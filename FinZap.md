<div align="center">

# 💸 FinanZap

### Controle financeiro pessoal pelo WhatsApp com IA

## 📌 Sobre o Projeto

O **FinanZap** é um sistema de controle financeiro pessoal que permite registrar despesas
diretamente pelo **WhatsApp**, utilizando **Inteligência Artificial para interpretar
mensagens em linguagem natural**.

A aplicação transforma mensagens simples enviadas pelo usuário em **registros estruturados
de despesas**, exibidos posteriormente em um **dashboard financeiro inteligente**.

**Exemplo de mensagem enviada pelo usuário:**

```
gastei 45 reais no almoço hoje
```

**Resposta processada pela IA:**

```json
{
  "valor": 45.00,
  "categoria": "alimentação",
  "descricao": "almoço",
  "data": "2026-03-15"
}
```

Esses dados são armazenados e apresentados em gráficos e relatórios financeiros.

---

## 🎯 Problema

Grande parte das pessoas não controla seus gastos porque:

- aplicativos financeiros exigem disciplina para abrir
- registrar despesas manualmente é cansativo
- planilhas são abandonadas rapidamente

Como resultado, muitos usuários perdem o controle financeiro ao longo do mês.

---

## 💡 Solução

O **FinanZap** resolve esse problema utilizando um canal que as pessoas já usam
diariamente: o **WhatsApp**.

- O usuário simplesmente envia uma mensagem como se estivesse conversando
- A IA interpreta a mensagem, extrai os dados e registra automaticamente a despesa

---

## 👤 Personas

### Persona 1 — Ana (28 anos)

| | |
|---|---|
| **Perfil** | Profissional autônoma que trabalha majoritariamente pelo WhatsApp |
| **Problema** | Esquece de registrar despesas nos aplicativos financeiros |
| **Solução** | Registrar gastos sem sair do WhatsApp |

### Persona 2 — Carlos (35 anos)

| | |
|---|---|
| **Perfil** | Funcionário CLT com família e despesas mensais fixas |
| **Problema** | Já tentou planilhas financeiras, mas abandona após algumas semanas |
| **Solução** | Visualizar gastos através de gráficos simples e automáticos |

---

## 🤖 Persona da IA

A IA do sistema atua como um **analista financeiro automatizado**.

| | |
|---|---|
| **Papel** | Interpretar mensagens enviadas pelos usuários e extrair informações estruturadas |

**Funções:**
- identificar valores monetários
- identificar categorias de despesas
- extrair descrição do gasto
- identificar datas relativas

**Características — a IA deve:**
- responder de forma objetiva
- retornar apenas JSON
- não inventar valores
- não adicionar texto extra

---

## 🧠 Engenharia de Prompt

A classificação das despesas utiliza **prompt estruturado**.

### Prompt principal

```
Você é um assistente que extrai dados financeiros de mensagens de usuários.

Sua tarefa é analisar a mensagem e retornar um JSON com:
- valor
- categoria
- descricao
- data

Categorias possíveis:
alimentação | transporte | moradia | lazer | compras | saúde | educação | outros

Mensagem do usuário:
{mensagem}
```

---

## ⚡ Vibe Coding

O desenvolvimento do projeto utilizou **IA generativa como assistente de programação**.

**Fluxo de desenvolvimento:**

```
Ideia → Prompt para IA → Geração de código → Revisão humana → Refinamento → Código final
```

**Ferramentas utilizadas:**

| Ferramenta | Uso |
|---|---|
| ChatGPT | Geração de código e debugging |
| Claude | Revisão e refatoração |
| GitHub Copilot | Sugestões em tempo real no editor |
| v0.dev | Prototipação visual do dashboard |

**A IA foi utilizada para:**
- geração de endpoints
- criação de componentes React
- geração de queries SQL
- revisão de código

> ⚠️ Todo código gerado foi **revisado manualmente** antes de ser aceito no projeto.

---

## 🏗️ Arquitetura do Sistema

```
Usuário
   │
   ▼
WhatsApp
   │
   ▼
Evolution API
   │
   ▼
Backend Node.js
   │
   ▼
OpenAI API
   │
   ▼
Supabase (PostgreSQL)
   │
   ▼
Dashboard React
```

---

## 🔁 Fluxo de Funcionamento

```
1. Usuário envia mensagem no WhatsApp
         ↓
2. Webhook recebe a mensagem
         ↓
3. Backend envia mensagem para OpenAI
         ↓
4. IA extrai dados estruturados (JSON)
         ↓
5. Dados são armazenados no Supabase
         ↓
6. Dashboard atualiza gráficos em tempo real
```

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

