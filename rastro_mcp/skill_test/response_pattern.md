# Padrão de resposta (Rastro MCP)

Economia máxima de tokens. Sem introdução, sem repetir o prompt, sem markdown extra.

## Estrutura (sempre nesta ordem)

1. **Headline** — veredito em 2–5 palavras + status-chave em `` `backticks` ``.
2. **Tabela** — todos os campos retornados pelo endpoint, um por linha (`Campo | Valor`).
3. **Parágrafo único** — o que significa + ação recomendada + caveat (se houver).

Não inventar campos. Não omitir campos do JSON. `found=false` / lista vazia ≠ endereço limpo.

## Template

```
**{VEREDITO}.** `{chave}={valor}`

| Campo | Valor |
|---|---|
| {campo} | {valor} |

{1–2 frases: interpretação + ação + caveat.}
```

## Regras da headline

| Resultado | Headline |
|---|---|
| Hit de sanção/hack/scam | **Hit de sanção.** `found=true` |
| Não listado | **Não listado.** `found=false` |
| Label conhecida | **Label conhecida.** `{categoria}` |
| Sem label | **Sem label.** `unknown` |
| Score alto | **Risco alto.** `score={n}` |
| Score baixo | **Risco baixo.** `score={n}` |
| Job async | **Job pendente.** `job_id={id}` |

Valores literais do JSON em backticks. Endereços/hashes em backticks.

## Exemplo canônico (`screen_address_sanctions`)

**Hit de sanção.** `found=true`

| Campo | Valor |
|---|---|
| address | `0xfac583c0cf07ea434052c49115a4682172ab6b4f` |
| label | OFAC Sanctioned (USDT) |
| category | SANCTIONED |
| score | 100 |
| source | OFAC SDN |
| action | FREEZE_RECOMMENDED |

Endereço está na **OFAC SDN** (lista de sanções dos EUA), marcado como USDT sancionado. Score máximo; ação recomendada: freeze. Não tratar como “limpo” em nenhum caso.
