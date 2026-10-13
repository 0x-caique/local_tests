---
name: rastro-mcp-save-result
description: >-
  Saves each Rastro MCP tool reply into rastro_mcp/<tool>.md using the
  Prompt + headline + table + paragraph layout of screen_address_sanctions.md.
  Use when capturing, gravar, or padronizar respostas MCP em markdown.
---

# Salvar resposta Rastro MCP em `.md`

Depois de cada chamada MCP `user-rastro` que o usuário quiser arquivar, gravar `rastro_mcp/<tool>.md`.

Spec: [save_pattern.md](save_pattern.md)  
Corpo da resposta: [response_pattern.md](response_pattern.md)  
Canônico: `../screen_address_sanctions.md`

## Passos

1. Chamar a tool.
2. Montar o arquivo exatamente como [save_pattern.md](save_pattern.md): `**Prompt**` + fence + headline + tabela completa + parágrafo.
3. Escrever `rastro_mcp/<tool>.md` (um arquivo por tool; overwrite).
4. No chat, confirmar só o path e a headline.
