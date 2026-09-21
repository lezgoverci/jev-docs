---
source_url: https://docs.typesafe.ai/sdk/javascript/api/interfaces/ScoreResponse.md
fetched_at: 2026-09-21
local_path: sdk/javascript/api/interfaces/ScoreResponse.md
---

> ## Documentation Index
> Fetch the complete documentation index at: https://docs.typesafe.ai/llms.txt
> Use this file to discover all available pages before exploring further.

# Interface: ScoreResponse\<T\>

An expected score with its rubric and probabilities.

## Type Parameters

### T

`T` *extends* [`ScoreCriteria`](../type-aliases/ScoreCriteria.md) = [`ScoreCriteria`](../type-aliases/ScoreCriteria.md)

## Properties

<a id="sdk-confidence"></a>

### confidence

```ts
readonly confidence: number;
```

Reported confidence in the score.

***

<a id="sdk-legend"></a>

### legend

```ts
readonly legend: ScoreLegend<T>;
```

Rubric descriptions keyed by score.

***

<a id="sdk-probabilities"></a>

### probabilities

```ts
readonly probabilities: { readonly [score in number | `${number}`]: number };
```

Probabilities keyed by score.

***

<a id="sdk-score"></a>

### score

```ts
readonly score: number;
```

Expected score, which may fall between integer rubric levels.

***

<a id="sdk-type"></a>

### type

```ts
readonly type: "score";
```
