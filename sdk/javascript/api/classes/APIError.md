---
source_url: https://docs.typesafe.ai/sdk/javascript/api/classes/APIError.md
fetched_at: 2026-09-21
local_path: sdk/javascript/api/classes/APIError.md
---

> ## Documentation Index
> Fetch the complete documentation index at: https://docs.typesafe.ai/llms.txt
> Use this file to discover all available pages before exploring further.

# Class: APIError

An unsuccessful HTTP response from the API.

## Extends

* [`TypeSafeError`](./TypeSafeError.md)

## Extended by

* [`AuthenticationError`](./AuthenticationError.md)
* [`BadRequestError`](./BadRequestError.md)
* [`InternalServerError`](./InternalServerError.md)
* [`NotFoundError`](./NotFoundError.md)
* [`PermissionDeniedError`](./PermissionDeniedError.md)
* [`RateLimitError`](./RateLimitError.md)
* [`UnprocessableEntityError`](./UnprocessableEntityError.md)

## Constructors

<a id="sdk-constructor"></a>

### Constructor

```ts
new APIError(
   status, 
   body, 
   headers, 
   message?
): APIError;
```

#### Parameters

##### status

`number`

##### body

`unknown`

##### headers

`Headers`

##### message?

`string`

#### Returns

`APIError`

#### Overrides

[`TypeSafeError`](./TypeSafeError.md).[`constructor`](./TypeSafeError.md#sdk-constructor)

## Properties

<a id="sdk-body"></a>

### body

```ts
readonly body: unknown;
```

Parsed JSON, response text, or `undefined` for an empty body.

***

<a id="sdk-headers"></a>

### headers

```ts
readonly headers: Headers;
```

HTTP response headers.

***

<a id="sdk-requestid"></a>

### requestId

```ts
readonly requestId: string | undefined;
```

Request ID from `x-typesafe-request-id`, or `undefined` when absent.

***

<a id="sdk-status"></a>

### status

```ts
readonly status: number;
```

HTTP response status code.

## Methods

<a id="sdk-fromresponse"></a>

### fromResponse()

```ts
static fromResponse(
   status, 
   body, 
   headers
): APIError;
```

Create the error subclass for an HTTP status code.

#### Parameters

##### status

`number`

##### body

`unknown`

##### headers

`Headers`

#### Returns

`APIError`
