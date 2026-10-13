**Prompt**

```
Utilize o mcp da rastro para verificar a label dessa wallet `0x66a9893cc07d91d95644aedd05d03f95e1dba8af`, utilizando a função `label_address`.

me retorne as informações retornadas pelo endpoint e uma explicação resumida, utilizando maximo de economia de tokens.
```

**Sem label.** `unknown`


| Campo          | Valor                                                                                                                                        |
| -------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| address        | `0x66a9893cc07d91d95644aedd05d03f95e1dba8af`                                                                                                 |
| labeled        | false                                                                                                                                        |
| label          | null                                                                                                                                         |
| category       | null                                                                                                                                         |
| is_exchange    | false                                                                                                                                        |
| is_mixer       | false                                                                                                                                        |
| source         | unknown                                                                                                                                      |
| checked_at     | 2026-10-13T00:12:09-03:00                                                                                                                    |
| interpretation | No label in Rastro's static registry of known exchanges, mixers, bridges and DeFi contracts. This does NOT mean the address is unremarkable. |


  
**Nota**. Não há label no registro estático da Rastro (exchanges, mixers, bridges, DeFi). Isso não prova que o endereço é irrelevante; para entidade/risco, use `investigate_wallet` ou `screen_address_sanctions`.