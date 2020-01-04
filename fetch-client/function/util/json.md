| Modifier(s)                            | Return Type                    | Generator                        | Overload                         | Implementation                        |
|----------------------------------------|--------------------------------|:--------------------------------:|:--------------------------------:|:-------------------------------------:|
| export | string | ✘ | ✘  | ✔ |

# &#10025; Summary

Serialize an object to JSON. Useful for easily creating JSON fetch request bodies.

**Parameter(s)**

| Name     | Description                                         |
| -------- | --------------------------------------------------- |
| body     |  The object to be serialized to JSON.               |
| replacer |  The JSON.stringify replacer used when serializing. |

**Returns**

A JSON string.

&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; body**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | unknown | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; replacer**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | ((key: string, value: unknown) =&gt; unknown) &#124; undefined | ✔  | ✘ | ✘ |