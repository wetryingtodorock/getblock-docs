---
metaTitle: Method (summary_markets)
title: summary_markets \[GET\]
description: Explore the GetBlock Explorer API to retrieve summary information about the blockchain markets. Leverage blockchain data for your applications effortlessly.
---

### Example

```GET /summary/market```

### Request

```
curl --location --request GET 'https://near.getblock.io/explorer/summary/markets' \
--header 'Accept: application/json' \
--header 'x-api-key: YOUR-API-KEY'
```

### Response

```
{
  "dominance": 0.1734034482758621,
  "market_cap": 1472731151.2078137,
  "price": {
    "BTC": 0.0001023192993560526,
    "USD": 1.71965776539297
  }
}
```
