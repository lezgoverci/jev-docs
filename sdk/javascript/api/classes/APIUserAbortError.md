---
source_url: https://docs.typesafe.ai/sdk/javascript/api/classes/APIUserAbortError.md
fetched_at: 2026-09-21
local_path: sdk/javascript/api/classes/APIUserAbortError.md
---

> ## Documentation Index
> Fetch the complete documentation index at: https://docs.typesafe.ai/llms.txt
> Use this file to discover all available pages before exploring further.

# Class: APIUserAbortError

The caller cancelled the request through an `AbortSignal`.

## Extends

* [`TypeSafeError`](./TypeSafeError.md)

## Constructors

<a id="sdk-constructor"></a>

### Constructor

```ts
new APIUserAbortError(message?, options?): APIUserAbortError;
```

#### Parameters

##### message?

`string` = `"Request was aborted."`

##### options?

`ErrorOptions`

#### Returns

`APIUserAbortError`

#### Overrides

[`TypeSafeError`](./TypeSafeError.md).[`constructor`](./TypeSafeError.md#sdk-constructor)
