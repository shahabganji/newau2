| Modifier(s)                            | Type                     |
|----------------------------------------|--------------------------|
| export | Overwrite&lt;T1, T2&gt; |

# &#10025; Type Parameter(s)

| Type | Constraint |
| ---- | ---------- |
| T1   | -          |

| Type | Constraint |
| ---- | ---------- |
| T2   | -          |

# &#10025; Initializer

```ts
Pick<T1, Exclude<keyof T1, keyof T2>> & T2
```