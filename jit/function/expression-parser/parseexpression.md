| Modifier(s)                            | Return Type                    | Generator                        | Overload                         | Implementation                        |
|----------------------------------------|--------------------------------|:--------------------------------:|:--------------------------------:|:-------------------------------------:|
| export | TType extends BindingType.Interpolation ? [IInterpolationExpression](/runtime/interface/ast/iinterpolationexpression) : TType extends BindingType.ForCommand ? [IForOfStatement](/runtime/interface/ast/iforofstatement) : IsBindingBehavior | ✘ | ✘  | ✔ |

# &#10025; Type Parameter(s)

| Type  | Constraint                                                         |
| ----- | ------------------------------------------------------------------ |
| TType | [BindingType](/runtime/binding/enum/expression-parser/bindingtype) |

&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; input**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | string | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; bindingType**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | TType &#124; undefined | ✔  | ✘ | ✘ |