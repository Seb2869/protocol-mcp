# CollectionLeaderBoard
(*collectionLeaderBoard*)

## Overview

### Available Operations

* [getCollectionLeaderboard](#getcollectionleaderboard) - Get NFT Collections leaderboard
* [getCollectionLeaderboardByOwner](#getcollectionleaderboardbyowner) - Get NFT Collections leaderboard for a specific owner adresses

## getCollectionLeaderboard

Collections leaderboard

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.collectionLeaderBoard.getCollectionLeaderboard({});

  // Handle the result
  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { RaribleProtocolMcpCore } from "@rarible/protocol-mcp/core.js";
import { collectionLeaderBoardGetCollectionLeaderboard } from "@rarible/protocol-mcp/funcs/collectionLeaderBoardGetCollectionLeaderboard.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const res = await collectionLeaderBoardGetCollectionLeaderboard(raribleProtocolMcp, {});

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
| `request`                                                                                                                                                                      | [operations.GetCollectionLeaderboardRequest](../../models/operations/getcollectionleaderboardrequest.md)                                                                       | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.OlapCollectionLeaderboardResponse](../../models/olapcollectionleaderboardresponse.md)\>**

### Errors

| Error Type       | Status Code      | Content Type     |
| ---------------- | ---------------- | ---------------- |
| errors.OlapError | 400              | application/json |
| errors.OlapError | 500              | application/json |
| errors.APIError  | 4XX, 5XX         | \*/\*            |

## getCollectionLeaderboardByOwner

User collections leaderboard

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.collectionLeaderBoard.getCollectionLeaderboardByOwner({
    owners: [
      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
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
import { collectionLeaderBoardGetCollectionLeaderboardByOwner } from "@rarible/protocol-mcp/funcs/collectionLeaderBoardGetCollectionLeaderboardByOwner.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLE_API_KEY"] ?? "",
});

async function run() {
  const res = await collectionLeaderBoardGetCollectionLeaderboardByOwner(raribleProtocolMcp, {
    owners: [
      "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
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
| `request`                                                                                                                                                                      | [operations.GetCollectionLeaderboardByOwnerRequest](../../models/operations/getcollectionleaderboardbyownerrequest.md)                                                         | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.OlapCollectionLeaderboardResponse](../../models/olapcollectionleaderboardresponse.md)\>**

### Errors

| Error Type       | Status Code      | Content Type     |
| ---------------- | ---------------- | ---------------- |
| errors.OlapError | 400              | application/json |
| errors.OlapError | 500              | application/json |
| errors.APIError  | 4XX, 5XX         | \*/\*            |