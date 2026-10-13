**Prompt**
```
Utilize o mcp da rastro para pegar pares e liquidez DEX (Uniswap, Ethereum) do token `USDT` `0xdac17f958d2ee523a2206206994597c13d831ec7`, utilizando a função `get_token_dex_info`.

me retorne as informações retornadas pelo endpoint e uma explicação resumida, utilizando maximo de economia de tokens.
```

**Pares DEX.** `pairs_total=5`

| Campo | Valor |
|---|---|
| token | `0xdac17f958d2ee523a2206206994597c13d831ec7` |
| source | DexScreener |
| pairs_total | 5 |
| truncated | false |
| pairs[0].dex | pulsex |
| pairs[0].chain | pulsechain |
| pairs[0].symbol | USDT |
| pairs[0].price_usd | 0.0006708 |
| pairs[0].liquidity | 175211.27 |
| pairs[0].volume_24h | 573.29 |
| pairs[0].url | https://dexscreener.com/pulsechain/0xd2335e1c634fc3a1ddf766161bcb8e7ec134cf03 |
| pairs[1].dex | pulsex |
| pairs[1].chain | pulsechain |
| pairs[1].symbol | USDT |
| pairs[1].price_usd | 0.0006922 |
| pairs[1].liquidity | 97493.98 |
| pairs[1].volume_24h | 136.68 |
| pairs[1].url | https://dexscreener.com/pulsechain/0x232911c6992e1f2f51fedd1f3d0be7d3a613f260 |
| pairs[2].dex | pulsex |
| pairs[2].chain | pulsechain |
| pairs[2].symbol | USDT |
| pairs[2].price_usd | 0.0006622 |
| pairs[2].liquidity | 26046.8 |
| pairs[2].volume_24h | 395.37 |
| pairs[2].url | https://dexscreener.com/pulsechain/0xa9607906406cf2cf98bc1a1f0224c85d779042bd |
| pairs[3].dex | pulsex |
| pairs[3].chain | pulsechain |
| pairs[3].symbol | USDT |
| pairs[3].price_usd | 0.0006688 |
| pairs[3].liquidity | 24388.67 |
| pairs[3].volume_24h | 1714.9 |
| pairs[3].url | https://dexscreener.com/pulsechain/0xfadc475639131c1eac3655c37eda430851d53716 |
| pairs[4].dex | pulsex |
| pairs[4].chain | pulsechain |
| pairs[4].symbol | USDT |
| pairs[4].price_usd | 0.0006653 |
| pairs[4].liquidity | 23426.71 |
| pairs[4].volume_24h | 81.93 |
| pairs[4].url | https://dexscreener.com/pulsechain/0x1ba4436daa19d77268ae1f13ca8294ec6a4c2486 |

DexScreener devolveu 5 pares PulseX em PulseChain (~$0.00067, não Uniswap Ethereum). Maior liquidez ~$175k; volume 24h máximo ~$1.7k. `truncated=false`; tool não filtra chain — não são pools Uniswap do USDT ~$1 na Ethereum.

**Nota.** `get_token_dex_info` só aceita `token` (contrato), sem `chain` nem DEX. Pedir Uniswap/Ethereum não muda o ranking do DexScreener: o mesmo endereço USDT existe na PulseChain e os 5 pares retornados foram PulseX (~$0.00067), não pools Uniswap (~$1).
