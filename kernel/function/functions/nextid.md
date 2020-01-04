| Modifier(s)                            | Return Type                    | Generator                        | Overload                         | Implementation                        |
|----------------------------------------|--------------------------------|:--------------------------------:|:--------------------------------:|:-------------------------------------:|
| export | number | ✘ | ✘  | ✔ |

# &#10025; Summary

Retrieve the next ID in a sequence for a given string, starting with `1`.
Used by Aurelia to assign unique ID's to controllers and resources.
Aurelia will always prepend the context name with `au$`, so as long as you avoid
using that convention you should be safe from collisions.

&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; context**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | string | ✘  | ✘ | ✘ |