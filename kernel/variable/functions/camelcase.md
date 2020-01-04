# &#9733; Summary

Efficiently convert a string to camelCase.
Non-alphanumeric characters are treated as separators.
Primarily used by Aurelia to convert DOM attribute names to ViewModel property names.
Results are cached.

| Modifier(s)                            |
|----------------------------------------|
| export |

# &#9733; Variable(s)

&nbsp;&nbsp; **&#10148; camelCase**

| Type                        |
|-----------------------------|
| (input: string) =&gt; string |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Initializer**

```ts
(function () {
  const cache = Object.create(null) as Record<string, string | undefined>;
    function callback(char: string, sep: boolean): string {
      return sep ? char.toUpperCase() : char.toLowerCase();
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