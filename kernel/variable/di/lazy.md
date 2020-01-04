| Modifier(s)                            |
|----------------------------------------|
| export |

# &#9733; Variable(s)

&nbsp;&nbsp; **&#10148; lazy**

| Type                        |
|-----------------------------|
| (key: any) =&gt; any |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Initializer**

```ts
createResolver((key: any, handler: IContainer, requestor: IContainer) =>  {
  let instance: unknown = null; // cache locally so that lazy always returns the same instance once resolved
  return () => {
    if (instance == null) {
      instance = requestor.get(key);
    }
    return instance;
  };
})
```