# Charts
(*charts*)

## Overview

### Available Operations

* [getFloorPriceChart](#getfloorpricechart) - Get historical data of floor price for collection for charting purposes
* [getVolumeChart](#getvolumechart) - Get historical data of collection volume (total sales worth) for charting purposes

## getFloorPriceChart

Returns list of historical floor prices aggregated at even intervals in the specified time period - last day, last month etc.  Each points represents the aggregated value of the interval after it.  The last point represents the current floor price.

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLEPROTOCOLMCP_API_KEY_AUTH"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.charts.getFloorPriceChart({
    id: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
    period: "D30",
    size: 308023,
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
import { chartsGetFloorPriceChart } from "@rarible/protocol-mcp/funcs/chartsGetFloorPriceChart.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLEPROTOCOLMCP_API_KEY_AUTH"] ?? "",
});

async function run() {
  const res = await chartsGetFloorPriceChart(raribleProtocolMcp, {
    id: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
    period: "D30",
    size: 308023,
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
| `request`                                                                                                                                                                      | [operations.GetFloorPriceChartRequest](../../models/operations/getfloorpricechartrequest.md)                                                                                   | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.OlapChartResponse](../../models/olapchartresponse.md)\>**

### Errors

| Error Type       | Status Code      | Content Type     |
| ---------------- | ---------------- | ---------------- |
| errors.OlapError | 400, 404         | application/json |
| errors.OlapError | 500              | application/json |
| errors.APIError  | 4XX, 5XX         | \*/\*            |

## getVolumeChart

Given a time period and the desired number of points, returns points which represent total worth of collection sales in the interval after that point.  The last point always has no value.

### Example Usage

```typescript
import { RaribleProtocolMcp } from "@rarible/protocol-mcp";

const raribleProtocolMcp = new RaribleProtocolMcp({
  apiKeyAuth: process.env["RARIBLEPROTOCOLMCP_API_KEY_AUTH"] ?? "",
});

async function run() {
  const result = await raribleProtocolMcp.charts.getVolumeChart({
    id: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
    period: "MIN5",
    size: 440267,
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
import { chartsGetVolumeChart } from "@rarible/protocol-mcp/funcs/chartsGetVolumeChart.js";

// Use `RaribleProtocolMcpCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const raribleProtocolMcp = new RaribleProtocolMcpCore({
  apiKeyAuth: process.env["RARIBLEPROTOCOLMCP_API_KEY_AUTH"] ?? "",
});

async function run() {
  const res = await chartsGetVolumeChart(raribleProtocolMcp, {
    id: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
    period: "MIN5",
    size: 440267,
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
| `request`                                                                                                                                                                      | [operations.GetVolumeChartRequest](../../models/operations/getvolumechartrequest.md)                                                                                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.OlapChartResponse](../../models/olapchartresponse.md)\>**

### Errors

| Error Type       | Status Code      | Content Type     |
| ---------------- | ---------------- | ---------------- |
| errors.OlapError | 400, 404         | application/json |
| errors.OlapError | 500              | application/json |
| errors.APIError  | 4XX, 5XX         | \*/\*            |