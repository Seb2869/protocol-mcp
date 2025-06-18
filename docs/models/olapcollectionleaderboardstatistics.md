# OlapCollectionLeaderboardStatistics

## Example Usage

```typescript
import { OlapCollectionLeaderboardStatistics } from "@rarible/protocol-mcp";

let value: OlapCollectionLeaderboardStatistics = {
  listed: 731611,
  items: 129742,
  owners: 393218,
};
```

## Fields

| Field                                                    | Type                                                     | Required                                                 | Description                                              |
| -------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------- |
| `listed`                                                 | *number*                                                 | :heavy_check_mark:                                       | N/A                                                      |
| `items`                                                  | *number*                                                 | :heavy_check_mark:                                       | N/A                                                      |
| `owners`                                                 | *number*                                                 | :heavy_check_mark:                                       | N/A                                                      |
| `floor`                                                  | [models.OlapPriceWithUsd](../models/olappricewithusd.md) | :heavy_minus_sign:                                       | N/A                                                      |
| `topOffer`                                               | [models.OlapPriceWithUsd](../models/olappricewithusd.md) | :heavy_minus_sign:                                       | N/A                                                      |