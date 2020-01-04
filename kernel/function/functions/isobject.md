| Modifier(s)                            | Return Type                    | Generator                        | Overload                         | Implementation                        |
|----------------------------------------|--------------------------------|:--------------------------------:|:--------------------------------:|:-------------------------------------:|
| export | boolean | ✘ | ✘  | ✔ |

# &#10025; Summary

Determine whether a value is an object.
Uses `typeof` to guarantee this works cross-realm, which is where `instanceof Object` might fail.
Some environments where these issues are known to arise:
- same-origin iframes (accessing the other realm via `window.top`)
- `jest`.
The exact test is:
```ts
typeof value === 'object' && value !== null || typeof value === 'function'
```
eslint-disable-next-line @typescript-eslint/ban-types

**Parameter(s)**

| Name  | Description         |
| ----- | ------------------- |
| value |  The value to test. |

**Returns**

`true` if the value is an object, otherwise `false`.
  Also performs a type assertion that defaults to `value is Object | Function` which, if the input type is a union with an object type, will infer the correct type.
  This can be overridden with the generic type argument.
  
  **Example**

```ts
class Foo {
  bar = 42;
}
function doStuff(input?: Foo | null) {
  input.bar; // Object is possibly 'null' or 'undefined'
  // input has an object type in its union (Foo) so that type will be extracted for the 'true' condition
  if (isObject(input)) {
    input.bar; // OK (input is now typed as Foo)
  }
}
function doOtherStuff(input: unknown) {
  input.bar; // Object is of type 'unknown'
  // input is 'unknown' so there is no union type to match and it will default to 'Object | Function'
  if (isObject(input)) {
    input.bar; // Property 'bar' does not exist on type 'Object | Function'
  }
  // if we know for sure that, if input is an object, it must be a specific type, we can explicitly tell the function to assert that for us
  if (isObject<Foo>(input)) {
    input.bar; // OK (input is now typed as Foo)
  }
  }
```

# &#10025; Type Guard

| On                             |
|--------------------------------|
| T |

# &#10025; Type Parameter(s)

| Type | Constraint |
| ---- | ---------- |
| T    | object     |

&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; value**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | unknown | ✘  | ✘ | ✘ |