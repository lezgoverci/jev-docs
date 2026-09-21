---
source_url: https://docs.typesafe.ai/sdk/javascript/api/interfaces/SystemOneResult.md
fetched_at: 2026-09-21
local_path: sdk/javascript/api/interfaces/SystemOneResult.md
---

> ## Documentation Index
> Fetch the complete documentation index at: https://docs.typesafe.ai/llms.txt
> Use this file to discover all available pages before exploring further.

# Interface: SystemOneResult\<Q\>

Answers keyed by question name, with model and usage metadata.

## Type Parameters

### Q

`Q` *extends* [`Questions`](./Questions.md)

## Properties

<a id="sdk-answers"></a>

### answers

```ts
readonly answers: { readonly [K in string | number | symbol]: ResultFor<Q[K]> };
```

Answers with types inferred from the supplied questions.

***

<a id="sdk-model"></a>

### model

```ts
readonly model: string;
```

The model used to answer the request.

***

<a id="sdk-usage"></a>

### usage

```ts
readonly usage: Usage;
```

Token usage for the request.
