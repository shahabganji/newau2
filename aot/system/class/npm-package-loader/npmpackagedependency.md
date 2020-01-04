| Modifier(s)                            | Extends                      | Implements                                    |
|----------------------------------------|------------------------------|-----------------------------------------------|
| export | - | - |

# &#10025; Constructor(s)

| Parameter-less                         | Implementation                          | Overload                          |
|:--------------------------------------:|:---------------------------------------:|:---------------------------------:|
| ✘ | ✔ | ✘ |

&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; issuer**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| [NPMPackage](/aot/system/class/npm-package-loader/npmpackage) | ✘  | ✘ | ✔ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; refName**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| string | ✘  | ✘ | ✔ |

# &#10025; Property(ies)

&nbsp;&nbsp; **&#10148; &#95;pkg**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| private | ✘ | [NPMPackage](/aot/system/class/npm-package-loader/npmpackage) &#124; undefined |

&nbsp;&nbsp; **&#10148; loadPromise**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| private | ✘ | Promise&lt;void&gt; &#124; undefined |

# &#10025; Get Accessor(s)

&nbsp;&nbsp; **&#10148; pkg**

| Modifier(s)                              | Return Type                       |
|------------------------------------------|-----------------------------------|
| public | [NPMPackage](/aot/system/class/npm-package-loader/npmpackage) |

# &#10025; Method(s)

&nbsp;&nbsp; **&#10148; loadCore**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| private, async | ✘ | Promise&lt;void&gt; |