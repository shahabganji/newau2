| Modifier(s)                            |
|----------------------------------------|
| export |

# &#9733; Variable(s)

&nbsp;&nbsp; **&#10148; IEventAggregator**

| Type                        |
|-----------------------------|
| InterfaceSymbol&lt;[IEventAggregator](/kernel/variable/eventaggregator/ieventaggregator)&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Initializer**

```ts
DI.createInterface<IEventAggregator>('IEventAggregator').withDefault(x => x.singleton(EventAggregator))
```