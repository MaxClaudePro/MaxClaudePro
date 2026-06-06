---
name: reuniao
description: >
  Processa anotações de reunião e gera ata estruturada com decisões e ações claras.
  Use quando o usuário pedir "ata de reunião", "resumir reunião", "o que ficou decidido",
  "processar minhas notas", ou /reuniao.
---

# /reuniao — Ata de reunião

Transforma anotações brutas em documento limpo — com decisões, responsáveis e prazos destacados.

## Dependências

- `_memoria/empresa.md`

---

## Fluxo

### 1. Receber o contexto

O usuário vai colar as anotações ou descrever o que aconteceu. Se não:
> "Cola suas anotações da reunião — pode ser bagunçado, eu organizo."

Perguntar também (se não estiver nas anotações):
- "Quem participou?"
- "Qual era o objetivo da reunião?"
- "Tem prazo pra alguma das ações definidas?"

### 2. Processar

Identificar:
- **Contexto:** data, participantes, objetivo
- **Pontos discutidos:** o que foi tratado
- **Decisões tomadas:** o que foi definido (não o que foi discutido)
- **Ações:** tarefa + responsável + prazo (quando houver)
- **Próxima reunião:** se marcada

### 3. Gerar ata

```markdown
# Ata — [Tema da Reunião]
**Data:** [data]
**Participantes:** [nomes]
**Objetivo:** [em uma frase]

## Pontos discutidos
- [ponto 1]
- [ponto 2]

## Decisões
- [decisão 1]
- [decisão 2]

## Ações
| Tarefa | Responsável | Prazo |
|--------|-------------|-------|
| [ação] | [pessoa]    | [data] |

## Próximos passos
[o que acontece depois — próxima reunião, entrega, etc.]
```

### 4. Salvar

`saidas/reunioes/ata-<tema>-<YYYY-MM-DD>.md`

---

## Regras

- Separar claramente decisões de discussões — são coisas diferentes
- Ações sem responsável explícito: perguntar quem é o responsável antes de finalizar
- Não inventar prazos — se não foi definido, registrar "a definir"
- Ata objetiva: sem paráfrases longas do que foi dito
