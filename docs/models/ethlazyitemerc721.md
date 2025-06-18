# EthLazyItemErc721

## Example Usage

```typescript
import { EthLazyItemErc721 } from "@rarible/protocol-mcp";

let value: EthLazyItemErc721 = {
  atType: "ETH_ERC721",
  id:
    "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
  uri: "https://snarling-pliers.com/",
  creators: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 124635,
    },
  ],
  royalties: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 965740,
    },
  ],
  signatures: [
    "<value>",
  ],
};
```

## Fields

| Field                                                                                                                             | Type                                                                                                                              | Required                                                                                                                          | Description                                                                                                                       | Example                                                                                                                           |
| --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| `atType`                                                                                                                          | [models.AtTypeEthErc721](../models/attypeetherc721.md)                                                                            | :heavy_check_mark:                                                                                                                | N/A                                                                                                                               |                                                                                                                                   |
| `id`                                                                                                                              | *string*                                                                                                                          | :heavy_check_mark:                                                                                                                | Item Id, has format `ETHEREUM:${token}:${tokenId}`                                                                                | ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410 |
| `uri`                                                                                                                             | *string*                                                                                                                          | :heavy_check_mark:                                                                                                                | N/A                                                                                                                               |                                                                                                                                   |
| `creators`                                                                                                                        | [models.Creator](../models/creator.md)[]                                                                                          | :heavy_check_mark:                                                                                                                | Addresses of the NFT item creators                                                                                                |                                                                                                                                   |
| `royalties`                                                                                                                       | [models.Royalty](../models/royalty.md)[]                                                                                          | :heavy_check_mark:                                                                                                                | List of royalties                                                                                                                 |                                                                                                                                   |
| `signatures`                                                                                                                      | *string*[]                                                                                                                        | :heavy_check_mark:                                                                                                                | Digital signatures                                                                                                                |                                                                                                                                   |