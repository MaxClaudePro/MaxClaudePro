---
name: responder
description: >
  Escreve respostas para mensagens de clientes, leads e parceiros — WhatsApp, email, DM.
  Use quando o usuário pedir "responde isso pra mim", "como respondo", "me ajuda a responder",
  ou /responder.
---

# /responder — Responder mensagens

Escreve a resposta certa, no tom certo, pra qualquer tipo de mensagem recebida.

## Dependências

- `_memoria/empresa.md`
- `_memoria/preferencias.md`

---

## Fluxo

### 1. Receber o contexto

O usuário vai colar a mensagem recebida. Se não colar:
> "Cola a mensagem que você quer responder — com isso eu calibro o tom e o contexto certo."

### 2. Identificar o tipo

**Dúvida ou interesse** → resposta informativa, clara, com próximo passo
**Reclamação** → empática, reconhece o problema, apresenta solução
**Negociação / preço** → firme sem ser rígido, valoriza o serviço
**Agendamento** → confirma, organiza, facilita
**Mensagem urgente** → direta, sem enrolação
**Mensagem ambígua** → perguntar antes de supor o que a pessoa quis dizer

### 3. Escrever

Regras:
- Tom segue `_memoria/preferencias.md`
- Nunca começar com "Olá, tudo bem?" como único conteúdo antes do ponto
- Reclamações: nunca defensivo, nunca prometer o que não pode cumprir
- Negociação: nunca baixar preço sem contrapartida (menor escopo, prazo maior, etc.)
- Máx 3-4 linhas no WhatsApp

### 4. Entregar

Gerar a resposta pronta + 1 variação alternativa (mais curta ou mais detalhada).

---

## Regras

- Tom sempre segue `_memoria/preferencias.md`
- Nunca inventar informações sobre o produto ou serviço
- Se a mensagem exigir uma decisão de negócio, apresentar a resposta e perguntar se o usuário concorda
