---
source_url: https://docs.typesafe.ai/sdk/javascript/api/interfaces/SystemOneRequest.md
fetched_at: 2026-09-21
local_path: sdk/javascript/api/interfaces/SystemOneRequest.md
---

> ## Documentation Index
> Fetch the complete documentation index at: https://docs.typesafe.ai/llms.txt
> Use this file to discover all available pages before exploring further.

# Interface: SystemOneRequest\<Q\>

State and named questions for `systemOne`.

Additional properties on a request variable are forwarded, including `null` values.

## Extended by

* [`SystemOneRequestPayload`](./SystemOneRequestPayload.md)

## Type Parameters

### Q

`Q` *extends* [`Questions`](./Questions.md) = [`Questions`](./Questions.md)

## Properties

<a id="sdk-model"></a>

### model?

```ts
optional model?: string;
```

Model override; omitted values inherit `defaultModel`.

***

<a id="sdk-questions"></a>

### questions

```ts
questions: Q;
```

Nonempty questions keyed by the names used to identify their answers.

***

<a id="sdk-state"></a>

### state

```ts
state: EntryType;
```

Text, a JSON object or array, or `null` to evaluate.
