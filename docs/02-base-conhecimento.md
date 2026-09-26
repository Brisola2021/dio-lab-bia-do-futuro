# 🧠 Base de Conhecimento

Esta documentação descreve as fontes de dados utilizadas como referência
para a construção da base de conhecimento do agente financeiro.

O projeto possui finalidade exclusivamente acadêmica e tem como foco
investimentos relacionados ao CDI, renda fixa, definição de metas,
simulações financeiras e geração de sugestões educacionais.

---

## 📊 Dados Utilizados

Os dados locais utilizados pelo projeto estão armazenados na pasta
[`data`](../data).

| Arquivo | Formato | Utilização no Agente |
|---|---|---|
| `historico_atendimento.csv` | CSV | Contextualizar interações anteriores |
| `perfil_investidor.json` | JSON | Personalizar sugestões conforme perfil simulado |
| `produtos_financeiros.json` | JSON | Apresentar produtos financeiros compatíveis com o contexto |
| `transacoes.csv` | CSV | Analisar padrões financeiros simulados |

> [!IMPORTANT]
> Todos os dados relacionados a usuários utilizados neste projeto são
> fictícios ou sintéticos. Nenhum dado pessoal, bancário ou informação
> financeira sensível de pessoas reais é utilizado.

---

# 📚 Datasets e Fontes de Referência

Para complementar a base de conhecimento foram selecionadas fontes públicas
voltadas a documentos, finanças, renda fixa e indicadores do mercado
financeiro brasileiro.

As fontes externas não representam dados pessoais dos usuários do agente.
Elas são utilizadas como referência acadêmica para análise, contextualização
e futuras integrações.

---

## 📄 1. IIT-CDIP-CSV — Processamento de Documentos

> [!IMPORTANT]
> **Dataset:** IIT-CDIP-CSV  
> **Plataforma:** Hugging Face  
> **Publicador:** RIPS-Goog-23  
> **Área:** Processamento documental / OCR  
> **Fonte:** [RIPS-Goog-23/IIT-CDIP-CSV](https://huggingface.co/datasets/RIPS-Goog-23/IIT-CDIP-CSV)

O dataset IIT-CDIP-CSV é utilizado como referência para demonstrar como
documentos digitalizados e dados não estruturados podem ser incorporados
a uma base de conhecimento.

### 🔎 Possíveis aplicações

- processamento de documentos digitalizados;
- extração de informações através de OCR;
- organização de informações não estruturadas;
- recuperação de informações;
- construção de bases de conhecimento;
- utilização de documentos como contexto para agentes de IA.

---

## 💰 2. NVIDIA Nemotron Specialized Domains — Finance

> [!IMPORTANT]
> **Dataset:** Nemotron-SpecializedDomains-Finance-v1  
> **Organização:** NVIDIA  
> **Plataforma:** Hugging Face  
> **Área:** Finanças e raciocínio financeiro  
> **Idioma:** Inglês  
> **Formato:** JSONL  
> **Licença:** CC BY 4.0  
> **Fonte:** [NVIDIA Nemotron Finance](https://huggingface.co/datasets/nvidia/Nemotron-SpecializedDomains-Finance-v1)

O Nemotron-SpecializedDomains-Finance-v1 é utilizado como referência para
conhecimento financeiro especializado e compreensão de documentos
corporativos.

O dataset possui mais de 326 mil pares de perguntas e respostas produzidos
a partir de documentos regulatórios de empresas do S&P 500, incluindo
relatórios 10-K e 10-Q publicados entre 2019 e 2024.

### 🧠 Conhecimentos complementares

- finanças corporativas;
- interpretação de indicadores financeiros;
- análise de desempenho;
- fatores de risco;
- governança;
- conformidade regulatória;
- compreensão de documentos financeiros;
- perguntas e respostas especializadas;
- raciocínio financeiro baseado em contexto.

> [!NOTE]
> Como o conteúdo é predominantemente relacionado ao mercado norte-americano,
> esta fonte é utilizada como complemento conceitual. Para informações
> relacionadas ao mercado brasileiro, são priorizadas fontes oficiais
> nacionais.

---

# 🇧🇷 Indicadores do Mercado Financeiro Brasileiro

Para contextualização de investimentos relacionados ao CDI e à renda fixa,
o projeto utiliza como referência séries públicas disponibilizadas pelo
Banco Central do Brasil.

Essas séries permitem complementar o agente com informações históricas
sobre juros e produtos financeiros pós-fixados.

---

## 📈 3. Taxa Selic — Série Histórica

> [!IMPORTANT]
> **Fonte:** Banco Central do Brasil  
> **Sistema:** SGS — Sistema Gerenciador de Séries Temporais  
> **Código SGS:** 11  
> **Indicador:** Taxa Selic  
> **Fonte oficial:** [Banco Central — Taxa Selic](https://dadosabertos.bcb.gov.br/dataset/11-taxa-de-juros---selic)

A série histórica da Taxa Selic pode ser utilizada como referência
macroeconômica para contextualizar o comportamento dos juros no Brasil.

Embora Selic e CDI não sejam o mesmo indicador, ambos apresentam forte
relação no mercado de juros de curto prazo.

### 🎯 Aplicações no projeto

- contextualização do cenário de juros;
- análise histórica;
- comparação entre períodos;
- apoio a simulações de renda fixa;
- acompanhamento da evolução das taxas;
- contextualização de investimentos pós-fixados.

---

## 📅 4. Taxa Selic Acumulada no Mês

> [!IMPORTANT]
> **Fonte:** Banco Central do Brasil  
> **Sistema:** SGS  
> **Código SGS:** 4390  
> **Periodicidade:** Mensal  
> **Unidade:** % ao mês  
> **Fonte oficial:** [BCB — Selic acumulada no mês](https://dadosabertos.bcb.gov.br/dataset/4390-taxa-de-juros---selic-acumulada-no-mes)

Esta série apresenta a Taxa Selic acumulada mensalmente e pode ser utilizada
em análises e simulações relacionadas à evolução de investimentos ao longo
do tempo.

### 🎯 Aplicações no projeto

- simulação mensal de investimentos;
- acompanhamento de metas financeiras;
- comparação de cenários;
- análise histórica de juros;
- projeções educacionais;
- comparação entre aportes e evolução de patrimônio.

---

## 🏦 5. CDB/RDB Pós-Fixados

> [!IMPORTANT]
> **Dataset:** Taxa média mensal pós-fixada de depósitos a prazo (CDB/RDB)  
> **Fonte:** Banco Central do Brasil  
> **Sistema:** SGS  
> **Código SGS:** 28663  
> **Periodicidade:** Mensal  
> **Unidade:** % ao ano  
> **Fonte oficial:** [BCB — CDB/RDB Pós-Fixados](https://dadosabertos.bcb.gov.br/dataset/28663-taxa-media-mensal-pos-fixada-de-depositos-a-prazo-cdb-rdb-total)

Esta série possui especial importância para o projeto por apresentar
informações sobre taxas médias praticadas em CDBs e RDBs pós-fixados.

Como produtos dessa categoria frequentemente possuem sua rentabilidade
associada a taxas pós-fixadas, essa base permite enriquecer as análises
relacionadas ao tema central do projeto.

### 🎯 Aplicações no projeto

- análise de investimentos pós-fixados;
- comparação de rentabilidade;
- contextualização de CDB e RDB;
- apoio a simulações relacionadas ao CDI;
- comparação entre diferentes cenários de juros;
- construção de exemplos educacionais de renda fixa.

---

## 📊 6. Fundos de Crédito do Brasil

> [!IMPORTANT]
> **Dataset:** Fundos de Crédito do Brasil  
> **Plataforma:** Hugging Face  
> **Origem dos dados:** Dados públicos da CVM  
> **Formato:** Parquet  
> **Área:** Fundos / Crédito / Renda Fixa  
> **Licença:** MIT  
> **Fonte:** [Fundos de Crédito do Brasil](https://huggingface.co/datasets/claudiormpaes/fundos-credito-br)

Este dataset reúne informações processadas a partir de dados públicos
da Comissão de Valores Mobiliários (CVM).

A base contém métricas relacionadas a fundos de crédito, incluindo
informações de patrimônio, retornos, volatilidade, fluxo de recursos
e características das carteiras.

### 📊 Exemplos de informações disponíveis

- patrimônio líquido;
- retorno;
- volatilidade;
- drawdown;
- captação;
- resgates;
- fluxo líquido;
- quantidade de cotistas;
- crédito privado;
- debêntures;
- títulos públicos;
- classificação e características dos fundos.

### 🎯 Aplicações no projeto

- comparação entre alternativas de renda fixa;
- análise educacional de risco e retorno;
- contextualização de fundos de crédito;
- comparação com estratégias pós-fixadas;
- demonstração de diversificação;
- construção de cenários financeiros.

---

# 🎯 Aplicação das Fontes no Agente

As diferentes fontes possuem funções complementares dentro da arquitetura
conceitual do projeto.

| Fonte | Categoria | Aplicação |
|---|---|---|
| Dados sintéticos locais | Usuário | Perfil, metas e comportamento financeiro fictício |
| IIT-CDIP-CSV | Documentos | Processamento e recuperação de informações |
| NVIDIA Nemotron Finance | Conhecimento | Raciocínio e compreensão financeira |
| BCB SGS 11 | Juros | Contextualização histórica da Selic |
| BCB SGS 4390 | Juros | Simulações e acompanhamento mensal |
| BCB SGS 28663 | Renda Fixa | Análise de CDB/RDB pós-fixados |
| Fundos de Crédito BR | Investimentos | Comparações de fundos, risco e retorno |

---

# 🧩 Estratégia de Integração

A base de conhecimento foi organizada em três camadas principais:

### 👤 1. Contexto do Usuário

Dados totalmente fictícios ou sintéticos utilizados para representar:

- perfil de investidor;
- objetivo financeiro;
- capital inicial;
- aporte mensal;
- horizonte de investimento;
- tolerância a risco.

### 📈 2. Contexto de Mercado

Dados públicos utilizados como referência para:

- Selic;
- investimentos pós-fixados;
- CDB/RDB;
- renda fixa;
- fundos de crédito;
- cenários históricos de juros.

### 🧠 3. Conhecimento Financeiro

Datasets e documentos utilizados como referência para:

- conceitos financeiros;
- interpretação de informações;
- raciocínio financeiro;
- educação financeira;
- explicação de produtos;
- comparação de cenários.

---

# 🤖 Objetivo da Base de Conhecimento

A combinação dessas fontes permitirá evoluir o agente para auxiliar,
em contexto acadêmico, na realização de tarefas como:

- 💰 simular investimentos relacionados ao CDI;
- 🎯 estabelecer metas financeiras;
- 📅 calcular aportes necessários para determinado objetivo;
- 📈 comparar cenários de rentabilidade;
- 🏦 explicar CDBs e outros investimentos pós-fixados;
- 📊 contextualizar Selic e CDI;
- 💡 apresentar sugestões educacionais conforme um perfil fictício;
- 🔄 acompanhar a evolução simulada de metas;
- 🧮 demonstrar o efeito de aportes recorrentes e juros compostos.

> [!WARNING]
> Este projeto possui finalidade exclusivamente acadêmica e educacional.
> As informações, simulações e sugestões produzidas pelo agente não
> constituem recomendação profissional de investimento.
>
> O projeto não utiliza dados bancários reais, documentos pessoais,
> credenciais, informações de contas ou qualquer outro dado pessoal
> sensível de usuários.

---

## 🚀 Expansões Futuras

Como evolução do projeto, poderão ser implementadas integrações automáticas
com APIs públicas para atualização de indicadores financeiros, mecanismos
de recuperação de conhecimento (RAG), simulações de investimentos e
acompanhamento de metas financeiras fictícias.

---

## Adaptações nos Dados

> Você modificou ou expandiu os dados mockados? Descreva aqui.

Eu não modifiquei os arquivos existentes em sí, porém complementei alguns arquivos e adicionei links de datasets para aumentar a robustez do projeto.

---

## Estratégia de Integração

### Como os dados são carregados?
> Descreva como seu agente acessa a base de conhecimento.

Podem ser injetados via prompt de comando ou executados via código, como no exemplo abaixo:

```
import pandas as pd
import json

# CSVs
historico = pd.read_csv('data/historico_atendimento.csv')
transacoes = pd.read_csv('data/transacoes.csv')

# JSONs
with open('data/perfil_investidor.json', 'r', encoding='utf-8') as f:
    perfil = json.load(f)

with open('data/produtos_financeiros.json', 'r', encoding='utf-8') as f:
    produtos = json.load(f)
```

### Como os dados são usados no prompt?
> Os dados vão no system prompt? São consultados dinamicamente?

Vamos injetar os dados em nosso prompt como no exemplo abaixo, para garantir que nosso agente tenha o melhor contexto possível.

```text

DADOS DO USUÁRIO E PERFIL: (data/perfil_investidor.json)

{
  "nome": "João Silva",
  "idade": 32,
  "profissao": "Analista de Sistemas",
  "renda_mensal": 5000.00,
  "perfil_investidor": "moderado",
  "objetivo_principal": "Construir reserva de emergência",
  "patrimonio_total": 15000.00,
  "reserva_emergencia_atual": 10000.00,
  "aceita_risco": false,
  "metas": [
    {
      "meta": "Completar reserva de emergência",
      "valor_necessario": 15000.00,
      "prazo": "2026-06"
    },
    {
      "meta": "Entrada do apartamento",
      "valor_necessario": 50000.00,
      "prazo": "2027-12"
    }
  ]
}


TRANSAÇÕES DO USUÁRIO: (data/transacoes.csv)
data,descricao,categoria,valor,tipo
2025-10-01,Salário,receita,5000.00,entrada
2025-10-02,Aluguel,moradia,1200.00,saida
2025-10-03,Supermercado,alimentacao,450.00,saida
2025-10-05,Netflix,lazer,55.90,saida
2025-10-07,Farmácia,saude,89.00,saida
2025-10-10,Restaurante,alimentacao,120.00,saida
2025-10-12,Uber,transporte,45.00,saida
2025-10-15,Conta de Luz,moradia,180.00,saida
2025-10-20,Academia,saude,99.00,saida
2025-10-25,Combustível,transporte,250.00,saida

HISTÓRICO DE ATENDIMENTO DO USUÁRIO
data,canal,tema,resumo,resolvido
2025-09-15,chat,CDB,Cliente perguntou sobre rentabilidade e prazos,sim
2025-09-22,telefone,Problema no app,Erro ao visualizar extrato foi corrigido,sim
2025-10-01,chat,Tesouro Selic,Cliente pediu explicação sobre o funcionamento do Tesouro Direto,sim
2025-10-12,chat,Metas financeiras,Cliente acompanhou o progresso da reserva de emergência,sim
2025-10-25,email,Atualização cadastral,Cliente atualizou e-mail e telefone,sim

PRODUTOS DISPONÍVEIS: (data/produtos_financeiros.json)
[
  {
    "nome": "Tesouro Selic",
    "categoria": "renda_fixa",
    "risco": "baixo",
    "rentabilidade": "100% da Selic",
    "aporte_minimo": 30.00,
    "indicado_para": "Reserva de emergência e iniciantes"
  },
  {
    "nome": "CDB Liquidez Diária",
    "categoria": "renda_fixa",
    "risco": "baixo",
    "rentabilidade": "102% do CDI",
    "aporte_minimo": 100.00,
    "indicado_para": "Quem busca segurança com rendimento diário"
  },
  {
    "nome": "LCI/LCA",
    "categoria": "renda_fixa",
    "risco": "baixo",
    "rentabilidade": "95% do CDI",
    "aporte_minimo": 1000.00,
    "indicado_para": "Quem pode esperar 90 dias (isento de IR)"
  },
  {
    "nome": "Fundo Multimercado",
    "categoria": "fundo",
    "risco": "medio",
    "rentabilidade": "CDI + 2%",
    "aporte_minimo": 500.00,
    "indicado_para": "Perfil moderado que busca diversificação"
  },
  {
    "nome": "Fundo de Ações",
    "categoria": "fundo",
    "risco": "alto",
    "rentabilidade": "Variável",
    "aporte_minimo": 100.00,
    "indicado_para": "Perfil arrojado com foco no longo prazo"
  }
]
```


---

## Exemplo de Contexto Montado

> Mostre um exemplo de como os dados são formatados para o agente.

O exemplo de contexto montado abaixo, se baseia nos dados originais de base de conhecimento, mas os sintetiza deixando apenas as informações mais relevantes, otimizando assim o consumo de tokens. Entretanto vale lembrar que mais importante do que economizar tokens, é ter todas as informações relevantes disponíveis em seu contexto.

```
DADOS DO USUÁRIO:
- Nome: João Silva
- Perfil: Moderado
- Objetivo: Construir reserva de emergência
- Reserva atual: R$ 10.000 (meta: R$ 15.000)

RESUMO DE GASTOS:
- Moradia: R$ 1.300
- Alimentação: R$ 570
- Transporte: R$ 295
- Saúde: R$ 188
- Lazer: R$ 55,90
- Total de saídas: R$ 2.488,90

PRODUTOS DISPONÍVEIS PARA EXPLICAR:
- Tesouro Selic (risco baixo)
- CDB Liquidez Diária (risco baixo)
- LCI/LCA (risco baixo)
- Fundo Imobiliário - FII (risco médio)
...
```
