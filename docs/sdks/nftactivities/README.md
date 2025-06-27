# NFTActivities
(*nftActivities*)

## Overview

### Available Operations

* [~~getActivitiesByUser~~](#getactivitiesbyuser) - Get user Activities :warning: **Deprecated**
* [~~getActivitiesByUsers~~](#getactivitiesbyusers) - Get users Activities :warning: **Deprecated**
* [~~getActivitiesByItem~~](#getactivitiesbyitem) - Get NFT Activities :warning: **Deprecated**
* [~~getActivitiesByCollection~~](#getactivitiesbycollection) - Get NFT Collection Activities :warning: **Deprecated**
* [getAllActivitiesSync](#getallactivitiessync) - Get all Activities (for sync)
* [~~getAllActivities~~](#getallactivities) - Get all Activities :warning: **Deprecated**
* [getSalesChart](#getsaleschart) - Get sales chart

## ~~getActivitiesByUser~~

Returns user's Activities (like transfers, mints, sells etc) sorted by date. This API is deprecated in favor of `Search Activities`

> :warning: **DEPRECATED**: This will be removed in a future release, please migrate away from it as soon as possible.

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.nftActivities.getActivitiesByUser({
    type: [
      "BURN",
      "BRIDGE_TO",
    ],
    blockchains: [
      "ETHEREUM",
    ],
    user: [
      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    ],
    bidCurrencies: [
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
import { nftActivitiesGetActivitiesByUser } from "@rarible/protocol-mcp/funcs/nftActivitiesGetActivitiesByUser.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const res = await nftActivitiesGetActivitiesByUser(raribleProtocolMcp, {
    type: [
      "BURN",
      "BRIDGE_TO",
    ],
    blockchains: [
      "ETHEREUM",
    ],
    user: [
      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    ],
    bidCurrencies: [
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
| `request`                                                                                                                                                                      | [operations.GetActivitiesByUserRequest](../../models/operations/getactivitiesbyuserrequest.md)                                                                                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.Activities](../../models/activities.md)\>**

### Errors

| Error Type                      | Status Code                     | Content Type                    |
| ------------------------------- | ------------------------------- | ------------------------------- |
| errors.UnionApiErrorBadRequest  | 400                             | application/json                |
| errors.UnionApiErrorServerError | 500                             | application/json                |
| errors.APIError                 | 4XX, 5XX                        | \*/\*                           |

## ~~getActivitiesByUsers~~

Returns users Activities (like transfers, mints, sells etc) sorted by date. This API is deprecated in favor of `Search Activities`

> :warning: **DEPRECATED**: This will be removed in a future release, please migrate away from it as soon as possible.

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.nftActivities.getActivitiesByUsers({
    types: [],
    users: [
      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    ],
    bidCurrencies: [
      "ETHEREUM:0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2",
    ],
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
import { nftActivitiesGetActivitiesByUsers } from "@rarible/protocol-mcp/funcs/nftActivitiesGetActivitiesByUsers.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const res = await nftActivitiesGetActivitiesByUsers(raribleProtocolMcp, {
    types: [],
    users: [
      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    ],
    bidCurrencies: [
      "ETHEREUM:0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2",
    ],
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
| `request`                                                                                                                                                                      | [models.ActivitiesByUsersRequest](../../models/activitiesbyusersrequest.md)                                                                                                    | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.Activities](../../models/activities.md)\>**

### Errors

| Error Type                      | Status Code                     | Content Type                    |
| ------------------------------- | ------------------------------- | ------------------------------- |
| errors.UnionApiErrorBadRequest  | 400                             | application/json                |
| errors.UnionApiErrorServerError | 500                             | application/json                |
| errors.APIError                 | 4XX, 5XX                        | \*/\*                           |

## ~~getActivitiesByItem~~

Returns Activities related to specified NFT and sorted by date. This API is deprecated in favor of `Search Activities`

> :warning: **DEPRECATED**: This will be removed in a future release, please migrate away from it as soon as possible.

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.nftActivities.getActivitiesByItem({
    type: [
      "MINT",
      "BRIDGE_TO",
    ],
    itemId: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
    bidCurrencies: [
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
import { nftActivitiesGetActivitiesByItem } from "@rarible/protocol-mcp/funcs/nftActivitiesGetActivitiesByItem.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const res = await nftActivitiesGetActivitiesByItem(raribleProtocolMcp, {
    type: [
      "MINT",
      "BRIDGE_TO",
    ],
    itemId: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
    bidCurrencies: [
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
| `request`                                                                                                                                                                      | [operations.GetActivitiesByItemRequest](../../models/operations/getactivitiesbyitemrequest.md)                                                                                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.Activities](../../models/activities.md)\>**

### Errors

| Error Type                      | Status Code                     | Content Type                    |
| ------------------------------- | ------------------------------- | ------------------------------- |
| errors.UnionApiErrorBadRequest  | 400                             | application/json                |
| errors.UnionApiErrorServerError | 500                             | application/json                |
| errors.APIError                 | 4XX, 5XX                        | \*/\*                           |

## ~~getActivitiesByCollection~~

Returns Activities related to NFTs from specified Collection and sorted by date. This API is deprecated in favor of `Search Activities`

> :warning: **DEPRECATED**: This will be removed in a future release, please migrate away from it as soon as possible.

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.nftActivities.getActivitiesByCollection({
    type: [],
    collection: [
      "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
    ],
    bidCurrencies: [
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
import { nftActivitiesGetActivitiesByCollection } from "@rarible/protocol-mcp/funcs/nftActivitiesGetActivitiesByCollection.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const res = await nftActivitiesGetActivitiesByCollection(raribleProtocolMcp, {
    type: [],
    collection: [
      "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
    ],
    bidCurrencies: [
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
| `request`                                                                                                                                                                      | [operations.GetActivitiesByCollectionRequest](../../models/operations/getactivitiesbycollectionrequest.md)                                                                     | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.Activities](../../models/activities.md)\>**

### Errors

| Error Type                      | Status Code                     | Content Type                    |
| ------------------------------- | ------------------------------- | ------------------------------- |
| errors.UnionApiErrorBadRequest  | 400                             | application/json                |
| errors.UnionApiErrorServerError | 500                             | application/json                |
| errors.APIError                 | 4XX, 5XX                        | \*/\*                           |

## getAllActivitiesSync

Returns all Activities in accordance with specified filters and sorted by `db updated` date. During internal updates (like migrations) Activities can be updated for technical reasons. In such case, `date` field won't be changed. If you want to store Activities in your own storage and keep it synced, use this method.

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.nftActivities.getAllActivitiesSync({
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
import { nftActivitiesGetAllActivitiesSync } from "@rarible/protocol-mcp/funcs/nftActivitiesGetAllActivitiesSync.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const res = await nftActivitiesGetAllActivitiesSync(raribleProtocolMcp, {
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
| `request`                                                                                                                                                                      | [operations.GetAllActivitiesSyncRequest](../../models/operations/getallactivitiessyncrequest.md)                                                                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.Activities](../../models/activities.md)\>**

### Errors

| Error Type                      | Status Code                     | Content Type                    |
| ------------------------------- | ------------------------------- | ------------------------------- |
| errors.UnionApiErrorBadRequest  | 400                             | application/json                |
| errors.UnionApiErrorServerError | 500                             | application/json                |
| errors.APIError                 | 4XX, 5XX                        | \*/\*                           |

## ~~getAllActivities~~

Returns all Activities in accordance with specified filters and sorted by date. This API is deprecated in favor of `Search Activities`

> :warning: **DEPRECATED**: This will be removed in a future release, please migrate away from it as soon as possible.

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.nftActivities.getAllActivities({
    blockchains: [
      "ETHEREUM",
    ],
    type: [],
    bidCurrencies: [
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
import { nftActivitiesGetAllActivities } from "@rarible/protocol-mcp/funcs/nftActivitiesGetAllActivities.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const res = await nftActivitiesGetAllActivities(raribleProtocolMcp, {
    blockchains: [
      "ETHEREUM",
    ],
    type: [],
    bidCurrencies: [
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
| `request`                                                                                                                                                                      | [operations.GetAllActivitiesRequest](../../models/operations/getallactivitiesrequest.md)                                                                                       | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.Activities](../../models/activities.md)\>**

### Errors

| Error Type                      | Status Code                     | Content Type                    |
| ------------------------------- | ------------------------------- | ------------------------------- |
| errors.UnionApiErrorBadRequest  | 400                             | application/json                |
| errors.UnionApiErrorServerError | 500                             | application/json                |
| errors.APIError                 | 4XX, 5XX                        | \*/\*                           |

## getSalesChart

Returns list of sales by collection

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.nftActivities.getSalesChart({
    id: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
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
import { nftActivitiesGetSalesChart } from "@rarible/protocol-mcp/funcs/nftActivitiesGetSalesChart.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const res = await nftActivitiesGetSalesChart(raribleProtocolMcp, {
    id: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
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
| `request`                                                                                                                                                                      | [operations.GetSalesChartRequest](../../models/operations/getsaleschartrequest.md)                                                                                             | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.SalesChart](../../models/saleschart.md)\>**

### Errors

| Error Type                      | Status Code                     | Content Type                    |
| ------------------------------- | ------------------------------- | ------------------------------- |
| errors.UnionApiErrorBadRequest  | 400                             | application/json                |
| errors.UnionApiErrorServerError | 500                             | application/json                |
| errors.APIError                 | 4XX, 5XX                        | \*/\*                           |