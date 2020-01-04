| Modifier(s)                            | Extends                      | Implements                                    |
|----------------------------------------|------------------------------|-----------------------------------------------|
| export | - | - |

# &#10025; Constructor(s)

| Parameter-less                         | Implementation                          | Overload                          |
|:--------------------------------------:|:---------------------------------------:|:---------------------------------:|
| ✔ | ✔ | ✘ |

# &#10025; Method(s)

&nbsp;&nbsp; **&#10148; createContainer**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public, static | ✘ | [IContainer](/kernel/interface/di/icontainer) |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; params**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | any[] | ✔  | ✔ | ✘ |

&nbsp;&nbsp; **&#10148; getDesignParamtypes**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public, static | ✘ | readonly Key[] &#124; undefined |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; Type**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | Constructable&lt;{}&gt; &#124; Injectable&lt;{}&gt; | ✘  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; getAnnotationParamtypes**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public, static | ✘ | readonly Key[] &#124; undefined |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; Type**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | Constructable&lt;{}&gt; &#124; Injectable&lt;{}&gt; | ✘  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; getOrCreateAnnotationParamTypes**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public, static | ✘ | Key[] |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; Type**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | Constructable&lt;{}&gt; &#124; Injectable&lt;{}&gt; | ✘  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; getDependencies**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public, static | ✘ | Key[] |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; Type**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | Constructable&lt;{}&gt; &#124; Injectable&lt;{}&gt; | ✘  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; createInterface**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public, static | ✘ | [IDefaultableInterfaceSymbol](/kernel/interface/di/idefaultableinterfacesymbol)&lt;K&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Type Parameter(s)**

| Type | Constraint |
| ---- | ---------- |
| K    | Key        |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; friendlyName**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | string &#124; undefined | ✔  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; inject**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public, static | ✘ | (target: Injectable&lt;{}&gt;, key?: string &#124; number &#124; undefined, descriptor?: number &#124; PropertyDescriptor &#124; undefined) =&gt; void |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; dependencies**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | Key[] | ✔  | ✔ | ✘ |

&nbsp;&nbsp; **&#10148; transient**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Registers the `target` class as a transient dependency; each time the dependency is resolved
a new instance will be created.

**Parameter(s)**

| Name   | Description                                                 |
| ------ | ----------------------------------------------------------- |
| target |  The class / constructor function to register as transient. |

**Returns**

The same class, with a static `register` method that takes a container and returns the appropriate resolver.

**Example**

```ts
// On an existing class
class Foo { }
DI.transient(Foo);
// Inline declaration
const Foo = DI.transient(class { });
// Foo is now strongly typed with register
Foo.register(container);
```

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public, static | ✘ | T & RegisterSelf&lt;T&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Type Parameter(s)**

| Type | Constraint              |
| ---- | ----------------------- |
| T    | Constructable&lt;{}&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; target**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | T & Partial&lt;RegisterSelf&lt;T&gt;&gt; | ✘  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; singleton**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Summary**

Registers the `target` class as a singleton dependency; the class will only be created once. Each
consecutive time the dependency is resolved, the same instance will be returned.
  
  **Parameter(s)**

| Name   | Description                                                   |
| ------ | ------------------------------------------------------------- |
| target |  The class / constructor function to register as a singleton. |

**Returns**

The same class, with a static `register` method that takes a container and returns the appropriate resolver.
  
  **Example**

```ts
// On an existing class
class Foo { }
DI.singleton(Foo);
// Inline declaration
const Foo = DI.singleton(class { });
// Foo is now strongly typed with register
Foo.register(container);
```

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public, static | ✘ | T & RegisterSelf&lt;T&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Type Parameter(s)**

| Type | Constraint              |
| ---- | ----------------------- |
| T    | Constructable&lt;{}&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; target**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | T & Partial&lt;RegisterSelf&lt;T&gt;&gt; | ✘  | ✘ | ✘ |