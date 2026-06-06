---
name: status
description: >
  Mostra um resumo do estado atual do sistema — o que está configurado, quais skills existem,
  e o que está na memória. Use quando o usuário pedir /status, "me mostra o que você sabe sobre mim",
  "o que está configurado", ou quiser uma visão geral rápida do MaxClaudePro.
---

# /status — Estado atual do sistema

Leitura rápida de tudo que está configurado. Útil pra checar se a memória está atualizada ou antes de uma sessão de trabalho intensa.

## Fluxo

1. Ler `_memoria/empresa.md`, `_memoria/preferencias.md`, `_memoria/estrategia.md`
2. Ler `identidade/design-guide.md`
3. Listar skills disponíveis em `.claude/skills/`
4. Apresentar resumo formatado

## Formato de saída

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  MAXCLAUDEPRO — STATUS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━

NEGÓCIO
  Nome: [nome]
  O que faz: [resumo]
  Cliente ideal: [perfil]
  Equipe: [solo / N pessoas]

FOCO ATUAL
  Fase: [fase]
  Prioridade: [prioridade principal]
  Gargalo: [gargalo]

COMUNICAÇÃO
  Tom: [resumo do tom de voz]
  Evitar: [lista resumida]

IDENTIDADE VISUAL
  [Configurada / Não configurada]
  Cores: [se configurada]
  Fonte: [se configurada]

SKILLS DISPONÍVEIS
  Sistema:    /instalar  /salvar  /atualizar  /status
  Conteúdo:   /carrossel  /legenda  /email-marketing  /seo  /blog
  Vendas:     /proposta  /followup  /script-vendas
  Atendimento: /responder  /avaliacoes
  Anúncios:   /anuncio-meta  /anuncio-google
  Operações:  /briefing  /relatorio  /reuniao

━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

Se algum arquivo de memória estiver incompleto ou vazio, indicar:
> "⚠ `_memoria/empresa.md` ainda tem campos em branco. Roda /instalar pra completar."

## Regras

- Não inventar informações — se está em branco, dizer que está em branco
- Manter o formato limpo e escaneável
- Não fazer perguntas após mostrar o status — só se o usuário quiser atualizar algo
