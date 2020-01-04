# &#10025; Summary

Enables loosely coupled publish/subscribe messaging.

| Modifier(s)                            | Extends                      | Implements                                    |
|----------------------------------------|------------------------------|-----------------------------------------------|
| export | - | [IEventAggregator](/kernel/variable/eventaggregator/ieventaggregator) |

# &#10025; Method(s)

&nbsp;&nbsp; **&#10148; publish**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public | ✘ | void |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Type Parameter(s)**

| Type | Constraint                            |
| ---- | ------------------------------------- |
| T    | string &#124; Constructable&lt;{}&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; channelOrInstance**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | T extends Constructable&lt;{}&gt; ? InstanceType&lt;T&gt; : T | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; data**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | unknown | ✔  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; subscribe**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public | ✘ | [IDisposable](/kernel/interface/interfaces/idisposable) |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Type Parameter(s)**

| Type | Constraint                            |
| ---- | ------------------------------------- |
| T    | string &#124; Constructable&lt;{}&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; channelOrType**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | T | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; callback**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | EventAggregatorCallback&lt;T extends Constructable&lt;{}&gt; ? InstanceType&lt;T&gt; : T&gt; | ✘  | ✘ | ✘ |

&nbsp;&nbsp; **&#10148; subscribeOnce**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public | ✘ | [IDisposable](/kernel/interface/interfaces/idisposable) |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Type Parameter(s)**

| Type | Constraint                            |
| ---- | ------------------------------------- |
| T    | string &#124; Constructable&lt;{}&gt; |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; channelOrType**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | T | ✘  | ✘ | ✘ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; callback**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | EventAggregatorCallback&lt;T&gt; | ✘  | ✘ | ✘ |