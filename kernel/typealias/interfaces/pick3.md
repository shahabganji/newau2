# &#10025; Summary

https:gist.github.com/staltz/368866ea6b8a167fbdac58cddf79c1bf=

| Modifier(s)                            | Type                     |
|----------------------------------------|--------------------------|
| export | Pick3&lt;T, K1, K2, K3&gt; |

# &#10025; Type Parameter(s)

| Type | Constraint |
| ---- | ---------- |
| T    | -          |

| Type | Constraint |
| ---- | ---------- |
| K1   | keyof T    |

| Type | Constraint  |
| ---- | ----------- |
| K2   | keyof T[K1] |

| Type | Constraint      |
| ---- | --------------- |
| K3   | keyof T[K1][K2] |

# &#10025; Initializer

```ts
{
  [P1 in K1]: { [P2 in K2]: { [P3 in K3]: ((T[K1])[K2])[P3] } }
}
```