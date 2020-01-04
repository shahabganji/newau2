# &#10025; Summary

A pre-processed piece of information about declared custom elements, attributes and
binding commands, optimized for consumption by the template compiler.

| Modifier(s)                            | Extends                      | Implements                                    |
|----------------------------------------|------------------------------|-----------------------------------------------|
| export | - | - |

# &#10025; Constructor(s)

| Parameter-less                         | Implementation                          | Overload                          |
|:--------------------------------------:|:---------------------------------------:|:---------------------------------:|
| ✘ | ✔ | ✘ |

&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; container**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| [IContainer](/kernel/interface/di/icontainer) | ✘  | ✘ | ✘ |

# &#10025; Property(ies)

&nbsp;&nbsp; **&#10148; elementLookup**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| private, readonly | ✘ | Record&lt;string, [ElementInfo](/jit/class/resource-model/elementinfo) &#124; null &#124; undefined&gt; |

&nbsp;&nbsp; **&#10148; attributeLookup**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| private, readonly | ✘ | Record&lt;string, [AttrInfo](/jit/class/resource-model/attrinfo) &#124; null &#124; undefined&gt; |

&nbsp;&nbsp; **&#10148; commandLookup**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| private, readonly | ✘ | Record&lt;string, { bindingType: BindingType; compile(binding: PlainAttributeSymbol &#124; BindingSymbol): ITargetedInstruction; } &#124; null &#124; undefined&gt; |

&nbsp;&nbsp; **&#10148; container**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| private, readonly | ✘ | [IContainer](/kernel/interface/di/icontainer) |

&nbsp;&nbsp; **&#10148; resourceResolvers**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| private, readonly | ✘ | Record&lt;string, [IResolver](/kernel/interface/di/iresolver)&lt;any&gt; &#124; null &#124; undefined&gt; |

&nbsp;&nbsp; **&#10148; rootResourceResolvers**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| private, readonly | ✘ | Record&lt;string, [IResolver](/kernel/interface/di/iresolver)&lt;any&gt; &#124; null &#124; undefined&gt; |

# &#10025; Method(s)

&nbsp;&nbsp; **&#10148; getOrCreate**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public, static | ✘ | [ResourceModel](/jit/class/resource-model/resourcemodel) |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; context**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | [IContainer](/kernel/interface/di/icontainer) | ✘  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; getElementInfo**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Retrieve information about a custom element resource.

**Parameter(s)**

The original DOM element.

**Returns**

The resource information if the element exists, or `null` if it does not exist.

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public | ✘ | [ElementInfo](/jit/class/resource-model/elementinfo) &#124; null |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; name**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | string | ✘  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; getAttributeInfo**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Retrieve information about a custom attribute resource.

**Parameter(s)**

| Name   | Description              |
| ------ | ------------------------ |
| syntax |  The parsed `AttrSyntax` |

**Returns**

The resource information if the attribute exists, or `null` if it does not exist.

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public | ✘ | [AttrInfo](/jit/class/resource-model/attrinfo) &#124; null |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; syntax**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | [AttrSyntax](/jit/class/ast/attrsyntax) | ✘  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; getBindingCommand**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Retrieve a binding command resource.

**Parameter(s)**

The parsed `AttrSyntax`

**Returns**

An instance of the command if it exists, or `null` if it does not exist.

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public | ✘ | { bindingType: BindingType; compile(binding: PlainAttributeSymbol &#124; BindingSymbol): ITargetedInstruction; } &#124; null |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; syntax**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | [AttrSyntax](/jit/class/ast/attrsyntax) | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; optional**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | boolean | ✘  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; find**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| private | ✘ | TDef &#124; null |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Type Parameter(s)**

| Type  | Constraint |
| ----- | ---------- |
| TType | any        |

| Type | Constraint |
| ---- | ---------- |
| TDef | any        |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; kind**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | [IResourceKind](/kernel/interface/resource/iresourcekind)&lt;TType, TDef, { new (...args: any[]): TDef & { constructor: {}; }; readonly prototype: TDef & { constructor: {}; }; }&gt; | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; name**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | string | ✘  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; create**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| private | ✘ | InstanceType&lt;TType&gt; &#124; null |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Type Parameter(s)**

| Type  | Constraint |
| ----- | ---------- |
| TType | any        |

| Type | Constraint |
| ---- | ---------- |
| TDef | any        |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; kind**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | [IResourceKind](/kernel/interface/resource/iresourcekind)&lt;TType, TDef, { new (...args: any[]): TDef & { constructor: {}; }; readonly prototype: TDef & { constructor: {}; }; }&gt; | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; name**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | string | ✘  | ✘ | ✘ |