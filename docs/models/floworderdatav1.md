# FlowOrderDataV1

## Example Usage

```typescript
import { FlowOrderDataV1 } from "@rarible/protocol-mcp";

let value: FlowOrderDataV1 = {
  atType: "FLOW_RARIBLE_V1",
  payouts: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 236353,
    },
  ],
  originFees: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 543456,
    },
  ],
};
```

## Fields

| Field                                                              | Type                                                               | Required                                                           | Description                                                        |
| ------------------------------------------------------------------ | ------------------------------------------------------------------ | ------------------------------------------------------------------ | ------------------------------------------------------------------ |
| `atType`                                                           | [models.FlowOrderDataV1AtType](../models/floworderdatav1attype.md) | :heavy_check_mark:                                                 | N/A                                                                |
| `payouts`                                                          | [models.Payout](../models/payout.md)[]                             | :heavy_check_mark:                                                 | N/A                                                                |
| `originFees`                                                       | [models.Payout](../models/payout.md)[]                             | :heavy_check_mark:                                                 | N/A                                                                |