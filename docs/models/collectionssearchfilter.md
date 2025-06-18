# CollectionsSearchFilter

Filter for collections search query

## Example Usage

```typescript
import { CollectionsSearchFilter } from "@rarible/protocol-mcp";

let value: CollectionsSearchFilter = {
  blockchains: [
    "ETHEREUM",
  ],
  text: "Apes",
};
```

## Fields

| Field                                          | Type                                           | Required                                       | Description                                    | Example                                        |
| ---------------------------------------------- | ---------------------------------------------- | ---------------------------------------------- | ---------------------------------------------- | ---------------------------------------------- |
| `blockchains`                                  | [models.Blockchain](../models/blockchain.md)[] | :heavy_minus_sign:                             | N/A                                            |                                                |
| `text`                                         | *string*                                       | :heavy_check_mark:                             | N/A                                            | Apes                                           |