# GetCollectionStatsRequest

## Example Usage

```typescript
import { GetCollectionStatsRequest } from "@rarible/protocol-mcp/models/operations";

let value: GetCollectionStatsRequest = {
  collection: "<value>",
};
```

## Fields

| Field                                                       | Type                                                        | Required                                                    | Description                                                 |
| ----------------------------------------------------------- | ----------------------------------------------------------- | ----------------------------------------------------------- | ----------------------------------------------------------- |
| `collection`                                                | *string*                                                    | :heavy_check_mark:                                          | Identifier of collection                                    |
| `currency`                                                  | [models.OlapCurrencyType](../../models/olapcurrencytype.md) | :heavy_minus_sign:                                          | Currency of statistics                                      |