# GetFloorPriceChartRequest

## Example Usage

```typescript
import { GetFloorPriceChartRequest } from "@rarible/protocol-mcp/models/operations";

let value: GetFloorPriceChartRequest = {
  id: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
  period: "D7",
  size: 136283,
};
```

## Fields

| Field                                                                                         | Type                                                                                          | Required                                                                                      | Description                                                                                   | Example                                                                                       |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `id`                                                                                          | *string*                                                                                      | :heavy_check_mark:                                                                            | Collection ID                                                                                 | ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8                                           |
| `period`                                                                                      | [models.OlapPeriod](../../models/olapperiod.md)                                               | :heavy_check_mark:                                                                            | Time period for aggregation                                                                   |                                                                                               |
| `size`                                                                                        | *number*                                                                                      | :heavy_check_mark:                                                                            | Number of data points to return                                                               |                                                                                               |
| `endTime`                                                                                     | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) | :heavy_minus_sign:                                                                            | Optionally, the date-time of the last point of the graph. Defaults to current time.           |                                                                                               |