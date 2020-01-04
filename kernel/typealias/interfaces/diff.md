| Modifier(s)                            | Type                     |
|----------------------------------------|--------------------------|
| export | ({ [P in T]: P; } & { [P in U]: never; } & { [x: string]: never; })[T] |

# &#10025; Type Parameter(s)

| Type | Constraint |
| ---- | ---------- |
| T    | string     |

| Type | Constraint |
| ---- | ---------- |
| U    | string     |

# &#10025; Initializer

```ts
({[P in T]: P } & {[P in U]: never } & { [x: string]: never })[T]
```