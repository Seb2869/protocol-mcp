# GetBalanceRequest

## Example Usage

```typescript
import { GetBalanceRequest } from "@rarible/protocol-mcp/models/operations";

let value: GetBalanceRequest = {
  currencyId: "ETHEREUM:0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2",
  owner: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
};
```

## Fields

| Field                                               | Type                                                | Required                                            | Description                                         | Example                                             |
| --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- |
| `currencyId`                                        | *string*                                            | :heavy_check_mark:                                  | N/A                                                 | ETHEREUM:0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2 |
| `owner`                                             | *string*                                            | :heavy_check_mark:                                  | Address of the token's owner                        | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb |