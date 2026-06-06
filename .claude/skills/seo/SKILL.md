---
name: seo
description: >
  Cria estratégia de SEO, meta tags, pesquisa de palavras-chave e conteúdo otimizado para buscadores.
  Use quando o usuário pedir "SEO", "aparecer no Google", "palavras-chave", "meta description",
  "otimizar o site", ou /seo.
---

# /seo — SEO e otimização para buscadores

Do levantamento de palavras-chave à meta tag pronta — tudo calibrado pro negócio e público real.

## Dependências

- `_memoria/empresa.md`
- `_memoria/preferencias.md`

---

## Modos

**1. PALAVRAS-CHAVE**
Levantar termos que o cliente ideal realmente usa pra buscar o serviço.

**2. META TAGS**
Escrever `<title>` e `<meta name="description">` prontos pra uma página.

**3. ARTIGO SEO**
Estrutura completa de artigo otimizado (esqueleto + copy principal).

**4. AUDITORIA RÁPIDA**
Revisar uma URL ou texto existente e apontar melhorias.

Se não estiver claro:
> "O que você precisa? (1) palavras-chave, (2) meta tags, (3) artigo SEO, (4) auditoria"

---

## Fluxo por modo

### Modo 1 — Palavras-chave

1. Ler `_memoria/empresa.md` pra entender serviço e público
2. Perguntar: "Qual página ou serviço específico você quer ranquear?"
3. Gerar 3 camadas de termos:
   - **Intenção direta** (ex: "agência de automação SP") — alta conversão
   - **Intenção de problema** (ex: "como automatizar atendimento whatsapp") — tráfego educativo
   - **Intenção local** (ex: "sistema CRM para clínicas") — se aplicável
4. Para cada termo: volume aproximado (alto/médio/baixo) e dificuldade (alta/média/baixa)

### Modo 2 — Meta Tags

Perguntar: "Qual página? Me passa a URL ou descreve o conteúdo."

Entregar:
```html
<title>[título da página — máx 60 caracteres]</title>
<meta name="description" content="[descrição — máx 155 caracteres, com palavra-chave principal]">
```
Gerar 2 opções de cada.

### Modo 3 — Artigo SEO

1. Perguntar: "Qual palavra-chave principal e qual o objetivo do artigo?"
2. Definir estrutura (H1, H2s, H3s)
3. **CHECKPOINT:** mostrar estrutura. Aprovada → escrever o artigo completo
4. Incluir: palavra-chave no H1, nos 2 primeiros parágrafos, e em 2-3 H2s naturalmente
5. Salvar em `marketing/blog/<slug>-<YYYY-MM-DD>.md`

### Modo 4 — Auditoria

1. Receber a URL ou o texto
2. Avaliar: H1 presente? Palavra-chave no início? Meta tags? Texto mínimo (300 palavras)?
3. Listar melhorias em ordem de impacto

---

## Regras

- Nunca forçar palavra-chave de forma antinatural no texto
- Priorizar intenção de busca real, não volume genérico
- Title tag: sempre incluir palavra-chave principal + nome da empresa
- Meta description: sempre ter um CTA implícito
