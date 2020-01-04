| Modifier(s)                            | Return Type                    | Generator                        | Overload                         | Implementation                        |
|----------------------------------------|--------------------------------|:--------------------------------:|:--------------------------------:|:-------------------------------------:|
| export | Required&lt;TDef&gt;[K] | ✘ | ✘  | ✔ |

# &#10025; Summary

The order in which the values are checked:
1. Definition properties.
2. The default property that is provided last. The function is only called if the default property is needed

# &#10025; Type Parameter(s)

| Type | Constraint                                                                        |
| ---- | --------------------------------------------------------------------------------- |
| TDef | { readonly name: string; readonly aliases?: readonly string[] &#124; undefined; } |

| Type | Constraint |
| ---- | ---------- |
| K    | keyof TDef |

&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; name**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | K | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; def**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | TDef | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; getDefault**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | () =&gt; Required&lt;TDef&gt;[K] | ✘  | ✘ | ✘ |