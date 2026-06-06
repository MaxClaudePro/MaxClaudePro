---
name: relatorio
description: >
  Gera relatórios de resultado, performance e progresso — para clientes ou uso interno.
  Use quando o usuário pedir "relatório", "report", "resumo de resultados", "apresentar resultados",
  ou /relatorio.
---

# /relatorio — Relatório

Do dado bruto ao relatório claro — que o cliente entende e que mostra o valor do trabalho.

## Dependências

- `_memoria/empresa.md`
- `_memoria/preferencias.md`

---

## Tipos de relatório

**1. RESULTADO DE CAMPANHA** — Ads, redes sociais, email marketing
**2. PROGRESSO DE PROJETO** — O que foi feito, o que falta, próximos passos
**3. RELATÓRIO MENSAL** — Visão geral do período, métricas, highlights
**4. RELATÓRIO INTERNO** — Pra uso próprio, análise, tomada de decisão

Se não estiver claro:
> "Que tipo de relatório? (1) campanha, (2) progresso de projeto, (3) mensal, (4) interno"

---

## Fluxo

### 1. Coletar dados

Perguntar:
- "Qual período cobre o relatório?"
- "Quais métricas ou entregas você quer incluir?"
- "Tem dados pra compartilhar? (pode colar ou descrever)"
- "É pra cliente ou uso interno?"

### 2. Estrutura

**Para cliente:**
1. Resumo executivo (o que aconteceu + número principal)
2. Resultados por área/canal
3. O que funcionou + o que ajustar
4. Próximos passos

**Para uso interno:**
1. Métricas e dados
2. Análise direta
3. Decisões e ações

### 3. Tom

Para cliente: linguagem acessível, foco em impacto, não em processo
Para interno: direto, técnico, sem enfeite

### 4. Salvar

`saidas/relatorios/<tipo>-<YYYY-MM-DD>.md`

---

## Regras

- Nunca inflar números ou omitir resultados negativos — relatório honesto é o que constrói confiança
- Resumo executivo primeiro: o cliente mais ocupado lê só esse
- Métricas sem contexto não valem — sempre comparar com meta ou período anterior
- Tom segue `_memoria/preferencias.md`
