# OpenSeaFillOrderSignatureInputForm

## Example Usage

```typescript
import { OpenSeaFillOrderSignatureInputForm } from "@rarible/protocol-mcp";

let value: OpenSeaFillOrderSignatureInputForm = {
  signature:
    "0xf3104d38a35c59d2612a6128c9e2bbfabf16f26b2db393801cc20398f10079f2",
  blockchain: "ETHEREUM",
};
```

## Fields

| Field                                                                    | Type                                                                     | Required                                                                 | Description                                                              | Example                                                                  |
| ------------------------------------------------------------------------ | ------------------------------------------------------------------------ | ------------------------------------------------------------------------ | ------------------------------------------------------------------------ | ------------------------------------------------------------------------ |
| `atType`                                                                 | [models.SignatureInputFormAtType](../models/signatureinputformattype.md) | :heavy_minus_sign:                                                       | N/A                                                                      |                                                                          |
| `signature`                                                              | *string*                                                                 | :heavy_minus_sign:                                                       | SeaPort order hash in 'native' format                                    | 0xf3104d38a35c59d2612a6128c9e2bbfabf16f26b2db393801cc20398f10079f2       |
| `blockchain`                                                             | [models.Blockchain](../models/blockchain.md)                             | :heavy_check_mark:                                                       | N/A                                                                      | ETHEREUM                                                                 |