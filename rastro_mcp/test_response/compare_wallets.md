**Prompt**
```
Utilize o mcp da rastro para comparar as wallets `0x47f425c7cd2ddc0294193994be84cf02a2360e77` e `0x3AD9dB589d201A710Ed237c829c7860Ba86510Fc`, utilizando a função `compare_wallets`.

me retorne as informações retornadas pelo endpoint e uma explicação resumida, utilizando maximo de economia de tokens.
```

**Risco alto.** `riskier=tie`

| Campo | Valor |
|---|---|
| left.wallet | `0x47f425c7cd2ddc0294193994be84cf02a2360e77` |
| left.chain | ETH |
| left.risk_score | 100 |
| left.classification | CRITICAL |
| left.total_usd | 127535.45 |
| left.transfer_count | 200 |
| left.inconclusive | false |
| right.wallet | `0x3ad9db589d201a710ed237c829c7860ba86510fc` |
| right.chain | ETH |
| right.risk_score | 100 |
| right.classification | CRITICAL |
| right.total_usd | 0.0 |
| right.transfer_count | 7 |
| right.inconclusive | false |
| comparable | true |
| riskier | tie |
| risk_score_diff | 0 |
| total_usd_diff | -127535.45 |
| transfer_count_diff | -193 |
| shared_counterparties | [] |
| shared_kyc_addresses | [] |
| note | null |

Ambas **CRITICAL** (`score=100`); empate de risco, comparáveis. Esquerda tem ~US$127k e 200 transfers; direita saldo 0 e 7 transfers. Sem counterparties/KYC compartilhados — lista vazia ≠ wallets limpas; aprofundar cada uma à parte.
