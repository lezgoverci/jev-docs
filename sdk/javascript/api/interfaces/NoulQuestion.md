---
source_url: https://docs.typesafe.ai/sdk/javascript/api/interfaces/NoulQuestion.md
fetched_at: 2026-09-21
local_path: sdk/javascript/api/interfaces/NoulQuestion.md
---

> ## Documentation Index
> Fetch the complete documentation index at: https://docs.typesafe.ai/llms.txt
> Use this file to discover all available pages before exploring further.

# Interface: NoulQuestion

A yes/no question with optional descriptions for either outcome.

## Properties

<a id="sdk-criteria"></a>

### criteria?

```ts
optional criteria?: 
  | {
  false?: EntryType;
  true?: EntryType;
}
  | null;
```

Optional descriptions of the yes and no outcomes.

#### Union Members

##### Type Literal

```ts
{
  false?: EntryType;
  true?: EntryType;
}
```

##### false?

```ts
optional false?: EntryType;
```

Description of the no outcome.

##### true?

```ts
optional true?: EntryType;
```

Description of the yes outcome.

***

`null`

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
type: "noul";
```
