# &#9733; Summary

For some reason rollup complains about `DI.createInterface<ITemplateElementFactory>().noDefault()` with this message:
"semantic error TS2742 The inferred type of 'ITemplateElementFactory' cannot be named without a reference to '@aurelia/jit/node_modules/@aurelia/kernel'. This is likely not portable. A type annotation is necessary"
So.. investigate why that happens (or rather, why it *only* happens here and not for the other 50)

| Modifier(s)                            |
|----------------------------------------|
| export |

# &#9733; Variable(s)

&nbsp;&nbsp; **&#10148; ITemplateElementFactory**

| Type                        |
|-----------------------------|
| InterfaceSymbol&lt;[ITemplateElementFactory](/jit-html/interface/template-element-factory/itemplateelementfactory)&lt;INode&gt;&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Initializer**

```ts
DI.createInterface<ITemplateElementFactory>('ITemplateElementFactory').noDefault()
```