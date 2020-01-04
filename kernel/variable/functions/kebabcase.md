# &#9733; Summary

Efficiently convert a string to kebab-case.
Non-alphanumeric characters are treated as separators.
Primarily used by Aurelia to convert ViewModel property names to DOM attribute names.
Results are cached.

| Modifier(s)                            |
|----------------------------------------|
| export |

# &#9733; Variable(s)

&nbsp;&nbsp; **&#10148; kebabCase**

| Type                        |
|-----------------------------|
| (input: string) =&gt; string |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Initializer**

```ts
(function () {
  const cache = Object.create(null) as Record<string, string | undefined>;
    function callback(char: string, sep: boolean): string {
      return sep ? `-${char.toLowerCase()}` : char.toLowerCase();
    }
    return function (input: string): string {
      let output = cache[input];
      if (output === void 0) {
        output = cache[input] = baseCase(input, callback);
      }
      return output;
    };
    })()
```