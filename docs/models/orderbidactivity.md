# OrderBidActivity

## Example Usage

```typescript
import { OrderBidActivity } from "@rarible/protocol-mcp";

let value: OrderBidActivity = {
  atType: "BID",
  orderId:
    "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
  hash: "<value>",
  maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  make: {
    type: {
      atType: "CURRENCY_TOKEN",
      contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
    },
    value: "123456.789",
  },
  take: {
    type: {
      atType: "ETH",
      blockchain: "ETHEREUM",
    },
    value: "123456.789",
  },
  price: "123456.789",
  priceUsd: "123456.789",
  id: "ETHEREUM:${id}",
  date: new Date("2025-01-17T18:05:23.814Z"),
};
```

## Fields

| Field                                                                                         | Type                                                                                          | Required                                                                                      | Description                                                                                   | Example                                                                                       |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `atType`                                                                                      | [models.AtTypeBid](../models/attypebid.md)                                                    | :heavy_check_mark:                                                                            | N/A                                                                                           |                                                                                               |
| `orderId`                                                                                     | *string*                                                                                      | :heavy_minus_sign:                                                                            | N/A                                                                                           | ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143                   |
| `hash`                                                                                        | *string*                                                                                      | :heavy_check_mark:                                                                            | N/A                                                                                           |                                                                                               |
| `maker`                                                                                       | *string*                                                                                      | :heavy_check_mark:                                                                            | Blockchain address in Union format `${blockchainGroup}:${token}`                              | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb                                           |
| `make`                                                                                        | [models.Asset](../models/asset.md)                                                            | :heavy_check_mark:                                                                            | N/A                                                                                           |                                                                                               |
| `take`                                                                                        | [models.Asset](../models/asset.md)                                                            | :heavy_check_mark:                                                                            | N/A                                                                                           |                                                                                               |
| `price`                                                                                       | *string*                                                                                      | :heavy_check_mark:                                                                            | N/A                                                                                           | 123456.789                                                                                    |
| `priceUsd`                                                                                    | *string*                                                                                      | :heavy_minus_sign:                                                                            | N/A                                                                                           | 123456.789                                                                                    |
| `source`                                                                                      | [models.OrderActivitySource](../models/orderactivitysource.md)                                | :heavy_minus_sign:                                                                            | N/A                                                                                           |                                                                                               |
| `marketplaceMarker`                                                                           | *string*                                                                                      | :heavy_minus_sign:                                                                            | N/A                                                                                           |                                                                                               |
| `id`                                                                                          | *string*                                                                                      | :heavy_check_mark:                                                                            | N/A                                                                                           | ETHEREUM:${id}                                                                                |
| `date`                                                                                        | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) | :heavy_check_mark:                                                                            | N/A                                                                                           |                                                                                               |
| `lastUpdatedAt`                                                                               | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) | :heavy_minus_sign:                                                                            | N/A                                                                                           |                                                                                               |
| `cursor`                                                                                      | *string*                                                                                      | :heavy_minus_sign:                                                                            | N/A                                                                                           |                                                                                               |
| `reverted`                                                                                    | *boolean*                                                                                     | :heavy_minus_sign:                                                                            | N/A                                                                                           |                                                                                               |
| `version`                                                                                     | *number*                                                                                      | :heavy_minus_sign:                                                                            | N/A                                                                                           |                                                                                               |