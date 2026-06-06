---
name: carrossel
description: >
  Cria carrosséis e posts visuais para Instagram, TikTok e LinkedIn com a identidade visual da marca.
  Gera HTML estilizado + renderiza em PNG 1080x1350 via Playwright, com legenda pronta no final.
  Use quando o usuário pedir "carrossel", "post", "conteúdo pro Instagram", "criar visual",
  "post educativo", ou /carrossel.
---

# /carrossel — Carrossel e posts visuais

Recebe um tema → entrega HTMLs estilizados + PNGs prontos pra postar + legenda no padrão da marca.

## Dependências

- **Identidade visual:** `identidade/design-guide.md` — LER ANTES de criar qualquer visual
- **Contexto do negócio:** `_memoria/empresa.md`
- **Tom de voz:** `_memoria/preferencias.md`
- **Playwright:** pra renderizar HTML em PNG
- **Outputs:** `marketing/carrosseis/<tema>-<YYYY-MM-DD>/`

---

## Tipos de conteúdo

Identificar qual tipo se encaixa:

**1. CARROSSEL TEXTO PURO**
- Posts educacionais, dicas, listas, explicações
- 1080x1350 (4:5), tipografia clean, cores da marca

**2. CARROSSEL COM FOTO**
- Conteúdo aspiracional, capa com personagem, apresentação visual
- Foto como capa com gradient overlay + slides internos no padrão

**3. POST ÚNICO**
- Frase de impacto, dado/estatística, depoimento
- 1080x1350

Se não estiver claro:
> "Que tipo? (1) carrossel texto, (2) carrossel com foto, (3) post único"

---

## Estilo visual padrão

Quando `identidade/design-guide.md` estiver vago ou em branco, usar esses defaults:

### Tipografia
- Fonte: Inter (Google Fonts), pesos 400 a 900
- Título de capa: 90-100px, weight 900, letter-spacing -0.04em
- H2 (slides internos): 60-72px, weight 800, letter-spacing -0.035em
- Corpo: 20-24px, weight 500, line-height 1.5
- Eyebrow/kicker: 13-16px, weight 700, UPPERCASE, letter-spacing 0.25em
- Counter (canto sup. dir.): 14px, weight 500, letter-spacing 0.18em

Regra: títulos grandes com kerning apertado (-0.035em), eyebrows pequenos com kerning aberto (0.25em+).

### Cores padrão
- Fundo escuro: `#0E1116`
- Fundo claro: `#FAFAF7`
- Texto sobre escuro: `#FAFAF7`
- Texto sobre claro: `#1A1A1A`
- Destaque: cor da marca (uma só — nunca quatro cores brigando)

### Layouts nomeados

- **CAPA** — eyebrow + título grande + subtítulo + @handle
- **SOLO** — split horizontal: visual à esquerda 50% + texto à direita 50%
- **NÚMERO** — numeral gigante como elemento gráfico + h2 + parágrafo
- **CITAÇÃO** — aspas grandes em watermark + frase em h2 + atribuição
- **CTA FINAL** — fundo na cor de destaque, logo centralizado, headline curta, @handle

Ritmo: alternar fundo escuro ↔ claro ↔ destaque. Nunca dois slides com mesmo fundo em sequência.

---

## Workflow

### Passo 1 — Planejar
1. Ler `_memoria/preferencias.md` e `_memoria/empresa.md`
2. Ler `identidade/design-guide.md`
3. Identificar o tipo (1, 2 ou 3)
4. Definir tema e ângulo

### Passo 2 — Texto
Escrever o conteúdo:
- Slide 1 (Capa): título impactante, máx 8 palavras. Oferecer 3 opções
- Slides internos: um insight por slide, frases naturais, sem bullet points
- Slide final: CTA + logo

**CHECKPOINT:** Mostrar texto completo. Aguardar aprovação antes do visual.

### Passo 3 — Gerar fotos (só se tipo 2)
Prompt em inglês:
```
Professional [TYPE] photography of [SUBJECT],
[DETAILS], [ENVIRONMENT],
[LIGHT STYLE] lighting, shallow depth of field,
shot from [ANGLE], editorial quality
```
**CHECKPOINT:** Foto aprovada → continuar.

### Passo 4 — Criar HTML + PNG
1. Um único `carrossel.html` com todos os slides como `<div class="slide">` — inline CSS, Google Fonts como única dependência
2. `render.js` na mesma pasta — Playwright screenshot de cada `.slide` em 1080x1350
3. Mostrar slides 1, 2 e o CTA final. Se aprovado, mostrar os intermediários.

### Passo 5 — Salvar

```
marketing/carrosseis/<tema>-<YYYY-MM-DD>/
  carrossel.html
  render.js
  instagram/
    slide-01.png ... slide-NN.png
  legenda.md
```

Ao terminar, **gerar legenda automaticamente** (não esperar o usuário pedir) — ver skill `/legenda`.

---

## Regras

- Ler `identidade/design-guide.md` sempre antes de criar
- Formato: 1080x1350 (4:5) — sempre. TikTok/Reels: 1080x1920 só quando pedido
- Nunca repetir layout entre slides
- Sempre gerar legenda ao final
- Fotos IA: prompts em inglês, nunca gerar rostos identificáveis
- HTML: um único arquivo com todos os slides + `render.js` separado
