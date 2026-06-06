---
name: legenda
description: >
  Gera legendas para posts no Instagram, LinkedIn, Facebook e TikTok no tom de voz da marca.
  Use quando o usuário pedir "legenda", "caption", "texto pro post", "escreve a legenda",
  ou quando chamado automaticamente pelo /carrossel.
---

# /legenda — Legenda para posts

Gera legendas prontas pra postar, no tom da marca, com hook forte, corpo relevante e CTA claro.

## Dependências

- `_memoria/empresa.md` — contexto do negócio
- `_memoria/preferencias.md` — tom de voz

---

## Fluxo

### 1. Entender o contexto

Se chamado diretamente (não pelo /carrossel), perguntar:
- "Qual é o tema do post?"
- "Qual plataforma? (Instagram / LinkedIn / TikTok / Facebook)"
- "Tem um objetivo específico? (ex: gerar mensagens, tráfego, engajamento)"

### 2. Definir o canal

**Instagram / Facebook / TikTok:**
- Hook direto e pessoal
- 3-5 parágrafos curtos
- CTA claro no final
- 10-15 hashtags (nicho + segmento + local)

**LinkedIn:**
- Abertura com dado ou insight
- Tom mais reflexivo
- Sem hashtags excessivas (3-5 no máximo)
- CTA profissional

### 3. Estrutura padrão (Instagram)

```
[Hook — frase que para o scroll]

[Contexto — 1-2 frases sobre o tema]

[Desenvolvimento — 2-3 frases com o valor principal]

[CTA — ação clara: arrastar, comentar, responder, clicar no link]

[Bloco de oferta — diferencial da empresa + contato]

[Hashtags]
```

### 4. Entrega

Gerar **2 versões** com ângulos diferentes. Usuário escolhe qual prefere ou mistura as duas.

Salvar em `legenda.md` na pasta do post (se chamado pelo /carrossel) ou em `marketing/legendas/<tema>-<YYYY-MM-DD>.md`.

---

## Regras

- Seguir estritamente `_memoria/preferencias.md`
- Frases naturais — sem jargão de marketing, sem corporativês
- Hook nunca começa com "Você sabia que..." ou "Hoje vou falar sobre..."
- CTA sempre presente — nunca terminar sem direcionamento
- Hashtags no final, nunca no meio do texto
