# OlapHistoryValuesByTimestamps

## Example Usage

```typescript
import { OlapHistoryValuesByTimestamps } from "@rarible/protocol-mcp";

let value: OlapHistoryValuesByTimestamps = {
  timestamps: [
    909839,
  ],
  values: [
    9654.99,
  ],
};
```

## Fields

| Field                               | Type                                | Required                            | Description                         |
| ----------------------------------- | ----------------------------------- | ----------------------------------- | ----------------------------------- |
| `timestamps`                        | *number*[]                          | :heavy_check_mark:                  | Timestamps of historical statistics |
| `values`                            | *number*[]                          | :heavy_check_mark:                  | Values of historical statistics     |