# 📊 Auditoria de Fluxo de Caixa e Margem de Lucro — Power BI

Solução de Business Intelligence desenvolvida para consolidar fluxos transacionais complexos, proporcionando previsibilidade e governança sobre o caixa da empresa, atuando como ferramenta direta de apoio à decisão C-Level.

## 🧩 O Problema de Negócio
Diretorias financeiras (CFOs e Gestores) frequentemente operam com "miopia de caixa". O fechamento do mês exige dias de trabalho manual cruzando planilhas de múltiplos bancos, notas fiscais e impostos. O resultado? Decisões baseadas em achismos, lentidão na apuração do lucro real e falta de rastreabilidade para onde o dinheiro está escoando.

Este painel substitui o caos das planilhas por um modelo de dados governado, entregando a resposta exata sobre a saúde financeira com dois cliques.

## ⚙️ Arquitetura da Solução

```text
Transações Brutas (Múltiplas Fontes)
        │
        ▼
┌─────────────────────┐
│  1. Power Query     │  Extração, limpeza de anomalias, tratamento de nulos
│     (ETL)           │  e padronização de tipos de dados.
└─────────────────────┘
        │
        ▼
┌─────────────────────┐
│  2. Data Modeling   │  Estruturação relacional otimizada (Fato/Dimensão)
│                     │  para performance de filtros cruzados.
└─────────────────────┘
        │
        ▼
┌─────────────────────┐
│  3. Linguagem DAX   │  Medidas avançadas (CALCULATE, Time Intelligence) para
│                     │  segmentação dinâmica de margem e lucros.
└─────────────────────┘
        │
        ▼
┌─────────────────────┐
│  4. Data Viz &      │  Dashboard interativo com Waterfall Chart, Image Grid
│     Storytelling    │  e KPIs instantâneos de caixa.
└─────────────────────┘
