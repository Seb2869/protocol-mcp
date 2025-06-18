# OlapPeriod

Period:
  * `MIN5` - Last 5 minutes
  * `MIN30` - Last 30 minutes
  * `H1` - Last 1 hour
  * `H6` - Last 6 hours
  * `D1` - Last 1 day
  * `D7` - Last 7 days
  * `D30` - Last 30 days
  * `D180` - Last 180 days (roughly 6 months)
  * `D365` - Last 365 days (roughly 1 year)
  * `ALL` - For all time


## Example Usage

```typescript
import { OlapPeriod } from "@rarible/protocol-mcp";

let value: OlapPeriod = "MIN5";
```

## Values

```typescript
"MIN5" | "MIN30" | "H1" | "H6" | "D1" | "D7" | "D30" | "D180" | "D365" | "ALL"
```