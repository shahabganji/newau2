| Modifier(s)                            |
|----------------------------------------|
| export |

# &#9733; Literal(s)

&nbsp;&nbsp; **&#10148; BindingCommand**

| Type                        | Array                           |
|-----------------------------|---------------------------------|
| BindingCommandKind | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Member(s)**

| Object                        |
|:-----------------------------:|
| ✔ |

**&#9733; Assignment(s)**

**&#10148; name**

| Type                      | Shorthand                         | Spread                        |
|---------------------------|:---------------------------------:|:-----------------------------:|
| { name: any; keyFrom(name: string): string; isType&lt;T&gt;(value: T): value is T extends Constructable&lt;{}&gt; ? any : never; define&lt;T extends Constructable&lt;{ bindingType: BindingType; compile(binding: PlainAttributeSymbol &#124; BindingSymbol): ITargetedInstruction; }&gt;&gt;(nameOrDef: any, Type: T): any; getDefinition&lt;T extends Constructable&lt;{}&gt;&gt;(Type: T): [BindingCommandDefinition](/jit/class/binding-command/bindingcommanddefinition)&lt;T&gt;; annotate&lt;K extends string &#124; number &#124; symbol&gt;(Type: Constructable&lt;{}&gt;, prop: K, value: any): void; getAnnotation&lt;K extends string &#124; number &#124; symbol&gt;(Type: Constructable&lt;{}&gt;, prop: K): any; } | ✘  | ✘ |

**&#9733; Value**

Protocol.resource.keyFor('binding-command')

**&#9733; Method(s)**

&nbsp;&nbsp; **&#10148; keyFrom**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| - | ✘ | string |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; -**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp; **&#10148; isType**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| - | ✘ | boolean |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Type Parameter(s)**

| Type | Constraint |
| ---- | ---------- |
| T    | -          |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; -**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp; **&#10148; define**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| - | ✘ | any |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Type Parameter(s)**

| Type | Constraint                                                                                                                            |
| ---- | ------------------------------------------------------------------------------------------------------------------------------------- |
| T    | Constructable&lt;{ bindingType: BindingType; compile(binding: PlainAttributeSymbol &#124; BindingSymbol): ITargetedInstruction; }&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; -**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp; **&#10148; getDefinition**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| - | ✘ | [BindingCommandDefinition](/jit/class/binding-command/bindingcommanddefinition)&lt;T&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Type Parameter(s)**

| Type | Constraint              |
| ---- | ----------------------- |
| T    | Constructable&lt;{}&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; -**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp; **&#10148; annotate**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| - | ✘ | void |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Type Parameter(s)**

| Type | Constraint                         |
| ---- | ---------------------------------- |
| K    | string &#124; number &#124; symbol |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; -**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp; **&#10148; getAnnotation**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| - | ✘ | any |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Type Parameter(s)**

| Type | Constraint                         |
| ---- | ---------------------------------- |
| K    | string &#124; number &#124; symbol |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; -**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | - | ✘  | ✘ | ✘ | - |