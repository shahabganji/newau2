| Modifier(s)                            |
|----------------------------------------|
| export |

# &#9733; Variable(s)

&nbsp;&nbsp; **&#10148; ILogConfig**

| Type                        |
|-----------------------------|
| InterfaceSymbol&lt;[ILogConfig](/kernel/interface/logger/ilogconfig)&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Initializer**

```ts
DI.createInterface<ILogConfig>('ILogConfig').withDefault(x => x.instance(new LogConfig(ColorOptions.noColors, LogLevel.warn)))
```