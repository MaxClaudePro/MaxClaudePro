---
name: salvar
description: >
  Salva uma informação relevante nos arquivos de memória do MaxClaudePro.
  Use quando o usuário disser "salva isso", "anota aí", "quero que você lembre",
  ou quando uma correção ou decisão permanente precisar ser registrada.
---

# /salvar — Salvar na memória

Registra informações permanentes nos arquivos de memória certos. Não salva coisas pontuais ou que só valem pra sessão atual.

## Fluxo

1. Identificar o que precisa ser salvo
2. Determinar o arquivo correto:
   - **Sobre o negócio** (serviços, clientes, equipe, canais) → `_memoria/empresa.md`
   - **Sobre tom e comunicação** (como escrever, o que evitar) → `_memoria/preferencias.md`
   - **Sobre prioridades e estratégia** (metas, foco, prazos) → `_memoria/estrategia.md`
   - **Sobre identidade visual** (cores, fontes, logo) → `identidade/design-guide.md`
   - **Sobre comportamento do sistema** (regra de como agir) → `CLAUDE.md`
3. Abrir o arquivo, encontrar a seção correta, adicionar a informação
4. Confirmar: "Salvo em `[arquivo]`."

## Regras

- Só salvar informações com valor permanente — não registrar contexto temporário
- Manter o estilo e formato já existente no arquivo
- Não duplicar informações que já estão lá
- Se a informação contradiz algo já salvo, atualizar o existente (não criar duplicata)
- Confirmar sempre o que foi salvo e onde
