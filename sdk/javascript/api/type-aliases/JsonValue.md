---
source_url: https://docs.typesafe.ai/sdk/javascript/api/type-aliases/JsonValue.md
fetched_at: 2026-09-21
local_path: sdk/javascript/api/type-aliases/JsonValue.md
---

> ## Documentation Index
> Fetch the complete documentation index at: https://docs.typesafe.ai/llms.txt
> Use this file to discover all available pages before exploring further.

# Type Alias: JsonValue

```ts
type JsonValue = 
  | string
  | number
  | boolean
  | null
  | JsonValue[]
  | {
[key: string]: JsonValue;
};
```

A JSON-compatible value.
