# &#10025; Summary

Style binding command. Compile attr with binding symbol with command `style` to `AttributeBindingInstruction`

| Modifier(s)                            | Extends                      | Implements                                    |
|----------------------------------------|------------------------------|-----------------------------------------------|
| export | - | any |

# &#10025; Decorators(s)

| Name                                | Decorator Factory                        |
|-------------------------------------|:----------------------------------------:|
| bindingCommand | ✔  |

| Argument(s)                                           |
|-------------------------------------------------------|
| 'style'  |

# &#10025; Property(ies)

&nbsp;&nbsp; **&#10148; bindingType**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public, readonly | ✘ | BindingType.IsProperty |

# &#10025; Method(s)

&nbsp;&nbsp; **&#10148; compile**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public | ✘ | HTMLAttributeInstruction |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; binding**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | [PlainAttributeSymbol](/jit/class/semantic-model/plainattributesymbol) &#124; [BindingSymbol](/jit/class/semantic-model/bindingsymbol) | ✘  | ✘ | ✘ |