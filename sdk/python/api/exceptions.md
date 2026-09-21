---
source_url: https://docs.typesafe.ai/sdk/python/api/exceptions.md
fetched_at: 2026-09-21
local_path: sdk/python/api/exceptions.md
---

> ## Documentation Index
> Fetch the complete documentation index at: https://docs.typesafe.ai/llms.txt
> Use this file to discover all available pages before exploring further.

# Exceptions

> Handle TypeSafe API errors, rate limits, connection failures, and timeouts.


<a id="exceptions"></a>

<h2 id="base-exception">
  Base exception
</h2>

<h2 id="typesafe_sdk.TypeSafeError">
  typesafe\_sdk.TypeSafeError
</h2>

Bases: <code><a href="https://docs.python.org/3/builtins/exceptions.html#Exception">Exception</a></code>

Base exception for SDK failures.

<h2 id="http-errors">
  HTTP errors
</h2>

<h2 id="typesafe_sdk.TypeSafeAPIError">
  typesafe\_sdk.TypeSafeAPIError
</h2>

Bases: <code><a href="./exceptions.md#typesafe_sdk.TypeSafeError">TypeSafeError</a></code>

An unsuccessful HTTP response with its body and request metadata.

<h3 id="typesafe_sdk.TypeSafeAPIError.status">
  status
</h3>

`instance-attribute`

```python
status = status
```

HTTP response status code.

<h3 id="typesafe_sdk.TypeSafeAPIError.body">
  body
</h3>

`instance-attribute`

```python
body = body
```

The server's JSON error body, plain response text, or `None` for an empty body.

<h3 id="typesafe_sdk.TypeSafeAPIError.headers">
  headers
</h3>

`instance-attribute`

```python
headers = headers
```

HTTP response headers.

<h3 id="typesafe_sdk.TypeSafeAPIError.endpoint">
  endpoint
</h3>

`instance-attribute`

```python
endpoint = endpoint
```

The request method and URL, without credentials, query parameters, or fragment, when available.

<h3 id="typesafe_sdk.TypeSafeAPIError.request_id">
  request\_id
</h3>

`property`

```python
request_id: str | None
```

The `x-typesafe-request-id` response header, or `None` if absent.

<h2 id="typesafe_sdk.TypeSafeBadRequestError">
  typesafe\_sdk.TypeSafeBadRequestError
</h2>

Bases: <code><a href="./exceptions.md#typesafe_sdk.TypeSafeAPIError">TypeSafeAPIError</a></code>

The request was invalid (400).

<h2 id="typesafe_sdk.TypeSafeAuthenticationError">
  typesafe\_sdk.TypeSafeAuthenticationError
</h2>

Bases: <code><a href="./exceptions.md#typesafe_sdk.TypeSafeAPIError">TypeSafeAPIError</a></code>

Authentication failed (401).

<h2 id="typesafe_sdk.TypeSafePermissionDeniedError">
  typesafe\_sdk.TypeSafePermissionDeniedError
</h2>

Bases: <code><a href="./exceptions.md#typesafe_sdk.TypeSafeAPIError">TypeSafeAPIError</a></code>

Access was denied (403).

<h2 id="typesafe_sdk.TypeSafeNotFoundError">
  typesafe\_sdk.TypeSafeNotFoundError
</h2>

Bases: <code><a href="./exceptions.md#typesafe_sdk.TypeSafeAPIError">TypeSafeAPIError</a></code>

The resource was not found (404).

<h2 id="typesafe_sdk.TypeSafeUnprocessableEntityError">
  typesafe\_sdk.TypeSafeUnprocessableEntityError
</h2>

Bases: <code><a href="./exceptions.md#typesafe_sdk.TypeSafeAPIError">TypeSafeAPIError</a></code>

The request failed server validation (422).

<h2 id="typesafe_sdk.TypeSafeRateLimitError">
  typesafe\_sdk.TypeSafeRateLimitError
</h2>

Bases: <code><a href="./exceptions.md#typesafe_sdk.TypeSafeAPIError">TypeSafeAPIError</a></code>

The rate limit was exceeded (429).

<h3 id="typesafe_sdk.TypeSafeRateLimitError.retry_after_ms">
  retry\_after\_ms
</h3>

`instance-attribute`

```python
retry_after_ms = parse_retry_after(headers)
```

The server's requested wait in milliseconds, or `None` if unavailable.

<h2 id="typesafe_sdk.TypeSafeInternalServerError">
  typesafe\_sdk.TypeSafeInternalServerError
</h2>

Bases: <code><a href="./exceptions.md#typesafe_sdk.TypeSafeAPIError">TypeSafeAPIError</a></code>

The server failed to process the request (5xx).

<h2 id="connection-errors">
  Connection errors
</h2>

<h2 id="typesafe_sdk.TypeSafeAPIConnectionError">
  typesafe\_sdk.TypeSafeAPIConnectionError
</h2>

Bases: <code><a href="./exceptions.md#typesafe_sdk.TypeSafeError">TypeSafeError</a></code>, <code><a href="https://docs.python.org/3/builtins/exceptions.html#ConnectionError">ConnectionError</a></code>

A request failed without an HTTP response.

<h2 id="typesafe_sdk.TypeSafeAPITimeoutError">
  typesafe\_sdk.TypeSafeAPITimeoutError
</h2>

Bases: <code><a href="./exceptions.md#typesafe_sdk.TypeSafeAPIConnectionError">TypeSafeAPIConnectionError</a></code>, <code><a href="https://docs.python.org/3/builtins/exceptions.html#TimeoutError">TimeoutError</a></code>

A request exceeded its configured timeout.

<h3 id="typesafe_sdk.TypeSafeAPITimeoutError.timeout">
  timeout
</h3>

`instance-attribute`

```python
timeout = timeout
```

The timeout setting used for the request, in seconds or as an `httpx2.Timeout`.

<h2 id="response-validation">
  Response validation
</h2>

<h2 id="typesafe_sdk.TypeSafeAPIResponseValidationError">
  typesafe\_sdk.TypeSafeAPIResponseValidationError
</h2>

Bases: <code><a href="./exceptions.md#typesafe_sdk.TypeSafeAPIError">TypeSafeAPIError</a></code>

A successful HTTP response whose body was missing or structurally invalid required data.

<h3 id="typesafe_sdk.TypeSafeAPIResponseValidationError.field_path">
  field\_path
</h3>

`instance-attribute`

```python
field_path = field_path
```

Dotted path to the offending field, such as `answers.tone.confidence`.

<h3 id="typesafe_sdk.TypeSafeAPIResponseValidationError.args">
  args
</h3>

`instance-attribute`

```python
args = (
    status,
    body,
    headers,
    field_path,
    endpoint,
)
```
