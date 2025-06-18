# EthLazyItemErc1155

## Example Usage

```typescript
import { EthLazyItemErc1155 } from "@rarible/protocol-mcp";

let value: EthLazyItemErc1155 = {
  atType: "ETH_ERC1155",
  supply: "123456",
  id:
    "ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410",
  uri: "https://meaty-instance.info",
  creators: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 411549,
    },
  ],
  royalties: [
    {
      account: "ETHEREUM:0x4765273c477c2dc484da4f1984639e943adccfeb",
      value: 834982,
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
| `atType`                                                                                                                          | [models.AtTypeEthErc1155](../models/attypeetherc1155.md)                                                                          | :heavy_check_mark:                                                                                                                | N/A                                                                                                                               |                                                                                                                                   |
| `supply`                                                                                                                          | *string*                                                                                                                          | :heavy_check_mark:                                                                                                                | N/A                                                                                                                               | 123456                                                                                                                            |
| `id`                                                                                                                              | *string*                                                                                                                          | :heavy_check_mark:                                                                                                                | Item Id, has format `ETHEREUM:${token}:${tokenId}`                                                                                | ETHEREUM:0xb66a603f4cfe17e3d27b87a8bfcad319856518b8:32292934596187112148346015918544186536963932779440027682601542850818403729410 |
| `uri`                                                                                                                             | *string*                                                                                                                          | :heavy_check_mark:                                                                                                                | N/A                                                                                                                               |                                                                                                                                   |
| `creators`                                                                                                                        | [models.Creator](../models/creator.md)[]                                                                                          | :heavy_check_mark:                                                                                                                | Addresses of the NFT item creators                                                                                                |                                                                                                                                   |
| `royalties`                                                                                                                       | [models.Royalty](../models/royalty.md)[]                                                                                          | :heavy_check_mark:                                                                                                                | List of royalties                                                                                                                 |                                                                                                                                   |
| `signatures`                                                                                                                      | *string*[]                                                                                                                        | :heavy_check_mark:                                                                                                                | Digital signatures                                                                                                                |                                                                                                                                   |