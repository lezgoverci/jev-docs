---
source_url: https://docs.typesafe.ai/sdk/javascript/api/interfaces/ChoiceQuestion.md
fetched_at: 2026-09-21
local_path: sdk/javascript/api/interfaces/ChoiceQuestion.md
---

> ## Documentation Index
> Fetch the complete documentation index at: https://docs.typesafe.ai/llms.txt
> Use this file to discover all available pages before exploring further.

# Interface: ChoiceQuestion\<T\>

A question that selects between named alternatives.

## Type Parameters

### T

`T` *extends* [`ChoiceCriteria`](../type-aliases/ChoiceCriteria.md) = [`ChoiceCriteria`](../type-aliases/ChoiceCriteria.md)

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
type: "choice";
```
