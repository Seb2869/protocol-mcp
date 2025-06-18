# TraitsRarityRequest

Request rarity of the properties in the collection

## Example Usage

```typescript
import { TraitsRarityRequest } from "@rarible/protocol-mcp";

let value: TraitsRarityRequest = {
  collectionId: "ETHEREUM:0x60e4d786628fea6478f785a6d7e704777c86a7c6",
  properties: [
    {
      key: "Hat",
      value: "Halo",
    },
  ],
};
```

## Fields

| Field                                                | Type                                                 | Required                                             | Description                                          | Example                                              |
| ---------------------------------------------------- | ---------------------------------------------------- | ---------------------------------------------------- | ---------------------------------------------------- | ---------------------------------------------------- |
| `collectionId`                                       | *string*                                             | :heavy_check_mark:                                   | N/A                                                  | ETHEREUM:0x60e4d786628fea6478f785a6d7e704777c86a7c6  |
| `properties`                                         | [models.TraitProperty](../models/traitproperty.md)[] | :heavy_check_mark:                                   | N/A                                                  |                                                      |