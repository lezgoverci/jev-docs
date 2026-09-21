---
source_url: https://docs.typesafe.ai/sdk/javascript/api/classes/TypeSafeError.md
fetched_at: 2026-09-21
local_path: sdk/javascript/api/classes/TypeSafeError.md
---

> ## Documentation Index
> Fetch the complete documentation index at: https://docs.typesafe.ai/llms.txt
> Use this file to discover all available pages before exploring further.

# Class: TypeSafeError

Base class for SDK errors.

## Extends

* `Error`

## Extended by

* [`APIConnectionError`](./APIConnectionError.md)
* [`APIError`](./APIError.md)
* [`APIUserAbortError`](./APIUserAbortError.md)

## Constructors

<a id="sdk-constructor"></a>

### Constructor

```ts
new TypeSafeError(message, options?): TypeSafeError;
```

#### Parameters

##### message

`string`

##### options?

`ErrorOptions`

#### Returns

`TypeSafeError`

#### Overrides

```ts
Error.constructor
```
