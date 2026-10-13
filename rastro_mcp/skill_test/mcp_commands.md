| Tool | O que faz | Custo |
|---|---|---|
| `screen_address_sanctions` | Está em lista de sanção/hack/scam (OFAC, SlowMist, Tornado…)? | instantâneo |
| `label_address` | É exchange, mixer, bridge ou contrato DeFi conhecido? | instantâneo |
| `get_token_prices` | Preço spot de até 50 símbolos (btc, eth…) | rápido |
| `get_historical_price` | Preço num dia passado (DD-MM-YYYY), USD e BRL | rápido |
| `get_token_dex_info` | Pares/liquidez DEX de um contrato, não ticker | rápido |
| `investigate_wallet` | Score 0–100, fatores, saldo, idade, funded_by | 2–8 s |
| `list_counterparties` | Grafo de 1 hop (com quem transacionou) | médio |
| `compare_wallets` | Duas wallets lado a lado + o que elas compartilham | médio |
| `lookup_transaction` | Transação por hash (com ou sem chain) | ~10 s |
| `scan_address_across_chains` | Mesmo endereço em até 6 chains | lento |
| `trace_fund_flow` | Segue o dinheiro hop a hop até exchange/mixer | lento |
| `generate_investigation_report` | Relatório completo (timeline, alerts, flow); job async | o mais caro |
