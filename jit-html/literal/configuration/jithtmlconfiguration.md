# &#9733; Summary

A DI configuration object containing html-specific (but environment-agnostic) registrations:
- `RuntimeHtmlConfiguration` from `@aurelia/runtime-html`
- `DefaultComponents` from `@aurelia/jit`
- `DefaultBindingSyntax` from `@aurelia/jit`
- `DefaultBindingLanguage` from `@aurelia/jit`
- `DefaultComponents`
- `DefaultBindingLanguage`

| Modifier(s)                            |
|----------------------------------------|
| export |

# &#9733; Literal(s)

&nbsp;&nbsp; **&#10148; JitHtmlConfiguration**

| Type                        | Array                           |
|-----------------------------|---------------------------------|
| { register(container: [IContainer](/kernel/interface/di/icontainer)): IContainer; createContainer(): IContainer; } | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Member(s)**

| Object                        |
|:-----------------------------:|
| ✔ |

**&#9733; Method(s)**

&nbsp;&nbsp; **&#10148; register**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**;
Apply this configuration to the provided container.

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| - | ✘ | [IContainer](/kernel/interface/di/icontainer) |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; -**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp; **&#10148; createContainer**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**;
Create a new container with this configuration applied to it.

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| - | ✘ | [IContainer](/kernel/interface/di/icontainer) |