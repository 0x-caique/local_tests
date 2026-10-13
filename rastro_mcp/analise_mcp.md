| serviço | status | nota | motivo |
|---|---|---|---|
| screen_address_sanctions | sucesso | 10 | Hit OFAC SDN correto (`found=true`, score 100, FREEZE_RECOMMENDED); payload completo, sem lacuna. |
| get_token_prices | sucesso | 10 | Precificou WBTC, USDC, USDT e PEPE; `unpriced` vazio e fontes explícitas. |
| get_historical_price | sucesso | 10 | WBTC em 13-10-2025 com USD e BRL (CoinGecko), no formato pedido. |
| compare_wallets | sucesso | 9 | Comparou as duas wallets (scores, USD, transfers, `riskier=tie`); listas compartilhadas vazias, mas o endpoint respondeu. |
| generate_investigation_report | sucesso | 8 | Job `succeeded` com relatório e flow; faltam counterparties, `funded_by`, totais USD e preço dos tokens. |
| scan_address_across_chains | parcial | 7 | 6 chains `ok`, atividade só em ETH; as outras 5 vieram `inconclusive` com score 25 que não vale. |
| list_counterparties | parcial | 7 | Grafo 1 hop retornou (87 nós / 200 arestas), mas truncado (30 nós, 89 edges omitidas) e todos `risk=low`. |
| lookup_transaction | parcial | 6 | Hash encontrado em ETH, porém só RPC cru; nome do contrato e ação foram inferidos fora do MCP. |
| investigate_wallet | parcial | 5 | Payload rico, mas wallet pública do Felipe bateu score 100; scoring precisa revisão e falta ENS. |
| label_address | falha | 4 | `labeled=false` em endereço DeFi conhecido (Uniswap Universal Router); registro estático incompleto. |
| get_token_dex_info | falha | 3 | Pedido Uniswap/Ethereum no USDT; devolveu 5 pares PulseX em PulseChain (~$0.00067), sem filtro de chain/DEX. |
| trace_fund_flow | falha | 2 | Não capturou entrada nem saída de AAVE; budget=30 deu 503, retry `incomplete=true`, árvore sem tx/data/valor. |
