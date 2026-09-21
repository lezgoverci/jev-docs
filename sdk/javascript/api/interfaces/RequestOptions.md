---
source_url: https://docs.typesafe.ai/sdk/javascript/api/interfaces/RequestOptions.md
fetched_at: 2026-09-21
local_path: sdk/javascript/api/interfaces/RequestOptions.md
---

> ## Documentation Index
> Fetch the complete documentation index at: https://docs.typesafe.ai/llms.txt
> Use this file to discover all available pages before exploring further.

# Interface: RequestOptions

Per-call options that override client settings.

## Properties

<a id="sdk-headers"></a>

### headers?

```ts
optional headers?: Record<string, string>;
```

Additional headers, merged over `defaultHeaders`.

***

<a id="sdk-retry"></a>

### retry?

```ts
optional retry?: Partial<RetryPolicy>;
```

Retry overrides for this call; omitted fields inherit client settings.

***

<a id="sdk-signal"></a>

### signal?

```ts
optional signal?: AbortSignal;
```

Cancellation signal for the request and pending retries.

***

<a id="sdk-timeout"></a>

### timeout?

```ts
optional timeout?: number;
```

Timeout per attempt in milliseconds; there is no total retry budget.
