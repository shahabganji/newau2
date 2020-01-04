| Modifier(s)                            | Extends                      | Implements                                    |
|----------------------------------------|------------------------------|-----------------------------------------------|
| export | - | [ILogger](/kernel/interface/logger/ilogger) |

# &#10025; Constructor(s)

| Parameter-less                         | Implementation                          | Overload                          |
|:--------------------------------------:|:---------------------------------------:|:---------------------------------:|
| ✘ | ✔ | ✘ |

&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; config**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| [ILogConfig](/kernel/interface/logger/ilogconfig) | ✘  | ✘ | ✔ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Decorator(s)**

| Name                                | Decorator Factory                        |
|-------------------------------------|:----------------------------------------:|
| ILogConfig | ✘  |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; factory**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| [ILogEventFactory](/kernel/interface/logger/ilogeventfactory) | ✘  | ✘ | ✔ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Decorator(s)**

| Name                                | Decorator Factory                        |
|-------------------------------------|:----------------------------------------:|
| ILogEventFactory | ✘  |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; sinks**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| [ISink](/kernel/interface/logger/isink)[] | ✘  | ✘ | ✔ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Decorator(s)**

| Name                                | Decorator Factory                        |
|-------------------------------------|:----------------------------------------:|
| all | ✔  |

| Argument(s)                                           |
|-------------------------------------------------------|
| ISink  |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; scope**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| string[] | ✔  | ✘ | ✔ |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#10149; parent**

| Type                        | Optional                           | Rest                          | Parameter Property                          |
|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| [ILogger](/kernel/interface/logger/ilogger) &#124; null | ✔  | ✘ | ✘ |

# &#10025; Property(ies)

&nbsp;&nbsp; **&#10148; root**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public, readonly | ✘ | [ILogger](/kernel/interface/logger/ilogger) |

&nbsp;&nbsp; **&#10148; parent**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public, readonly | ✘ | [ILogger](/kernel/interface/logger/ilogger) |

&nbsp;&nbsp; **&#10148; trace**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public, readonly | ✘ | (...args: unknown[]) =&gt; void |

&nbsp;&nbsp; **&#10148; debug**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public, readonly | ✘ | (...args: unknown[]) =&gt; void |

&nbsp;&nbsp; **&#10148; info**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public, readonly | ✘ | (...args: unknown[]) =&gt; void |

&nbsp;&nbsp; **&#10148; warn**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public, readonly | ✘ | (...args: unknown[]) =&gt; void |

&nbsp;&nbsp; **&#10148; error**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public, readonly | ✘ | (...args: unknown[]) =&gt; void |

&nbsp;&nbsp; **&#10148; fatal**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| public, readonly | ✘ | (...args: unknown[]) =&gt; void |

&nbsp;&nbsp; **&#10148; scopedLoggers**

| Modifier(s)                               | Optional                           | Type                         |
|-------------------------------------------|:----------------------------------:|------------------------------|
| private, readonly | ✘ | { [key: string]: [ILogger](/kernel/interface/logger/ilogger) &#124; undefined; } |

# &#10025; Method(s)

&nbsp;&nbsp; **&#10148; scopeTo**

| Modifier(s)                              | Generator                          | Return Type                       |
|------------------------------------------|:----------------------------------:|-----------------------------------|
| public | ✘ | [ILogger](/kernel/interface/logger/ilogger) |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **&#9733; Parameter(s)**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; _**&#10149; name**_

| Modifier(s)                              | Type                        | Optional                           | Rest                          | Parameter Property                          |
|------------------------------------------|-----------------------------|:----------------------------------:|:-----------------------------:|:-------------------------------------------:|
| - | string | ✘  | ✘ | ✘ |