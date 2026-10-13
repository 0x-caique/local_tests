**Prompt**
```
Utilize o mcp da rastro para consultar a transação `0xafed05f17eaac7892c86a22609235ddddd7d4ad6884f3dd0e775aa8d157d6380`, utilizando a função `lookup_transaction`.

me retorne as informações retornadas pelo endpoint e uma explicação resumida, utilizando maximo de economia de tokens.
```

**Tx encontrada.** `found=true`

| Campo | Valor |
|---|---|
| hash | `0xafed05f17eaac7892c86a22609235ddddd7d4ad6884f3dd0e775aa8d157d6380` |
| found | true |
| matches.ETH.jsonrpc | 2.0 |
| matches.ETH.id | 1 |
| matches.ETH.result.blockHash | `0x9f595c7fd8ed36ebc16cc0d719db353961fb4a7df7954971bba7ee87acb9d5a4` |
| matches.ETH.result.blockNumber | 0x18f7e66 |
| matches.ETH.result.blockTimestamp | 0x6acdb56b |
| matches.ETH.result.from | `0xabb17dfe30f201ad7e7d37319fa829ce15f2e5f8` |
| matches.ETH.result.gas | 0x493e0 |
| matches.ETH.result.gasPrice | 0x39e54aa |
| matches.ETH.result.maxFeePerGas | 0x750c110 |
| matches.ETH.result.maxPriorityFeePerGas | 0x0 |
| matches.ETH.result.hash | `0xafed05f17eaac7892c86a22609235ddddd7d4ad6884f3dd0e775aa8d157d6380` |
| matches.ETH.result.input | `0x38ed17390000000000000000000000000000000000000000000000000429d069189e0000000000000000000000000000000000000000000000010b384e00409a3040d94f00000000000000000000000000000000000000000000000000000000000000a0000000000000000000000000abb17dfe30f201ad7e7d37319fa829ce15f2e5f8000000000000000000000000000000000000000000000000000000006acdb6920000000000000000000000000000000000000000000000000000000000000002000000000000000000000000c02aaa39b223fe8d0a0e5c4f27ead9083c756cc20000000000000000000000001edc13773be64d5f5cceb1ddc252928d8a6620df` |
| matches.ETH.result.nonce | 0x9b5 |
| matches.ETH.result.to | `0x7a250d5630b4cf539739df2c5dacb4c659f2488d` |
| matches.ETH.result.transactionIndex | 0x57 |
| matches.ETH.result.value | 0x0 |
| matches.ETH.result.type | 0x2 |
| matches.ETH.result.accessList | [] |
| matches.ETH.result.chainId | 0x1 |
| matches.ETH.result.v | 0x0 |
| matches.ETH.result.r | `0xd7083561bccc92c401d9015c950fbb7d929f1ef6cb9a702996fb047f731652fb` |
| matches.ETH.result.s | `0x5189e4855094a69722f60a61c313b1fd382e29f9987504177cba93b5e04cabfd` |
| matches.ETH.result.yParity | 0x0 |
| chains_tried | ETH |
| truncated | false |
| note | null |

Hash encontrado só em **ETH** (`chainId=0x1`, EIP-1559, `value=0`). `from` chama `to` Uniswap V2 Router (`0x7a250d…`), selector `swapExactTokensForTokens`; payload é o objeto RPC cru (sem receipt/logs). `truncated=false`; `found=true` não implica risco — para score/sanção use `investigate_wallet` / `screen_address_sanctions`.

**Nota.** Nomes de contrato e ação (Uniswap V2 Router, `swapExactTokensForTokens`) **não vêm do MCP**. O endpoint só devolve objeto RPC cru (`from`/`to` hex, `input` calldata). Essa leitura foi inferida pelo agente (`to` conhecido + selector `0x38ed1739`). Para label do `to`, use `label_address`.
