# OlapGlobalCollectionStatisticsResponse

## Example Usage

```typescript
import { OlapGlobalCollectionStatisticsResponse } from "@rarible/protocol-mcp";

let value: OlapGlobalCollectionStatisticsResponse = {
  id: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
  listed: 252687,
  items: 19547,
  owners: 71824,
  volume: {
    currency: "Hong Kong Dollar",
    value: 2414.69,
  },
};
```

## Fields

| Field                                                    | Type                                                     | Required                                                 | Description                                              | Example                                                  |
| -------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------- |
| `id`                                                     | *string*                                                 | :heavy_minus_sign:                                       | Collection id                                            | ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8      |
| `listed`                                                 | *number*                                                 | :heavy_check_mark:                                       | N/A                                                      |                                                          |
| `items`                                                  | *number*                                                 | :heavy_check_mark:                                       | N/A                                                      |                                                          |
| `owners`                                                 | *number*                                                 | :heavy_check_mark:                                       | N/A                                                      |                                                          |
| `floor`                                                  | [models.OlapPriceWithUsd](../models/olappricewithusd.md) | :heavy_minus_sign:                                       | N/A                                                      |                                                          |
| `volume`                                                 | [models.OlapPriceWithUsd](../models/olappricewithusd.md) | :heavy_check_mark:                                       | N/A                                                      |                                                          |