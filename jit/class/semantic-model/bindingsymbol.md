# &#10025; Summary

Either an attribute on an custom element that maps to a declared bindable property of that element,
a single-value bound custom attribute, or one of several bindables that were extracted from the attribute
value of a dynamicOptions custom attribute.
This will always target a bindable property of a custom attribute or element;

| Modifier(s)                            | Extends                      | Implements                                    |
|----------------------------------------|------------------------------|-----------------------------------------------|
| export | - | [ISymbol](/jit/interface/semantic-model/isymbol) |

# &#10025; Constructor(s)

| Parameter-less                         | Implementation                          | Overload                          |
|:--------------------------------------:|:---------------------------------------:|:---------------------------------:|
| ✘ | ✘ | ✔ |

&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; command**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| [IBindingCommand](/jit/interface/binding-command/ibindingcommand) &#124; null | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; bindable**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| [BindableInfo](/jit/class/resource-model/bindableinfo) | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; expression**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| IAccessThisExpression &#124; IAccessScopeExpression &#124; IArrayLiteralExpression &#124; IObjectLiteralExpression &#124; IPrimitiveLiteralExpression&lt;StrictPrimitive&gt; &#124; ITemplateExpression &#124; ICallFunctionExpression &#124; ICallMemberExpression &#124; ICallScopeExpression &#124; IAccessMemberExpression &#124; IAccessKeyedExpression &#124; ITaggedTemplateExpression &#124; IUnaryExpression &#124; IBinaryExpression &#124; IConditionalExpression &#124; IAssignExpression &#124; IValueConverterExpression &#124; IBindingBehaviorExpression &#124; IInterpolationExpression &#124; IForOfStatement &#124; null | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; rawValue**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| string | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; target**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| string | ✘  | ✘ | ✘ |

# &#10025; Property(ies)

&nbsp;&nbsp; **&#10148; flags**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| - | ✘ | [SymbolFlags](/jit/enum/semantic-model/symbolflags) |

&nbsp;&nbsp; **&#10148; command**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| - | ✘ | [IBindingCommand](/jit/interface/binding-command/ibindingcommand) &#124; null |

&nbsp;&nbsp; **&#10148; bindable**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| - | ✘ | [BindableInfo](/jit/class/resource-model/bindableinfo) |

&nbsp;&nbsp; **&#10148; expression**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| - | ✘ | IAccessThisExpression &#124; IAccessScopeExpression &#124; IArrayLiteralExpression &#124; IObjectLiteralExpression &#124; IPrimitiveLiteralExpression&lt;StrictPrimitive&gt; &#124; ITemplateExpression &#124; ICallFunctionExpression &#124; ICallMemberExpression &#124; ICallScopeExpression &#124; IAccessMemberExpression &#124; IAccessKeyedExpression &#124; ITaggedTemplateExpression &#124; IUnaryExpression &#124; IBinaryExpression &#124; IConditionalExpression &#124; IAssignExpression &#124; IValueConverterExpression &#124; IBindingBehaviorExpression &#124; IInterpolationExpression &#124; IForOfStatement &#124; null |

&nbsp;&nbsp; **&#10148; rawValue**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| - | ✘ | string |

&nbsp;&nbsp; **&#10148; target**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| - | ✘ | string |