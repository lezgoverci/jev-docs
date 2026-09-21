---
source_url: https://docs.typesafe.ai/sdk/javascript/api/classes/APITimeoutError.md
fetched_at: 2026-09-21
local_path: sdk/javascript/api/classes/APITimeoutError.md
---

> ## Documentation Index
> Fetch the complete documentation index at: https://docs.typesafe.ai/llms.txt
> Use this file to discover all available pages before exploring further.

# Class: APITimeoutError

The full response did not arrive within the timeout. A kind of `APIConnectionError`.

## Extends

* [`APIConnectionError`](./APIConnectionError.md)

## Constructors

<a id="sdk-constructor"></a>

### Constructor

```ts
new APITimeoutError(timeoutMs, options?): APITimeoutError;
```

#### Parameters

##### timeoutMs

`number`

##### options?

`ErrorOptions`

#### Returns

`APITimeoutError`

#### Overrides

[`APIConnectionError`](./APIConnectionError.md).[`constructor`](./APIConnectionError.md#sdk-constructor)

## Properties

<a id="sdk-timeoutms"></a>

### timeoutMs

```ts
readonly timeoutMs: number;
```

Configured timeout in milliseconds.
