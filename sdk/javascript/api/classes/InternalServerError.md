---
source_url: https://docs.typesafe.ai/sdk/javascript/api/classes/InternalServerError.md
fetched_at: 2026-09-21
local_path: sdk/javascript/api/classes/InternalServerError.md
---

> ## Documentation Index
> Fetch the complete documentation index at: https://docs.typesafe.ai/llms.txt
> Use this file to discover all available pages before exploring further.

# Class: InternalServerError

HTTP 5xx: the server failed to handle the request.

## Extends

* [`APIError`](./APIError.md)

## Constructors

<a id="sdk-constructor"></a>

### Constructor

```ts
new InternalServerError(
   status, 
   body, 
   headers, 
   message?
): InternalServerError;
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

`InternalServerError`

#### Inherited from

[`APIError`](./APIError.md).[`constructor`](./APIError.md#sdk-constructor)

## Properties

<a id="sdk-body"></a>

### body

```ts
readonly body: unknown;
```

Parsed JSON, response text, or `undefined` for an empty body.

#### Inherited from

[`APIError`](./APIError.md).[`body`](./APIError.md#sdk-body)

***

<a id="sdk-headers"></a>

### headers

```ts
readonly headers: Headers;
```

HTTP response headers.

#### Inherited from

[`APIError`](./APIError.md).[`headers`](./APIError.md#sdk-headers)

***

<a id="sdk-requestid"></a>

### requestId

```ts
readonly requestId: string | undefined;
```

Request ID from `x-typesafe-request-id`, or `undefined` when absent.

#### Inherited from

[`APIError`](./APIError.md).[`requestId`](./APIError.md#sdk-requestid)

***

<a id="sdk-status"></a>

### status

```ts
readonly status: number;
```

HTTP response status code.

#### Inherited from

[`APIError`](./APIError.md).[`status`](./APIError.md#sdk-status)

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

[`APIError`](./APIError.md)

#### Inherited from

[`APIError`](./APIError.md).[`fromResponse`](./APIError.md#sdk-fromresponse)
