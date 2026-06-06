---
name: proposta
description: >
  Cria propostas comerciais profissionais em HTML, prontas para enviar ao cliente.
  Use quando o usuário pedir "proposta", "orçamento", "montar proposta", "proposta comercial",
  ou /proposta.
---

# /proposta — Proposta comercial

Do briefing ao HTML impresso — proposta profissional que fecha.

## Dependências

- `_memoria/empresa.md`
- `_memoria/preferencias.md`
- `identidade/design-guide.md`

---

## Fluxo

### 1. Briefing do cliente

Perguntar:
- "Qual o nome do cliente (empresa ou pessoa)?"
- "O que você vai entregar pra ele? (descreve o escopo)"
- "Qual o valor? (valor único, mensalidade, ou precisa de ajuda pra precificar?)"
- "Tem prazo de entrega ou vigência?"
- "Algo específico que você quer destacar ou que o cliente mencionou como prioridade?"

### 2. Estrutura da proposta

Montar:
1. **Capa** — nome do cliente, nome do serviço, data, logo
2. **Contexto** — o que o cliente enfrenta hoje (problema que justifica a proposta)
3. **Solução** — o que será entregue, em linguagem de benefício (não de feature)
4. **Escopo detalhado** — lista do que está incluído e o que não está
5. **Investimento** — valor, condições de pagamento, prazo
6. **Próximos passos** — como fechar (assinatura, PIX, link, reunião)
7. **Sobre a empresa** — mini apresentação, credenciais, contato

**CHECKPOINT:** mostrar estrutura + valores. Aprovado → gerar HTML.

### 3. Gerar HTML

Criar `proposta-<cliente>-<YYYY-MM-DD>.html` com:
- Identidade visual de `identidade/design-guide.md`
- Layout de leitura limpa (largura máx 800px, padding generoso)
- Tipografia da marca ou Inter como fallback
- Cores da marca para destaques e cabeçalhos
- Print-friendly: sem shadows nem backgrounds difíceis de imprimir

Salvar em `saidas/propostas/`.

---

## Regras

- Escopo claro: o que está incluído **e** o que não está — ambos explícitos
- Linguagem de benefício, não de feature ("você ganha X" em vez de "entregamos Y")
- Nunca incluir valor sem mostrar antes pro usuário confirmar
- Proposta deve ter data de validade (sugerir 7-15 dias se o usuário não definir)
- Tom segue `_memoria/preferencias.md`
