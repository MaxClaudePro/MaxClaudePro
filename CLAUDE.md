# MaxClaudePro — Sistema Operacional do Negócio

> Antes de responder qualquer coisa, ler os arquivos de memória abaixo.

## Contexto do negócio

No início de toda conversa, ler silenciosamente:
1. `_memoria/empresa.md` — quem é a empresa, o que faz, perfil de cliente
2. `_memoria/preferencias.md` — tom de voz, o que evitar, como comunicar
3. `_memoria/estrategia.md` — foco atual, prioridades, metas

Para tarefas visuais (carrossel, proposta, apresentação), ler `identidade/design-guide.md`.

Usar essas informações naturalmente — sem confirmar em voz alta o que foi lido.

## Fluxo de trabalho

Antes de executar qualquer tarefa:
1. Verificar se existe skill relevante em `.claude/skills/`
2. Se encontrar, seguir as instruções da skill
3. Se não encontrar, executar normalmente
4. Ao concluir tarefa repetível sem skill: perguntar "Isso pode virar uma skill pra próxima vez. Quer que eu crie?"

## Aprender com correções

Quando o usuário corrigir algo com caráter permanente, perguntar:
> "Quer que eu salve isso pra não precisar repetir?"

Se sim, salvar em:
- Sobre o negócio → `_memoria/empresa.md`
- Sobre preferências → `_memoria/preferencias.md`
- Sobre prioridades → `_memoria/estrategia.md`
- Regra de comportamento → `CLAUDE.md`

## Manter contexto atualizado

Depois de completar trabalho que muda o contexto relevante (novo cliente fechado, nova estratégia, mudança de tom), oferecer:
> "Quer que eu atualize a memória com isso?"

Não perguntar em tarefas pontuais, perguntas simples, ou quando o contexto já foi salvo.

## Criação de novas skills

Quando o usuário pedir uma skill nova:
1. Verificar se existe algo parecido em `.claude/skills/`
2. Ler arquivos de memória e `identidade/design-guide.md` pra calibrar
3. Criar em `.claude/skills/<nome>/SKILL.md`

## Estrutura de pastas

- `_memoria/` — contexto do negócio, tom de voz, estratégia
- `identidade/` — marca, cores, fontes, logo
- `marketing/` — conteúdo produzido (carrosséis, legendas, artigos, emails)
- `saidas/` — documentos pontuais (emails, textos avulsos, relatórios)
- `dados/` — arquivos a analisar
- `scripts/` — automações e scripts internos

## Ferramentas conectadas

- [ ] Make.com / n8n
- [ ] WhatsApp (Z-API / Evolution API)
- [ ] Google Calendar / Cal.com
- [ ] Gmail
- [ ] Notion / Obsidian

*(Marcar conforme forem conectando as integrações)*
