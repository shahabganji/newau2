| Modifier(s)                            |
|----------------------------------------|
| export |

# &#9733; Variable(s)

&nbsp;&nbsp; **&#10148; ILogger**

| Type                        |
|-----------------------------|
| InterfaceSymbol&lt;[ILogger](/kernel/interface/logger/ilogger)&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Initializer**

```ts
DI.createInterface<ILogger>('ILogger').withDefault(x => x.singleton(DefaultLogger))
```