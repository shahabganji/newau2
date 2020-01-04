# &#10025; Summary

Pre-processed information about a custom element resource, optimized
for consumption by the template compiler.

| Modifier(s)                            | Extends                      | Implements                                    |
|----------------------------------------|------------------------------|-----------------------------------------------|
| export | - | - |

# &#10025; Constructor(s)

| Parameter-less                         | Implementation                          | Overload                          |
|:--------------------------------------:|:---------------------------------------:|:---------------------------------:|
| ✘ | ✔ | ✘ |

&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; name**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| string | ✘  | ✘ | ✔ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; containerless**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| boolean | ✘  | ✘ | ✔ |

# &#10025; Property(ies)

&nbsp;&nbsp; **&#10148; bindables**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

A lookup of the bindables of this element, indexed by the (pre-processed)
attribute names as they would be found in parsed markup.

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public | ✘ | Record&lt;string, [BindableInfo](/jit/class/resource-model/bindableinfo) &#124; undefined&gt; |

# &#10025; Method(s)

&nbsp;&nbsp; **&#10148; from**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public, static | ✘ | [ElementInfo](/jit/class/resource-model/elementinfo) |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; def**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | any | ✘  | ✘ | ✘ |