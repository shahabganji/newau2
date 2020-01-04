# &#10025; Summary

Utility that creates a `HTMLTemplateElement` out of string markup or an existing DOM node.
It is idempotent in the sense that passing in an existing template element will simply return that template element,
so it is always safe to pass in a node without causing unnecessary DOM parsing or template creation.

| Modifier(s)                            | Extends                                    |
|----------------------------------------|--------------------------------------------|
| export | - |

# &#10025; Type Parameter(s)

| Type  | Constraint                            |
| ----- | ------------------------------------- |
| TNode | [INode](/runtime/interface/dom/inode) |

# &#10025; Method(s)

&nbsp;&nbsp; **&#10148; createTemplate**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Create a `HTMLTemplateElement` from a provided html string.

**Parameter(s)**

| Name   | Description                                                                  |
| ------ | ---------------------------------------------------------------------------- |
| markup |  A raw html string that may or may not be wrapped in `<template></template>` |

| Return Type                       |
|-----------------------------------|
| TNode |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; markup**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp; **&#10148; createTemplate**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Create a `HTMLTemplateElement` from a provided DOM node. If the node is already a template, it
will be returned as-is (and removed from the DOM).

**Parameter(s)**

| Name | Description                                                           |
| ---- | --------------------------------------------------------------------- |
| node |  A DOM node that may or may not be wrapped in `<template></template>` |

| Return Type                       |
|-----------------------------------|
| TNode |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; node**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp; **&#10148; createTemplate**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Create a `HTMLTemplateElement` from a provided DOM node or html string.

**Parameter(s)**

| Name  | Description                                                                              |
| ----- | ---------------------------------------------------------------------------------------- |
| input |  A DOM node or raw html string that may or may not be wrapped in `<template></template>` |

| Return Type                       |
|-----------------------------------|
| TNode |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; input**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp; **&#10148; createTemplate**

| Return Type                       |
|-----------------------------------|
| TNode |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; input**_

| Modifier(s)                              | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | ✘  | ✘ | ✘ | - |