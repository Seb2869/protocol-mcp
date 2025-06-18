# GetGmvRequest

## Example Usage

```typescript
import { GetGmvRequest } from "@rarible/protocol-mcp/models/operations";

let value: GetGmvRequest = {
  collection: "<value>",
};
```

## Fields

| Field                                                       | Type                                                        | Required                                                    | Description                                                 |
| ----------------------------------------------------------- | ----------------------------------------------------------- | ----------------------------------------------------------- | ----------------------------------------------------------- |
| `collection`                                                | *string*                                                    | :heavy_check_mark:                                          | Identifier of collection                                    |
| `currency`                                                  | [models.OlapCurrencyType](../../models/olapcurrencytype.md) | :heavy_minus_sign:                                          | Currency of statistics                                      |
| `period`                                                    | [models.OlapPeriod](../../models/olapperiod.md)             | :heavy_minus_sign:                                          | Time period of statistics. Default: D1                      |
| `filters`                                                   | *string*                                                    | :heavy_minus_sign:                                          | Filters of statistics                                       |