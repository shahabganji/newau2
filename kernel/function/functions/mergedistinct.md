| Modifier(s)                            | Return Type                    | Generator                        | Overload                         | Implementation                        |
|----------------------------------------|--------------------------------|:--------------------------------:|:--------------------------------:|:-------------------------------------:|
| export | T[] | ✘ | ✘  | ✔ |

# &#10025; Summary

Efficiently merge and deduplicate the (primitive) values in two arrays.
Does not deduplicate existing values in the first array.
Guards against null or undefined arrays.
Returns `PLATFORM.emptyArray` if both arrays are either `null`, `undefined` or `PLATFORM.emptyArray`

**Parameter(s)**

| Name  | Description                                                                       |
| ----- | --------------------------------------------------------------------------------- |
| slice |  If `true`, always returns a new array copy (unless neither array is/has a value) |

# &#10025; Type Parameter(s)

| Type | Constraint |
| ---- | ---------- |
| T    | -          |

&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; arr1**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | T[] &#124; readonly T[] &#124; null &#124; undefined | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; arr2**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | T[] &#124; readonly T[] &#124; null &#124; undefined | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; slice**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | boolean | ✘  | ✘ | ✘ |