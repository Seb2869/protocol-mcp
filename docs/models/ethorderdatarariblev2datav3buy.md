# EthOrderDataRaribleV2DataV3Buy

## Example Usage

```typescript
import { EthOrderDataRaribleV2DataV3Buy } from "@rarible/protocol-mcp";

let value: EthOrderDataRaribleV2DataV3Buy = {
  atType: "ETH_RARIBLE_V2_DATA_V3_BUY",
  payout: {
    account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    value: 813374,
  },
  originFeeFirst: {
    account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    value: 302710,
  },
  originFeeSecond: {
    account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
    value: 304132,
  },
};
```

## Fields

| Field                                                                                            | Type                                                                                             | Required                                                                                         | Description                                                                                      |
| ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ |
| `atType`                                                                                         | [models.EthOrderDataRaribleV2DataV3BuyAtType](../models/ethorderdatarariblev2datav3buyattype.md) | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `payout`                                                                                         | [models.Payout](../models/payout.md)                                                             | :heavy_minus_sign:                                                                               | N/A                                                                                              |
| `originFeeFirst`                                                                                 | [models.Payout](../models/payout.md)                                                             | :heavy_minus_sign:                                                                               | N/A                                                                                              |
| `originFeeSecond`                                                                                | [models.Payout](../models/payout.md)                                                             | :heavy_minus_sign:                                                                               | N/A                                                                                              |
| `marketplaceMarker`                                                                              | *string*                                                                                         | :heavy_minus_sign:                                                                               | N/A                                                                                              |