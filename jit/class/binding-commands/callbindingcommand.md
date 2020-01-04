| Modifier(s)                            | Extends                      | Implements                                    |
|----------------------------------------|------------------------------|-----------------------------------------------|
| export | - | { bindingType: [BindingType](/runtime/binding/enum/expression-parser/bindingtype); compile(binding: [PlainAttributeSymbol](/jit/class/semantic-model/plainattributesymbol) &#124; [BindingSymbol](/jit/class/semantic-model/bindingsymbol)): ITargetedInstruction; } |

# &#10025; Decorators(s)

| Name                                | Decorator Factory                        |
|-------------------------------------|:----------------------------------------:|
| bindingCommand | ✔  |

| Argument(s)                                           |
|-------------------------------------------------------|
| 'call'  |

# &#10025; Property(ies)

&nbsp;&nbsp; **&#10148; bindingType**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public, readonly | ✘ | BindingType.CallCommand |

# &#10025; Method(s)

&nbsp;&nbsp; **&#10148; compile**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public | ✘ | AttributeInstruction |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; binding**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | [PlainAttributeSymbol](/jit/class/semantic-model/plainattributesymbol) &#124; [BindingSymbol](/jit/class/semantic-model/bindingsymbol) | ✘  | ✘ | ✘ |