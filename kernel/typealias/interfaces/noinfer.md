# &#10025; Summary

https:github.com/Microsoft/TypeScript/issues/14829#issuecomment-322267089

| Modifier(s)                            | Type                     |
|----------------------------------------|--------------------------|
| export | NoInfer&lt;T&gt; |

# &#10025; Type Parameter(s)

| Type | Constraint |
| ---- | ---------- |
| T    | -          |

# &#10025; Initializer

```ts
T & { [K in keyof T]: T[K] }
```