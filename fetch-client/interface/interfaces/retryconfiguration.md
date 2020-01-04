| Modifier(s)                            | Extends                                    |
|----------------------------------------|--------------------------------------------|
| export | - |

# &#10025; Property(ies)

&nbsp;&nbsp; **&#10148; maxRetries**

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✘ | number |

&nbsp;&nbsp; **&#10148; interval**

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | number &#124; undefined |

&nbsp;&nbsp; **&#10148; strategy**

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | number &#124; ((retryCount: number) =&gt; number) &#124; undefined |

&nbsp;&nbsp; **&#10148; minRandomInterval**

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | number &#124; undefined |

&nbsp;&nbsp; **&#10148; maxRandomInterval**

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | number &#124; undefined |

&nbsp;&nbsp; **&#10148; counter**

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | number &#124; undefined |

&nbsp;&nbsp; **&#10148; requestClone**

| Optional                           | Type                         |
|:----------------------------------:|------------------------------|
| ✔ | Request &#124; undefined |

# &#10025; Method(s)

&nbsp;&nbsp; **&#10148; doRetry**

| Return Type                       |
|-----------------------------------|
| boolean &#124; Promise&lt;boolean&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; response**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; request**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp; **&#10148; beforeRetry**

| Return Type                       |
|-----------------------------------|
| Request &#124; Promise&lt;Request&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; request**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; client**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✘  | ✘ | ✘ | - |