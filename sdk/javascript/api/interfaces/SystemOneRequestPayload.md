---
source_url: https://docs.typesafe.ai/sdk/javascript/api/interfaces/SystemOneRequestPayload.md
fetched_at: 2026-09-21
local_path: sdk/javascript/api/interfaces/SystemOneRequestPayload.md
---

> ## Documentation Index
> Fetch the complete documentation index at: https://docs.typesafe.ai/llms.txt
> Use this file to discover all available pages before exploring further.

# Interface: SystemOneRequestPayload

Request body for `POST /v1/systemone`, with the model resolved.

## Extends

* [`SystemOneRequest`](./SystemOneRequest.md)

## Properties

<a id="sdk-model"></a>

### model

```ts
model: string;
```

Model override; omitted values inherit `defaultModel`.

#### Overrides

[`SystemOneRequest`](./SystemOneRequest.md).[`model`](./SystemOneRequest.md#sdk-model)

***

<a id="sdk-questions"></a>

### questions

```ts
questions: Questions;
```

Nonempty questions keyed by the names used to identify their answers.

#### Inherited from

[`SystemOneRequest`](./SystemOneRequest.md).[`questions`](./SystemOneRequest.md#sdk-questions)

***

<a id="sdk-state"></a>

### state

```ts
state: EntryType;
```

Text, a JSON object or array, or `null` to evaluate.

#### Inherited from

[`SystemOneRequest`](./SystemOneRequest.md).[`state`](./SystemOneRequest.md#sdk-state)
