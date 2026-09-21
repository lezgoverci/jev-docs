---
source_url: https://docs.typesafe.ai/sdk/javascript/api/interfaces/TypeSafeClientConfig.md
fetched_at: 2026-09-21
local_path: sdk/javascript/api/interfaces/TypeSafeClientConfig.md
---

> ## Documentation Index
> Fetch the complete documentation index at: https://docs.typesafe.ai/llms.txt
> Use this file to discover all available pages before exploring further.

# Interface: TypeSafeClientConfig

Client options. Explicit values take precedence over environment variables, then SDK defaults.

## Properties

<a id="sdk-apikey"></a>

### apiKey?

```ts
optional apiKey?: string;
```

Required API key; falls back to `TYPESAFE_API_KEY`.

***

<a id="sdk-baseurl"></a>

### baseURL?

```ts
optional baseURL?: string;
```

API root; falls back to `TYPESAFE_BASE_URL`, then `https://api.typesafe.ai`.

***

<a id="sdk-dangerouslyallowbrowser"></a>

### dangerouslyAllowBrowser?

```ts
optional dangerouslyAllowBrowser?: boolean;
```

Allow browser use, exposing the API key to page users. Default: false.

***

<a id="sdk-defaultheaders"></a>

### defaultHeaders?

```ts
optional defaultHeaders?: Record<string, string>;
```

Additional request headers; per-call headers take precedence.

***

<a id="sdk-defaultmodel"></a>

### defaultModel?

```ts
optional defaultModel?: string;
```

Default model; falls back to `TYPESAFE_DEFAULT_MODEL`, then `jev-latest`.

***

<a id="sdk-fetch"></a>

### fetch?

```ts
optional fetch?: Fetch;
```

Custom HTTP fetch implementation for transport configuration or tests. Default: global `fetch`.

***

<a id="sdk-logger"></a>

### logger?

```ts
optional logger?: Logger;
```

Logger filtered to `logLevel` and above. Default: prefixed `console`.

***

<a id="sdk-loglevel"></a>

### logLevel?

```ts
optional logLevel?: LogLevel;
```

Log level; falls back to `TYPESAFE_LOG_LEVEL`, then `warn`.
`info` logs request summaries; `debug` adds headers and bodies.
Known credential headers are redacted; bodies are not.

***

<a id="sdk-retry"></a>

### retry?

```ts
optional retry?: Partial<RetryPolicy>;
```

Retry overrides; omitted fields use the defaults in `RetryPolicy`.

***

<a id="sdk-timeout"></a>

### timeout?

```ts
optional timeout?: number;
```

Timeout per attempt in milliseconds, without a total retry budget. Default: 10000.
