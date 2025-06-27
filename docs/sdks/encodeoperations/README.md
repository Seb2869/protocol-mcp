# EncodeOperations
(*encodeOperations*)

## Overview

### Available Operations

* [encode](#encode) - Generate order encode data for sign operations

## encode

Generate order encode data for sign operations

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.encodeOperations.encode({
    data: {
      atType: "ETH_RARIBLE_V2_3",
      payouts: [
        {
          account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          value: 798033,
        },
      ],
      originFees: [
        {
          account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          value: 147768,
        },
      ],
      isMakeFill: false,
    },
    maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    make: {
      assetType: {
        atType: "COLLECTION",
        contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
        collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
      },
      value: "123456",
    },
    take: {
      assetType: {
        atType: "SOLANA_SOL",
      },
      value: "123456",
    },
    endedAt: new Date("2025-07-31T15:23:51.405Z"),
    salt: "123456",
    signature: "<value>",
    blockchain: "ETHEREUM",
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
import { encodeOperationsEncode } from "@rarible/protocol-mcp/funcs/encodeOperationsEncode.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const res = await encodeOperationsEncode(raribleProtocolMcp, {
    data: {
      atType: "ETH_RARIBLE_V2_2",
      payouts: [
        {
          account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          value: 174494,
        },
      ],
      originFees: [
        {
          account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          value: 348451,
        },
      ],
      isMakeFill: false,
    },
    maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    make: {
      assetType: {
        atType: "CURRENCY_TOKEN",
        contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
      },
      value: "123456",
    },
    take: {
      assetType: {
        atType: "FLOW_NFT",
        contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
        collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
        tokenId: "123456",
      },
      value: "123456",
    },
    endedAt: new Date("2023-02-27T17:35:06.179Z"),
    salt: "123456",
    signature: "<value>",
    blockchain: "ETHEREUM",
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
| `request`                                                                                                                                                                      | [models.OrderForm](../../models/orderform.md)                                                                                                                                  | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.EncodedOrder](../../models/encodedorder.md)\>**

### Errors

| Error Type                      | Status Code                     | Content Type                    |
| ------------------------------- | ------------------------------- | ------------------------------- |
| errors.UnionApiErrorBadRequest  | 400                             | application/json                |
| errors.UnionApiErrorServerError | 500                             | application/json                |
| errors.APIError                 | 4XX, 5XX                        | \*/\*                           |