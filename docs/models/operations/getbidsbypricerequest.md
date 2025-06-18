# GetBidsByPriceRequest

## Example Usage

```typescript
import { GetBidsByPriceRequest } from "@rarible/protocol-mcp/models/operations";

let value: GetBidsByPriceRequest = {
  id: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
};
```

## Fields

| Field                                                             | Type                                                              | Required                                                          | Description                                                       | Example                                                           |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| `id`                                                              | *string*                                                          | :heavy_check_mark:                                                | Collection ID                                                     | ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8               |
| `continuation`                                                    | *string*                                                          | :heavy_minus_sign:                                                | Continuation token from the previous response                     |                                                                   |
| `size`                                                            | *number*                                                          | :heavy_minus_sign:                                                | The number of results to return                                   |                                                                   |
| `sort`                                                            | [models.OlapBidsByPriceSort](../../models/olapbidsbypricesort.md) | :heavy_minus_sign:                                                | Result sorting                                                    |                                                                   |