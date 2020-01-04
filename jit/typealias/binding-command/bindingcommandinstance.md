| Modifier(s)                            | Type                     |
|----------------------------------------|--------------------------|
| export | BindingCommandInstance&lt;T&gt; |

# &#10025; Type Parameter(s)

| Type | Constraint |
| ---- | ---------- |
| T    | {}         |

# &#10025; Initializer

```ts
{
  bindingType: BindingType;
  compile(binding: PlainAttributeSymbol | BindingSymbol): ITargetedInstruction;
} & T
```