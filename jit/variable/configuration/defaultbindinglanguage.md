# &#9733; Summary

Default runtime/environment-agnostic binding commands:
- Property observation: `.bind`, `.one-time`, `.from-view`, `.to-view`, `.two-way`
- Function call: `.call`
- Collection observation: `.for`

| Modifier(s)                            |
|----------------------------------------|
| export |

# &#9733; Variable(s)

&nbsp;&nbsp; **&#10148; DefaultBindingLanguage**

| Type                        |
|-----------------------------|
| [IRegistry](/kernel/interface/di/iregistry)[] |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Initializer**

```ts
[
  DefaultBindingCommandRegistration,
  OneTimeBindingCommandRegistration,
  FromViewBindingCommandRegistration,
  ToViewBindingCommandRegistration,
  TwoWayBindingCommandRegistration,
  CallBindingCommandRegistration,
  ForBindingCommandRegistration
]
```