# GetTransactionsRequest

## Example Usage

```typescript
import { GetTransactionsRequest } from "@rarible/protocol-mcp/models/operations";

let value: GetTransactionsRequest = {
  collection: "<value>",
};
```

## Fields

| Field                    | Type                     | Required                 | Description              |
| ------------------------ | ------------------------ | ------------------------ | ------------------------ |
| `collection`             | *string*                 | :heavy_check_mark:       | Identifier of collection |
| `filters`                | *string*                 | :heavy_minus_sign:       | Filters of statistics    |