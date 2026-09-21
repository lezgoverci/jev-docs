---
source_url: https://docs.typesafe.ai/sdk/javascript/api/interfaces/ChoiceResponse.md
fetched_at: 2026-09-21
local_path: sdk/javascript/api/interfaces/ChoiceResponse.md
---

> ## Documentation Index
> Fetch the complete documentation index at: https://docs.typesafe.ai/llms.txt
> Use this file to discover all available pages before exploring further.

# Interface: ChoiceResponse\<T\>

A selected label and its probabilities.

## Type Parameters

### T

`T` *extends* [`ChoiceCriteria`](../type-aliases/ChoiceCriteria.md) = [`ChoiceCriteria`](../type-aliases/ChoiceCriteria.md)

## Properties

<a id="sdk-choice"></a>

### choice

```ts
readonly choice: keyof T & string;
```

The selected label.

***

<a id="sdk-confidence"></a>

### confidence

```ts
readonly confidence: number;
```

Reported confidence in the selected label.

***

<a id="sdk-probabilities"></a>

### probabilities

```ts
readonly probabilities: { readonly [label in string | number | symbol]: number };
```

Probabilities keyed by label.

***

<a id="sdk-type"></a>

### type

```ts
readonly type: "choice";
```
