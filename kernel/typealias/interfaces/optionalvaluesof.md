| Modifier(s)                            | Type                     |
|----------------------------------------|--------------------------|
| export | OptionalValuesOf&lt;T&gt; |

# &#10025; Type Parameter(s)

| Type | Constraint |
| ---- | ---------- |
| T    | -          |

# &#10025; Initializer

```ts
T extends { [_ in keyof T]: infer U } ? U : never
```