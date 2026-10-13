**Prompt**
```
Utilize o mcp da rastro para verificar se essa wallet `0xfac583c0cf07ea434052c49115a4682172ab6b4f` está na lista de sanções, utilizando a função `screen_address_sanctions`.

me retorne as informações retornadas pelo endpoint e uma explicação resumida, utilizando maximo de economia de tokens.
```

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
