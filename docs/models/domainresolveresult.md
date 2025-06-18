# DomainResolveResult

## Example Usage

```typescript
import { DomainResolveResult } from "@rarible/protocol-mcp";

let value: DomainResolveResult = {
  blockchain: "ETHEREUM",
  registrant: "<value>",
};
```

## Fields

| Field                                        | Type                                         | Required                                     | Description                                  | Example                                      |
| -------------------------------------------- | -------------------------------------------- | -------------------------------------------- | -------------------------------------------- | -------------------------------------------- |
| `blockchain`                                 | [models.Blockchain](../models/blockchain.md) | :heavy_check_mark:                           | N/A                                          | ETHEREUM                                     |
| `registrant`                                 | *string*                                     | :heavy_check_mark:                           | Resolved domain value                        |                                              |