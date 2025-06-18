# Currency

## Example Usage

```typescript
import { Currency } from "@rarible/protocol-mcp";

let value: Currency = {
  currencyId: "ETHEREUM:0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2",
  symbol: "<value>",
  rate: "123456.789",
  decimals: 374941,
};
```

## Fields

| Field                                                                         | Type                                                                          | Required                                                                      | Description                                                                   | Example                                                                       |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `currencyId`                                                                  | *string*                                                                      | :heavy_check_mark:                                                            | Currency Id, has format `ETHEREUM:${token}` or `ETHEREUM:${token}:${tokenId}` | ETHEREUM:0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2                           |
| `symbol`                                                                      | *string*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |                                                                               |
| `abbreviation`                                                                | *string*                                                                      | :heavy_minus_sign:                                                            | N/A                                                                           |                                                                               |
| `alias`                                                                       | *string*                                                                      | :heavy_minus_sign:                                                            | Alias to real coin, 'usd' means 1:1 to USD                                    |                                                                               |
| `rate`                                                                        | *string*                                                                      | :heavy_minus_sign:                                                            | N/A                                                                           | 123456.789                                                                    |
| `decimals`                                                                    | *number*                                                                      | :heavy_check_mark:                                                            | Number of decimals                                                            |                                                                               |