---
source_url: https://docs.typesafe.ai/sdk/javascript/api/classes/APIConnectionError.md
fetched_at: 2026-09-21
local_path: sdk/javascript/api/classes/APIConnectionError.md
---

> ## Documentation Index
> Fetch the complete documentation index at: https://docs.typesafe.ai/llms.txt
> Use this file to discover all available pages before exploring further.

# Class: APIConnectionError

The request or response-body delivery failed (DNS, TLS, connection closed, etc.).

## Extends

* [`TypeSafeError`](./TypeSafeError.md)

## Extended by

* [`APITimeoutError`](./APITimeoutError.md)

## Constructors

<a id="sdk-constructor"></a>

### Constructor

```ts
new APIConnectionError(message?, options?): APIConnectionError;
```

#### Parameters

##### message?

`string` = `"Connection error."`

##### options?

`ErrorOptions`

#### Returns

`APIConnectionError`

#### Overrides

[`TypeSafeError`](./TypeSafeError.md).[`constructor`](./TypeSafeError.md#sdk-constructor)
