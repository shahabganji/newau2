# &#9733; Summary

Efficiently convert a string to PascalCase.
Non-alphanumeric characters are treated as separators.
Primarily used by Aurelia to convert element names to class names for synthetic types.
Results are cached.

| Modifier(s)                            |
|----------------------------------------|
| export |

# &#9733; Variable(s)

&nbsp;&nbsp; **&#10148; pascalCase**

| Type                        |
|-----------------------------|
| (input: string) =&gt; string |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Initializer**

```ts
(function () {
  const cache = Object.create(null) as Record<string, string | undefined>;
    return function (input: string): string {
      let output = cache[input];
      if (output === void 0) {
        output = camelCase(input);
        if (output.length > 0) {
          output = output[0].toUpperCase() + output.slice(1);
        }
        cache[input] = output;
      }
      return output;
    };
    })()
```