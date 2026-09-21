---
source_url: https://docs.typesafe.ai/sdk/javascript/api/interfaces/WithResponse.md
fetched_at: 2026-09-21
local_path: sdk/javascript/api/interfaces/WithResponse.md
---

> ## Documentation Index
> Fetch the complete documentation index at: https://docs.typesafe.ai/llms.txt
> Use this file to discover all available pages before exploring further.

# Interface: WithResponse\<T\>

Parsed data with its HTTP response and request ID.

## Type Parameters

### T

`T`

## Properties

<a id="sdk-data"></a>

### data

```ts
data: T;
```

The parsed response body.

***

<a id="sdk-requestid"></a>

### requestId

```ts
requestId: string | undefined;
```

Request ID from `x-typesafe-request-id`, or `undefined` when absent.

***

<a id="sdk-response"></a>

### response

```ts
response: Response;
```

The HTTP response, with its body consumed by parsing.
