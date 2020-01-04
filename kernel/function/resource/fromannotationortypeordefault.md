| Modifier(s)                            | Return Type                    | Generator                        | Overload                         | Implementation                        |
|----------------------------------------|--------------------------------|:--------------------------------:|:--------------------------------:|:-------------------------------------:|
| export | V | ✘ | ✘  | ✔ |

# &#10025; Summary

The order in which the values are checked:
1. Annotations (usually set by decorators) have the highest priority; they override static properties on the type.
2. Static properties on the typ. Note that this does not look up the prototype chain (bindables are an exception here, but we do that differently anyway)
3. The default property that is provided last. The function is only called if the default property is needed

# &#10025; Type Parameter(s)

| Type | Constraint |
| ---- | ---------- |
| T    | -          |

| Type | Constraint |
| ---- | ---------- |
| K    | keyof T    |

| Type | Constraint |
| ---- | ---------- |
| V    | -          |

&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; name**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | K | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; Type**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | T | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; getDefault**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | () =&gt; V | ✘  | ✘ | ✘ |