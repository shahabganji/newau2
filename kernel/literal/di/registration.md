| Modifier(s)                            |
|----------------------------------------|
| export |

# &#9733; Literal(s)

&nbsp;&nbsp; **&#10148; Registration**

| Type                        | Array                           |
|-----------------------------|---------------------------------|
| { instance&lt;T&gt;(key: Key, value: T): [IRegistration](/kernel/interface/di/iregistration)&lt;T&gt;; singleton&lt;T extends Constructable&lt;{}&gt;&gt;(key: Key, value: T): IRegistration&lt;InstanceType&lt;T&gt;&gt;; transient&lt;T extends Constructable&lt;{}&gt;&gt;(key: Key, value: T): IRegistration&lt;InstanceType&lt;T&gt;&gt;; callback&lt;T&gt;(key: Key, callback: ResolveCallback&lt;T&gt;): IRegistration&lt;Resolved&lt;T&gt;&gt;; alias&lt;T&gt;(originalKey: T, aliasKey: Key): IRegistration&lt;Resolved&lt;T&gt;&gt;; defer(key: Key, ...params: unknown[]): [IRegistry](/kernel/interface/di/iregistry); } | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Member(s)**

| Object                        |
|:-----------------------------:|
| ✔ |

**&#9733; Method(s)**

&nbsp;&nbsp; **&#10148; instance**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| - | ✘ | [IRegistration](/kernel/interface/di/iregistration)&lt;T&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Type Parameter(s)**

| Type | Constraint |
| ---- | ---------- |
| T    | -          |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; -**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp; **&#10148; singleton**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| - | ✘ | [IRegistration](/kernel/interface/di/iregistration)&lt;InstanceType&lt;T&gt;&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Type Parameter(s)**

| Type | Constraint              |
| ---- | ----------------------- |
| T    | Constructable&lt;{}&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; -**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp; **&#10148; transient**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| - | ✘ | [IRegistration](/kernel/interface/di/iregistration)&lt;InstanceType&lt;T&gt;&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Type Parameter(s)**

| Type | Constraint              |
| ---- | ----------------------- |
| T    | Constructable&lt;{}&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; -**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp; **&#10148; callback**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| - | ✘ | [IRegistration](/kernel/interface/di/iregistration)&lt;Resolved&lt;T&gt;&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Type Parameter(s)**

| Type | Constraint |
| ---- | ---------- |
| T    | -          |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; -**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp; **&#10148; alias**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| - | ✘ | [IRegistration](/kernel/interface/di/iregistration)&lt;Resolved&lt;T&gt;&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Type Parameter(s)**

| Type | Constraint |
| ---- | ---------- |
| T    | -          |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; -**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | - | ✘  | ✘ | ✘ | - |

&nbsp;&nbsp; **&#10148; defer**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| - | ✘ | [IRegistry](/kernel/interface/di/iregistry) |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; -**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          | Initializer                       |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|-----------------------------------|
| - | - | ✘  | ✘ | ✘ | - |