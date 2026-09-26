# 🦅 Griffin — Agente de Educação e Consultoria Financeira

Griffin é um agente de Inteligência Artificial **educacional e consultivo**, criado para ajudar pessoas a entender conceitos financeiros, organizar metas e simular cenários de investimento — com foco especial em **CDI, renda fixa e planejamento por objetivos ("caixinhas")**.

> ⚠️ Projeto de finalidade **exclusivamente acadêmica**. O Griffin não substitui um profissional certificado e suas simulações não são garantia de rentabilidade.

---

## 🎯 Problema que resolve

Muita gente quer guardar ou investir dinheiro, mas trava em perguntas como:
- Quanto preciso investir por mês para chegar na minha meta?
- Quanto tempo vou levar para atingi-la?
- O que significa render "100% do CDI" ou "110% do CDI"?

O Griffin transforma essas dúvidas em planejamento simples e visual, sem prometer retornos e sem inventar dados.

## 🐦 Persona

| | |
|---|---|
| **Nome** | Griffin |
| **Personalidade** | Consultivo e educativo |
| **Tom** | Informal, claro e acessível a quem não entende de finanças |

## 🏗️ Como funciona

```
Usuário → Interface → LLM → Base de Conhecimento → Validação → Resposta
```

| Componente | Descrição |
|---|---|
| LLM | Ollama (local) |
| Base de Conhecimento | JSON/CSV mockados (`data/`) + datasets públicos de referência (BCB, Hugging Face) |
| Validação | Checagem anti-alucinação |

## 🧠 Base de Conhecimento

Além dos dados mockados originais (`transacoes.csv`, `perfil_investidor.json`, `produtos_financeiros.json`, `historico_atendimento.csv`), a base foi complementada com fontes públicas de referência:

- Séries do Banco Central (Selic, Selic acumulada, CDB/RDB pós-fixados)
- Dataset NVIDIA Nemotron (raciocínio financeiro)
- Dataset de Fundos de Crédito do Brasil (CVM)

Todos os dados de usuário utilizados são **fictícios ou sintéticos**.

## 🛡️ Segurança e Anti-Alucinação

O Griffin foi instruído a:
- Nunca inventar taxas, produtos ou rentabilidades
- Admitir quando não tem uma informação
- Nunca solicitar dados sensíveis (senha, CPF, conta bancária, etc.)
- Nunca prometer ou garantir retorno futuro
- Diferenciar sempre fatos, hipóteses e simulações

## 📊 Avaliação

O agente é avaliado por métricas como assertividade, precisão de cálculos, coerência financeira, anti-alucinação, privacidade e clareza educacional, através de 12 cenários de teste estruturados e avaliação por usuários (nota de 1 a 5).

## 📁 Estrutura

```
├── data/        # Dados mockados (perfil, transações, produtos, atendimentos)
├── docs/        # Documentação completa do agente
│   ├── 01-documentacao-agente.md
│   ├── 02-base-conhecimento.md
│   ├── 03-prompts.md
│   ├── 04-metricas.md
│   └── 05-pitch.md
├── src/         # Código do protótipo
└── assets/      # Imagens e diagramas
```

## 📄 Documentação completa

Para detalhes de arquitetura, system prompt completo, exemplos de interação e edge cases, veja a pasta [`docs/`](./docs).
