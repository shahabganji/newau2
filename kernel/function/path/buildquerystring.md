| Modifier(s)                            | Return Type                    | Generator                        | Overload                         | Implementation                        |
|----------------------------------------|--------------------------------|:--------------------------------:|:--------------------------------:|:-------------------------------------:|
| export | string | ✘ | ✘  | ✔ |

# &#10025; Summary

Generate a query string from an object.

**Parameter(s)**

| Name        | Description                                          |
| ----------- | ---------------------------------------------------- |
| params      |  Object containing the keys and values to be used.   |
| traditional |  Boolean Use the old URI template standard (RFC6570) |

**Returns**

The generated query string, excluding leading '?'.

&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; params**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | [IQueryParams](/kernel/interface/path/iqueryparams) &#124; undefined | ✔  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; traditional**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | boolean &#124; undefined | ✔  | ✘ | ✘ |