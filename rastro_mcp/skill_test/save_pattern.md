# Padrão de salvamento (Rastro MCP → `.md`)

Um arquivo por tool: `rastro_mcp/<tool>.md`. Sobrescrever se a mesma tool for salva de novo.

O `.md` **não** é só a resposta do chat. É Prompt + resposta. Espelho: `rastro_mcp/screen_address_sanctions.md`.

## Estrutura (sempre nesta ordem)

1. `**Prompt**`
2. Fence ` ``` ` com o prompt completo (alvo literal + nome da tool + economia de tokens).
3. Headline + tabela (todos os campos do JSON) + parágrafo único — igual [response_pattern.md](response_pattern.md).

## Template

**Prompt**
```
Utilize o mcp da rastro para {ação} `{alvo}`, utilizando a função `{tool}`.

me retorne as informações retornadas pelo endpoint e uma explicação resumida, utilizando maximo de economia de tokens.
```

**{VEREDITO}.** `{chave}={valor}`

| Campo | Valor |
|---|---|
| {campo} | {valor} |

{1–2 frases: interpretação + ação + caveat.}

## Regras

- Não inventar campos. Não omitir campos do JSON.
- `found=false` / `labeled=false` / lista vazia ≠ endereço limpo.
- Endereços e hashes em backticks.
- Segunda linha do prompt: texto fixo (`me retorne as informações... economia de tokens.`).
- Sem frontmatter, sem H1, sem JSON cru.

## Exemplo canônico

Ver `rastro_mcp/screen_address_sanctions.md`.
