# OrderMatchSwap

## Example Usage

```typescript
import { OrderMatchSwap } from "@rarible/protocol-mcp";

let value: OrderMatchSwap = {
  left: {
    maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    asset: {
      type: {
        atType: "GEN_ART",
        contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
        collection: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
      },
      value: "123456.789",
    },
  },
  right: {
    maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    asset: {
      type: {
        atType: "SOLANA_SOL",
      },
      value: "123456.789",
    },
  },
  orderId:
    "ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143",
  source: "CRYPTO_PUNKS",
  transactionHash: "<value>",
  id: "ETHEREUM:${id}",
  date: new Date("2025-10-03T07:34:54.127Z"),
};
```

## Fields

| Field                                                                                                                   | Type                                                                                                                    | Required                                                                                                                | Description                                                                                                             | Example                                                                                                                 |
| ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| `atType`                                                                                                                | [models.OrderMatchActivityAtType](../models/ordermatchactivityattype.md)                                                | :heavy_minus_sign:                                                                                                      | N/A                                                                                                                     |                                                                                                                         |
| `left`                                                                                                                  | [models.OrderActivityMatchSide](../models/orderactivitymatchside.md)                                                    | :heavy_check_mark:                                                                                                      | N/A                                                                                                                     |                                                                                                                         |
| `right`                                                                                                                 | [models.OrderActivityMatchSide](../models/orderactivitymatchside.md)                                                    | :heavy_check_mark:                                                                                                      | N/A                                                                                                                     |                                                                                                                         |
| `orderId`                                                                                                               | *string*                                                                                                                | :heavy_minus_sign:                                                                                                      | N/A                                                                                                                     | ETHEREUM:0x19f487016770542dc6137b06499a4f7b42c9580f12d85d6347964b03b7682143                                             |
| `source`                                                                                                                | [models.OrderActivitySource](../models/orderactivitysource.md)                                                          | :heavy_check_mark:                                                                                                      | N/A                                                                                                                     |                                                                                                                         |
| `transactionHash`                                                                                                       | *string*                                                                                                                | :heavy_check_mark:                                                                                                      | N/A                                                                                                                     |                                                                                                                         |
| ~~`blockchainInfo`~~                                                                                                    | [models.ActivityBlockchainInfo](../models/activityblockchaininfo.md)                                                    | :heavy_minus_sign:                                                                                                      | : warning: ** DEPRECATED **: This will be removed in a future release, please migrate away from it as soon as possible. |                                                                                                                         |
| `id`                                                                                                                    | *string*                                                                                                                | :heavy_check_mark:                                                                                                      | N/A                                                                                                                     | ETHEREUM:${id}                                                                                                          |
| `date`                                                                                                                  | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)                           | :heavy_check_mark:                                                                                                      | N/A                                                                                                                     |                                                                                                                         |
| `lastUpdatedAt`                                                                                                         | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)                           | :heavy_minus_sign:                                                                                                      | N/A                                                                                                                     |                                                                                                                         |
| `cursor`                                                                                                                | *string*                                                                                                                | :heavy_minus_sign:                                                                                                      | N/A                                                                                                                     |                                                                                                                         |
| `reverted`                                                                                                              | *boolean*                                                                                                               | :heavy_minus_sign:                                                                                                      | N/A                                                                                                                     |                                                                                                                         |
| `version`                                                                                                               | *number*                                                                                                                | :heavy_minus_sign:                                                                                                      | N/A                                                                                                                     |                                                                                                                         |