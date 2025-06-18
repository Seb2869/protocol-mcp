# EthOrderDataRaribleV2DataV3

## Example Usage

```typescript
import { EthOrderDataRaribleV2DataV3 } from "@rarible/protocol-mcp";

let value: EthOrderDataRaribleV2DataV3 = {
  atType: "ETH_RARIBLE_V2_3",
  payouts: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 469816,
    },
  ],
  originFees: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 889852,
    },
  ],
  isMakeFill: false,
};
```

## Fields

| Field                                                                                          | Type                                                                                           | Required                                                                                       | Description                                                                                    |
| ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| `atType`                                                                                       | [models.EthOrderDataRaribleV2DataV3AtType](../models/ethorderdatarariblev2datav3attype.md)     | :heavy_check_mark:                                                                             | N/A                                                                                            |
| `payouts`                                                                                      | [models.Payout](../models/payout.md)[]                                                         | :heavy_check_mark:                                                                             | N/A                                                                                            |
| `originFees`                                                                                   | [models.Payout](../models/payout.md)[]                                                         | :heavy_check_mark:                                                                             | N/A                                                                                            |
| `isMakeFill`                                                                                   | *boolean*                                                                                      | :heavy_check_mark:                                                                             | If true, the 'fill' part of the order applies to the 'make' side, otherwise to the 'take' side |