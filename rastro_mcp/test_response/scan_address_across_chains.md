**Prompt**
```
Utilize o mcp da rastro para escanear essa wallet `0x47f425c7cd2ddc0294193994be84cf02a2360e77` em várias chains, utilizando a função `scan_address_across_chains`.

me retorne as informações retornadas pelo endpoint e uma explicação resumida, utilizando maximo de economia de tokens.
```

**Risco alto.** `score=100`

| Campo | Valor |
|---|---|
| address | `0x47f425c7cd2ddc0294193994be84cf02a2360e77` |
| chains_scanned | 6 |
| chains_failed | 0 |
| chains_not_scanned | [] |
| chains_with_balance | 1 |
| total_usd | 98073.42 |
| networks[0].chain | ETH |
| networks[0].ok | true |
| networks[0].error | null |
| networks[0].inconclusive | false |
| networks[0].risk_score | 100 |
| networks[0].classification | CRITICAL |
| networks[0].total_usd | 98073.42 |
| networks[0].native_balance | 11.718866163068544 |
| networks[0].native_unit | ETH |
| networks[0].transfer_count | 200 |
| networks[1].chain | BSC |
| networks[1].ok | true |
| networks[1].error | null |
| networks[1].inconclusive | true |
| networks[1].risk_score | 25 |
| networks[1].classification | LOW |
| networks[1].total_usd | 0.0 |
| networks[1].native_balance | 0.0 |
| networks[1].native_unit | BNB |
| networks[1].transfer_count | 0 |
| networks[2].chain | POLYGON |
| networks[2].ok | true |
| networks[2].error | null |
| networks[2].inconclusive | true |
| networks[2].risk_score | 25 |
| networks[2].classification | LOW |
| networks[2].total_usd | 0.0 |
| networks[2].native_balance | 0.0 |
| networks[2].native_unit | MATIC |
| networks[2].transfer_count | 0 |
| networks[3].chain | ARBITRUM |
| networks[3].ok | true |
| networks[3].error | null |
| networks[3].inconclusive | true |
| networks[3].risk_score | 25 |
| networks[3].classification | LOW |
| networks[3].total_usd | 0.0 |
| networks[3].native_balance | 0.0 |
| networks[3].native_unit | ETH |
| networks[3].transfer_count | 0 |
| networks[4].chain | BASE |
| networks[4].ok | true |
| networks[4].error | null |
| networks[4].inconclusive | true |
| networks[4].risk_score | 25 |
| networks[4].classification | LOW |
| networks[4].total_usd | 0.0 |
| networks[4].native_balance | 0.0 |
| networks[4].native_unit | ETH |
| networks[4].transfer_count | 0 |
| networks[5].chain | OPTIMISM |
| networks[5].ok | true |
| networks[5].error | null |
| networks[5].inconclusive | true |
| networks[5].risk_score | 25 |
| networks[5].classification | LOW |
| networks[5].total_usd | 0.0 |
| networks[5].native_balance | 0.0 |
| networks[5].native_unit | ETH |
| networks[5].transfer_count | 0 |
| note | A chain with ok=false failed (timeout or provider error): it was NOT scanned clean. A chain with inconclusive=true returned no transfer history. |

Atividade só em **ETH** (`risk_score=100`, CRITICAL, ~US$98k, 200 transfers); BSC/Polygon/Arbitrum/Base/Optimism deram `inconclusive=true` (sem histórico — score 25 não vale). Sanção `found=false` e sem label; profundidade em ETH via `investigate_wallet`.
