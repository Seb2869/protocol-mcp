# GetPeriodCollectionStatisticsRequest

## Example Usage

```typescript
import { GetPeriodCollectionStatisticsRequest } from "@rarible/protocol-mcp/models/operations";

let value: GetPeriodCollectionStatisticsRequest = {
  id: "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8",
  period: "H6",
};
```

## Fields

| Field                                               | Type                                                | Required                                            | Description                                         | Example                                             |
| --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- |
| `id`                                                | *string*                                            | :heavy_check_mark:                                  | Collection ID                                       | ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8 |
| `period`                                            | [models.OlapPeriod](../../models/olapperiod.md)     | :heavy_check_mark:                                  | Time period for aggregation                         |                                                     |