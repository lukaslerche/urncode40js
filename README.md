# urncode40js

JavaScript library to encode and decode URN Code 40

## How to use

```typescript
import { encode, decode, validate } from "urncode40";

const text = "urn:example:12345";
const encoded = encode(text);
if (!encoded) {
    throw new Error("Encoding failed");
}
const isValid = validate(encoded);
const decoded = decode(encoded); 
```