# OlapStatsGraphResponse

## Example Usage

```typescript
import { OlapStatsGraphResponse } from "@rarible/protocol-mcp";

let value: OlapStatsGraphResponse = {
  historicalDates: [
    "<value>",
  ],
  historicalValues: [
    5587.95,
  ],
};
```

## Fields

| Field                           | Type                            | Required                        | Description                     |
| ------------------------------- | ------------------------------- | ------------------------------- | ------------------------------- |
| `historicalDates`               | *string*[]                      | :heavy_check_mark:              | Dates of historical statistics  |
| `historicalValues`              | *number*[]                      | :heavy_check_mark:              | Values of historical statistics |
| `currentValue`                  | *number*                        | :heavy_minus_sign:              | Current value                   |