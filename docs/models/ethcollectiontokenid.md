# EthCollectionTokenId

## Example Usage

```typescript
import { EthCollectionTokenId } from "@rarible/protocol-mcp";

let value: EthCollectionTokenId = {
  atType: "ETHEREUM",
  signature: {
    v: 835981,
    r: "<value>",
    s: "<value>",
  },
  tokenId: "123456",
};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        | Example                                                                            |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `atType`                                                                           | [models.AtTypeEthereum](../models/attypeethereum.md)                               | :heavy_check_mark:                                                                 | N/A                                                                                |                                                                                    |
| `signature`                                                                        | [models.EthCollectionTokenIdSignature](../models/ethcollectiontokenidsignature.md) | :heavy_check_mark:                                                                 | N/A                                                                                |                                                                                    |
| `tokenId`                                                                          | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                | 123456                                                                             |