---
source_url: https://docs.typesafe.ai/sdk/javascript/api/interfaces/RetryPolicy.md
fetched_at: 2026-09-21
local_path: sdk/javascript/api/interfaces/RetryPolicy.md
---

> ## Documentation Index
> Fetch the complete documentation index at: https://docs.typesafe.ai/llms.txt
> Use this file to discover all available pages before exploring further.

# Interface: RetryPolicy

Retry configuration. Partial overrides inherit unset fields from the client or SDK defaults.

## Properties

<a id="sdk-apiconnectionerror"></a>

### apiConnectionError

```ts
readonly apiConnectionError: boolean;
```

Retry connection failures, including interrupted response bodies (`APIConnectionError`). Default: true.

***

<a id="sdk-apitimeouterror"></a>

### apiTimeoutError

```ts
readonly apiTimeoutError: boolean;
```

Whether to retry `APITimeoutError`. Default: true.

***

<a id="sdk-backoffinitialms"></a>

### backoffInitialMs

```ts
readonly backoffInitialMs: number;
```

First backoff delay in milliseconds, doubled up to `backoffMaxMs`. Default: 500.

***

<a id="sdk-backoffjitter"></a>

### backoffJitter

```ts
readonly backoffJitter: number;
```

Fraction of each backoff delay randomly subtracted, from 0 to 1. Default: 0.25.

***

<a id="sdk-backoffmaxms"></a>

### backoffMaxMs

```ts
readonly backoffMaxMs: number;
```

Maximum backoff delay in milliseconds. Default: 5000.

***

<a id="sdk-httpstatuses"></a>

### httpStatuses

```ts
readonly httpStatuses: ReadonlySet<number>;
```

HTTP status codes to retry. Default: 408, 429, and 500–599.

***

<a id="sdk-maxretries"></a>

### maxRetries

```ts
readonly maxRetries: number;
```

Maximum retries after the initial attempt; `0` disables retries. Default: 2.

***

<a id="sdk-maxretryafterms"></a>

### maxRetryAfterMs

```ts
readonly maxRetryAfterMs: number;
```

Maximum server retry delay in milliseconds; longer delays use backoff. Default: 60000.

***

<a id="sdk-respectretryafter"></a>

### respectRetryAfter

```ts
readonly respectRetryAfter: boolean;
```

Honor `Retry-After` and `retry-after-ms` up to `maxRetryAfterMs`. Default: true.
