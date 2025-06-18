# ItemLastSale

## Example Usage

```typescript
import { ItemLastSale } from "@rarible/protocol-mcp";

let value: ItemLastSale = {
  date: new Date("2023-04-15T14:26:37.378Z"),
  seller: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  buyer: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
  value: "123456.789",
  currency: {
    atType: "ETH",
    blockchain: "ETHEREUM",
  },
  price: "123456.789",
};
```

## Fields

| Field                                                                                         | Type                                                                                          | Required                                                                                      | Description                                                                                   | Example                                                                                       |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `date`                                                                                        | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) | :heavy_check_mark:                                                                            | N/A                                                                                           |                                                                                               |
| `seller`                                                                                      | *string*                                                                                      | :heavy_minus_sign:                                                                            | Blockchain address in Union format `${blockchainGroup}:${token}`                              | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb                                           |
| `buyer`                                                                                       | *string*                                                                                      | :heavy_minus_sign:                                                                            | Blockchain address in Union format `${blockchainGroup}:${token}`                              | ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb                                           |
| `value`                                                                                       | *string*                                                                                      | :heavy_check_mark:                                                                            | N/A                                                                                           | 123456.789                                                                                    |
| `currency`                                                                                    | *models.AssetType*                                                                            | :heavy_check_mark:                                                                            | N/A                                                                                           |                                                                                               |
| `price`                                                                                       | *string*                                                                                      | :heavy_check_mark:                                                                            | N/A                                                                                           | 123456.789                                                                                    |