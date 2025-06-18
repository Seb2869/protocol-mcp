# Balance

## Example Usage

```typescript
import { Balance } from "@rarible/protocol-mcp";

let value: Balance = {
  currencyId: "ETHEREUM:0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2",
  owner: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  balance: "123456",
  decimal: "123456.789",
};
```

## Fields

| Field                                                                         | Type                                                                          | Required                                                                      | Description                                                                   | Example                                                                       |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `currencyId`                                                                  | *string*                                                                      | :heavy_check_mark:                                                            | Currency Id, has format `ETHEREUM:${token}` or `ETHEREUM:${token}:${tokenId}` | ETHEREUM:0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2                           |
| `owner`                                                                       | *string*                                                                      | :heavy_check_mark:                                                            | Blockchain address in Union format `${blockchainGroup}:${token}`              | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb                           |
| `balance`                                                                     | *string*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           | 123456                                                                        |
| `decimal`                                                                     | *string*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           | 123456.789                                                                    |