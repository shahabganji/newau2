# &#9733; Summary

Determine whether the value is a native function.

**Parameter(s)**

The function to check.

**Returns**

`true` is the function is a native function, otherwise `false`

| Modifier(s)                            |
|----------------------------------------|
| export |

# &#9733; Variable(s)

&nbsp;&nbsp; **&#10148; isNativeFunction**

| Type                        |
|-----------------------------|
| (fn: Function) =&gt; boolean |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Initializer**

```ts
(function () {
  // eslint-disable-next-line @typescript-eslint/ban-types
  const lookup: WeakMap<Function, boolean> = new WeakMap();
    let isNative = false as boolean | undefined;
    let sourceText = '';
    let i = 0;
    // eslint-disable-next-line @typescript-eslint/ban-types
    return function (fn: Function) {
      isNative = lookup.get(fn);
      if (isNative === void 0) {
        sourceText = fn.toString();
        i = sourceText.length;
        // http://www.ecma-international.org/ecma-262/#prod-NativeFunction
        isNative = (
          // 29 is the length of 'function () { [native code] }' which is the smallest length of a native function string
          i >= 29 &&
          // 100 seems to be a safe upper bound of the max length of a native function. In Chrome and FF it's 56, in Edge it's 61.
          i <= 100 &&
          // This whole heuristic *could* be tricked by a comment. Do we need to care about that?
          sourceText.charCodeAt(i -  1) === 0x7D && // }
          // TODO: the spec is a little vague about the precise constraints, so we do need to test this across various browsers to make sure just one whitespace is a safe assumption.
          sourceText.charCodeAt(i -  2)  <= 0x20 && // whitespace
          sourceText.charCodeAt(i -  3) === 0x5D && // ]
          sourceText.charCodeAt(i -  4) === 0x65 && // e
          sourceText.charCodeAt(i -  5) === 0x64 && // d
          sourceText.charCodeAt(i -  6) === 0x6F && // o
          sourceText.charCodeAt(i -  7) === 0x63 && // c
          sourceText.charCodeAt(i -  8) === 0x20 && //
          sourceText.charCodeAt(i -  9) === 0x65 && // e
          sourceText.charCodeAt(i - 10) === 0x76 && // v
          sourceText.charCodeAt(i - 11) === 0x69 && // i
          sourceText.charCodeAt(i - 12) === 0x74 && // t
          sourceText.charCodeAt(i - 13) === 0x61 && // a
          sourceText.charCodeAt(i - 14) === 0x6E && // n
          sourceText.charCodeAt(i - 15) === 0x58    // [
        );
        lookup.set(fn, isNative);
      }
      return isNative;
    };
    })()
```