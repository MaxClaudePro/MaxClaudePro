---
name: anuncio-google
description: >
  Cria textos para campanhas de Google Ads (Search, Display e Performance Max).
  Use quando o usuário pedir "anúncio no Google", "Google Ads", "campanha de pesquisa",
  "aparecer no Google pago", ou /anuncio-google.
---

# /anuncio-google — Anúncio Google Ads

Textos otimizados para campanhas de busca e display — com keywords certas, headlines que clicam e extensões prontas.

## Dependências

- `_memoria/empresa.md`
- `_memoria/preferencias.md`

---

## Fluxo

### 1. Briefing

Perguntar:
- "Qual o objetivo da campanha? (ex: gerar ligações, visitas ao site, formulários, WhatsApp)"
- "Qual produto ou serviço?"
- "Tem palavras-chave específicas que você quer trabalhar? (ou posso sugerir)"
- "Qual a URL de destino?"
- "Tem oferta, diferencial ou urgência?"

### 2. Palavras-chave

Sugerir lista de palavras-chave por intenção:
- **Alta intenção** (pesquisa com intenção de compra): prioridade máxima
- **Média intenção** (comparação, informação): secundário
- **Negativas** (termos que não devem acionar o anúncio): sempre incluir

### 3. Anúncio responsivo de pesquisa (RSA)

Gerar:
- **15 headlines** (máx 30 caracteres cada) — variadas: benefício, feature, local, urgência, CTA
- **4 descrições** (máx 90 caracteres cada) — complementares, não repetitivas

**CHECKPOINT:** Mostrar headlines e descrições. Aprovar antes de continuar.

### 4. Extensões de anúncio

Sugerir:
- **Sitelinks** (4 links extras): páginas relevantes do site
- **Callouts** (frases de destaque): diferenciais em 25 caracteres
- **Snippets estruturados**: lista de serviços ou categorias

### 5. Salvar

`marketing/anuncios/google-<campanha>-<YYYY-MM-DD>.md`

---

## Regras

- Headlines: incluir palavra-chave principal em pelo menos 3 delas
- Nunca prometer resultado financeiro específico
- Descrições: sempre incluir ao menos um CTA claro
- Palavras negativas: essencial para não desperdiçar budget
- Tom segue `_memoria/preferencias.md` — adaptado ao contexto de busca (mais direto)
