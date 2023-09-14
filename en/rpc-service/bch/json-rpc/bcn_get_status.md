---
title: bcn:get_status \[POST\]
description: Get status about state of bytecoind. This method supports longpolling.If you specify all input parameters, and they are equal to the currentstate of the bytecoind, you will get response only when some of themchange.But if you specify only certain argument, changes to other argumentswont trigger the longpoll. For example, if you are interested inoutgoing_peer_count only, you can specify only outgoing_peer_count inrequest and get response when outgoing_peer_count changes.
---

### Parameters


`top_block_hash` - string

Optional.

Value received in previous get_status response.

`transaction_pool_version` - uint32

Optional.

Value received in previous get_status response.

`incoming_peer_count` - uint32

Optional.

Value received in previous get_status response.

`outgoing_peer_count` - uint32

Optional.

Value received in previous get_status response.

`lower_level_error` - string

Optional.

Value received in previous get_status response.

### Request

``` java
curl --location --request POST 'https://bcn.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "get_status",
"params": {},
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "incoming_peer_count": 0,
        "lower_level_error": "",
        "next_block_effective_median_size": 98872,
        "outgoing_peer_count": 8,
        "recommended_fee_per_byte": 100,
        "recommended_max_transaction_size": 98872,
        "top_block_cumulative_difficulty": 30676358330795090,
        "top_block_difficulty": 10361588328,
        "top_block_hash": "5099fb0b04b83d4f9862109608349d7a25938e6aa00b509366848589fe69917a",
        "top_block_height": 2403323,
        "top_block_timestamp": 1631799662,
        "top_block_timestamp_median": 1631795442,
        "top_known_block_height": 2403323,
        "transaction_pool_version": 2438
    }
}
```

