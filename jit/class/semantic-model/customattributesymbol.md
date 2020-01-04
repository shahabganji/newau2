# &#10025; Summary

A html attribute that is associated with a registered resource, but not a template controller.

| Modifier(s)                            | Extends                      | Implements                                    |
|----------------------------------------|------------------------------|-----------------------------------------------|
| export | - | [ICustomAttributeSymbol](/jit/interface/semantic-model/icustomattributesymbol) |

# &#10025; Constructor(s)

| Parameter-less                         | Implementation                          | Overload                          |
|:--------------------------------------:|:---------------------------------------:|:---------------------------------:|
| ✘ | ✘ | ✔ |

&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; syntax**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| [AttrSyntax](/jit/class/ast/attrsyntax) | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; info**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| [AttrInfo](/jit/class/resource-model/attrinfo) | ✘  | ✘ | ✘ |

# &#10025; Property(ies)

&nbsp;&nbsp; **&#10148; flags**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| - | ✘ | [SymbolFlags](/jit/enum/semantic-model/symbolflags) |

&nbsp;&nbsp; **&#10148; res**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| - | ✘ | string |

&nbsp;&nbsp; **&#10148; syntax**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| - | ✘ | [AttrSyntax](/jit/class/ast/attrsyntax) |

&nbsp;&nbsp; **&#10148; &#95;bindings**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| private | ✘ | any |

&nbsp;&nbsp; **&#10148; bindings**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| readonly | ✘ | [BindingSymbol](/jit/class/semantic-model/bindingsymbol)[] |