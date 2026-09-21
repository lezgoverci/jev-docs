---
source_url: https://docs.typesafe.ai/sdk/python/api/types/common.md
fetched_at: 2026-09-21
local_path: sdk/python/api/types/common.md
---

> ## Documentation Index
> Fetch the complete documentation index at: https://docs.typesafe.ai/llms.txt
> Use this file to discover all available pages before exploring further.

# Common types

> Common types for TypeSafe API SDK.


<a id="common-types"></a>

<h2 id="typesafe_sdk.JSONValue">
  typesafe\_sdk.JSONValue
</h2>

`module-attribute`

```python
JSONValue = TypeAliasType(
    "JSONValue",
    "str | int | float | bool | Sequence[JSONValue | None] | Mapping[str, JSONValue | None]",
)
```

A JSON-like value. May be nested and contain `None`.

<h2 id="typesafe_sdk.JSONContent">
  typesafe\_sdk.JSONContent
</h2>

`module-attribute`

```python
JSONContent = TypeAliasType(
    "JSONContent",
    "str | Mapping[str, JSONValue | None] | Sequence[JSONValue | None]",
)
```

Either a plain string or a mapping/sequence of [`JSONValue`](./common.md#typesafe_sdk.JSONValue) entries.
