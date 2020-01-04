# &#10025; Summary

A standalone text node that has an interpolation.

| Modifier(s)                            | Extends                      | Implements                                    |
|----------------------------------------|------------------------------|-----------------------------------------------|
| export | - | - |

# &#10025; Type Parameter(s)

| Type  | Constraint                            |
| ----- | ------------------------------------- |
| TText | [INode](/runtime/interface/dom/inode) |

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
| TText | ✘  | ✘ | ✔ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; interpolation**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| [IInterpolationExpression](/runtime/interface/ast/iinterpolationexpression) | ✘  | ✘ | ✔ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; marker**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| TMarker | ✔  | ✘ | ✔ |

# &#10025; Property(ies)

&nbsp;&nbsp; **&#10148; flags**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public | ✘ | [SymbolFlags](/jit/enum/semantic-model/symbolflags) |