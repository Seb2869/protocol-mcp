# PrepareOrderTxForm

## Example Usage

```typescript
import { PrepareOrderTxForm } from "@rarible/protocol-mcp";

let value: PrepareOrderTxForm = {
  maker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  taker: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  amount: "123456",
  payouts: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 834638,
    },
  ],
  originFees: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 361243,
    },
  ],
};
```

## Fields

| Field                                                            | Type                                                             | Required                                                         | Description                                                      | Example                                                          |
| ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- |
| `maker`                                                          | *string*                                                         | :heavy_check_mark:                                               | Blockchain address in Union format `${blockchainGroup}:${token}` | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb              |
| `taker`                                                          | *string*                                                         | :heavy_minus_sign:                                               | Blockchain address in Union format `${blockchainGroup}:${token}` | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb              |
| `amount`                                                         | *string*                                                         | :heavy_check_mark:                                               | N/A                                                              | 123456                                                           |
| `payouts`                                                        | [models.Payout](../models/payout.md)[]                           | :heavy_check_mark:                                               | Value of the payouts for the order                               |                                                                  |
| `originFees`                                                     | [models.Payout](../models/payout.md)[]                           | :heavy_check_mark:                                               | Value of the origin fees for the order                           |                                                                  |