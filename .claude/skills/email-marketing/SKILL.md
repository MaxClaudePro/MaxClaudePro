---
name: email-marketing
description: >
  Escreve emails de marketing, nutrição, lançamento, prospecção e comunicados no tom da marca.
  Use quando o usuário pedir "email", "escreve um email", "email marketing", "email pra lista",
  "email de prospecção", ou /email-marketing.
---

# /email-marketing — Email

Escreve emails que chegam, são abertos e geram ação — do email frio de prospecção ao disparo pra lista.

## Dependências

- `_memoria/empresa.md`
- `_memoria/preferencias.md`

---

## Tipos de email

Identificar qual tipo o usuário precisa:

**1. PROSPECÇÃO (frio)**
- Objetivo: abrir conversa com potencial cliente
- Curto, direto, personalizado, sem pitch longo
- Foco em dor específica do destinatário

**2. NUTRIÇÃO (lista)**
- Objetivo: manter relacionamento, gerar confiança
- Valor primeiro, promoção depois (ou nenhuma)
- Tom de conversa, não de broadcast

**3. LANÇAMENTO / OFERTA**
- Objetivo: converter — venda, cadastro, agendamento
- Urgência real (não artificial), benefício claro, CTA único
- Versão curta (2-3 parágrafos) e versão longa (5-7 parágrafos) se pedido

**4. COMUNICADO / OPERACIONAL**
- Objetivo: informar — confirmação, atualização, onboarding
- Claro, sem ruído, direto ao ponto

Se não estiver claro:
> "Que tipo de email? (1) prospecção, (2) nutrição/lista, (3) lançamento/oferta, (4) comunicado"

---

## Fluxo

### 1. Entender o contexto
- "Pra quem vai esse email? (descreva o destinatário ou segmento)"
- "Qual a ação que você quer que a pessoa tome depois de ler?"
- "Tem algum contexto específico? (ex: evento, oferta, problema que eles têm)"

### 2. Escrever

**Assunto:** gerar 3 opções de assunto. Regras:
- Máx 50 caracteres
- Nunca usar ALL CAPS ou excesso de pontuação
- Um dos três deve ser direto (sem criatividade), um deve ser curioso, um deve ser pessoal

**Corpo:**
- Abertura que conecta (sem "Espero que esteja bem")
- Transição natural pro ponto principal
- Um CTA claro — não três

### 3. Entregar

Formato:
```
ASSUNTO (3 opções):
1. [opção direta]
2. [opção curiosa]
3. [opção pessoal]

---

[CORPO DO EMAIL]
```

Salvar em `marketing/emails/<tipo>-<tema>-<YYYY-MM-DD>.md`.

---

## Regras

- Tom segue `_memoria/preferencias.md` estritamente
- Um CTA por email — nunca dois
- Nunca começar com "Olá! Espero que esteja bem" ou variações
- Email frio: máx 150 palavras no corpo
- Assunto: nunca prometer algo que o email não entrega
