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
```

## 📈 Valor Gerado e Resultados
Visão consolidada do fluxo de caixa e comportamento transacional, eliminando dias de apuração manual.

```text
FINANCIAL PERFORMANCE REPORT — CONSOLIDADO
════════════════════════════════════════════

AUDITORIA DE CAIXA
Recebimentos Totais:         R$ 94,6 Mi
Pagamentos e Impostos:       R$ 58,8 Mi

RENTABILIDADE E COMPORTAMENTO
Margem de Lucro Real:        37,58%
Adoção de Pagamentos Pix:    44,04%  (1.200 de 2.725 registros)
```

## 🔍 Visões Analíticas do Dashboard
- **Evolução de DRE:** Gráfico de cascata (Waterfall) para identificar exatamente em quais meses a empresa queimou caixa ou gerou lucro.
- **Rastreabilidade Bancária:** Filtros Image Grid para isolar o fluxo de caixa por instituição bancária (Itaú, Nubank, Safra, etc).
- **Métricas Geográficas:** Segmentação instantânea da margem de lucro de acordo com a região e o município faturado.

## 🛠️ Stack Utilizada
- **Microsoft Power BI** — Engine de visualização e orquestração.
- **Power Query (M)** — Higienização e transformação da base bruta.
- **DAX** — Lógica de negócios e cálculos complexos.
- **Modelagem Relacional** — Garantia de integridade da análise.

> **Auditoria Técnica:** O arquivo original `Dashboard Financeiro.pbix` contendo toda a modelagem, as etapas de ETL e o código DAX está disponível neste repositório para avaliação.
