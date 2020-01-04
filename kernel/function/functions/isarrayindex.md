| Modifier(s)                            | Return Type                    | Generator                        | Overload                         | Implementation                        |
|----------------------------------------|--------------------------------|:--------------------------------:|:--------------------------------:|:-------------------------------------:|
| export | boolean | ✘ | ✘  | ✔ |

# &#10025; Summary

Efficiently determine whether the provided property key is numeric
(and thus could be an array indexer) or not.
Always returns true for values of type `'number'`.
Otherwise, only returns true for strings that consist only of positive integers.
Results are cached.

# &#10025; Type Guard

| On                             |
|--------------------------------|
| string &#124; number |

&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; value**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | unknown | ✘  | ✘ | ✘ |