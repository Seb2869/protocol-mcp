# Meta

## Example Usage

```typescript
import { Meta } from "@rarible/protocol-mcp";

let value: Meta = {
  name: "<value>",
  attributes: [
    {
      key: "<key>",
    },
  ],
  content: [
    {
      url: "https://defenseless-joy.info",
      representation: "PREVIEW",
      mimeType: "image/png",
    },
  ],
  extraContent: [
    {
      url: "https://alert-tarragon.net",
      representation: "PREVIEW",
      mimeType: "image/png",
    },
  ],
};
```

## Fields

| Field                                                                                         | Type                                                                                          | Required                                                                                      | Description                                                                                   |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `name`                                                                                        | *string*                                                                                      | :heavy_check_mark:                                                                            | Name of the NFT item                                                                          |
| `description`                                                                                 | *string*                                                                                      | :heavy_minus_sign:                                                                            | Description of the NFT item                                                                   |
| `createdAt`                                                                                   | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `updatedAt`                                                                                   | [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `tags`                                                                                        | *string*[]                                                                                    | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `genres`                                                                                      | *string*[]                                                                                    | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `language`                                                                                    | *string*                                                                                      | :heavy_minus_sign:                                                                            | Language in RFC 1176 format                                                                   |
| `rights`                                                                                      | *string*                                                                                      | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `rightsUri`                                                                                   | *string*                                                                                      | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `externalUri`                                                                                 | *string*                                                                                      | :heavy_minus_sign:                                                                            | URI to external page related to the Item                                                      |
| `originalMetaUri`                                                                             | *string*                                                                                      | :heavy_minus_sign:                                                                            | URI to the original meta JSON                                                                 |
| `attributes`                                                                                  | [models.MetaAttribute](../models/metaattribute.md)[]                                          | :heavy_check_mark:                                                                            | Attributes of the NFT item                                                                    |
| `content`                                                                                     | *models.MetaContent*[]                                                                        | :heavy_check_mark:                                                                            | NFT content information                                                                       |
| `extraContent`                                                                                | *models.MetaContent*[]                                                                        | :heavy_minus_sign:                                                                            | NFT additional content information                                                            |