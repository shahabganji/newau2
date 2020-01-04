| Modifier(s)                            | Return Type                    | Generator                        | Overload                         | Implementation                        |
|----------------------------------------|--------------------------------|:--------------------------------:|:--------------------------------:|:-------------------------------------:|
| export | boolean | ✘ | ✘  | ✔ |

# &#10025; Summary

Determine whether a value is `null` or `undefined`.

**Parameter(s)**

| Name  | Description         |
| ----- | ------------------- |
| value |  The value to test. |

**Returns**

`true` if the value is `null` or `undefined`, otherwise `false`.
Also performs a type assertion that ensures TypeScript treats the value appropriately in the `if` and `else` branches after this check.

# &#10025; Type Guard

| On                             |
|--------------------------------|
| null &#124; undefined |

&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; value**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | unknown | ✘  | ✘ | ✘ |