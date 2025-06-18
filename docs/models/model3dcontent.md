# Model3dContent

## Example Usage

```typescript
import { Model3dContent } from "@rarible/protocol-mcp";

let value: Model3dContent = {
  url: "https://shady-chasuble.name/",
  representation: "PREVIEW",
  mimeType: "image/png",
};
```

## Fields

| Field                                                              | Type                                                               | Required                                                           | Description                                                        | Example                                                            |
| ------------------------------------------------------------------ | ------------------------------------------------------------------ | ------------------------------------------------------------------ | ------------------------------------------------------------------ | ------------------------------------------------------------------ |
| `atType`                                                           | [models.AtTypeModel3D](../models/attypemodel3d.md)                 | :heavy_minus_sign:                                                 | N/A                                                                |                                                                    |
| `fileName`                                                         | *string*                                                           | :heavy_minus_sign:                                                 | N/A                                                                |                                                                    |
| `url`                                                              | *string*                                                           | :heavy_check_mark:                                                 | N/A                                                                |                                                                    |
| `representation`                                                   | [models.RepresentationModel3D](../models/representationmodel3d.md) | :heavy_check_mark:                                                 | N/A                                                                |                                                                    |
| `mimeType`                                                         | *string*                                                           | :heavy_minus_sign:                                                 | N/A                                                                | image/png                                                          |
| `size`                                                             | *number*                                                           | :heavy_minus_sign:                                                 | N/A                                                                |                                                                    |
| `available`                                                        | *boolean*                                                          | :heavy_minus_sign:                                                 | N/A                                                                |                                                                    |