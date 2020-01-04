| Modifier(s)                            |
|----------------------------------------|
| export |

# &#9733; Variable(s)

&nbsp;&nbsp; **&#10148; ILogEventFactory**

| Type                        |
|-----------------------------|
| InterfaceSymbol&lt;[ILogEventFactory](/kernel/interface/logger/ilogeventfactory)&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Initializer**

```ts
DI.createInterface<ILogEventFactory>('ILogEventFactory').withDefault(x => x.singleton(DefaultLogEventFactory))
```