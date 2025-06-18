# OlapCurrencyAmountWithChange

## Example Usage

```typescript
import { OlapCurrencyAmountWithChange } from "@rarible/protocol-mcp";

let value: OlapCurrencyAmountWithChange = {
  value: 4102.36,
};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `currency`                                                                            | [models.OlapCurrencyType](../models/olapcurrencytype.md)                              | :heavy_minus_sign:                                                                    | N/A                                                                                   |
| `value`                                                                               | *number*                                                                              | :heavy_check_mark:                                                                    | Amount of currency                                                                    |
| `changePercent`                                                                       | *number*                                                                              | :heavy_minus_sign:                                                                    | Change in percent. Calculated as <current period value> / <previous period value> - 1 |