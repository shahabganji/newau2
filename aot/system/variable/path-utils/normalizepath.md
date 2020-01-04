| Modifier(s)                            |
|----------------------------------------|
| export |

# &#9733; Variable(s)

&nbsp;&nbsp; **&#10148; normalizePath**

| Type                        |
|-----------------------------|
| (path: string) =&gt; string |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Initializer**

```ts
(function () {
  const cache: Record<string, string | undefined> = Object.create(null);
    const regex = /\\/g;
    return function (path: string) {
      let normalized = cache[path];
      if (normalized === void 0) {
        normalized = cache[path] = path.replace(regex, '/');
      }
      return normalized;
    };
    })()
```