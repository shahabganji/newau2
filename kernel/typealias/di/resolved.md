| Modifier(s)                            | Type                     |
|----------------------------------------|--------------------------|
| export | Resolved&lt;K&gt; |

# &#10025; Type Parameter(s)

| Type | Constraint |
| ---- | ---------- |
| K    | -          |

# &#10025; Initializer

```ts
(
  K extends InterfaceSymbol<infer T>
    ? T
      : K extends Constructable
    ? InstanceType<K>
      : K extends IResolverLike<any, infer T1>
        ? T1 extends Constructable
          ? InstanceType<T1>
            : T1
            : K
            )
```