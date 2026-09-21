---
source_url: https://docs.typesafe.ai/sdk/javascript/api/interfaces/ScoreQuestion.md
fetched_at: 2026-09-21
local_path: sdk/javascript/api/interfaces/ScoreQuestion.md
---

> ## Documentation Index
> Fetch the complete documentation index at: https://docs.typesafe.ai/llms.txt
> Use this file to discover all available pages before exploring further.

# Interface: ScoreQuestion\<T\>

A question that assigns a score using an ordered rubric.

## Type Parameters

### T

`T` *extends* [`ScoreCriteria`](../type-aliases/ScoreCriteria.md) = [`ScoreCriteria`](../type-aliases/ScoreCriteria.md)

## Properties

<a id="sdk-criteria"></a>

### criteria

```ts
criteria: T;
```

Descriptions of the available outcomes.

***

<a id="sdk-instructions"></a>

### instructions?

```ts
optional instructions?: EntryType;
```

The question as text, a JSON object, or an array; optional or `null`.

***

<a id="sdk-type"></a>

### type

```ts
type: "score";
```
