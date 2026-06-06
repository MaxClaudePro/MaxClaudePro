---
name: atualizar
description: >
  Atualiza os arquivos de memória com mudanças recentes no negócio.
  Use quando o usuário disser "atualiza minha memória", "mudou minha estratégia",
  "tenho um cliente novo", "mudei o foco", ou /atualizar.
---

# /atualizar — Atualizar memória

Mantém os arquivos de memória alinhados com a realidade atual do negócio. Funciona como revisão guiada.

## Fluxo

### 1. Identificar o que mudou

Perguntar:
> "O que mudou desde a última vez? Pode ser um novo cliente, mudança de foco, nova ferramenta, novo serviço — qualquer coisa relevante pro sistema saber."

### 2. Mapear os arquivos afetados

Com base na resposta, identificar quais arquivos precisam de update:
- Novo cliente / novo serviço / nova equipe → `_memoria/empresa.md`
- Mudança de tom / novo exemplo real de escrita → `_memoria/preferencias.md`
- Nova prioridade / nova meta / deadline → `_memoria/estrategia.md`
- Nova cor / nova fonte / novo logo → `identidade/design-guide.md`

### 3. Atualizar

Abrir cada arquivo afetado, localizar a seção certa, atualizar com precisão cirúrgica — não reescrever o arquivo inteiro.

### 4. Confirmar

Listar o que foi atualizado:
```
Atualizado:
✓ _memoria/empresa.md — [o que mudou]
✓ _memoria/estrategia.md — [o que mudou]
```

## Regras

- Não apagar informações históricas relevantes — atualizar, não substituir cegamente
- Se o usuário mencionar algo que contradiz a memória atual, perguntar antes de sobrescrever
- Atualizar só o necessário — não reescrever o arquivo inteiro por uma mudança pequena
