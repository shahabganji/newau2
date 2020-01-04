| Modifier(s)                            | Type                     |
|----------------------------------------|--------------------------|
| export | Unwrap&lt;T&gt; |

# &#10025; Type Parameter(s)

| Type | Constraint |
| ---- | ---------- |
| T    | -          |

# &#10025; Initializer

```ts
T extends (infer U)[] ? U :
T extends (...args: unknown[]) => infer U ? U :
T extends Promise<infer U> ? U :
  T
```