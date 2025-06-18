# EthOrderDataRaribleV2DataV1

## Example Usage

```typescript
import { EthOrderDataRaribleV2DataV1 } from "@rarible/protocol-mcp";

let value: EthOrderDataRaribleV2DataV1 = {
  atType: "ETH_RARIBLE_V2",
  payouts: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 109944,
    },
  ],
  originFees: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 858441,
    },
  ],
};
```

## Fields

| Field                                                                                      | Type                                                                                       | Required                                                                                   | Description                                                                                |
| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| `atType`                                                                                   | [models.EthOrderDataRaribleV2DataV1AtType](../models/ethorderdatarariblev2datav1attype.md) | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `payouts`                                                                                  | [models.Payout](../models/payout.md)[]                                                     | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `originFees`                                                                               | [models.Payout](../models/payout.md)[]                                                     | :heavy_check_mark:                                                                         | N/A                                                                                        |