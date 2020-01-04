| Modifier(s)                            |
|----------------------------------------|
| export |

# &#9733; Variable(s)

&nbsp;&nbsp; **&#10148; optional**

| Type                        |
|-----------------------------|
| (key: any) =&gt; any |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Initializer**

```ts
createResolver((key: any, handler: IContainer, requestor: IContainer) =>  {
  if (requestor.has(key, true)) {
    return requestor.get(key);
  } else {
    return null;
  }
})
```