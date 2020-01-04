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
| [IContainer](/kernel/interface/di/icontainer) | ✘  | ✘ | ✔ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; logger**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| any | ✘  | ✘ | ✔ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; fs**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| [IFileSystem](/aot/system/interface/interfaces/ifilesystem) | ✘  | ✘ | ✔ |

# &#10025; Property(ies)

&nbsp;&nbsp; **&#10148; pkgCache**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| private, readonly | ✘ | Map&lt;string, [NPMPackage](/aot/system/class/npm-package-loader/npmpackage)&gt; |

&nbsp;&nbsp; **&#10148; pkgPromiseCache**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| private, readonly | ✘ | Map&lt;string, Promise&lt;[NPMPackage](/aot/system/class/npm-package-loader/npmpackage)&gt;&gt; |

&nbsp;&nbsp; **&#10148; pkgResolveCache**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| private, readonly | ✘ | Map&lt;string, string&gt; |

&nbsp;&nbsp; **&#10148; pkgResolvePromiseCache**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| private, readonly | ✘ | Map&lt;string, Promise&lt;string&gt;&gt; |

# &#10025; Get Accessor(s)

&nbsp;&nbsp; **&#10148; inject**

| Modifier(s)                              | Return Type                       |
|------------------------------------------|-----------------------------------|
| public, static | any[] |

# &#10025; Method(s)

&nbsp;&nbsp; **&#10148; loadEntryPackage**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public, async | ✘ | Promise&lt;[NPMPackage](/aot/system/class/npm-package-loader/npmpackage)&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; projectDir**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | string | ✘  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; getCachedPackage**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public | ✘ | [NPMPackage](/aot/system/class/npm-package-loader/npmpackage) |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; refName**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | string | ✘  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; loadPackageCore**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| private, async | ✘ | Promise&lt;[NPMPackage](/aot/system/class/npm-package-loader/npmpackage)&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; dir**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | string &#124; null | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; issuer**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | [NPMPackageDependency](/aot/system/class/npm-package-loader/npmpackagedependency) &#124; null | ✘  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; resolvePackagePath**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| private, async | ✘ | Promise&lt;string&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; dep**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | [NPMPackageDependency](/aot/system/class/npm-package-loader/npmpackagedependency) | ✘  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; resolvePackagePathCore**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| private, async | ✘ | Promise&lt;string&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; dep**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | [NPMPackageDependency](/aot/system/class/npm-package-loader/npmpackagedependency) | ✘  | ✘ | ✘ |