# ImmutablexOrderDataV1

## Example Usage

```typescript
import { ImmutablexOrderDataV1 } from "@rarible/protocol-mcp";

let value: ImmutablexOrderDataV1 = {
  atType: "IMMUTABLEX_RARIBLE_V1",
  payouts: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 370406,
    },
  ],
  originFees: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 910748,
    },
  ],
};
```

## Fields

| Field                                                                          | Type                                                                           | Required                                                                       | Description                                                                    |
| ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ |
| `atType`                                                                       | [models.ImmutablexOrderDataV1AtType](../models/immutablexorderdatav1attype.md) | :heavy_check_mark:                                                             | N/A                                                                            |
| `payouts`                                                                      | [models.Payout](../models/payout.md)[]                                         | :heavy_check_mark:                                                             | N/A                                                                            |
| `originFees`                                                                   | [models.Payout](../models/payout.md)[]                                         | :heavy_check_mark:                                                             | N/A                                                                            |