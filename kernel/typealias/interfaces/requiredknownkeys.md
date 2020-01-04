| Modifier(s)                            | Type                     |
|----------------------------------------|--------------------------|
| export | RequiredKnownKeys&lt;T&gt; |

# &#10025; Type Parameter(s)

| Type | Constraint |
| ---- | ---------- |
| T    | -          |

# &#10025; Initializer

```ts
{
  [K in keyof T]: {} extends Pick<T, K> ? never : K
    } extends { [_ in keyof T]: infer U } ? ({} extends U ? never : U) : never
```