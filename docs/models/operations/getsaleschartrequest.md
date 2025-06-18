# GetSalesChartRequest

## Example Usage

```typescript
import { GetSalesChartRequest } from "@rarible/protocol-mcp/models/operations";

let value: GetSalesChartRequest = {
  id: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
};
```

## Fields

| Field                                                                                         | Type                                                                                          | Required                                                                                      | Description                                                                                   | Example                                                                                       |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `id`                                                                                          | *string*                                                                                      | :heavy_check_mark:                                                                            | Collection ID                                                                                 | ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8                                           |
| `from`                                                                                        | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) | :heavy_minus_sign:                                                                            | Time period from                                                                              |                                                                                               |
| `to`                                                                                          | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) | :heavy_minus_sign:                                                                            | Time period to                                                                                |                                                                                               |
| `size`                                                                                        | *number*                                                                                      | :heavy_minus_sign:                                                                            | Number of data points to return                                                               |                                                                                               |
| `cursor`                                                                                      | *string*                                                                                      | :heavy_minus_sign:                                                                            | Cursor from previous response                                                                 |                                                                                               |