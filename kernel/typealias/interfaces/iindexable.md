| Modifier(s)                            | Type                     |
|----------------------------------------|--------------------------|
| export | IIndexable&lt;TBase, TValue, TKey&gt; |

# &#10025; Type Parameter(s)

| Type  | Constraint |
| ----- | ---------- |
| TBase | {}         |

| Type   | Constraint |
| ------ | ---------- |
| TValue | -          |

| Type | Constraint                         |
| ---- | ---------------------------------- |
| TKey | string &#124; number &#124; symbol |

# &#10025; Initializer

```ts
{ [K in TKey]: TValue } & TBase
```