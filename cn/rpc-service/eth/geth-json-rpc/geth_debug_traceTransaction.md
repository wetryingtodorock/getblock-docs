---
title: geth:debug_traceTransaction \[POST\] {disallowed}
description: OBS In most scenarios, debug.standardTraceBlockToFile is better suitedfor tracing!The traceTransaction debugging method will attempt to run thetransaction in the exact same manner as it was executed on the network.It will replay any transaction that may have been executed prior to thisone before it will finally attempt to execute the transaction thatcorresponds to the given hash.In addition to the hash of the transaction you may give it a secondaryoptional argument, which specifies the options for this specific call.The possible options are disableStorage BOOL. Setting this to falsewill disable storage capture (default = false). disableStack BOOL.Setting this to false will disable stack capture (default = false).enableMemory BOOL. Setting this to false will enable memory capture(default = false). enableReturnData BOOL. Setting this to false willenable return data capture (default = false). tracer STRING. Settingthis will enable JavaScript-based transaction tracing, described below.If set, the previous four arguments will be ignored. timeout STRING.Overrides the default timeout of 5 seconds for JavaScript-based tracingcalls. Valid values are described here.
---

### Parameters


`txHash` - string

hash of a transactions

`options` - array of string

additional options

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_traceTransaction",
"params": ["0x6470a89b9e7f0665781360c369ab57c0c199df4cc32d973f2d4a7b34f084c3a4"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "result": "null",
    "id": "getblock.io",
    "status_code": 405,
    "message": "Method not allowed"
}
```

