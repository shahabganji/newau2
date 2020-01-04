# &#10025; Summary

Pre-processed information about a custom attribute resource, optimized
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

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; isTemplateController**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| boolean | ✘  | ✘ | ✔ |

# &#10025; Property(ies)

&nbsp;&nbsp; **&#10148; bindables**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

A lookup of the bindables of this attribute, indexed by the (pre-processed)
bindable names as they would be found in the attribute value.
Only applicable to multi attribute bindings (semicolon-separated).

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public | ✘ | Record&lt;string, [BindableInfo](/jit/class/resource-model/bindableinfo) &#124; undefined&gt; |

&nbsp;&nbsp; **&#10148; bindable**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

The single or first bindable of this attribute, or a default 'value'
bindable if no bindables were defined on the attribute.
Only applicable to single attribute bindings (where the attribute value
contains no semicolons)

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public | ✘ | [BindableInfo](/jit/class/resource-model/bindableinfo) &#124; null |

# &#10025; Method(s)

&nbsp;&nbsp; **&#10148; from**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public, static | ✘ | [AttrInfo](/jit/class/resource-model/attrinfo) |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; def**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | any | ✘  | ✘ | ✘ |