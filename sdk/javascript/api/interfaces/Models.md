---
source_url: https://docs.typesafe.ai/sdk/javascript/api/interfaces/Models.md
fetched_at: 2026-09-21
local_path: sdk/javascript/api/interfaces/Models.md
---

> ## Documentation Index
> Fetch the complete documentation index at: https://docs.typesafe.ai/llms.txt
> Use this file to discover all available pages before exploring further.

# Interface: Models

Access to the Models API resource.

## Methods

<a id="sdk-list"></a>

### list()

```ts
list(options?): APIPromise<ModelCard[]>;
```

List the models available to the account.

#### Parameters

##### options?

[`RequestOptions`](./RequestOptions.md) = `{}`

#### Returns

[`APIPromise`](../classes/APIPromise.md)\<[`ModelCard`](./ModelCard.md)\[]>
