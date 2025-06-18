# Structure

Collection structure can be described as:
- REGULAR: a standalone collection that has a corresponding contract address on the blockchain.
- COMPOSITE: an artificial collection that is composed of one or more regular collections or items.
- PART: an artificial collection that is a part of a larger regular collection, thus has a parent collection.


## Example Usage

```typescript
import { Structure } from "@rarible/protocol-mcp";

let value: Structure = "COMPOSITE";
```

## Values

```typescript
"REGULAR" | "COMPOSITE" | "PART"
```