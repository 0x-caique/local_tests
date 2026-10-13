**Prompt**
```
Utilize o mcp da rastro para investigar essa wallet `0x961c5be54a2ffc17cf4cb021d863c42dacd47fc1`, utilizando a função `investigate_wallet`.

me retorne as informações retornadas pelo endpoint e uma explicação resumida, utilizando maximo de economia de tokens.
```

**Risco alto.** `score=100`

| Campo | Valor |
|---|---|
| wallet | `0x961c5be54a2ffc17cf4cb021d863c42dacd47fc1` |
| chain | ETH |
| inconclusive | false |
| inconclusive_reason | null |
| risk_score | 100 |
| classification | CRITICAL |
| action | FREEZE_RECOMMENDED |
| generated_at | 2026-10-13T01:08:45-03:00 |
| response_time | 3s |
| risk_factors[0].rule | kyc_hit |
| risk_factors[0].score | 100.0 |
| risk_factors[0].description | 1 high-risk address found |
| risk_factors[0].critical | true |
| risk_factors[1].rule | round_values |
| risk_factors[1].score | 12.0 |
| risk_factors[1].description | 13 outbound transfers with exact round values — scam payout pattern |
| risk_factors[1].critical | false |
| risk_factors[2].rule | intermediate_wallets |
| risk_factors[2].score | 25.0 |
| risk_factors[2].description | 31 intermediate wallets — possible layering / hops |
| risk_factors[2].critical | false |
| risk_factors[3].rule | outbound_burst |
| risk_factors[3].score | 10.0 |
| risk_factors[3].description | 22 outbound transfers from origin — high dispersion |
| risk_factors[3].critical | false |
| risk_factors[4].rule | high_volume |
| risk_factors[4].score | 8.0 |
| risk_factors[4].description | 59 transactions — elevated activity volume |
| risk_factors[4].critical | false |
| kyc_hits[0].address | `0x961c5be54a2ffc17cf4cb021d863c42dacd47fc1` |
| kyc_hits[0].label | OFAC Sanctioned (ETH) |
| kyc_hits[0].category | SANCTIONED |
| kyc_hits[0].source | OFAC SDN |
| funded_by.address | `0xf26f397fef9f338b7502c6fc42aa18ebd1af756d` |
| funded_by.name | null |
| funded_by.category | wallet |
| funded_by.label | null |
| funded_by.tx_hash | `0x1122044f51ccc524ff5d3ad459e6385d419b91369a606cae6641374e1cb98154` |
| funded_by.funded_at | 2022-05-09T06:43:49Z |
| funded_by.value | 345.3 |
| funded_by.token_symbol | USDT |
| funded_by.approximate | false |
| funded_by_note | null |
| native_balance | 0.004048339864717564 |
| native_unit | ETH |
| total_usd | 10.15 |
| inflow_usd | 85053.56 |
| outflow_usd | 84979.61 |
| age_days | 1618 |
| first_tx_at | 2022-05-09T06:43:49Z |
| last_tx_at | 2023-08-15T14:26:11Z |
| transfer_count | 59 |
| transaction_count | 59 |
| counterparty_count | 32 |
| exchange_count | 1 |
| mixer_count | 0 |
| labeled_counterparties[0].address | `0x28c6c06298d514db089934071355e5743bf21d60` |
| labeled_counterparties[0].label | Binance |
| labeled_counterparties[0].category | exchange |
| labeled_counterparties_total | 1 |
| top_tokens[0].symbol | 0x17158e |
| top_tokens[0].balance | 8e-16 |
| top_tokens[0].usd_value | 0.0 |
| top_tokens[0].contract | `0x17158e788771ebff629e00e9b0b62a9c921e2134` |
| tokens_total | 1 |
| spam_count | 0 |
| dust_count | 1 |
| notes[0] | Risk is computed from the transfer history the provider returned, which can be a recent window for very active wallets. |
| notes[1] | usd_value 0 means the token could not be priced or is worthless; it is not a valuation. |

Endereço **OFAC SDN** (ETH sancionado): score 100, `CRITICAL`, freeze. Histórico ETH 2022–2023 (~$85k in/out, 1 hop Binance, funded_by `0xf26f397fef9f338b7502c6fc42aa18ebd1af756d` em USDT); saldo residual ~$10. Layering/round payouts agravantes, não o hit. Não tratar como limpo.

**Prompt**
```
Utilize o mcp da rastro para investigar essa wallet `0x47f425c7cd2ddc0294193994be84cf02a2360e77`, utilizando a função `investigate_wallet`.

me retorne as informações retornadas pelo endpoint e uma explicação resumida, utilizando maximo de economia de tokens.
```

**Risco alto.** `score=100`

| Campo | Valor |
|---|---|
| wallet | `0x47f425c7cd2ddc0294193994be84cf02a2360e77` |
| chain | ETH |
| inconclusive | false |
| inconclusive_reason | null |
| risk_score | 100 |
| classification | CRITICAL |
| action | FREEZE_RECOMMENDED |
| generated_at | 2026-10-13T01:18:33-03:00 |
| response_time | 5s |
| risk_factors[0].rule | high_frequency |
| risk_factors[0].score | 15.0 |
| risk_factors[0].description | High transaction frequency (200) |
| risk_factors[0].critical | false |
| risk_factors[1].rule | fan_out |
| risk_factors[1].score | 20.0 |
| risk_factors[1].description | Extreme fan-out (52 unique destinations) |
| risk_factors[1].critical | true |
| risk_factors[2].rule | layering_burst |
| risk_factors[2].score | 25.0 |
| risk_factors[2].description | 6 outbound transfers on the same day — typical fractioning pattern |
| risk_factors[2].critical | true |
| risk_factors[3].rule | round_values |
| risk_factors[3].score | 12.0 |
| risk_factors[3].description | 32 outbound transfers with exact round values — scam payout pattern |
| risk_factors[3].critical | false |
| risk_factors[4].rule | structuring |
| risk_factors[4].score | 15.0 |
| risk_factors[4].description | 22 low-value outbound transfers — possible smurfing / structuring |
| risk_factors[4].critical | false |
| risk_factors[5].rule | intermediate_wallets |
| risk_factors[5].score | 25.0 |
| risk_factors[5].description | 86 intermediate wallets — possible layering / hops |
| risk_factors[5].critical | false |
| risk_factors[6].rule | outbound_burst |
| risk_factors[6].score | 10.0 |
| risk_factors[6].description | 100 outbound transfers from origin — high dispersion |
| risk_factors[6].critical | false |
| risk_factors[7].rule | high_volume |
| risk_factors[7].score | 8.0 |
| risk_factors[7].description | 200 transactions — elevated activity volume |
| risk_factors[7].critical | false |
| kyc_hits[0].address | `0xab5801a7d398351b8be11c439e05c5b3259aec9b` |
| kyc_hits[0].label | Vitalik Buterin |
| kyc_hits[0].category | LEGITIMATE |
| kyc_hits[0].source | Etherscan |
| funded_by.address | `0xdb1fef381e342ffe7d9d554555ef392b0fe932e1` |
| funded_by.name | null |
| funded_by.category | wallet |
| funded_by.label | null |
| funded_by.tx_hash | `0x20e196659c7fcdcbf110636cbd536dd22159b76953d71cf78e1d4477fc95f4c7` |
| funded_by.funded_at | 2022-09-09T03:23:11Z |
| funded_by.value | 4.0 |
| funded_by.token_symbol | ETH |
| funded_by.approximate | false |
| funded_by_note | null |
| native_balance | 11.718866163068544 |
| native_unit | ETH |
| total_usd | 126974.15 |
| inflow_usd | 207020.22 |
| outflow_usd | 267884.2 |
| age_days | 1495 |
| first_tx_at | 2022-09-09T03:23:11Z |
| last_tx_at | 2023-12-23T22:08:47Z |
| transfer_count | 200 |
| transaction_count | 200 |
| counterparty_count | 86 |
| exchange_count | 0 |
| mixer_count | 0 |
| labeled_counterparties | [] |
| labeled_counterparties_total | 0 |
| top_tokens[0].symbol | AAVE |
| top_tokens[0].balance | 539.2768514522185 |
| top_tokens[0].usd_value | 85750.41 |
| top_tokens[0].contract | `0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9` |
| top_tokens[1].symbol | UNI |
| top_tokens[1].balance | 1622.3132653186153 |
| top_tokens[1].usd_value | 11859.11 |
| top_tokens[1].contract | `0x1f9840a85d5af5bf1d1762f925bdaddc4201f984` |
| top_tokens[2].symbol | RESOLV |
| top_tokens[2].balance | 4.0 |
| top_tokens[2].usd_value | 0.07 |
| top_tokens[2].contract | `0x259338656198ec7a76c729514d3cb45dfbf768a1` |
| top_tokens[3].symbol | MATIC |
| top_tokens[3].balance | 0.0928862811803547 |
| top_tokens[3].usd_value | 0.01 |
| top_tokens[3].contract | `0x7d1afa7b718fb893db30a3abc0cfc608aacfebb0` |
| top_tokens[4].symbol | 0x00e2b6 |
| top_tokens[4].balance | 1.0 |
| top_tokens[4].usd_value | 0.0 |
| top_tokens[4].contract | `0x00e2b6d170740c15bf9fb01d0b6e77c0d4510e32` |
| top_tokens[5].symbol | 0x12b01a |
| top_tokens[5].balance | 4.83e-15 |
| top_tokens[5].usd_value | 0.0 |
| top_tokens[5].contract | `0x12b01aa62e87fd0191b4f8e5b9dc28ced876d16d` |
| top_tokens[6].symbol | 0x132e6c |
| top_tokens[6].balance | 30.1265608837823 |
| top_tokens[6].usd_value | 0.0 |
| top_tokens[6].contract | `0x132e6c9c33a62d7727cd359b1f51e5b566e485eb` |
| top_tokens[7].symbol | 0x1e30af |
| top_tokens[7].balance | 5.5995281e-11 |
| top_tokens[7].usd_value | 0.0 |
| top_tokens[7].contract | `0x1e30afeb27c0544f335f8aa21e0a9599c273823a` |
| top_tokens[8].symbol | HEX |
| top_tokens[8].balance | 1e-10 |
| top_tokens[8].usd_value | 0.0 |
| top_tokens[8].contract | `0x2b591e99afe9f32eaa6214f7b7629768c40eeb39` |
| top_tokens[9].symbol | 0x35063f |
| top_tokens[9].balance | 2.97633022968e-7 |
| top_tokens[9].usd_value | 0.0 |
| top_tokens[9].contract | `0x35063f51d5430da284be8c4c6673498334a89f76` |
| tokens_total | 45 |
| spam_count | 0 |
| dust_count | 43 |
| notes[0] | Risk is computed from the transfer history the provider returned, which can be a recent window for very active wallets. |
| notes[1] | usd_value 0 means the token could not be priced or is worthless; it is not a valuation. |

Não está em lista de sanção; score 100 vem de **comportamento** (fan-out, layering, round payouts, structuring), não de OFAC. `kyc_hits` = Vitalik (`LEGITIMATE`). Freeze por padrão de fluxo; ausência em sanções ≠ limpo. Histórico ETH 2022–2023, ~$127k saldo (AAVE/UNI), 200 txs, 86 hops.

**Nota.** A wallet pública do Felipe bateu 100 de score; precisamos analisar como os riscos estão sendo avaliados e adicionar um ENS (Ethereum Name Service) da wallet.
