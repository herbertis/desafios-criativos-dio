# 🎯 Desafio Criativo: Prototipação do Educador Financeiro Inteligente
### Curso: IA React — DIO

---

## 🧱 Passo 1: Defina o papel do Educador Financeiro

```txt
Crie a ideia de um Educador Financeiro Inteligente voltado para trabalhadores autônomos e freelancers.

O principal problema dessa pessoa é a renda irregular mês a mês, o que dificulta o planejamento
de despesas fixas, o pagamento de impostos e a criação de reservas financeiras.

A solução deve ajudar o usuário a organizar suas receitas variáveis, separar automaticamente
percentuais para impostos e emergências, e visualizar se o mês será positivo ou negativo
com base no histórico.

O sistema deve se comunicar de forma direta, sem julgamentos, com linguagem acessível e
exemplos do dia a dia do trabalhador independente.

A interface será construída com React, aproveitando componentes reutilizáveis, gerenciamento
de estado com hooks e integração com APIs de IA para geração de dicas personalizadas em tempo real.
```

---

## 🧱 Passo 2: Adicione recursos e experiências inteligentes

```txt
O Educador Financeiro Inteligente deve possuir os seguintes recursos:

1. Registro rápido de entradas e saídas com categorização automática por tipo
   (serviço prestado, despesa fixa, imposto, lazer) — implementado como um componente
   React com formulário controlado e validação em tempo real via useState e useReducer.

2. Simulação de cenários interativos: "Se eu receber X este mês, quanto posso gastar com Y?"
   — renderizado como um componente de simulador com sliders e gráficos usando Recharts ou Chart.js
   integrado ao React.

3. Chat com IA Financeira: painel de conversa onde o usuário faz perguntas sobre suas finanças
   e recebe respostas personalizadas geradas por um modelo de linguagem (ex: OpenAI API ou
   Vercel AI SDK), com streaming de respostas via useChat hook.

A IA deve adaptar as recomendações com base no histórico de receitas dos últimos 3 meses,
nas metas definidas pelo usuário e no percentual de impostos do seu regime tributário.
Esses dados serão armazenados via Context API ou Zustand para persistência entre componentes.

Evite respostas genéricas como "gaste menos" sem contexto, linguagem bancária formal e
sugestões que ignoram a realidade da renda variável.

As sugestões devem ser apresentadas no formato de cards React reutilizáveis com alerta
visual (cor, ícone) e no máximo 3 passos práticos por recomendação.
```

---

## 🧱 Passo 3: Prompt Final — Proposta Completa

```txt
Atue como um especialista em educação financeira digital e desenvolvimento frontend com React.

Crie a proposta de um Educador Financeiro Inteligente para trabalhadores autônomos e
freelancers brasileiros com renda variável, desenvolvido como uma aplicação React com
integração a uma API de IA (como OpenAI ou Gemini).

O sistema deve ajudar o usuário a:
- Organizar receitas irregulares e projetar o fluxo de caixa mensal
- Separar automaticamente reservas para impostos, emergências e investimentos
- Conversar com uma IA financeira contextualizada ao seu perfil e histórico
- Aprender conceitos financeiros de forma progressiva e interativa

As principais funcionalidades devem incluir:
- Dashboard React com gráficos de fluxo de caixa (Recharts) e projeção inteligente
- Componente de simulador de cenários com sliders interativos
- Chat com IA usando streaming de respostas (Vercel AI SDK ou OpenAI API)
- Sistema de alertas personalizados renderizados como cards com status visual

Stack tecnológica:
- React 18+ com hooks (useState, useEffect, useContext, useReducer)
- Vercel AI SDK ou OpenAI SDK para integração com modelo de linguagem
- Recharts ou Chart.js para visualização de dados financeiros
- Tailwind CSS para estilização dos componentes
- React Router para navegação entre telas (Dashboard, Chat, Metas, Histórico)
- Context API ou Zustand para gerenciamento de estado global

A comunicação deve ser direta, empática e sem jargões — como um amigo que entende de
finanças e respeita a realidade do trabalhador independente.

As respostas da IA devem chegar via streaming, com feedback visual de "digitando..."
para uma experiência fluida e moderna.

Evite sugestões genéricas desconectadas da renda variável, comparações com assalariados
e recomendações que exijam aportes fixos mensais sem flexibilidade.

Ao final, apresente sugestões criativas para o projeto React, incluindo:
- Estrutura de pastas e principais componentes a criar
- Paleta de cores e identidade visual sugerida
- Ideia de onboarding gamificado com React (ex: wizard de 3 etapas com animações Framer Motion)
- Como integrar a IA de forma progressiva: primeiro regras, depois modelo generativo
```

---

## 🛠️ Estrutura React Sugerida

```
src/
├── components/
│   ├── Dashboard/        # Gráficos e resumo financeiro
│   ├── ChatIA/           # Interface de chat com streaming
│   ├── Simulador/        # Simulador de cenários
│   ├── AlertCard/        # Cards de alertas personalizados
│   └── Onboarding/       # Wizard de configuração inicial
├── context/
│   └── FinanceContext.js # Estado global (receitas, metas, perfil)
├── hooks/
│   ├── useFinance.js     # Lógica de cálculos financeiros
│   └── useAIChat.js      # Hook de integração com IA
├── pages/
│   ├── Home.jsx
│   ├── Chat.jsx
│   ├── Metas.jsx
│   └── Historico.jsx
└── services/
    └── aiService.js      # Chamadas à API de IA
```

---

*Desafio concluído — Herbert Ishimura Sousa | Curso IA React — DIO | 2026*
