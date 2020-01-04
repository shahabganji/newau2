| Modifier(s)                            | Type                     |
|----------------------------------------|--------------------------|
| export | Omit&lt;T, K&gt; |

# &#10025; Type Parameter(s)

| Type | Constraint |
| ---- | ---------- |
| T    | -          |

| Type | Constraint |
| ---- | ---------- |
| K    | keyof T    |

# &#10025; Initializer

```ts
T extends {} ? Pick<T, Exclude<keyof T, K>> : never
```