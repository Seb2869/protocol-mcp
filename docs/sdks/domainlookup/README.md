# DomainLookup
(*domainLookup*)

## Overview

### Available Operations

* [resolve](#resolve) - Resolve domain

## resolve

Resolves domain's blockchain address by its name (for example, from ENS domains collection)

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLEPROTOCOLMCP_API_KEY_AUTH"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.domainLookup.resolve({
    domain: "nick.eth",
  });

  // Handle the result
  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { RaribleProtocolMcpCore } from "@rarible/protocol-mcp/core.js";
import { domainLookupResolve } from "@rarible/protocol-mcp/funcs/domainLookupResolve.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLEPROTOCOLMCP_API_KEY_AUTH"] ?? "",
});

async function run() {
  const res = await domainLookupResolve(raribleProtocolMcp, {
    domain: "nick.eth",
  });

  if (!res.ok) {
    throw res.error;
  }

  const { value: result } = res;

  // Handle the result
  console.log(result);
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ResolveRequest](../../models/operations/resolverequest.md)                                                                                                         | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.DomainResolveResult](../../models/domainresolveresult.md)\>**

### Errors

| Error Type                         | Status Code                        | Content Type                       |
| ---------------------------------- | ---------------------------------- | ---------------------------------- |
| errors.UnionApiErrorBadRequest     | 400                                | application/json                   |
| errors.UnionApiErrorEntityNotFound | 404                                | application/json                   |
| errors.UnionApiErrorServerError    | 500                                | application/json                   |
| errors.APIError                    | 4XX, 5XX                           | \*/\*                              |