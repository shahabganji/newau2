| Modifier(s)                            | Type                     |
|----------------------------------------|--------------------------|
| export | OptionalKnownKeys&lt;T&gt; |

# &#10025; Type Parameter(s)

| Type | Constraint |
| ---- | ---------- |
| T    | -          |

# &#10025; Initializer

```ts
{
  [K in keyof T]: string extends K ? never : number extends K ? never : {} extends Pick<T, K> ? K : never
    } extends { [_ in keyof T]: infer U } ? ({} extends U ? never : U) : never
```