# &#10025; Summary

A html attribute that is associated with a registered resource, specifically a template controller.

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

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; syntax**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| [AttrSyntax](/jit/class/ast/attrsyntax) | ✘  | ✘ | ✔ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; info**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| [AttrInfo](/jit/class/resource-model/attrinfo) | ✘  | ✘ | ✔ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; partName**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| string &#124; null | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; res**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| string | ✔  | ✘ | ✔ |

# &#10025; Property(ies)

&nbsp;&nbsp; **&#10148; flags**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public | ✘ | [SymbolFlags](/jit/enum/semantic-model/symbolflags) |

&nbsp;&nbsp; **&#10148; partName**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public | ✘ | string &#124; null |

&nbsp;&nbsp; **&#10148; physicalNode**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public | ✘ | TElement &#124; null |

&nbsp;&nbsp; **&#10148; template**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public | ✘ | CustomElementSymbol&lt;TText, TElement, TMarker&gt; &#124; PlainElementSymbol&lt;TText, TElement, TMarker&gt; &#124; TemplateControllerSymbol&lt;TText, TElement, TMarker&gt; &#124; null |

&nbsp;&nbsp; **&#10148; templateController**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public | ✘ | [TemplateControllerSymbol](/jit/class/semantic-model/templatecontrollersymbol)&lt;TText, TElement, TMarker&gt; &#124; null |

&nbsp;&nbsp; **&#10148; marker**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public | ✘ | TMarker |

&nbsp;&nbsp; **&#10148; &#95;bindings**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| private | ✘ | [BindingSymbol](/jit/class/semantic-model/bindingsymbol)[] &#124; null |

&nbsp;&nbsp; **&#10148; &#95;parts**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| private | ✘ | [ReplacePartSymbol](/jit/class/semantic-model/replacepartsymbol)&lt;TText, TElement, TMarker&gt;[] &#124; null |

# &#10025; Get Accessor(s)

&nbsp;&nbsp; **&#10148; bindings**

| Modifier(s)                              | Return Type                       |
|------------------------------------------|-----------------------------------|
| public | [BindingSymbol](/jit/class/semantic-model/bindingsymbol)[] |

&nbsp;&nbsp; **&#10148; parts**

| Modifier(s)                              | Return Type                       |
|------------------------------------------|-----------------------------------|
| public | [ReplacePartSymbol](/jit/class/semantic-model/replacepartsymbol)&lt;TText, TElement, TMarker&gt;[] |