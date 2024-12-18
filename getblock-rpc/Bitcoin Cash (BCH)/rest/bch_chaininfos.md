# bch:chaininfos \[GET\]

Returns various state info regarding block chain processing. Only
supports JSON as output format.

-   chain : (string) current network name (main, test, signet, regtest)

-   blocks : (numeric) the current number of blocks processed in the
    server

-   headers : (numeric) the current number of headers we have validated

-   bestblockhash : (string) the hash of the currently best block

-   difficulty : (numeric) the current difficulty

-   mediantime : (numeric) the median time of the 11 blocks before the
    most recent block on the blockchain

-   verificationprogress : (numeric) estimate of verification progress
    \[0..1\]

-   chainwork : (string) total amount of work in active chain, in
    hexadecimal

-   pruned : (boolean) if the blocks are subject to pruning

-   pruneheight : (numeric) highest block available

-   softforks : (array) status of softforks in progress

### Example

`GET /rest/chaininfo.json`

### Request

``` java
curl --location --request GET 'https://bch.getblock.io/mainnet/rest/chaininfo.json' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json'
```

### Response

``` java
{
    "chain": "main",
    "blocks": 680033,
    "headers": 680033,
    "bestblockhash": "00000000000000000006f41442a30e745e177dff2a3ef65bdd77b96d015ac489",
    "difficulty": 23581981443663.85,
    "mediantime": 1619019097,
    "verificationprogress": 0.9999982448971894,
    "initialblockdownload": false,
    "chainwork": "00000000000000000000000000000000000000001c529f37380904dd8e2fae58",
    "size_on_disk": 386449729745,
    "pruned": false,
    "softforks": {
        "bip34": {
            "type": "buried", 
            "active": true, 
            "height": 227931
        },
        "bip66": {
            "type": "buried", 
            "active": true,
            "height": 363725
        },
        "bip65": {
            "type": "buried", 
            "active": true, 
            "height": 388381
        },
        "csv": {
            "type": "buried", 
            "active": true, 
            "height": 419328
        },
        "segwit": {
            "type": "buried",
            "active": true, 
            "height": 481824
        }
    }, 
    "warnings": ""
}
```
