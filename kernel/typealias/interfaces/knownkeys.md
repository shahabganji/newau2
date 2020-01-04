| Modifier(s)                            | Type                     |
|----------------------------------------|--------------------------|
| export | KnownKeys&lt;T&gt; |

# &#10025; Type Parameter(s)

| Type | Constraint |
| ---- | ---------- |
| T    | -          |

# &#10025; Initializer

```ts
{
  [K in keyof T]: string extends K ? never : number extends K ? never : K
} extends {[_ in keyof T]: infer U} ? U : never
```