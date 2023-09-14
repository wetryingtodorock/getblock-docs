---
title: zec:setlogfilter \[POST\] {disallowed}
description: Sets the filter to be used for selecting events to log.A filter is a comma-separated list of directives.The syntax for each directive is target\[spanfield=value\]=levelThe default filter, derived from the -debug=target flags, iserror,main=infoPassing a valid filter here will replace the existing filter.Passing an empty string will reset the filter to the default.
---

### Parameters


`newFilterDirectives` - string

The new log filter.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "setlogfilter",
"params": [null],
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

