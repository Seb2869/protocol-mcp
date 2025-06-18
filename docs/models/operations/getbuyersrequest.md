# GetBuyersRequest

## Example Usage

```typescript
import { GetBuyersRequest } from "@rarible/protocol-mcp/models/operations";

let value: GetBuyersRequest = {
  collection: "<value>",
};
```

## Fields

| Field                    | Type                     | Required                 | Description              |
| ------------------------ | ------------------------ | ------------------------ | ------------------------ |
| `collection`             | *string*                 | :heavy_check_mark:       | Identifier of collection |
| `filters`                | *string*                 | :heavy_minus_sign:       | Filters of statistics    |