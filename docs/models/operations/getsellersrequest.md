# GetSellersRequest

## Example Usage

```typescript
import { GetSellersRequest } from "@rarible/protocol-mcp/models/operations";

let value: GetSellersRequest = {
  collection: "<value>",
};
```

## Fields

| Field                    | Type                     | Required                 | Description              |
| ------------------------ | ------------------------ | ------------------------ | ------------------------ |
| `collection`             | *string*                 | :heavy_check_mark:       | Identifier of collection |
| `filters`                | *string*                 | :heavy_minus_sign:       | Filters of statistics    |