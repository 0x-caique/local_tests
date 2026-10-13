**Prompt**
```
Utilize o mcp da rastro para pegar o preço dos tokens `WBTC, USDC, USDT, PEPE`, utilizando a função `get_token_prices`.

me retorne as informações retornadas pelo endpoint e uma explicação resumida, utilizando maximo de economia de tokens.
```

**Preços spot.** `currency=usd`

| Campo | Valor |
|---|---|
| currency | usd |
| prices.wbtc | 83089.0 |
| prices.usdc | 1.0 |
| prices.usdt | 1.0 |
| prices.pepe | 4.026e-6 |
| unpriced | [] |
| sources.wbtc | coingecko |
| sources.usdc | stable |
| sources.usdt | stable |
| sources.pepe | dexscreener |

WBTC ~$83k (CoinGecko); USDC/USDT = $1 (fonte stable); PEPE ~$4.03e-6 (DEX). `unpriced` vazio; nenhum símbolo veio como 0.
