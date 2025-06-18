# OlapBidsByPriceStatistics

## Example Usage

```typescript
import { OlapBidsByPriceStatistics } from "@rarible/protocol-mcp";

let value: OlapBidsByPriceStatistics = {
  maxVolumeNative: 5082.66,
  prices: [
    {
      price: 246.61,
      bidsCount: 34243,
      volumeNative: 2464.96,
      buyersCount: 763044,
      buyer: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    },
  ],
};
```

## Fields

| Field                                                    | Type                                                     | Required                                                 | Description                                              |
| -------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------- |
| `maxVolumeNative`                                        | *number*                                                 | :heavy_check_mark:                                       | N/A                                                      |
| `prices`                                                 | [models.OlapBidsByPrice](../models/olapbidsbyprice.md)[] | :heavy_check_mark:                                       | N/A                                                      |
| `continuation`                                           | *string*                                                 | :heavy_minus_sign:                                       | Continuation token to paginate result                    |