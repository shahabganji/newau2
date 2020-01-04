| Modifier(s)                            | Type                     |
|----------------------------------------|--------------------------|
| export | { [P in keyof T]-?: IfEquals&lt;{ [Q in P]: T[P]; }, { -readonly [Q in P]: T[P]; }, P, never&gt;; }[keyof T] |

# &#10025; Type Parameter(s)

| Type | Constraint |
| ---- | ---------- |
| T    | -          |

# &#10025; Initializer

```ts
{
  [P in keyof T]-?: IfEquals<{ [Q in P]: T[P] }, { -readonly [Q in P]: T[P] }, P>
}[keyof T]
```