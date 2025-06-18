# OlapTradesLeaderboardSort

Sort order:
  * `VOLUME_USD_ASC` - sort by usd collection volume, ascending order
  * `VOLUME_USD_DESC` - sort by usd collection volume, descending order
  * `COLLECTION_ASC` - sort by collection id, ascending order
  * `COLLECTION_DESC` - sort by collection id, descending order


## Example Usage

```typescript
import { OlapTradesLeaderboardSort } from "@rarible/protocol-mcp";

let value: OlapTradesLeaderboardSort = "COLLECTION_DESC";
```

## Values

```typescript
"VOLUME_USD_ASC" | "VOLUME_USD_DESC" | "COLLECTION_ASC" | "COLLECTION_DESC"
```