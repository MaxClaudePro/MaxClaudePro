---
name: briefing
description: >
  Conduz um briefing completo de projeto com o cliente e gera o documento estruturado.
  Use quando o usuário pedir "briefing", "levantar requisitos", "entender o que o cliente quer",
  "documentar o projeto", ou /briefing.
---

# /briefing — Briefing de projeto

Levantamento estruturado que evita retrabalho — captura tudo que importa antes de começar.

## Dependências

- `_memoria/empresa.md`
- `_memoria/preferencias.md`

---

## Fluxo

### 1. Contexto

Perguntar:
- "Qual o nome do cliente e o projeto?"
- "Você já teve uma conversa inicial com ele, ou esse briefing é o primeiro contato?"
- "Qual é o serviço sendo contratado?"

### 2. Conduzir o briefing

Fazer as perguntas em ordem, uma de cada vez:

**Sobre o negócio do cliente:**
1. "O que sua empresa faz e quem é seu cliente ideal?"
2. "Qual o principal problema que esse projeto resolve?"

**Sobre o projeto:**
3. "O que você espera que esteja pronto ao final?"
4. "Tem exemplos de referência — sites, concorrentes, algo que você gosta?"
5. "O que definitivamente não pode ter nesse projeto?"

**Sobre prazos e orçamento:**
6. "Tem uma data de entrega em mente?"
7. "Já tem orçamento definido ou ainda está em aberto?"

**Sobre decisões:**
8. "Quem aprova o projeto do lado de vocês? (um ou mais decisores)"
9. "Qual o melhor canal pra comunicação durante o projeto? (WhatsApp, email, outro)"

### 3. Gerar documento

Criar `briefing-<cliente>-<YYYY-MM-DD>.md` com:
- Resumo executivo (2-3 frases do projeto)
- Informações do cliente
- Escopo levantado
- Referências mencionadas
- O que não pode ter
- Prazo e orçamento
- Decisores e canal de comunicação
- Próximos passos

Salvar em `saidas/briefings/` ou na pasta do cliente se existir.

---

## Regras

- Uma pergunta por vez — não mandar tudo junto
- Se uma resposta for vaga, pedir concretude uma vez só e registrar o que vier
- Não inventar requisitos — registrar exatamente o que o cliente disse
- Ao final, perguntar se o cliente quer revisar o documento antes de usar
