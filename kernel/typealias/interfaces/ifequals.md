| Modifier(s)                            | Type                     |
|----------------------------------------|--------------------------|
| export | IfEquals&lt;X, Y, A, B&gt; |

# &#10025; Type Parameter(s)

| Type | Constraint |
| ---- | ---------- |
| X    | -          |

| Type | Constraint |
| ---- | ---------- |
| Y    | -          |

| Type | Constraint |
| ---- | ---------- |
| A    | -          |

| Type | Constraint |
| ---- | ---------- |
| B    | -          |

# &#10025; Initializer

```ts
(<T>() => T extends X ? 1 : 2) extends
  (<T>() => T extends Y ? 1 : 2) ? A : B
```