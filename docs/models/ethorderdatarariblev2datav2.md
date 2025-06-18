# EthOrderDataRaribleV2DataV2

## Example Usage

```typescript
import { EthOrderDataRaribleV2DataV2 } from "@rarible/protocol-mcp";

let value: EthOrderDataRaribleV2DataV2 = {
  atType: "ETH_RARIBLE_V2_2",
  payouts: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 259791,
    },
  ],
  originFees: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 257986,
    },
  ],
  isMakeFill: false,
};
```

## Fields

| Field                                                                                          | Type                                                                                           | Required                                                                                       | Description                                                                                    |
| ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| `atType`                                                                                       | [models.EthOrderDataRaribleV2DataV2AtType](../models/ethorderdatarariblev2datav2attype.md)     | :heavy_check_mark:                                                                             | N/A                                                                                            |
| `payouts`                                                                                      | [models.Payout](../models/payout.md)[]                                                         | :heavy_check_mark:                                                                             | N/A                                                                                            |
| `originFees`                                                                                   | [models.Payout](../models/payout.md)[]                                                         | :heavy_check_mark:                                                                             | N/A                                                                                            |
| `isMakeFill`                                                                                   | *boolean*                                                                                      | :heavy_check_mark:                                                                             | If true, the 'fill' part of the order applies to the 'make' side, otherwise to the 'take' side |