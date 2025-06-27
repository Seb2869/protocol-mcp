# NFTSales
(*nftSales*)

## Overview

### Available Operations

* [getOrderById](#getorderbyid) - Get Order
* [prepareOrderTransaction](#prepareordertransaction) - Prepare order transaction
* [prepareOrderCancelTransaction](#prepareordercanceltransaction) - Prepare order cancel transaction
* [reportOrderById](#reportorderbyid) - Report Order
* [upsertOrder](#upsertorder) - Create or update Order
* [getValidatedOrderById](#getvalidatedorderbyid) - Get validated Order by Id
* [getOrdersByIds](#getordersbyids) - Get Orders by Ids
* [getOrdersAll](#getordersall) - Get all Orders
* [getAllSync](#getallsync) - Get all Orders (for sync)
* [getSellOrdersByMaker](#getsellordersbymaker) - Get user's sell Orders
* [getSellOrdersByItem](#getsellordersbyitem) - Get sell Orders for NFT
* [getSellOrders](#getsellorders) - Get sell Orders
* [getOrderBidsByMaker](#getorderbidsbymaker) - Get user's bid Orders
* [getOrderBidsByItem](#getorderbidsbyitem) - Get bid Orders for NFT
* [getOrderFloorBidsByCollection](#getorderfloorbidsbycollection) - Get floor bids for Collection
* [getOrderFees](#getorderfees) - Get fee settings

## getOrderById

Returns Order by Id

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.nftSales.getOrderById({
    id: "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
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
import { nftSalesGetOrderById } from "@rarible/protocol-mcp/funcs/nftSalesGetOrderById.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const res = await nftSalesGetOrderById(raribleProtocolMcp, {
    id: "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
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
| `request`                                                                                                                                                                      | [operations.GetOrderByIdRequest](../../models/operations/getorderbyidrequest.md)                                                                                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.Order](../../models/order.md)\>**

### Errors

| Error Type                         | Status Code                        | Content Type                       |
| ---------------------------------- | ---------------------------------- | ---------------------------------- |
| errors.UnionApiErrorBadRequest     | 400                                | application/json                   |
| errors.UnionApiErrorEntityNotFound | 404                                | application/json                   |
| errors.UnionApiErrorServerError    | 500                                | application/json                   |
| errors.APIError                    | 4XX, 5XX                           | \*/\*                              |

## prepareOrderTransaction

Prepare all required data to match given order on the blockchain

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.nftSales.prepareOrderTransaction({
    id: "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
    prepareOrderTxForm: {
      maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      amount: "123456",
      payouts: [
        {
          account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          value: 711413,
        },
      ],
      originFees: [
        {
          account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          value: 173208,
        },
        {
          account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          value: 173208,
        },
      ],
    },
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
import { nftSalesPrepareOrderTransaction } from "@rarible/protocol-mcp/funcs/nftSalesPrepareOrderTransaction.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const res = await nftSalesPrepareOrderTransaction(raribleProtocolMcp, {
    id: "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
    prepareOrderTxForm: {
      maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      amount: "123456",
      payouts: [
        {
          account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          value: 711413,
        },
      ],
      originFees: [
        {
          account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          value: 173208,
        },
        {
          account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          value: 173208,
        },
      ],
    },
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
| `request`                                                                                                                                                                      | [operations.PrepareOrderTransactionRequest](../../models/operations/prepareordertransactionrequest.md)                                                                         | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.PrepareOrderTxResponse](../../models/prepareordertxresponse.md)\>**

### Errors

| Error Type                         | Status Code                        | Content Type                       |
| ---------------------------------- | ---------------------------------- | ---------------------------------- |
| errors.UnionApiErrorBadRequest     | 400                                | application/json                   |
| errors.UnionApiErrorEntityNotFound | 404                                | application/json                   |
| errors.UnionApiErrorServerError    | 500                                | application/json                   |
| errors.APIError                    | 4XX, 5XX                           | \*/\*                              |

## prepareOrderCancelTransaction

Prepare all required data to cancel given order on the blockchain

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.nftSales.prepareOrderCancelTransaction({
    id: "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
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
import { nftSalesPrepareOrderCancelTransaction } from "@rarible/protocol-mcp/funcs/nftSalesPrepareOrderCancelTransaction.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const res = await nftSalesPrepareOrderCancelTransaction(raribleProtocolMcp, {
    id: "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
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
| `request`                                                                                                                                                                      | [operations.PrepareOrderCancelTransactionRequest](../../models/operations/prepareordercanceltransactionrequest.md)                                                             | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.PreparedOrderTx](../../models/preparedordertx.md)\>**

### Errors

| Error Type                         | Status Code                        | Content Type                       |
| ---------------------------------- | ---------------------------------- | ---------------------------------- |
| errors.UnionApiErrorBadRequest     | 400                                | application/json                   |
| errors.UnionApiErrorEntityNotFound | 404                                | application/json                   |
| errors.UnionApiErrorServerError    | 500                                | application/json                   |
| errors.APIError                    | 4XX, 5XX                           | \*/\*                              |

## reportOrderById

Report Error Order

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  await raribleProtocolMcp.nftSales.reportOrderById({
    id: "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { RaribleProtocolMcpCore } from "@rarible/protocol-mcp/core.js";
import { nftSalesReportOrderById } from "@rarible/protocol-mcp/funcs/nftSalesReportOrderById.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const res = await nftSalesReportOrderById(raribleProtocolMcp, {
    id: "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
  });

  if (!res.ok) {
    throw res.error;
  }

  const { value: result } = res;

  
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ReportOrderByIdRequest](../../models/operations/reportorderbyidrequest.md)                                                                                         | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type                         | Status Code                        | Content Type                       |
| ---------------------------------- | ---------------------------------- | ---------------------------------- |
| errors.UnionApiErrorBadRequest     | 400                                | application/json                   |
| errors.UnionApiErrorEntityNotFound | 404                                | application/json                   |
| errors.UnionApiErrorServerError    | 500                                | application/json                   |
| errors.APIError                    | 4XX, 5XX                           | \*/\*                              |

## upsertOrder

Create or update off-chain Order (supported only for some blockchains)

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.nftSales.upsertOrder({
    data: {
      atType: "ETH_RARIBLE_V2_2",
      payouts: [
        {
          account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          value: 520418,
        },
      ],
      originFees: [
        {
          account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          value: 504403,
        },
      ],
      isMakeFill: false,
    },
    maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    make: {
      assetType: {
        atType: "FLOW_FT",
        contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
      },
      value: "123456",
    },
    take: {
      assetType: {
        atType: "NFT",
        collectionId: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
        itemId: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
      },
      value: "123456",
    },
    endedAt: new Date("2024-10-14T10:55:34.398Z"),
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
import { nftSalesUpsertOrder } from "@rarible/protocol-mcp/funcs/nftSalesUpsertOrder.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const res = await nftSalesUpsertOrder(raribleProtocolMcp, {
    data: {
      atType: "ETH_RARIBLE_V2_2",
      payouts: [
        {
          account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          value: 893339,
        },
      ],
      originFees: [
        {
          account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
          value: 642475,
        },
      ],
      isMakeFill: false,
    },
    maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    make: {
      assetType: {
        atType: "NFT",
        collectionId: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
        itemId: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
      },
      value: "123456",
    },
    take: {
      assetType: {
        atType: "NFT",
        collectionId: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
        itemId: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
      },
      value: "123456",
    },
    endedAt: new Date("2024-02-24T21:44:24.221Z"),
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

**Promise\<[models.Order](../../models/order.md)\>**

### Errors

| Error Type                      | Status Code                     | Content Type                    |
| ------------------------------- | ------------------------------- | ------------------------------- |
| errors.UnionApiErrorBadRequest  | 400                             | application/json                |
| errors.UnionApiErrorServerError | 500                             | application/json                |
| errors.APIError                 | 4XX, 5XX                        | \*/\*                           |

## getValidatedOrderById

Validates and returns order by Id. IMPORTANT - validation is time-consuming operation!

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.nftSales.getValidatedOrderById({
    id: "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
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
import { nftSalesGetValidatedOrderById } from "@rarible/protocol-mcp/funcs/nftSalesGetValidatedOrderById.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const res = await nftSalesGetValidatedOrderById(raribleProtocolMcp, {
    id: "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
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
| `request`                                                                                                                                                                      | [operations.GetValidatedOrderByIdRequest](../../models/operations/getvalidatedorderbyidrequest.md)                                                                             | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.Order](../../models/order.md)\>**

### Errors

| Error Type                         | Status Code                        | Content Type                       |
| ---------------------------------- | ---------------------------------- | ---------------------------------- |
| errors.UnionApiErrorBadRequest     | 400                                | application/json                   |
| errors.UnionApiErrorEntityNotFound | 404                                | application/json                   |
| errors.UnionApiErrorServerError    | 500                                | application/json                   |
| errors.APIError                    | 4XX, 5XX                           | \*/\*                              |

## getOrdersByIds

Returns Orders by specified list of Ids

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.nftSales.getOrdersByIds({
    ids: [
      "<value 1>",
    ],
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
import { nftSalesGetOrdersByIds } from "@rarible/protocol-mcp/funcs/nftSalesGetOrdersByIds.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const res = await nftSalesGetOrdersByIds(raribleProtocolMcp, {
    ids: [
      "<value 1>",
    ],
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
| `request`                                                                                                                                                                      | [models.OrderIds](../../models/orderids.md)                                                                                                                                    | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.Orders](../../models/orders.md)\>**

### Errors

| Error Type                      | Status Code                     | Content Type                    |
| ------------------------------- | ------------------------------- | ------------------------------- |
| errors.UnionApiErrorBadRequest  | 400                             | application/json                |
| errors.UnionApiErrorServerError | 500                             | application/json                |
| errors.APIError                 | 4XX, 5XX                        | \*/\*                           |

## getOrdersAll

Returns all Orders in accordance with specified filters and sorted by `last updated` date

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.nftSales.getOrdersAll({
    blockchains: [
      "ETHEREUM",
    ],
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
import { nftSalesGetOrdersAll } from "@rarible/protocol-mcp/funcs/nftSalesGetOrdersAll.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const res = await nftSalesGetOrdersAll(raribleProtocolMcp, {
    blockchains: [
      "ETHEREUM",
    ],
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
| `request`                                                                                                                                                                      | [operations.GetOrdersAllRequest](../../models/operations/getordersallrequest.md)                                                                                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.Orders](../../models/orders.md)\>**

### Errors

| Error Type                      | Status Code                     | Content Type                    |
| ------------------------------- | ------------------------------- | ------------------------------- |
| errors.UnionApiErrorBadRequest  | 400                             | application/json                |
| errors.UnionApiErrorServerError | 500                             | application/json                |
| errors.APIError                 | 4XX, 5XX                        | \*/\*                           |

## getAllSync

Returns all sales & transfers in accordance with specified filters and sorted by `db updated` date. During internal updates (like migrations) Orders can be updated for technical reasons. In such case, `last update` date won't be changed. If you want to store Orders in your own storage and keep it synced, use this method.

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.nftSales.getAllSync({
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
import { nftSalesGetAllSync } from "@rarible/protocol-mcp/funcs/nftSalesGetAllSync.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const res = await nftSalesGetAllSync(raribleProtocolMcp, {
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
| `request`                                                                                                                                                                      | [operations.GetAllSyncRequest](../../models/operations/getallsyncrequest.md)                                                                                                   | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.Orders](../../models/orders.md)\>**

### Errors

| Error Type                      | Status Code                     | Content Type                    |
| ------------------------------- | ------------------------------- | ------------------------------- |
| errors.UnionApiErrorBadRequest  | 400                             | application/json                |
| errors.UnionApiErrorServerError | 500                             | application/json                |
| errors.APIError                 | 4XX, 5XX                        | \*/\*                           |

## getSellOrdersByMaker

Returns sell NFT Sales created by specified user and sorted by `last update` date

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.nftSales.getSellOrdersByMaker({
    blockchains: [
      "ETHEREUM",
    ],
    maker: [
      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    ],
    collection: [
      "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
    ],
    origin: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
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
import { nftSalesGetSellOrdersByMaker } from "@rarible/protocol-mcp/funcs/nftSalesGetSellOrdersByMaker.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const res = await nftSalesGetSellOrdersByMaker(raribleProtocolMcp, {
    blockchains: [
      "ETHEREUM",
    ],
    maker: [
      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    ],
    collection: [
      "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
    ],
    origin: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
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
| `request`                                                                                                                                                                      | [operations.GetSellOrdersByMakerRequest](../../models/operations/getsellordersbymakerrequest.md)                                                                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.Orders](../../models/orders.md)\>**

### Errors

| Error Type                      | Status Code                     | Content Type                    |
| ------------------------------- | ------------------------------- | ------------------------------- |
| errors.UnionApiErrorBadRequest  | 400                             | application/json                |
| errors.UnionApiErrorServerError | 500                             | application/json                |
| errors.APIError                 | 4XX, 5XX                        | \*/\*                           |

## getSellOrdersByItem

Returns sell sales & transfer created for specified NFT and sorted by price in USD (cheapest first)

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.nftSales.getSellOrdersByItem({
    itemId: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
    maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    origin: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
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
import { nftSalesGetSellOrdersByItem } from "@rarible/protocol-mcp/funcs/nftSalesGetSellOrdersByItem.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const res = await nftSalesGetSellOrdersByItem(raribleProtocolMcp, {
    itemId: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
    maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    origin: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
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
| `request`                                                                                                                                                                      | [operations.GetSellOrdersByItemRequest](../../models/operations/getsellordersbyitemrequest.md)                                                                                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.Orders](../../models/orders.md)\>**

### Errors

| Error Type                      | Status Code                     | Content Type                    |
| ------------------------------- | ------------------------------- | ------------------------------- |
| errors.UnionApiErrorBadRequest  | 400                             | application/json                |
| errors.UnionApiErrorServerError | 500                             | application/json                |
| errors.APIError                 | 4XX, 5XX                        | \*/\*                           |

## getSellOrders

Returns sell Orders satisfying specified filters and sorted by `last update` date

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.nftSales.getSellOrders({
    blockchains: [
      "ETHEREUM",
    ],
    origin: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
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
import { nftSalesGetSellOrders } from "@rarible/protocol-mcp/funcs/nftSalesGetSellOrders.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const res = await nftSalesGetSellOrders(raribleProtocolMcp, {
    blockchains: [
      "ETHEREUM",
    ],
    origin: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
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
| `request`                                                                                                                                                                      | [operations.GetSellOrdersRequest](../../models/operations/getsellordersrequest.md)                                                                                             | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.Orders](../../models/orders.md)\>**

### Errors

| Error Type                      | Status Code                     | Content Type                    |
| ------------------------------- | ------------------------------- | ------------------------------- |
| errors.UnionApiErrorBadRequest  | 400                             | application/json                |
| errors.UnionApiErrorServerError | 500                             | application/json                |
| errors.APIError                 | 4XX, 5XX                        | \*/\*                           |

## getOrderBidsByMaker

Returns bid Orders created by specified user and sorted by `last update` date

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.nftSales.getOrderBidsByMaker({
    maker: [
      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    ],
    blockchains: [
      "ETHEREUM",
    ],
    collection: [
      "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
    ],
    origin: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    currencies: [
      "ETHEREUM:0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2",
    ],
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
import { nftSalesGetOrderBidsByMaker } from "@rarible/protocol-mcp/funcs/nftSalesGetOrderBidsByMaker.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const res = await nftSalesGetOrderBidsByMaker(raribleProtocolMcp, {
    maker: [
      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    ],
    blockchains: [
      "ETHEREUM",
    ],
    collection: [
      "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
    ],
    origin: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    currencies: [
      "ETHEREUM:0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2",
    ],
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
| `request`                                                                                                                                                                      | [operations.GetOrderBidsByMakerRequest](../../models/operations/getorderbidsbymakerrequest.md)                                                                                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.Orders](../../models/orders.md)\>**

### Errors

| Error Type                      | Status Code                     | Content Type                    |
| ------------------------------- | ------------------------------- | ------------------------------- |
| errors.UnionApiErrorBadRequest  | 400                             | application/json                |
| errors.UnionApiErrorServerError | 500                             | application/json                |
| errors.APIError                 | 4XX, 5XX                        | \*/\*                           |

## getOrderBidsByItem

Returns bid Orders created for specified NFT and sorted by price in USD (expensive first)

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.nftSales.getOrderBidsByItem({
    itemId: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
    maker: [
      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    ],
    origin: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    currencies: [
      "ETHEREUM:0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2",
    ],
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
import { nftSalesGetOrderBidsByItem } from "@rarible/protocol-mcp/funcs/nftSalesGetOrderBidsByItem.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const res = await nftSalesGetOrderBidsByItem(raribleProtocolMcp, {
    itemId: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
    maker: [
      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    ],
    origin: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    currencies: [
      "ETHEREUM:0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2",
    ],
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
| `request`                                                                                                                                                                      | [operations.GetOrderBidsByItemRequest](../../models/operations/getorderbidsbyitemrequest.md)                                                                                   | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.Orders](../../models/orders.md)\>**

### Errors

| Error Type                      | Status Code                     | Content Type                    |
| ------------------------------- | ------------------------------- | ------------------------------- |
| errors.UnionApiErrorBadRequest  | 400                             | application/json                |
| errors.UnionApiErrorServerError | 500                             | application/json                |
| errors.APIError                 | 4XX, 5XX                        | \*/\*                           |

## getOrderFloorBidsByCollection

Returns floor bids created for specified NFT Collection and sorted by price in USD (expensive first)

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.nftSales.getOrderFloorBidsByCollection({
    collectionId: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
    origin: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    currencies: [
      "ETHEREUM:0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2",
    ],
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
import { nftSalesGetOrderFloorBidsByCollection } from "@rarible/protocol-mcp/funcs/nftSalesGetOrderFloorBidsByCollection.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const res = await nftSalesGetOrderFloorBidsByCollection(raribleProtocolMcp, {
    collectionId: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
    origin: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    currencies: [
      "ETHEREUM:0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2",
    ],
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
| `request`                                                                                                                                                                      | [operations.GetOrderFloorBidsByCollectionRequest](../../models/operations/getorderfloorbidsbycollectionrequest.md)                                                             | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.Orders](../../models/orders.md)\>**

### Errors

| Error Type                      | Status Code                     | Content Type                    |
| ------------------------------- | ------------------------------- | ------------------------------- |
| errors.UnionApiErrorBadRequest  | 400                             | application/json                |
| errors.UnionApiErrorServerError | 500                             | application/json                |
| errors.APIError                 | 4XX, 5XX                        | \*/\*                           |

## getOrderFees

Returns Protocol fee settings for Orders

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.nftSales.getOrderFees({
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
import { nftSalesGetOrderFees } from "@rarible/protocol-mcp/funcs/nftSalesGetOrderFees.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const res = await nftSalesGetOrderFees(raribleProtocolMcp, {
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
| `request`                                                                                                                                                                      | [operations.GetOrderFeesRequest](../../models/operations/getorderfeesrequest.md)                                                                                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.OrderFees](../../models/orderfees.md)\>**

### Errors

| Error Type                      | Status Code                     | Content Type                    |
| ------------------------------- | ------------------------------- | ------------------------------- |
| errors.UnionApiErrorBadRequest  | 400                             | application/json                |
| errors.UnionApiErrorServerError | 500                             | application/json                |
| errors.APIError                 | 4XX, 5XX                        | \*/\*                           |