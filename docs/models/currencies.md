# Currencies

## Example Usage

```typescript
import { Currencies } from "@rarible/protocol-mcp";

let value: Currencies = {
  currencies: [
    {
      currencyId: "ETHEREUM:0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2",
      symbol: "<value>",
      rate: "123456.789",
      decimals: 240806,
    },
  ],
};
```

## Fields

| Field                                      | Type                                       | Required                                   | Description                                |
| ------------------------------------------ | ------------------------------------------ | ------------------------------------------ | ------------------------------------------ |
| `currencies`                               | [models.Currency](../models/currency.md)[] | :heavy_check_mark:                         | N/A                                        |