# EthOrderDataRaribleV2DataV3Sell

## Example Usage

```typescript
import { EthOrderDataRaribleV2DataV3Sell } from "@rarible/protocol-mcp";

let value: EthOrderDataRaribleV2DataV3Sell = {
  atType: "ETH_RARIBLE_V2_DATA_V3_SELL",
  payout: {
    account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    value: 816593,
  },
  originFeeFirst: {
    account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    value: 323253,
  },
  originFeeSecond: {
    account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    value: 310340,
  },
  maxFeesBasePoint: 637774,
};
```

## Fields

| Field                                                                                              | Type                                                                                               | Required                                                                                           | Description                                                                                        |
| -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| `atType`                                                                                           | [models.EthOrderDataRaribleV2DataV3SellAtType](../models/ethorderdatarariblev2datav3sellattype.md) | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `payout`                                                                                           | [models.Payout](../models/payout.md)                                                               | :heavy_minus_sign:                                                                                 | N/A                                                                                                |
| `originFeeFirst`                                                                                   | [models.Payout](../models/payout.md)                                                               | :heavy_minus_sign:                                                                                 | N/A                                                                                                |
| `originFeeSecond`                                                                                  | [models.Payout](../models/payout.md)                                                               | :heavy_minus_sign:                                                                                 | N/A                                                                                                |
| `maxFeesBasePoint`                                                                                 | *number*                                                                                           | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `marketplaceMarker`                                                                                | *string*                                                                                           | :heavy_minus_sign:                                                                                 | N/A                                                                                                |