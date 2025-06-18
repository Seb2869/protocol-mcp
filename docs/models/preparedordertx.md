# PreparedOrderTx

## Example Usage

```typescript
import { PreparedOrderTx } from "@rarible/protocol-mcp";

let value: PreparedOrderTx = {
  to: "ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430",
  data: "<value>",
};
```

## Fields

| Field                                                           | Type                                                            | Required                                                        | Description                                                     | Example                                                         |
| --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- |
| `to`                                                            | *string*                                                        | :heavy_check_mark:                                              | Blockchain contract address in Union format `ETHEREUM:${token}` | ETHEREUM:0xd07dc4262bcdbf85190c01c996b4c06a461d2430             |
| `data`                                                          | *string*                                                        | :heavy_check_mark:                                              | N/A                                                             |                                                                 |