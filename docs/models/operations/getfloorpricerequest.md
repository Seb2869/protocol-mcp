# GetFloorPriceRequest

## Example Usage

```typescript
import { GetFloorPriceRequest } from "@rarible/protocol-mcp/models/operations";

let value: GetFloorPriceRequest = {
  collection: "<value>",
};
```

## Fields

| Field                                                       | Type                                                        | Required                                                    | Description                                                 |
| ----------------------------------------------------------- | ----------------------------------------------------------- | ----------------------------------------------------------- | ----------------------------------------------------------- |
| `collection`                                                | *string*                                                    | :heavy_check_mark:                                          | Identifier of collection                                    |
| `currency`                                                  | [models.OlapCurrencyType](../../models/olapcurrencytype.md) | :heavy_minus_sign:                                          | Currency of statistics                                      |
| `filters`                                                   | *string*                                                    | :heavy_minus_sign:                                          | Filters of statistics                                       |