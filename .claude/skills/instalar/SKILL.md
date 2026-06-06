---
name: instalar
description: >
  Instala o MaxClaudePro no negócio do usuário. Entrevista sobre empresa, tom de voz,
  foco atual e identidade visual, e preenche _memoria/empresa.md, _memoria/preferencias.md,
  _memoria/estrategia.md, identidade/design-guide.md e adapta o CLAUDE.md conforme o perfil.
  Use quando o usuário acabar de clonar o repositório ou pedir explicitamente /instalar.
---

# /instalar — Setup inicial do MaxClaudePro

Primeiro comando depois de clonar. Não pode soar burocrático — é uma conversa de descoberta. Pergunta uma coisa por vez, ouve de verdade, não enfileira tudo. O objetivo é o sistema sair daqui sabendo quem é a empresa, como ela fala, e onde está o atrito do dia a dia.

## Pré-checagem

### 1. Nome da pasta

Verificar o nome da pasta atual. Se for `maxclaudepro`, `MaxClaudePro`, `max-claude-pro` ou variação genérica:

> "Notei que a pasta ainda tem nome genérico. O ideal é ter o nome do seu negócio. Quando terminarmos, te lembro de renomear — é rápido. Bora?"

### 2. Arquivos de memória

Verificar se `_memoria/empresa.md`, `_memoria/preferencias.md` ou `_memoria/estrategia.md` já têm conteúdo real (não só placeholders).

Se sim:
> "Já tem contexto preenchido aqui. Quer recomeçar do zero ou só completar o que falta?"

Se não, seguir direto.

---

## Fase 1 — Perfil do negócio

Perguntar qual perfil mais combina:

1. **Solopreneur / criador solo** — uma pessoa, mistura de marca pessoal e negócio
2. **Freelancer** — atende clientes, organiza por projeto
3. **Agência / consultoria** — equipe pequena, vários clientes
4. **Empresa** — estrutura com setores (marketing, comercial, operações)

---

## Fase 2 — Entrevista

Fazer em ordem, uma por vez. Se vier resposta vaga, pedir concretude uma vez só. Registrar o que vier.

**Sobre o negócio:**
1. "Como você chama o que você faz? (nome da empresa ou seu nome, se for marca pessoal)"
2. "O que sua empresa entrega — em uma frase, do jeito que você falaria pro vizinho?"
3. "Quem te paga? Descreve o perfil real do cliente em uma ou duas frases."
4. "Você toca sozinho ou tem equipe? Se tem, quantos e cada um fazendo o quê?"

**Sobre voz:**
5. "Me cola um exemplo da tua escrita — uma legenda do Insta, um email pra cliente, qualquer coisa real e recente. Assim eu calibro sem precisar adivinhar."
6. "O que te dá ranço quando alguém escreve assim? (ex: 'vamos juntos!', emoji em email formal, 'alavancar', 'sinergia', 'caro cliente')"

**Sobre foco:**
7. "Qual o maior gargalo do seu negócio hoje? O que está travando o crescimento?"
8. "Se eu pudesse tirar UMA tarefa que você repete toda semana das suas costas, qual seria?"

**Sobre identidade visual:**
9. "Tem identidade visual definida? Se sim, me passa as cores principais e a fonte usada."
10. "Tem logo? Se sim, joga o arquivo em `identidade/logo.png` e me confirma."

---

## Fase 3 — Preenchimento dos arquivos

### `_memoria/empresa.md`
Preencher com base nas perguntas 1-4: nome, o que faz, perfil de cliente, equipe.

### `_memoria/preferencias.md`
Com base nas perguntas 5-6: tom de voz derivado do exemplo real, lista do que evitar.

### `_memoria/estrategia.md`
Com base nas perguntas 7-8: gargalo atual, a tarefa candidata a virar skill, próximas prioridades.

### `identidade/design-guide.md`
Se o usuário passou cores/fontes/logo (perguntas 9-10), preencher os campos. Se não:
> "Deixei o design-guide.md em branco. Quando você definir a identidade visual, preenche lá — as skills de carrossel e proposta leem esse arquivo antes de criar qualquer visual."

### `CLAUDE.md`
Adaptar com o nome do negócio e o perfil escolhido na Fase 1.

---

## Fase 4 — Resumo

Mostrar o que foi configurado:

```
✓ Perfil: [perfil]
✓ Contexto do negócio: _memoria/empresa.md
✓ Tom de voz: _memoria/preferencias.md
✓ Foco atual: _memoria/estrategia.md
✓ Identidade visual: identidade/design-guide.md  [preenchida | em branco]
✓ CLAUDE.md adaptado
```

---

## Fase 5 — Renomear pasta (se necessário)

Se a pasta ainda tem nome genérico, gerar slug do nome da empresa:
- minúsculas, sem acentos, espaços viram hífen

> "Última coisa: a pasta ainda está com nome genérico.
> Recomendo renomear pra '<slug>'.
>
> Como fazer:
> 1. Fecha o VS Code
> 2. Renomeia a pasta no Explorer (Windows) ou Finder (Mac)
> 3. Abre o VS Code de novo na pasta renomeada"

---

## Fase 6 — Próximos passos

> "Pronto. O MaxClaudePro já te conhece.
>
> Você mencionou que repete '<resposta da pergunta 8>' toda semana.
> Quando quiser automatizar isso, me fala que eu monto uma skill sob medida.
>
> Skills disponíveis: /carrossel, /proposta, /followup, /seo, /blog,
> /anuncio-meta, /anuncio-google, /briefing, /reuniao, /relatorio e mais."

---

## Regras

- Não inventar dados — se a resposta for vaga, registrar como veio
- Setup deve durar no máximo 7 minutos
- Não fazer perguntas extras além das listadas
- Nos arquivos finais, não deixar avisos de placeholder — preencher com o conteúdo real
