# PrepareOrderTxResponse

## Example Usage

```typescript
import { PrepareOrderTxResponse } from "@rarible/protocol-mcp";

let value: PrepareOrderTxResponse = {
  transferProxyAddress: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  asset: {
    type: {
      atType: "CURRENCY_TOKEN",
      contract: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
    },
    value: "123456.789",
  },
  transaction: {
    to: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
    data: "<value>",
  },
  value: "123456",
};
```

## Fields

| Field                                                           | Type                                                            | Required                                                        | Description                                                     | Example                                                         |
| --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- |
| `transferProxyAddress`                                          | *string*                                                        | :heavy_minus_sign:                                              | Blockchain contract address in Union format `ETHEREUM:${token}` | ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430             |
| `asset`                                                         | [models.Asset](../models/asset.md)                              | :heavy_check_mark:                                              | N/A                                                             |                                                                 |
| `transaction`                                                   | [models.PreparedOrderTx](../models/preparedordertx.md)          | :heavy_check_mark:                                              | N/A                                                             |                                                                 |
| `value`                                                         | *string*                                                        | :heavy_check_mark:                                              | N/A                                                             | 123456                                                          |