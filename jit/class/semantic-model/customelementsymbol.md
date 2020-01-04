# &#10025; Summary

A html element that is associated with a registered resource either via its (lowerCase) `nodeName`
or the value of its `as-element` attribute.

| Modifier(s)                            | Extends                      | Implements                                    |
|----------------------------------------|------------------------------|-----------------------------------------------|
| export | - | - |

# &#10025; Type Parameter(s)

| Type  | Constraint                            |
| ----- | ------------------------------------- |
| TText | [INode](/runtime/interface/dom/inode) |

| Type     | Constraint                            |
| -------- | ------------------------------------- |
| TElement | [INode](/runtime/interface/dom/inode) |

| Type    | Constraint                            |
| ------- | ------------------------------------- |
| TMarker | [INode](/runtime/interface/dom/inode) |

# &#10025; Constructor(s)

| Parameter-less                         | Implementation                          | Overload                          |
|:--------------------------------------:|:---------------------------------------:|:---------------------------------:|
| ✘ | ✔ | ✘ |

&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; dom**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| [IDOM](/runtime/variable/dom/idom)&lt;INode&gt; | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; physicalNode**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| TElement | ✘  | ✘ | ✔ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; info**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| [ElementInfo](/jit/class/resource-model/elementinfo) | ✘  | ✘ | ✔ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; res**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| string | ✔  | ✘ | ✔ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; bindables**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| Record&lt;string, [BindableInfo](/jit/class/resource-model/bindableinfo) &#124; undefined&gt; | ✔  | ✘ | ✔ |

# &#10025; Property(ies)

&nbsp;&nbsp; **&#10148; flags**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public | ✘ | [SymbolFlags](/jit/enum/semantic-model/symbolflags) |

&nbsp;&nbsp; **&#10148; isTarget**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public | ✘ | true |

&nbsp;&nbsp; **&#10148; templateController**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public | ✘ | [TemplateControllerSymbol](/jit/class/semantic-model/templatecontrollersymbol)&lt;TText, TElement, TMarker&gt; &#124; null |

&nbsp;&nbsp; **&#10148; isContainerless**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public | ✘ | boolean |

&nbsp;&nbsp; **&#10148; marker**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public | ✘ | TMarker |

&nbsp;&nbsp; **&#10148; &#95;customAttributes**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| private | ✘ | [CustomAttributeSymbol](/jit/class/semantic-model/customattributesymbol)[] &#124; null |

&nbsp;&nbsp; **&#10148; &#95;plainAttributes**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| private | ✘ | [PlainAttributeSymbol](/jit/class/semantic-model/plainattributesymbol)[] &#124; null |

&nbsp;&nbsp; **&#10148; &#95;bindings**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| private | ✘ | [BindingSymbol](/jit/class/semantic-model/bindingsymbol)[] &#124; null |

&nbsp;&nbsp; **&#10148; &#95;childNodes**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| private | ✘ | NodeSymbol&lt;TText, TElement, TMarker&gt;[] &#124; null |

&nbsp;&nbsp; **&#10148; &#95;parts**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| private | ✘ | [ReplacePartSymbol](/jit/class/semantic-model/replacepartsymbol)&lt;TText, TElement, TMarker&gt;[] &#124; null |

# &#10025; Get Accessor(s)

&nbsp;&nbsp; **&#10148; customAttributes**

| Modifier(s)                              | Return Type                       |
|------------------------------------------|-----------------------------------|
| public | [CustomAttributeSymbol](/jit/class/semantic-model/customattributesymbol)[] |

&nbsp;&nbsp; **&#10148; plainAttributes**

| Modifier(s)                              | Return Type                       |
|------------------------------------------|-----------------------------------|
| public | [PlainAttributeSymbol](/jit/class/semantic-model/plainattributesymbol)[] |

&nbsp;&nbsp; **&#10148; bindings**

| Modifier(s)                              | Return Type                       |
|------------------------------------------|-----------------------------------|
| public | [BindingSymbol](/jit/class/semantic-model/bindingsymbol)[] |

&nbsp;&nbsp; **&#10148; childNodes**

| Modifier(s)                              | Return Type                       |
|------------------------------------------|-----------------------------------|
| public | NodeSymbol&lt;TText, TElement, TMarker&gt;[] |

&nbsp;&nbsp; **&#10148; parts**

| Modifier(s)                              | Return Type                       |
|------------------------------------------|-----------------------------------|
| public | [ReplacePartSymbol](/jit/class/semantic-model/replacepartsymbol)&lt;TText, TElement, TMarker&gt;[] |